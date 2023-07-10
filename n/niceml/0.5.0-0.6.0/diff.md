# Comparing `tmp/niceml-0.5.0.tar.gz` & `tmp/niceml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niceml-0.5.0.tar", max compression
+gzip compressed data, was "niceml-0.6.0.tar", max compression
```

## Comparing `niceml-0.5.0.tar` & `niceml-0.6.0.tar`

### file list

```diff
@@ -1,330 +1,338 @@
--rw-r--r--   0        0        0     1068 2023-06-23 12:03:11.100200 niceml-0.5.0/LICENSE
--rw-r--r--   0        0        0     1135 2023-06-23 12:03:11.100200 niceml-0.5.0/README.md
--rw-r--r--   0        0        0       22 2023-06-23 12:03:53.668643 niceml-0.5.0/niceml/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/cli/__init__.py
--rw-r--r--   0        0        0     3070 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/cli/clicommands.py
--rw-r--r--   0        0        0      228 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/cli/climain.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/config/__init__.py
--rw-r--r--   0        0        0     9485 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/config/configschemas.py
--rw-r--r--   0        0        0      889 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/config/envconfig.py
--rw-r--r--   0        0        0     5117 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/config/hydra.py
--rw-r--r--   0        0        0      744 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/config/subsetnames.py
--rw-r--r--   0        0        0      310 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/config/trainparams.py
--rw-r--r--   0        0        0      506 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/config/writeopconfig.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/jobs/__init__.py
--rw-r--r--   0        0        0     3212 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/jobs/jobs.py
--rw-r--r--   0        0        0      512 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/jobs/repository.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/__init__.py
--rw-r--r--   0        0        0     2305 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/analysis.py
--rw-r--r--   0        0        0     2317 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/copyexp.py
--rw-r--r--   0        0        0     3900 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/cropnumbers.py
--rw-r--r--   0        0        0      921 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/datageneration.py
--rw-r--r--   0        0        0     3396 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/evalcopyexp.py
--rw-r--r--   0        0        0     2058 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/experiment.py
--rw-r--r--   0        0        0     1176 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/exptests.py
--rw-r--r--   0        0        0     1281 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/filelockops.py
--rw-r--r--   0        0        0     4556 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/imagetotable.py
--rw-r--r--   0        0        0     2220 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/localizeexperiment.py
--rw-r--r--   0        0        0     6008 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/prediction.py
--rw-r--r--   0        0        0     3003 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/splitdata.py
--rw-r--r--   0        0        0     3117 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/ops/train.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/resources/__init__.py
--rw-r--r--   0        0        0     3668 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dagster/resources/locations.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/__init__.py
--rw-r--r--   0        0        0     6736 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/binprobvisu.py
--rw-r--r--   0        0        0     4033 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/cam.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/components/__init__.py
--rw-r--r--   0        0        0     3870 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/components/downloadexpviscomponent.py
--rw-r--r--   0        0        0     4603 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/components/expviscomponent.py
--rw-r--r--   0        0        0     1835 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/components/linearviscomponent.py
--rw-r--r--   0        0        0     1329 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/components/metaviscomponent.py
--rw-r--r--   0        0        0     3769 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/components/prefixviscomponent.py
--rw-r--r--   0        0        0     2892 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/components/selectionviscomponent.py
--rw-r--r--   0        0        0     1446 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/configviscomponent.py
--rw-r--r--   0        0        0     3006 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/dashboard.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/expvisuhelper.py
--rw-r--r--   0        0        0     3126 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/imagenetdataloggerviscomponent.py
--rw-r--r--   0        0        0     3294 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/metricviscomponent.py
--rw-r--r--   0        0        0      293 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/netdataloggerviscomponent.py
--rw-r--r--   0        0        0     5961 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/remotettrainutils.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/visualizers/__init__.py
--rw-r--r--   0        0        0     3125 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/visualizers/boundingboxvisualizer.py
--rw-r--r--   0        0        0     4554 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/visualizers/imagevisualizer.py
--rw-r--r--   0        0        0     3206 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/dashboard/visualizers/maskvisualizer.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/augmentation/__init__.py
--rw-r--r--   0        0        0      362 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/augmentation/augmentation.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/__init__.py
--rw-r--r--   0        0        0     2369 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/clsdatadescription.py
--rw-r--r--   0        0        0      260 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/datadescription.py
--rw-r--r--   0        0        0     1247 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/inputdatadescriptions.py
--rw-r--r--   0        0        0     2687 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/objdetdatadescription.py
--rw-r--r--   0        0        0     5136 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/outputdatadescriptions.py
--rw-r--r--   0        0        0     2734 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/regdatadescription.py
--rw-r--r--   0        0        0     2996 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datadescriptions/semsegdatadescritption.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfolistings/__init__.py
--rw-r--r--   0        0        0     4942 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfolistings/clsdatainfolisting.py
--rw-r--r--   0        0        0      493 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfolistings/datainfolisting.py
--rw-r--r--   0        0        0     3905 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfolistings/objdetdatainfolisting.py
--rw-r--r--   0        0        0     2585 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfolistings/semsegdatainfolisting.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfos/__init__.py
--rw-r--r--   0        0        0     2388 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfos/clsdatainfo.py
--rw-r--r--   0        0        0      458 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfos/datainfo.py
--rw-r--r--   0        0        0      755 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfos/imagedatainfo.py
--rw-r--r--   0        0        0     1120 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfos/objdetdatainfo.py
--rw-r--r--   0        0        0     1112 2023-06-23 12:03:11.108200 niceml-0.5.0/niceml/data/datainfos/semsegdatainfo.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataiterators/__init__.py
--rw-r--r--   0        0        0     2783 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataiterators/boundingboxdataiterator.py
--rw-r--r--   0        0        0      560 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataiterators/dataiterator.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/__init__.py
--rw-r--r--   0        0        0     2229 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/cachedimageloader.py
--rw-r--r--   0        0        0     1094 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/clsdataloader.py
--rw-r--r--   0        0        0      747 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/dataloader.py
--rw-r--r--   0        0        0     2934 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/dfloaders.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/factories/__init__.py
--rw-r--r--   0        0        0      516 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/factories/dfloaderfactory.py
--rw-r--r--   0        0        0      509 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/factories/imageloaderfactory.py
--rw-r--r--   0        0        0     1572 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/imageloaders.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/interfaces/__init__.py
--rw-r--r--   0        0        0      338 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/interfaces/dfloader.py
--rw-r--r--   0        0        0      753 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/interfaces/imageloader.py
--rw-r--r--   0        0        0     1137 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/objdetdataloader.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/semseg/__init__.py
--rw-r--r--   0        0        0     1615 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx
--rw-r--r--   0        0        0     1938 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/semseg/semsegdataloader.py
--rw-r--r--   0        0        0      844 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/dataloaders/semseg/transformmaskimage.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datasets/__init__.py
--rw-r--r--   0        0        0     4453 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datasets/clsclassinfo.py
--rw-r--r--   0        0        0     1546 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datasets/dataset.py
--rw-r--r--   0        0        0     4914 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datasets/dfdataset.py
--rw-r--r--   0        0        0     5362 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datasets/genericdataset.py
--rw-r--r--   0        0        0     1088 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datasets/healthdataset.py
--rw-r--r--   0        0        0     1147 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datasets/sinusdataset.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datashuffler/__init__.py
--rw-r--r--   0        0        0      603 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datashuffler/datashuffler.py
--rw-r--r--   0        0        0      536 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datashuffler/defaultshuffler.py
--rw-r--r--   0        0        0     2613 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datashuffler/uniformdistributionshuffler.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datastatsgenerator/__init__.py
--rw-r--r--   0        0        0      426 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datastatsgenerator/datastatsgenerator.py
--rw-r--r--   0        0        0      472 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/datastatsgenerator/defaultstatsgenerator.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/netdataloggers/__init__.py
--rw-r--r--   0        0        0     1952 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/netdataloggers/netdatalogger.py
--rw-r--r--   0        0        0     4732 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/netdataloggers/objdetnetdatalogger.py
--rw-r--r--   0        0        0     5023 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/netdataloggers/semsegnetdatalogger.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/storages/__init__.py
--rw-r--r--   0        0        0     3013 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/storages/fsfilesystemstorage.py
--rw-r--r--   0        0        0     3485 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/storages/fsspecstorage.py
--rw-r--r--   0        0        0     2306 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/storages/localstorage.py
--rw-r--r--   0        0        0      898 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/storages/storagehandler.py
--rw-r--r--   0        0        0      973 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/data/storages/storageinterface.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/__init__.py
--rw-r--r--   0        0        0     3566 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py
--rw-r--r--   0        0        0     1662 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py
--rw-r--r--   0        0        0     4227 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py
--rw-r--r--   0        0        0      922 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py
--rw-r--r--   0        0        0      929 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/kerasmetrics.py
--rw-r--r--   0        0        0     1404 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/kerasmodelloader.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/learners/__init__.py
--rw-r--r--   0        0        0     2344 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/learners/defaultlearner.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/losses/__init__.py
--rw-r--r--   0        0        0     1488 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py
--rw-r--r--   0        0        0     3957 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/losses/objdetlosses.py
--rw-r--r--   0        0        0     2055 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/losses/semseglosses.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/metrics/__init__.py
--rw-r--r--   0        0        0     3048 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py
--rw-r--r--   0        0        0     2212 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/modelcompiler/__init__.py
--rw-r--r--   0        0        0     2136 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/__init__.py
--rw-r--r--   0        0        0     3701 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py
--rw-r--r--   0        0        0     2530 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/layerfactory.py
--rw-r--r--   0        0        0     1569 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py
--rw-r--r--   0        0        0     1979 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/mlp.py
--rw-r--r--   0        0        0     2250 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/mobilenet.py
--rw-r--r--   0        0        0     1813 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/premodellayers.py
--rw-r--r--   0        0        0     7749 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/retinanet.py
--rw-r--r--   0        0        0    11007 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/models/unets.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/optimizers/schedules/__init__.py
--rw-r--r--   0        0        0     1158 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/__init__.py
--rw-r--r--   0        0        0     4437 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/confextractionmetafunction.py
--rw-r--r--   0        0        0     1431 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/expdatalocalstorageloader.py
--rw-r--r--   0        0        0     3277 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/expdatastorageloader.py
--rw-r--r--   0        0        0     4447 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimentcontext.py
--rw-r--r--   0        0        0    14860 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimentdata.py
--rw-r--r--   0        0        0     2109 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimentdownloader.py
--rw-r--r--   0        0        0      673 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimenterrors.py
--rw-r--r--   0        0        0     3122 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimentinfo.py
--rw-r--r--   0        0        0    12258 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimentmanager.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimenttests/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimenttests/checkfilesfolderstest.py
--rw-r--r--   0        0        0      904 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimenttests/exptests.py
--rw-r--r--   0        0        0     1667 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimenttests/metriccheck.py
--rw-r--r--   0        0        0     2320 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimenttests/testinitializer.py
--rw-r--r--   0        0        0     3521 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/experimenttests/validateexps.py
--rw-r--r--   0        0        0     3007 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/expfilenames.py
--rw-r--r--   0        0        0     3153 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/expoutinitializer.py
--rw-r--r--   0        0        0     1199 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/exppathfinder.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/filters/__init__.py
--rw-r--r--   0        0        0     1922 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/filters/datefilter.py
--rw-r--r--   0        0        0      547 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/filters/experimentfilter.py
--rw-r--r--   0        0        0     2142 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/filters/expselectionfilter.py
--rw-r--r--   0        0        0     1867 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/filters/selectboxfilter.py
--rw-r--r--   0        0        0     2911 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/filters/sliderfilter.py
--rw-r--r--   0        0        0     2304 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/loaddatafunctions.py
--rw-r--r--   0        0        0      828 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/loadexpinfo.py
--rw-r--r--   0        0        0     6149 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/localexperimentcache.py
--rw-r--r--   0        0        0     2683 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/metafunctions.py
--rw-r--r--   0        0        0     1598 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/metainfotables.py
--rw-r--r--   0        0        0     3300 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/metalists.py
--rw-r--r--   0        0        0      512 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/metatablefactory.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/schemas/__init__.py
--rw-r--r--   0        0        0      669 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/schemas/baseexpschema.py
--rw-r--r--   0        0        0      637 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/schemas/expdocstring.py
--rw-r--r--   0        0        0     2533 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/schemas/expmember.py
--rw-r--r--   0        0        0     1416 2023-06-23 12:03:11.112201 niceml-0.5.0/niceml/experiments/schemas/objdetexpschema.py
--rw-r--r--   0        0        0     1210 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/experiments/schemas/parquetframeexpmember.py
--rw-r--r--   0        0        0     1474 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/experiments/schemas/sampleexpschemas.py
--rw-r--r--   0        0        0      390 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/experiments/schemas/schemalist.py
--rw-r--r--   0        0        0      788 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/experiments/schemas/schemavalidation.py
--rw-r--r--   0        0        0     2179 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/experiments/schemas/yamlexpmember.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/filechecksumprocessors/__init__.py
--rw-r--r--   0        0        0     8593 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/filechecksumprocessors/filechecksumprocessor.py
--rw-r--r--   0        0        0     7412 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/filechecksumprocessors/zippedcsvtoparqprocessor.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mkdocs/__init__.py
--rw-r--r--   0        0        0      517 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mkdocs/mdgraph.py
--rw-r--r--   0        0        0      839 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mkdocs/mdjob.py
--rw-r--r--   0        0        0     1105 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mkdocs/mdop.py
--rw-r--r--   0        0        0     1189 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mkdocs/mdtable.py
--rw-r--r--   0        0        0     1422 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mkdocs/schemadocgeneration.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/callbacks/__init__.py
--rw-r--r--   0        0        0      921 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/callbacks/callbackinitializer.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/learners/__init__.py
--rw-r--r--   0        0        0     1125 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/learners/fitgenerators.py
--rw-r--r--   0        0        0      994 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/learners/learner.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/modelcompiler/__init__.py
--rw-r--r--   0        0        0      575 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/modelcompiler/modelcompiler.py
--rw-r--r--   0        0        0      563 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/modelloader/__init__.py
--rw-r--r--   0        0        0      600 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/modelloader/modelloader.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/models/__init__.py
--rw-r--r--   0        0        0      160 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/models/modelbundle.py
--rw-r--r--   0        0        0      476 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/models/modelfactory.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/objdet/__init__.py
--rw-r--r--   0        0        0     7607 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/objdet/anchorencoding.py
--rw-r--r--   0        0        0     2905 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/objdet/anchorgenerator.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/predictionhandlers/__init__.py
--rw-r--r--   0        0        0     1404 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py
--rw-r--r--   0        0        0     6251 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py
--rw-r--r--   0        0        0     1383 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/predictionhandlers/predictionhandler.py
--rw-r--r--   0        0        0    10584 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py
--rw-r--r--   0        0        0     4896 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py
--rw-r--r--   0        0        0     2550 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/__init__.py
--rw-r--r--   0        0        0      836 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/analyzer.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/__init__.py
--rw-r--r--   0        0        0     4118 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py
--rw-r--r--   0        0        0     2320 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py
--rw-r--r--   0        0        0     3806 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py
--rw-r--r--   0        0        0     3328 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/__init__.py
--rw-r--r--   0        0        0     1709 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py
--rw-r--r--   0        0        0      603 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py
--rw-r--r--   0        0        0     1658 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py
--rw-r--r--   0        0        0     3007 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py
--rw-r--r--   0        0        0      723 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/__init__.py
--rw-r--r--   0        0        0     1181 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx
--rw-r--r--   0        0        0     2412 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py
--rw-r--r--   0        0        0      611 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py
--rw-r--r--   0        0        0     1959 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py
--rw-r--r--   0        0        0     3051 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py
--rw-r--r--   0        0        0     2223 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py
--rw-r--r--   0        0        0     1357 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py
--rw-r--r--   0        0        0     1698 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py
--rw-r--r--   0        0        0     2208 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/targettransformer/__init__.py
--rw-r--r--   0        0        0      630 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/targettransformer/imageinputtransformer.py
--rw-r--r--   0        0        0     1770 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/targettransformer/objdettargettransformer.py
--rw-r--r--   0        0        0     2410 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/targettransformer/semsegtargettransformer.py
--rw-r--r--   0        0        0      649 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/targettransformer/targettransformer.py
--rw-r--r--   0        0        0     1854 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/mlcomponents/targettransformer/targettransformercls.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/py.typed
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/scripts/__init__.py
--rw-r--r--   0        0        0     2031 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/scripts/hydraconfreader.py
--rw-r--r--   0        0        0      745 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/scripts/rundatatests.py
--rw-r--r--   0        0        0     2457 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/scripts/splitdatasetindex.py
--rw-r--r--   0        0        0     1530 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/storages/abs.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/utilities/__init__.py
--rw-r--r--   0        0        0   207256 2023-06-23 12:03:11.116201 niceml-0.5.0/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg
--rw-r--r--   0        0        0   585133 2023-06-23 12:03:11.120200 niceml-0.5.0/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg
--rw-r--r--   0        0        0   292520 2023-06-23 12:03:11.120200 niceml-0.5.0/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg
--rw-r--r--   0        0        0   424191 2023-06-23 12:03:11.120200 niceml-0.5.0/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg
--rw-r--r--   0        0        0    48852 2023-06-23 12:03:11.120200 niceml-0.5.0/niceml/utilities/assets/fonts/DMMono-Regular.ttf
--rw-r--r--   0        0        0    72744 2023-06-23 12:03:11.124201 niceml-0.5.0/niceml/utilities/assets/fonts/Dosis-Regular.ttf
--rw-r--r--   0        0        0    33040 2023-06-23 12:03:11.124201 niceml-0.5.0/niceml/utilities/assets/fonts/Heebo-Regular.ttf
--rw-r--r--   0        0        0    38304 2023-06-23 12:03:11.124201 niceml-0.5.0/niceml/utilities/assets/fonts/Karla-Regular.ttf
--rw-r--r--   0        0        0   129796 2023-06-23 12:03:11.124201 niceml-0.5.0/niceml/utilities/assets/fonts/OpenSans-Regular.ttf
--rw-r--r--   0        0        0    63900 2023-06-23 12:03:11.124201 niceml-0.5.0/niceml/utilities/assets/fonts/Oswald-Regular.ttf
--rw-r--r--   0        0        0    67476 2023-06-23 12:03:11.124201 niceml-0.5.0/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf
--rw-r--r--   0        0        0    86908 2023-06-23 12:03:11.124201 niceml-0.5.0/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0   124236 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/assets/fonts/Rubik-Regular.ttf
--rw-r--r--   0        0        0   299684 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/__init__.py
--rw-r--r--   0        0        0     8325 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/bboxconversion.py
--rw-r--r--   0        0        0     3619 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/bboxdrawing.py
--rw-r--r--   0        0        0     2459 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/bboxencoding.py
--rw-r--r--   0        0        0     3748 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/bboxlabeling.py
--rw-r--r--   0        0        0    10406 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/boundingbox.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/filtering/__init__.py
--rw-r--r--   0        0        0     3515 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/filtering/nmsfilter.py
--rw-r--r--   0        0        0     2978 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/filtering/predictionfilter.py
--rw-r--r--   0        0        0      231 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/filtering/predictionfiltertype.py
--rw-r--r--   0        0        0     1427 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/filtering/thresholdfilter.py
--rw-r--r--   0        0        0     3995 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py
--rw-r--r--   0        0        0     3163 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/chartutils.py
--rw-r--r--   0        0        0     3094 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/checksums.py
--rw-r--r--   0        0        0     2752 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/colorutils.py
--rw-r--r--   0        0        0     3633 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/commonutils.py
--rw-r--r--   0        0        0     3292 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/copyutils.py
--rw-r--r--   0        0        0     1229 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/encoding.py
--rw-r--r--   0        0        0     3846 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/factoryutils.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/filtering/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/filtering/probabilityclassselector.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/fsspec/__init__.py
--rw-r--r--   0        0        0     3020 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/fsspec/locationutils.py
--rw-r--r--   0        0        0     1938 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/gitutils.py
--rw-r--r--   0        0        0     3582 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/hydrautils.py
--rw-r--r--   0        0        0     1716 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/idutils.py
--rw-r--r--   0        0        0    18139 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/imagegeneration.py
--rw-r--r--   0        0        0     2720 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/imageloading.py
--rw-r--r--   0        0        0     4667 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/imagesize.py
--rw-r--r--   0        0        0     4951 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/imageutils.py
--rw-r--r--   0        0        0     3066 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/instancelabeling.py
--rw-r--r--   0        0        0     2256 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/instancelabelmatching.py
--rw-r--r--   0        0        0     5785 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/ioumatrix.py
--rw-r--r--   0        0        0     9836 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/ioutils.py
--rw-r--r--   0        0        0      284 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/logutils.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/masks/__init__.py
--rw-r--r--   0        0        0     1208 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/masks/cymaskdownscale.pyx
--rw-r--r--   0        0        0     1371 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/masks/maskdownscale.py
--rw-r--r--   0        0        0     8463 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/matchingresult.py
--rw-r--r--   0        0        0     2553 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/omegaconfutils.py
--rw-r--r--   0        0        0     2032 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/pytestutils.py
--rw-r--r--   0        0        0     8073 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/readwritelock.py
--rw-r--r--   0        0        0      590 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/regexutils.py
--rw-r--r--   0        0        0        0 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/semseg/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/semseg/semsegdrawing.py
--rw-r--r--   0        0        0     1664 2023-06-23 12:03:11.128201 niceml-0.5.0/niceml/utilities/semseg/semseginstancelabeling.py
--rw-r--r--   0        0        0     1457 2023-06-23 12:03:11.132201 niceml-0.5.0/niceml/utilities/sinusgeneration.py
--rw-r--r--   0        0        0     5710 2023-06-23 12:03:11.132201 niceml-0.5.0/niceml/utilities/splitutils.py
--rw-r--r--   0        0        0     1317 2023-06-23 12:03:11.132201 niceml-0.5.0/niceml/utilities/thumbnailshower.py
--rw-r--r--   0        0        0      472 2023-06-23 12:03:11.132201 niceml-0.5.0/niceml/utilities/timeutils.py
--rw-r--r--   0        0        0     2789 2023-06-23 12:03:11.132201 niceml-0.5.0/niceml/utilities/userselection.py
--rw-r--r--   0        0        0     3677 2023-06-23 12:03:53.704644 niceml-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4398 1970-01-01 00:00:00.000000 niceml-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-10 15:20:35.888509 niceml-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1135 2023-07-10 15:20:35.888509 niceml-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-10 15:21:24.947975 niceml-0.6.0/niceml/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.900509 niceml-0.6.0/niceml/cli/__init__.py
+-rw-r--r--   0        0        0     3070 2023-07-10 15:20:35.900509 niceml-0.6.0/niceml/cli/clicommands.py
+-rw-r--r--   0        0        0      228 2023-07-10 15:20:35.900509 niceml-0.6.0/niceml/cli/climain.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.900509 niceml-0.6.0/niceml/config/__init__.py
+-rw-r--r--   0        0        0     9485 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/config/configschemas.py
+-rw-r--r--   0        0        0      889 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/config/envconfig.py
+-rw-r--r--   0        0        0     5110 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/config/hydra.py
+-rw-r--r--   0        0        0      744 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/config/subsetnames.py
+-rw-r--r--   0        0        0      310 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/config/trainparams.py
+-rw-r--r--   0        0        0      506 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/config/writeopconfig.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/jobs/__init__.py
+-rw-r--r--   0        0        0     3270 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/jobs/jobs.py
+-rw-r--r--   0        0        0      512 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/jobs/repository.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/__init__.py
+-rw-r--r--   0        0        0     2305 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/analysis.py
+-rw-r--r--   0        0        0     2317 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/copyexp.py
+-rw-r--r--   0        0        0     3900 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/cropnumbers.py
+-rw-r--r--   0        0        0      921 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/datageneration.py
+-rw-r--r--   0        0        0     4911 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/dfnormalization.py
+-rw-r--r--   0        0        0     3396 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/evalcopyexp.py
+-rw-r--r--   0        0        0     2058 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/experiment.py
+-rw-r--r--   0        0        0     1176 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/exptests.py
+-rw-r--r--   0        0        0     1281 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/filelockops.py
+-rw-r--r--   0        0        0     4556 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/imagetotable.py
+-rw-r--r--   0        0        0     2220 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/localizeexperiment.py
+-rw-r--r--   0        0        0     6008 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/prediction.py
+-rw-r--r--   0        0        0     3003 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/splitdata.py
+-rw-r--r--   0        0        0     3117 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/ops/train.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/resources/__init__.py
+-rw-r--r--   0        0        0     3668 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dagster/resources/locations.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/__init__.py
+-rw-r--r--   0        0        0     6736 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/binprobvisu.py
+-rw-r--r--   0        0        0     4033 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/cam.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/components/__init__.py
+-rw-r--r--   0        0        0     3870 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/components/downloadexpviscomponent.py
+-rw-r--r--   0        0        0     4603 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/components/expviscomponent.py
+-rw-r--r--   0        0        0     1835 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/components/linearviscomponent.py
+-rw-r--r--   0        0        0     1329 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/components/metaviscomponent.py
+-rw-r--r--   0        0        0     3769 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/components/prefixviscomponent.py
+-rw-r--r--   0        0        0     2892 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/components/selectionviscomponent.py
+-rw-r--r--   0        0        0     1446 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/configviscomponent.py
+-rw-r--r--   0        0        0     3006 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/dashboard.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/expvisuhelper.py
+-rw-r--r--   0        0        0     3126 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/imagenetdataloggerviscomponent.py
+-rw-r--r--   0        0        0     3294 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/metricviscomponent.py
+-rw-r--r--   0        0        0      293 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/netdataloggerviscomponent.py
+-rw-r--r--   0        0        0     5961 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/remotettrainutils.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/visualizers/__init__.py
+-rw-r--r--   0        0        0     3125 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/visualizers/boundingboxvisualizer.py
+-rw-r--r--   0        0        0     4554 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/visualizers/imagevisualizer.py
+-rw-r--r--   0        0        0     3206 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/dashboard/visualizers/maskvisualizer.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/augmentation/__init__.py
+-rw-r--r--   0        0        0      362 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/augmentation/augmentation.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/__init__.py
+-rw-r--r--   0        0        0     2369 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/clsdatadescription.py
+-rw-r--r--   0        0        0      260 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/datadescription.py
+-rw-r--r--   0        0        0     1247 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/inputdatadescriptions.py
+-rw-r--r--   0        0        0     2687 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/objdetdatadescription.py
+-rw-r--r--   0        0        0     5136 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/outputdatadescriptions.py
+-rw-r--r--   0        0        0     2734 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/regdatadescription.py
+-rw-r--r--   0        0        0     2996 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datadescriptions/semsegdatadescritption.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datafilters/__init__.py
+-rw-r--r--   0        0        0     1459 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datafilters/dataframefilter.py
+-rw-r--r--   0        0        0     1374 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datafilters/nandataframefilter.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfolistings/__init__.py
+-rw-r--r--   0        0        0     4942 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfolistings/clsdatainfolisting.py
+-rw-r--r--   0        0        0      493 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfolistings/datainfolisting.py
+-rw-r--r--   0        0        0     3905 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfolistings/objdetdatainfolisting.py
+-rw-r--r--   0        0        0     2585 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfolistings/semsegdatainfolisting.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfos/__init__.py
+-rw-r--r--   0        0        0     2388 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfos/clsdatainfo.py
+-rw-r--r--   0        0        0      458 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfos/datainfo.py
+-rw-r--r--   0        0        0      755 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfos/imagedatainfo.py
+-rw-r--r--   0        0        0     1120 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfos/objdetdatainfo.py
+-rw-r--r--   0        0        0     1112 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datainfos/semsegdatainfo.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataiterators/__init__.py
+-rw-r--r--   0        0        0     2783 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataiterators/boundingboxdataiterator.py
+-rw-r--r--   0        0        0      560 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataiterators/dataiterator.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/__init__.py
+-rw-r--r--   0        0        0     2229 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/cachedimageloader.py
+-rw-r--r--   0        0        0     1094 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/clsdataloader.py
+-rw-r--r--   0        0        0      747 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/dataloader.py
+-rw-r--r--   0        0        0     2934 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/dfloaders.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/factories/__init__.py
+-rw-r--r--   0        0        0      516 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/factories/dfloaderfactory.py
+-rw-r--r--   0        0        0      509 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/factories/imageloaderfactory.py
+-rw-r--r--   0        0        0     1572 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/imageloaders.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/interfaces/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/interfaces/dfloader.py
+-rw-r--r--   0        0        0      753 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/interfaces/imageloader.py
+-rw-r--r--   0        0        0     1137 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/objdetdataloader.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/semseg/__init__.py
+-rw-r--r--   0        0        0     1615 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx
+-rw-r--r--   0        0        0     1938 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/semseg/semsegdataloader.py
+-rw-r--r--   0        0        0      844 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/dataloaders/semseg/transformmaskimage.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datasets/__init__.py
+-rw-r--r--   0        0        0     4453 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datasets/clsclassinfo.py
+-rw-r--r--   0        0        0     1546 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4914 2023-07-10 15:20:35.904509 niceml-0.6.0/niceml/data/datasets/dfdataset.py
+-rw-r--r--   0        0        0     5362 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datasets/genericdataset.py
+-rw-r--r--   0        0        0     1088 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datasets/healthdataset.py
+-rw-r--r--   0        0        0     1147 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datasets/sinusdataset.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datashuffler/__init__.py
+-rw-r--r--   0        0        0      603 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datashuffler/datashuffler.py
+-rw-r--r--   0        0        0      536 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datashuffler/defaultshuffler.py
+-rw-r--r--   0        0        0     2613 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datashuffler/uniformdistributionshuffler.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datastatsgenerator/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datastatsgenerator/datastatsgenerator.py
+-rw-r--r--   0        0        0      472 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/datastatsgenerator/defaultstatsgenerator.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/netdataloggers/__init__.py
+-rw-r--r--   0        0        0     1952 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/netdataloggers/netdatalogger.py
+-rw-r--r--   0        0        0     4732 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/netdataloggers/objdetnetdatalogger.py
+-rw-r--r--   0        0        0     5023 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/netdataloggers/semsegnetdatalogger.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/normalization/__init__.py
+-rw-r--r--   0        0        0     1218 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/normalization/dataframe.py
+-rw-r--r--   0        0        0      193 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/normalization/normalization.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/storages/__init__.py
+-rw-r--r--   0        0        0     3013 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/storages/fsfilesystemstorage.py
+-rw-r--r--   0        0        0     3485 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/storages/fsspecstorage.py
+-rw-r--r--   0        0        0     2306 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/storages/localstorage.py
+-rw-r--r--   0        0        0      898 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/storages/storagehandler.py
+-rw-r--r--   0        0        0      973 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/data/storages/storageinterface.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/__init__.py
+-rw-r--r--   0        0        0     3566 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py
+-rw-r--r--   0        0        0     1662 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py
+-rw-r--r--   0        0        0     4227 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py
+-rw-r--r--   0        0        0      922 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py
+-rw-r--r--   0        0        0      929 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/kerasmetrics.py
+-rw-r--r--   0        0        0     1404 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/kerasmodelloader.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/learners/__init__.py
+-rw-r--r--   0        0        0     2344 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/learners/defaultlearner.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/losses/__init__.py
+-rw-r--r--   0        0        0     1488 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py
+-rw-r--r--   0        0        0     3957 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/losses/objdetlosses.py
+-rw-r--r--   0        0        0     2055 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/losses/semseglosses.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/metrics/__init__.py
+-rw-r--r--   0        0        0     3048 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py
+-rw-r--r--   0        0        0     2212 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/modelcompiler/__init__.py
+-rw-r--r--   0        0        0     2136 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/__init__.py
+-rw-r--r--   0        0        0     3701 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py
+-rw-r--r--   0        0        0     2530 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/layerfactory.py
+-rw-r--r--   0        0        0     1569 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py
+-rw-r--r--   0        0        0     1979 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/mlp.py
+-rw-r--r--   0        0        0     2250 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/mobilenet.py
+-rw-r--r--   0        0        0     1813 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/premodellayers.py
+-rw-r--r--   0        0        0     7749 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/retinanet.py
+-rw-r--r--   0        0        0    11007 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/models/unets.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/optimizers/schedules/__init__.py
+-rw-r--r--   0        0        0     1158 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/__init__.py
+-rw-r--r--   0        0        0     4437 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/confextractionmetafunction.py
+-rw-r--r--   0        0        0     1431 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/expdatalocalstorageloader.py
+-rw-r--r--   0        0        0     3277 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/expdatastorageloader.py
+-rw-r--r--   0        0        0     4447 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimentcontext.py
+-rw-r--r--   0        0        0    14860 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimentdata.py
+-rw-r--r--   0        0        0     2109 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimentdownloader.py
+-rw-r--r--   0        0        0      673 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimenterrors.py
+-rw-r--r--   0        0        0     3122 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimentinfo.py
+-rw-r--r--   0        0        0    12258 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimentmanager.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimenttests/__init__.py
+-rw-r--r--   0        0        0     1790 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimenttests/checkfilesfolderstest.py
+-rw-r--r--   0        0        0      904 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimenttests/exptests.py
+-rw-r--r--   0        0        0     1667 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimenttests/metriccheck.py
+-rw-r--r--   0        0        0     2320 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimenttests/testinitializer.py
+-rw-r--r--   0        0        0     3521 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/experimenttests/validateexps.py
+-rw-r--r--   0        0        0     3007 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/expfilenames.py
+-rw-r--r--   0        0        0     3153 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/expoutinitializer.py
+-rw-r--r--   0        0        0     1199 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/exppathfinder.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/filters/__init__.py
+-rw-r--r--   0        0        0     1922 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/filters/datefilter.py
+-rw-r--r--   0        0        0      547 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/filters/experimentfilter.py
+-rw-r--r--   0        0        0     2142 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/filters/expselectionfilter.py
+-rw-r--r--   0        0        0     1867 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/filters/selectboxfilter.py
+-rw-r--r--   0        0        0     2911 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/filters/sliderfilter.py
+-rw-r--r--   0        0        0     2304 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/loaddatafunctions.py
+-rw-r--r--   0        0        0      828 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/loadexpinfo.py
+-rw-r--r--   0        0        0     6149 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/localexperimentcache.py
+-rw-r--r--   0        0        0     2683 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/metafunctions.py
+-rw-r--r--   0        0        0     1598 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/metainfotables.py
+-rw-r--r--   0        0        0     3300 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/metalists.py
+-rw-r--r--   0        0        0      512 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/metatablefactory.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/__init__.py
+-rw-r--r--   0        0        0      669 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/baseexpschema.py
+-rw-r--r--   0        0        0     2158 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/defaultexpschema.py
+-rw-r--r--   0        0        0      637 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/expdocstring.py
+-rw-r--r--   0        0        0     2533 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/expmember.py
+-rw-r--r--   0        0        0     1431 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/objdetexpschema.py
+-rw-r--r--   0        0        0     1210 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/parquetframeexpmember.py
+-rw-r--r--   0        0        0     1489 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/sampleexpschemas.py
+-rw-r--r--   0        0        0      390 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/schemalist.py
+-rw-r--r--   0        0        0      788 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/schemavalidation.py
+-rw-r--r--   0        0        0     2179 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/experiments/schemas/yamlexpmember.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/filechecksumprocessors/__init__.py
+-rw-r--r--   0        0        0     8697 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/filechecksumprocessors/filechecksumprocessor.py
+-rw-r--r--   0        0        0     7545 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/filechecksumprocessors/zippedcsvtoparqprocessor.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mkdocs/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mkdocs/mdgraph.py
+-rw-r--r--   0        0        0      839 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mkdocs/mdjob.py
+-rw-r--r--   0        0        0     1105 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mkdocs/mdop.py
+-rw-r--r--   0        0        0     1189 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mkdocs/mdtable.py
+-rw-r--r--   0        0        0     1422 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mkdocs/schemadocgeneration.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/callbacks/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/callbacks/callbackinitializer.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/learners/__init__.py
+-rw-r--r--   0        0        0     1125 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/learners/fitgenerators.py
+-rw-r--r--   0        0        0      994 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/learners/learner.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/modelcompiler/__init__.py
+-rw-r--r--   0        0        0      575 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/modelcompiler/modelcompiler.py
+-rw-r--r--   0        0        0      563 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/modelloader/__init__.py
+-rw-r--r--   0        0        0      600 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/modelloader/modelloader.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/models/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/models/modelbundle.py
+-rw-r--r--   0        0        0      476 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/models/modelfactory.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/objdet/__init__.py
+-rw-r--r--   0        0        0     7607 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/objdet/anchorencoding.py
+-rw-r--r--   0        0        0     2905 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/objdet/anchorgenerator.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/predictionhandlers/__init__.py
+-rw-r--r--   0        0        0     1404 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py
+-rw-r--r--   0        0        0     6251 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py
+-rw-r--r--   0        0        0     1383 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/predictionhandlers/predictionhandler.py
+-rw-r--r--   0        0        0    10584 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py
+-rw-r--r--   0        0        0     4896 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py
+-rw-r--r--   0        0        0     2550 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/__init__.py
+-rw-r--r--   0        0        0      836 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/analyzer.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/__init__.py
+-rw-r--r--   0        0        0     4118 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py
+-rw-r--r--   0        0        0     2320 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py
+-rw-r--r--   0        0        0     3806 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py
+-rw-r--r--   0        0        0     3328 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py
+-rw-r--r--   0        0        0      603 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py
+-rw-r--r--   0        0        0     1658 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py
+-rw-r--r--   0        0        0     3007 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py
+-rw-r--r--   0        0        0      723 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx
+-rw-r--r--   0        0        0     2412 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py
+-rw-r--r--   0        0        0      611 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py
+-rw-r--r--   0        0        0     1959 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py
+-rw-r--r--   0        0        0     2999 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py
+-rw-r--r--   0        0        0     2223 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py
+-rw-r--r--   0        0        0     1357 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py
+-rw-r--r--   0        0        0     1698 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py
+-rw-r--r--   0        0        0     2208 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/targettransformer/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/targettransformer/imageinputtransformer.py
+-rw-r--r--   0        0        0     1770 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/targettransformer/objdettargettransformer.py
+-rw-r--r--   0        0        0     2410 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/targettransformer/semsegtargettransformer.py
+-rw-r--r--   0        0        0      649 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/targettransformer/targettransformer.py
+-rw-r--r--   0        0        0     1854 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/mlcomponents/targettransformer/targettransformercls.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/scripts/__init__.py
+-rw-r--r--   0        0        0     2031 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/scripts/hydraconfreader.py
+-rw-r--r--   0        0        0      745 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/scripts/rundatatests.py
+-rw-r--r--   0        0        0     2457 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/scripts/splitdatasetindex.py
+-rw-r--r--   0        0        0     1530 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/storages/abs.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.908509 niceml-0.6.0/niceml/utilities/__init__.py
+-rw-r--r--   0        0        0   207256 2023-07-10 15:20:35.916509 niceml-0.6.0/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg
+-rw-r--r--   0        0        0   585133 2023-07-10 15:20:35.916509 niceml-0.6.0/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg
+-rw-r--r--   0        0        0   292520 2023-07-10 15:20:35.916509 niceml-0.6.0/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg
+-rw-r--r--   0        0        0   424191 2023-07-10 15:20:35.916509 niceml-0.6.0/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg
+-rw-r--r--   0        0        0    48852 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/DMMono-Regular.ttf
+-rw-r--r--   0        0        0    72744 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/Dosis-Regular.ttf
+-rw-r--r--   0        0        0    33040 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/Heebo-Regular.ttf
+-rw-r--r--   0        0        0    38304 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/Karla-Regular.ttf
+-rw-r--r--   0        0        0   129796 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0    63900 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/Oswald-Regular.ttf
+-rw-r--r--   0        0        0    67476 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf
+-rw-r--r--   0        0        0    86908 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0   124236 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/Rubik-Regular.ttf
+-rw-r--r--   0        0        0   299684 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/__init__.py
+-rw-r--r--   0        0        0     8325 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/bboxconversion.py
+-rw-r--r--   0        0        0     3619 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/bboxdrawing.py
+-rw-r--r--   0        0        0     2459 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/bboxencoding.py
+-rw-r--r--   0        0        0     3748 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/bboxlabeling.py
+-rw-r--r--   0        0        0    10406 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/boundingbox.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/filtering/__init__.py
+-rw-r--r--   0        0        0     3515 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/filtering/nmsfilter.py
+-rw-r--r--   0        0        0     2978 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/filtering/predictionfilter.py
+-rw-r--r--   0        0        0      231 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/filtering/predictionfiltertype.py
+-rw-r--r--   0        0        0     1427 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/filtering/thresholdfilter.py
+-rw-r--r--   0        0        0     3995 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py
+-rw-r--r--   0        0        0     3163 2023-07-10 15:20:35.920509 niceml-0.6.0/niceml/utilities/chartutils.py
+-rw-r--r--   0        0        0     3094 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/checksums.py
+-rw-r--r--   0        0        0     2752 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/colorutils.py
+-rw-r--r--   0        0        0     3633 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/commonutils.py
+-rw-r--r--   0        0        0     3292 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/copyutils.py
+-rw-r--r--   0        0        0     1229 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/encoding.py
+-rw-r--r--   0        0        0     3846 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/factoryutils.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/filtering/__init__.py
+-rw-r--r--   0        0        0     2138 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/filtering/probabilityclassselector.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/fsspec/__init__.py
+-rw-r--r--   0        0        0     3020 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/fsspec/locationutils.py
+-rw-r--r--   0        0        0     1938 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/gitutils.py
+-rw-r--r--   0        0        0     3582 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/hydrautils.py
+-rw-r--r--   0        0        0     1716 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/idutils.py
+-rw-r--r--   0        0        0    18139 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/imagegeneration.py
+-rw-r--r--   0        0        0     2720 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/imageloading.py
+-rw-r--r--   0        0        0     4667 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/imagesize.py
+-rw-r--r--   0        0        0     4951 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/imageutils.py
+-rw-r--r--   0        0        0     3066 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/instancelabeling.py
+-rw-r--r--   0        0        0     2256 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/instancelabelmatching.py
+-rw-r--r--   0        0        0     5785 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/ioumatrix.py
+-rw-r--r--   0        0        0    10009 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/ioutils.py
+-rw-r--r--   0        0        0      284 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/logutils.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/masks/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/masks/cymaskdownscale.pyx
+-rw-r--r--   0        0        0     1371 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/masks/maskdownscale.py
+-rw-r--r--   0        0        0     8463 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/matchingresult.py
+-rw-r--r--   0        0        0     2553 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/omegaconfutils.py
+-rw-r--r--   0        0        0     2032 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/pytestutils.py
+-rw-r--r--   0        0        0     8073 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/readwritelock.py
+-rw-r--r--   0        0        0      590 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/regexutils.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/semseg/__init__.py
+-rw-r--r--   0        0        0     1885 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/semseg/semsegdrawing.py
+-rw-r--r--   0        0        0     1664 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/semseg/semseginstancelabeling.py
+-rw-r--r--   0        0        0     1457 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/sinusgeneration.py
+-rw-r--r--   0        0        0     5710 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/splitutils.py
+-rw-r--r--   0        0        0     1317 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/thumbnailshower.py
+-rw-r--r--   0        0        0      472 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/timeutils.py
+-rw-r--r--   0        0        0     2789 2023-07-10 15:20:35.924510 niceml-0.6.0/niceml/utilities/userselection.py
+-rw-r--r--   0        0        0     3669 2023-07-10 15:21:24.991978 niceml-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4398 1970-01-01 00:00:00.000000 niceml-0.6.0/PKG-INFO
```

### Comparing `niceml-0.5.0/LICENSE` & `niceml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/README.md` & `niceml-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/cli/clicommands.py` & `niceml-0.6.0/niceml/cli/clicommands.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/config/configschemas.py` & `niceml-0.6.0/niceml/config/configschemas.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/config/envconfig.py` & `niceml-0.6.0/niceml/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/config/hydra.py` & `niceml-0.6.0/niceml/config/hydra.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,43 +30,46 @@
 ) -> Dict[str, Any]:
     """Add searchpaths to config under hydra/searchpath."""
     config_hydra = config.get("hydra", {})
     config_hydra_searchpaths = list(searchpaths) + config_hydra.get("searchpath", [])
     return {**config, "hydra": {**config_hydra, "searchpath": config_hydra_searchpaths}}
 
 
-@config_mapping
-def hydra_conf_mapping(config: Dict[str, Any]):
-    """Load hydra configuration from ``config``.
+def hydra_conf_mapping_factory(drop: Iterable[str] = ("globals",)):
+    """
+    Load hydra configuration from ``config``.
 
     Args:
-       config: Configuration to be processed with hydra.
-       drop: Keys to remove from the processed configuration after processing
-             with hydra. Useful to define configuration variables that shall be used
-             for interpolation during processing but not enter the processed
-             configuration. Default: ``("globals",)``.
+        config: Configuration to be processed with hydra.
+        drop: Keys to remove from the processed configuration after processing
+               with hydra. Useful to define configuration variables that shall be used
+               for interpolation during processing but not enter the processed
+               configuration. Default: ``("globals",)``.
     """
-    drop: Iterable[str] = ("globals",)
-    register_niceml_resolvers()
-    config = json.loads(json.dumps(config))
-    config_dir = TemporaryDirectory()  # pylint: disable=consider-using-with
-    new_search_paths = [f"file://{config_dir}"]
-    config_with_searchpath = prepend_hydra_search_paths(config, new_search_paths)
-    _, config_file = mkstemp(suffix=".yaml", dir=config_dir.name, text=True)
-    with open(config_file, "wt", encoding="utf-8") as file:
-        yaml.dump(config_with_searchpath, file, Dumper=yaml.SafeDumper)
-
-    conf = load_hydra_conf(config_file)
-    try:
-        config_dir.cleanup()
-    except (PermissionError, NotADirectoryError):
-        pass
 
-    conf = {key: value for key, value in conf.items() if key not in set(drop)}
-    return conf
+    @config_mapping
+    def hydra_conf_mapping(config: Dict[str, Any]):
+        register_niceml_resolvers()
+        config = json.loads(json.dumps(config))
+        config_dir = TemporaryDirectory()  # pylint: disable=consider-using-with
+
+        _, config_file = mkstemp(suffix=".yaml", dir=config_dir.name, text=True)
+        with open(config_file, "wt", encoding="utf-8") as file:
+            yaml.dump(config, file, Dumper=yaml.SafeDumper)
+
+        conf = load_hydra_conf(config_file)
+        try:
+            config_dir.cleanup()
+        except (PermissionError, NotADirectoryError):
+            pass
+
+        conf = {key: value for key, value in conf.items() if key not in set(drop)}
+        return conf
+
+    return hydra_conf_mapping
 
 
 class HydraInitField(Field):
     """Used to configure Dagster Ops"""
 
     def __init__(
         self,
@@ -74,19 +77,21 @@
         description: Optional[str] = None,
         default_value: Optional[dict] = None,
         example_value: Optional[dict] = None,
         **kwargs,
     ):
         """
         Used to configure Dagster Ops with a target class
-        :param target_class: class which is instantiated from the op
-        :param description: description of the class or field
-        :param default_value: default value of the field when nothing is provided
-        :param example_value: example value of the field shown in the documentation
-        :param kwargs: additional kwargs passed to the Field class
+
+        Args:
+            target_class: class which is instantiated from the op
+            description: description of the class or field
+            default_value: default value of the field when nothing is provided
+            example_value: example value of the field shown in the documentation
+            **kwargs: additional kwargs passed to the Field class
         """
         if description is None:
             description = target_class.__doc__
         if default_value is None:
             default_value = dict()
         if example_value is None:
             impl_str: str = "implementation_of_" if isabstract(target_class) else ""
@@ -107,19 +112,21 @@
         description: Optional[str] = None,
         default_value: Optional[dict] = None,
         example_value: Optional[dict] = None,
         **kwargs,
     ):
         """
         Used to configure Dagster Ops with a map
-        :param target_class: class which is instantiated from the op in the map
-        :param description: description of the class or field
-        :param default_value: default value of the field when nothing is provided
-        :param example_value: example value of the field shown in the documentation
-        :param kwargs: additional kwargs passed to the Field class
+
+        Args:
+            target_class: class which is instantiated from the op in the map
+            description: description of the class or field
+            default_value: default value of the field when nothing is provided
+            example_value: example value of the field shown in the documentation
+            **kwargs: additional kwargs passed to the Field class
         """
         if description is None:
             description = target_class.__doc__
         if default_value is None:
             default_value = dict()
         if example_value is None:
             impl_str: str = "implementation_of_" if isabstract(target_class) else ""
```

### Comparing `niceml-0.5.0/niceml/config/subsetnames.py` & `niceml-0.6.0/niceml/config/subsetnames.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/jobs/jobs.py` & `niceml-0.6.0/niceml/dagster/jobs/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module containing all dagster jobs"""
-from niceml.config.hydra import hydra_conf_mapping
+from niceml.config.hydra import hydra_conf_mapping_factory
 from niceml.dagster.ops.analysis import analysis
 from niceml.dagster.ops.copyexp import copy_exp
 from niceml.dagster.ops.cropnumbers import crop_numbers
 from niceml.dagster.ops.datageneration import data_generation
 from niceml.dagster.ops.evalcopyexp import eval_copy_exp
 from niceml.dagster.ops.experiment import experiment
 from niceml.dagster.ops.exptests import exptests
@@ -13,25 +13,25 @@
 from niceml.dagster.ops.prediction import prediction
 from niceml.dagster.ops.splitdata import split_data
 from niceml.dagster.ops.train import train
 from niceml.dagster.resources.locations import locations_resource
 from dagster import job
 
 
-@job(config=hydra_conf_mapping)
+@job(config=hydra_conf_mapping_factory())
 def job_data_generation():
     """Job for data generation"""
 
     output_loc = data_generation()  # pylint: disable=no-value-for-parameter
     output_loc = split_data(output_loc)  # pylint: disable=no-value-for-parameter
     output_loc = crop_numbers(output_loc)  # pylint: disable=no-value-for-parameter
     image_to_tabular_data(output_loc)
 
 
-@job(config=hydra_conf_mapping)
+@job(config=hydra_conf_mapping_factory())
 def job_train():
     """Job for training an experiment"""
     filelock_dict = acquire_locks()  # pylint: disable=no-value-for-parameter
     exp_context = experiment()  # pylint: disable=no-value-for-parameter
     exp_context, filelock_dict = train(
         exp_context, filelock_dict
     )  # pylint: disable=no-value-for-parameter
@@ -41,15 +41,15 @@
     exp_context, filelock_dict = analysis(
         exp_context, filelock_dict
     )  # pylint: disable=no-value-for-parameter
     release_locks(filelock_dict)  # pylint: disable=no-value-for-parameter
     exptests(exp_context)  # pylint: disable=no-value-for-parameter
 
 
-@job(config=hydra_conf_mapping)
+@job(config=hydra_conf_mapping_factory())
 def job_eval():
     """Job for evaluating experiment"""
     filelock_dict = acquire_locks()  # pylint: disable=no-value-for-parameter
     exp_context = localize_experiment()  # pylint: disable=no-value-for-parameter
     exp_context = eval_copy_exp(exp_context)  # pylint: disable=no-value-for-parameter
     exp_context, filelock_dict = prediction(
         exp_context, filelock_dict
@@ -58,23 +58,23 @@
         exp_context, filelock_dict
     )  # pylint: disable=no-value-for-parameter
     release_locks(filelock_dict)  # pylint: disable=no-value-for-parameter
     exptests(exp_context)  # pylint: disable=no-value-for-parameter
 
 
 @job(
-    config=hydra_conf_mapping,
+    config=hydra_conf_mapping_factory(),
     resource_defs={
         "locations": locations_resource,
     },
 )
 def job_copy_exp():
     """Copy an experiment from one location to another"""
     copy_exp()  # pylint: disable=no-value-for-parameter
 
 
 @job(
-    config=hydra_conf_mapping,
+    config=hydra_conf_mapping_factory(),
 )
 def job_clearlocks():
     """Clear locks from given lock entries"""
     clear_locks()  # pylint: disable=no-value-for-parameter
```

### Comparing `niceml-0.5.0/niceml/dagster/jobs/repository.py` & `niceml-0.6.0/niceml/dagster/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/analysis.py` & `niceml-0.6.0/niceml/dagster/ops/analysis.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/copyexp.py` & `niceml-0.6.0/niceml/dagster/ops/copyexp.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/cropnumbers.py` & `niceml-0.6.0/niceml/dagster/ops/cropnumbers.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/datageneration.py` & `niceml-0.6.0/niceml/dagster/ops/datageneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/evalcopyexp.py` & `niceml-0.6.0/niceml/dagster/ops/evalcopyexp.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/experiment.py` & `niceml-0.6.0/niceml/dagster/ops/experiment.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/exptests.py` & `niceml-0.6.0/niceml/dagster/ops/exptests.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/filelockops.py` & `niceml-0.6.0/niceml/dagster/ops/filelockops.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/imagetotable.py` & `niceml-0.6.0/niceml/dagster/ops/imagetotable.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/localizeexperiment.py` & `niceml-0.6.0/niceml/dagster/ops/localizeexperiment.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/prediction.py` & `niceml-0.6.0/niceml/dagster/ops/prediction.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/splitdata.py` & `niceml-0.6.0/niceml/dagster/ops/splitdata.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/ops/train.py` & `niceml-0.6.0/niceml/dagster/ops/train.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dagster/resources/locations.py` & `niceml-0.6.0/niceml/dagster/resources/locations.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/binprobvisu.py` & `niceml-0.6.0/niceml/dashboard/binprobvisu.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/cam.py` & `niceml-0.6.0/niceml/dashboard/cam.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/components/downloadexpviscomponent.py` & `niceml-0.6.0/niceml/dashboard/components/downloadexpviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/components/expviscomponent.py` & `niceml-0.6.0/niceml/dashboard/components/expviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/components/linearviscomponent.py` & `niceml-0.6.0/niceml/dashboard/components/linearviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/components/metaviscomponent.py` & `niceml-0.6.0/niceml/dashboard/components/metaviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/components/prefixviscomponent.py` & `niceml-0.6.0/niceml/dashboard/components/prefixviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/components/selectionviscomponent.py` & `niceml-0.6.0/niceml/dashboard/components/selectionviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/configviscomponent.py` & `niceml-0.6.0/niceml/dashboard/configviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/dashboard.py` & `niceml-0.6.0/niceml/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/imagenetdataloggerviscomponent.py` & `niceml-0.6.0/niceml/dashboard/imagenetdataloggerviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/metricviscomponent.py` & `niceml-0.6.0/niceml/dashboard/metricviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/remotettrainutils.py` & `niceml-0.6.0/niceml/dashboard/remotettrainutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/visualizers/boundingboxvisualizer.py` & `niceml-0.6.0/niceml/dashboard/visualizers/boundingboxvisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/visualizers/imagevisualizer.py` & `niceml-0.6.0/niceml/dashboard/visualizers/imagevisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dashboard/visualizers/maskvisualizer.py` & `niceml-0.6.0/niceml/dashboard/visualizers/maskvisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datadescriptions/clsdatadescription.py` & `niceml-0.6.0/niceml/data/datadescriptions/clsdatadescription.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datadescriptions/inputdatadescriptions.py` & `niceml-0.6.0/niceml/data/datadescriptions/inputdatadescriptions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datadescriptions/objdetdatadescription.py` & `niceml-0.6.0/niceml/data/datadescriptions/objdetdatadescription.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datadescriptions/outputdatadescriptions.py` & `niceml-0.6.0/niceml/data/datadescriptions/outputdatadescriptions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datadescriptions/regdatadescription.py` & `niceml-0.6.0/niceml/data/datadescriptions/regdatadescription.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datadescriptions/semsegdatadescritption.py` & `niceml-0.6.0/niceml/data/datadescriptions/semsegdatadescritption.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datainfolistings/clsdatainfolisting.py` & `niceml-0.6.0/niceml/data/datainfolistings/clsdatainfolisting.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datainfolistings/objdetdatainfolisting.py` & `niceml-0.6.0/niceml/data/datainfolistings/objdetdatainfolisting.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datainfolistings/semsegdatainfolisting.py` & `niceml-0.6.0/niceml/data/datainfolistings/semsegdatainfolisting.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datainfos/clsdatainfo.py` & `niceml-0.6.0/niceml/data/datainfos/clsdatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datainfos/imagedatainfo.py` & `niceml-0.6.0/niceml/data/datainfos/imagedatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datainfos/objdetdatainfo.py` & `niceml-0.6.0/niceml/data/datainfos/objdetdatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datainfos/semsegdatainfo.py` & `niceml-0.6.0/niceml/data/datainfos/semsegdatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataiterators/boundingboxdataiterator.py` & `niceml-0.6.0/niceml/data/dataiterators/boundingboxdataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataiterators/dataiterator.py` & `niceml-0.6.0/niceml/data/dataiterators/dataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/cachedimageloader.py` & `niceml-0.6.0/niceml/data/dataloaders/cachedimageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/clsdataloader.py` & `niceml-0.6.0/niceml/data/dataloaders/clsdataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/dataloader.py` & `niceml-0.6.0/niceml/data/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/dfloaders.py` & `niceml-0.6.0/niceml/data/dataloaders/dfloaders.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/factories/dfloaderfactory.py` & `niceml-0.6.0/niceml/data/dataloaders/factories/dfloaderfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/imageloaders.py` & `niceml-0.6.0/niceml/data/dataloaders/imageloaders.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/interfaces/imageloader.py` & `niceml-0.6.0/niceml/data/dataloaders/interfaces/imageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/objdetdataloader.py` & `niceml-0.6.0/niceml/data/dataloaders/objdetdataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx` & `niceml-0.6.0/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/semseg/semsegdataloader.py` & `niceml-0.6.0/niceml/data/dataloaders/semseg/semsegdataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/dataloaders/semseg/transformmaskimage.py` & `niceml-0.6.0/niceml/data/dataloaders/semseg/transformmaskimage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datasets/clsclassinfo.py` & `niceml-0.6.0/niceml/data/datasets/clsclassinfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datasets/dataset.py` & `niceml-0.6.0/niceml/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datasets/dfdataset.py` & `niceml-0.6.0/niceml/data/datasets/dfdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datasets/genericdataset.py` & `niceml-0.6.0/niceml/data/datasets/genericdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datasets/healthdataset.py` & `niceml-0.6.0/niceml/data/datasets/healthdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datasets/sinusdataset.py` & `niceml-0.6.0/niceml/data/datasets/sinusdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datashuffler/datashuffler.py` & `niceml-0.6.0/niceml/data/datashuffler/datashuffler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datashuffler/defaultshuffler.py` & `niceml-0.6.0/niceml/data/datashuffler/defaultshuffler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/datashuffler/uniformdistributionshuffler.py` & `niceml-0.6.0/niceml/data/datashuffler/uniformdistributionshuffler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/netdataloggers/netdatalogger.py` & `niceml-0.6.0/niceml/data/netdataloggers/netdatalogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/netdataloggers/objdetnetdatalogger.py` & `niceml-0.6.0/niceml/data/netdataloggers/objdetnetdatalogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/netdataloggers/semsegnetdatalogger.py` & `niceml-0.6.0/niceml/data/netdataloggers/semsegnetdatalogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/storages/fsfilesystemstorage.py` & `niceml-0.6.0/niceml/data/storages/fsfilesystemstorage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/storages/fsspecstorage.py` & `niceml-0.6.0/niceml/data/storages/fsspecstorage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/storages/localstorage.py` & `niceml-0.6.0/niceml/data/storages/localstorage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/storages/storagehandler.py` & `niceml-0.6.0/niceml/data/storages/storagehandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/data/storages/storageinterface.py` & `niceml-0.6.0/niceml/data/storages/storageinterface.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/kerasmetrics.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/kerasmetrics.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/kerasmodelloader.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/kerasmodelloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/learners/defaultlearner.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/learners/defaultlearner.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/losses/objdetlosses.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/losses/objdetlosses.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/losses/semseglosses.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/losses/semseglosses.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/layerfactory.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/layerfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/mlp.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/mlp.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/mobilenet.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/premodellayers.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/premodellayers.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/retinanet.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/retinanet.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/models/unets.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/models/unets.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py` & `niceml-0.6.0/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/confextractionmetafunction.py` & `niceml-0.6.0/niceml/experiments/confextractionmetafunction.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/expdatalocalstorageloader.py` & `niceml-0.6.0/niceml/experiments/expdatalocalstorageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/expdatastorageloader.py` & `niceml-0.6.0/niceml/experiments/expdatastorageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimentcontext.py` & `niceml-0.6.0/niceml/experiments/experimentcontext.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimentdata.py` & `niceml-0.6.0/niceml/experiments/experimentdata.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimentdownloader.py` & `niceml-0.6.0/niceml/experiments/experimentdownloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimenterrors.py` & `niceml-0.6.0/niceml/experiments/experimenterrors.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimentinfo.py` & `niceml-0.6.0/niceml/experiments/experimentinfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimentmanager.py` & `niceml-0.6.0/niceml/experiments/experimentmanager.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimenttests/checkfilesfolderstest.py` & `niceml-0.6.0/niceml/experiments/experimenttests/checkfilesfolderstest.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimenttests/exptests.py` & `niceml-0.6.0/niceml/experiments/experimenttests/exptests.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimenttests/metriccheck.py` & `niceml-0.6.0/niceml/experiments/experimenttests/metriccheck.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimenttests/testinitializer.py` & `niceml-0.6.0/niceml/experiments/experimenttests/testinitializer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/experimenttests/validateexps.py` & `niceml-0.6.0/niceml/experiments/experimenttests/validateexps.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/expfilenames.py` & `niceml-0.6.0/niceml/experiments/expfilenames.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/expoutinitializer.py` & `niceml-0.6.0/niceml/experiments/expoutinitializer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/exppathfinder.py` & `niceml-0.6.0/niceml/experiments/exppathfinder.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/filters/datefilter.py` & `niceml-0.6.0/niceml/experiments/filters/datefilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/filters/experimentfilter.py` & `niceml-0.6.0/niceml/experiments/filters/experimentfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/filters/expselectionfilter.py` & `niceml-0.6.0/niceml/experiments/filters/expselectionfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/filters/selectboxfilter.py` & `niceml-0.6.0/niceml/experiments/filters/selectboxfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/filters/sliderfilter.py` & `niceml-0.6.0/niceml/experiments/filters/sliderfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/loaddatafunctions.py` & `niceml-0.6.0/niceml/experiments/loaddatafunctions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/loadexpinfo.py` & `niceml-0.6.0/niceml/experiments/loadexpinfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/localexperimentcache.py` & `niceml-0.6.0/niceml/experiments/localexperimentcache.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/metafunctions.py` & `niceml-0.6.0/niceml/experiments/metafunctions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/metainfotables.py` & `niceml-0.6.0/niceml/experiments/metainfotables.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/metalists.py` & `niceml-0.6.0/niceml/experiments/metalists.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/metatablefactory.py` & `niceml-0.6.0/niceml/experiments/metatablefactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/schemas/baseexpschema.py` & `niceml-0.6.0/niceml/experiments/schemas/baseexpschema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Module containing the base experiment scheme"""
+"""Module containing the base experiment schema"""
 from niceml.experiments.expfilenames import ExperimentFilenames
 from niceml.experiments.schemas.expmember import FolderMember, LogCsvMember
 from niceml.experiments.schemas.yamlexpmember import ExpInfoMember
 
 
 class BaseExperimentSchema:  # pylint: disable=too-few-public-methods
-    """base experiment scheme for subclassing"""
+    """base experiment schema for subclassing"""
 
     exp_info = ExpInfoMember()
     log_data = LogCsvMember()
     model_folder = FolderMember(
         ExperimentFilenames.MODELS_FOLDER,
         required=True,
         min_required_files=1,
```

### Comparing `niceml-0.5.0/niceml/experiments/schemas/expdocstring.py` & `niceml-0.6.0/niceml/experiments/schemas/expdocstring.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/schemas/expmember.py` & `niceml-0.6.0/niceml/experiments/schemas/expmember.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/schemas/objdetexpschema.py` & `niceml-0.6.0/niceml/experiments/schemas/objdetexpschema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for object detection experiment schema"""
 import pandera as pa
 
-from niceml.experiments.schemas.baseexpschema import BaseExperimentSchema
+from niceml.experiments.schemas.defaultexpschema import DefaultExperimentSchema
 from niceml.experiments.schemas.parquetframeexpmember import ParquetMember
 
 obj_det_df_schema = pa.DataFrameSchema(
     {
         "image_location": pa.Column(pa.String),
         "detection_index": pa.Column(pa.Int),
         "x_pos": pa.Column(pa.Float),
@@ -13,15 +13,17 @@
         "width": pa.Column(pa.Float),
         "height": pa.Column(pa.Float),
         "pred_0000": pa.Column(pa.Float, checks=pa.Check.in_range(-1.0, 1.0)),
     }
 )
 
 
-class ObjDetExpSchema(BaseExperimentSchema):  # pylint: disable=too-few-public-methods
+class ObjDetExpSchema(
+    DefaultExperimentSchema
+):  # pylint: disable=too-few-public-methods
     """This is the experiment for object detection"""
 
     test_parq = ParquetMember(
         path="predictions/test.parq",
         description="Here the predictions of the objdet testset are stored.",
         required=True,
         df_schema=obj_det_df_schema,
```

### Comparing `niceml-0.5.0/niceml/experiments/schemas/parquetframeexpmember.py` & `niceml-0.6.0/niceml/experiments/schemas/parquetframeexpmember.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/schemas/sampleexpschemas.py` & `niceml-0.6.0/niceml/experiments/schemas/sampleexpschemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Module containing classes which describe the sample experiments"""
 import pandera as pa
 
-from niceml.experiments.schemas.baseexpschema import BaseExperimentSchema
+from niceml.experiments.schemas.defaultexpschema import DefaultExperimentSchema
 from niceml.experiments.schemas.parquetframeexpmember import ParquetMember
 
 sin_reg_df_schema = pa.DataFrameSchema(
     {
         "dataid": pa.Column(pa.Float, checks=pa.Check.in_range(0.0, 20.0)),
         "xs": pa.Column(pa.Float, checks=pa.Check.in_range(0.0, 20.0)),
         "ys": pa.Column(pa.Float, checks=pa.Check.in_range(-1.0, 1.0)),
         "pred_0000": pa.Column(pa.Float32, checks=pa.Check.in_range(-1.0, 1.0)),
     }
 )
 
 
-class SinRegExpSchema(BaseExperimentSchema):  # pylint: disable=too-few-public-methods
+class SinRegExpSchema(
+    DefaultExperimentSchema
+):  # pylint: disable=too-few-public-methods
     """This is the experiment for regression"""
 
     test_parq = ParquetMember(
         path="predictions/test.parq",
         description="Here the predictions of the sinus testset are stored.",
         required=True,
         df_schema=sin_reg_df_schema,
```

### Comparing `niceml-0.5.0/niceml/experiments/schemas/schemavalidation.py` & `niceml-0.6.0/niceml/experiments/schemas/schemavalidation.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/experiments/schemas/yamlexpmember.py` & `niceml-0.6.0/niceml/experiments/schemas/yamlexpmember.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/filechecksumprocessors/filechecksumprocessor.py` & `niceml-0.6.0/niceml/filechecksumprocessors/filechecksumprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     # ruff: noqa: PLR0913
     def __init__(
         self,
         input_location: Union[dict, LocationConfig],
         output_location: Union[dict, LocationConfig],
         lockfile_location: Union[dict, LocationConfig],
+        lock_file_name: str = "lock.yaml",
         debug: bool = False,
         process_count: int = 8,
         batch_size: int = 16,
     ):
         """
         FileChecksumProcessor that can be used as part of a pipeline to process
         files based on the checksum.
@@ -37,28 +38,29 @@
             input_location: Input location of the Processor
             output_location: Output location of the Processor
             lockfile_location: Location of the checksum lockfile
             debug: Flag to activate the debug mode
             process_count: Amount of processes for parallel execution
             batch_size: Size of a batch
         """
+        self.lock_file_name = lock_file_name
         self.input_location = input_location
         self.output_location = output_location
         self.lockfile_location = lockfile_location
         self.debug = debug
         self.process_count = process_count
         self.lock_data: Dict[str, dict] = defaultdict(dict)
         self.batch_size = batch_size
 
     def load_checksums(self) -> Dict[str, Dict[str, str]]:
         """Loads checksums from lockfile"""
         with open_location(self.lockfile_location) as (lockfile_fs, lockfile_path):
             try:
                 checksum_dict = read_yaml(
-                    join_fs_path(lockfile_fs, lockfile_path, "lock.yaml"),
+                    join_fs_path(lockfile_fs, lockfile_path, self.lock_file_name),
                     file_system=lockfile_fs,
                 )
             except FileNotFoundError:
                 checksum_dict = defaultdict(dict)
         return checksum_dict
 
     @abstractmethod
@@ -145,15 +147,15 @@
             if (index % 10 == 0) or (len(processing_list) == (index + 1)):
                 with open_location(self.lockfile_location) as (
                     lockfile_fs,
                     lockfile_root,
                 ):
                     write_yaml(
                         dict(self.lock_data),
-                        join_fs_path(lockfile_fs, lockfile_root, "lock.yaml"),
+                        join_fs_path(lockfile_fs, lockfile_root, self.lock_file_name),
                         file_system=lockfile_fs,
                     )
 
         if self.debug:
             for idx, batch in enumerate(processing_list):
                 process_result = self.process(batch)
                 _process_result(process_result, idx)
```

### Comparing `niceml-0.5.0/niceml/filechecksumprocessors/zippedcsvtoparqprocessor.py` & `niceml-0.6.0/niceml/filechecksumprocessors/zippedcsvtoparqprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     # ruff: noqa: PLR0913
     def __init__(
         self,
         input_location: Union[dict, LocationConfig],
         output_location: Union[dict, LocationConfig],
         lockfile_location: Union[dict, LocationConfig],
+        lock_file_name: str = "lock.yaml",
         debug: bool = False,
         process_count: int = 8,
         batch_size: int = 16,
         csv_seperator: str = ";",
         clear: bool = False,
         recursive: bool = False,
     ):
@@ -49,20 +50,21 @@
             batch_size: Size of a batch
             csv_seperator: Seperator character for the csv files.
             clear: Flag to clear the output location when initialize the Processor
             recursive: Flag indicating whether the input location should be
                         searched for files recursively
         """
         super().__init__(
-            input_location,
-            output_location,
-            lockfile_location,
-            debug,
-            process_count,
-            batch_size,
+            input_location=input_location,
+            output_location=output_location,
+            lockfile_location=lockfile_location,
+            debug=debug,
+            process_count=process_count,
+            batch_size=batch_size,
+            lock_file_name=lock_file_name,
         )
         self.recursive = recursive
         self.clear = clear
         self.csv_seperator = csv_seperator
 
         if self.clear:
             clear_folder(self.output_location)
@@ -77,31 +79,31 @@
             A tuple of two lists
         """
         with open_location(self.input_location) as (input_fs, input_path):
             input_files = list_dir(
                 path=input_path,
                 recursive=self.recursive,
                 file_system=input_fs,
+                filter_ext=[".zip"],
             )
             input_files = [
                 join_fs_path(input_fs, input_path, input_file)
                 for input_file in input_files
-                if splitext(input_file)[1] == ".zip"
             ]
         with open_location(self.output_location) as (output_fs, output_path):
             output_fs.makedirs(output_path, exist_ok=True)
             output_files = list_dir(
                 path=output_path,
                 recursive=self.recursive,
                 file_system=output_fs,
+                filter_ext=[".parq"],
             )
             output_files = [
                 join_fs_path(output_fs, output_path, output_file)
                 for output_file in output_files
-                if splitext(output_file)[1] == ".parq"
             ]
 
         return input_files, output_files
 
     def generate_batches(
         self,
         input_file_list: List[str],
```

### Comparing `niceml-0.5.0/niceml/mkdocs/mdgraph.py` & `niceml-0.6.0/niceml/mkdocs/mdgraph.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mkdocs/mdjob.py` & `niceml-0.6.0/niceml/mkdocs/mdjob.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mkdocs/mdop.py` & `niceml-0.6.0/niceml/mkdocs/mdop.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mkdocs/mdtable.py` & `niceml-0.6.0/niceml/mkdocs/mdtable.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mkdocs/schemadocgeneration.py` & `niceml-0.6.0/niceml/mkdocs/schemadocgeneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/callbacks/callbackinitializer.py` & `niceml-0.6.0/niceml/mlcomponents/callbacks/callbackinitializer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/learners/fitgenerators.py` & `niceml-0.6.0/niceml/mlcomponents/learners/fitgenerators.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/learners/learner.py` & `niceml-0.6.0/niceml/mlcomponents/learners/learner.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/modelcompiler/modelcompiler.py` & `niceml-0.6.0/niceml/mlcomponents/modelcompiler/modelcompiler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py` & `niceml-0.6.0/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/modelloader/modelloader.py` & `niceml-0.6.0/niceml/mlcomponents/modelloader/modelloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/objdet/anchorencoding.py` & `niceml-0.6.0/niceml/mlcomponents/objdet/anchorencoding.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/objdet/anchorgenerator.py` & `niceml-0.6.0/niceml/mlcomponents/objdet/anchorgenerator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py` & `niceml-0.6.0/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py` & `niceml-0.6.0/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/predictionhandlers/predictionhandler.py` & `niceml-0.6.0/niceml/mlcomponents/predictionhandlers/predictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py` & `niceml-0.6.0/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py` & `niceml-0.6.0/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py` & `niceml-0.6.0/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/analyzer.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 """Module for tensorgraphanalyzer"""
-import logging
-from os.path import basename, join
+from os.path import join
 from typing import List
 
 from niceml.data.datasets.dataset import Dataset
 from niceml.experiments.experimentcontext import ExperimentContext
 from niceml.experiments.expfilenames import ExperimentFilenames
 from niceml.mlcomponents.resultanalyzers.analyzer import ResultAnalyzer
 from niceml.mlcomponents.resultanalyzers.tensors.tensordataiterators import (
     TensordataIterator,
 )
 from niceml.mlcomponents.resultanalyzers.tensors.tensormetric import TensorMetric
 from niceml.utilities.fsspec.locationutils import open_location
-from niceml.utilities.logutils import get_logstr_from_dict
 
 
 class TensorGraphAnalyzer(ResultAnalyzer):
     """Resultanalyzer for analyzing datapoints seperately. Results
     from a previous applied TensorMetric are accessible in the following
     TensorMetrics. For access the `key` attribute is used in each tensormetric."""
 
     def __init__(
         self,
         metrics: List[TensorMetric],
         dataiterator: TensordataIterator,
         zarr_file_prefix: str = "",
     ):
+        """Initializes the TensorGraphAnalyzer"""
         super().__init__()
         self.zarr_file_prefix = zarr_file_prefix
         self.df_metrics: List[TensorMetric] = metrics
         self.dataiterator: TensordataIterator = dataiterator
 
     def __call__(
         self, dataset: Dataset, exp_context: ExperimentContext, dataset_name: str
     ):  # pylint: disable=too-many-locals
+        """Analyzes the dataset with the given metrics"""
         with open_location(exp_context.fs_config) as (exp_fs, exp_root):
             input_file: str = join(
                 exp_root,
                 ExperimentFilenames.PREDICTION_FOLDER,
                 f"{self.zarr_file_prefix}{dataset_name}",
             )
             self.dataiterator.open(input_file, file_system=exp_fs)
 
-        output_filename = f"result_{dataset_name}.yaml"
-
         cur_metric: TensorMetric
         for cur_metric in self.df_metrics:
             cur_metric.initialize(
                 data_description=self.data_description,
                 exp_context=exp_context,
                 dataset_name=dataset_name,
             )
@@ -66,13 +64,12 @@
 
         out_dict = {}
         for cur_met in self.df_metrics:
             final_metric = cur_met.get_final_metric()
             if final_metric is not None:
                 out_dict.update(final_metric)
 
-        log_str = f"{basename(output_filename)}\n" f"========================\n"
-
-        log_str += get_logstr_from_dict(out_dict)
-        logging.getLogger(__name__).info(log_str)
-
-        exp_context.write_yaml(out_dict, output_filename)
+        output_file = join(
+            ExperimentFilenames.ANALYSIS_FOLDER,
+            ExperimentFilenames.ANALYSIS_FILE.format(dataset_name=dataset_name),
+        )
+        exp_context.write_yaml(out_dict, output_file)
```

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py` & `niceml-0.6.0/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/targettransformer/imageinputtransformer.py` & `niceml-0.6.0/niceml/mlcomponents/targettransformer/imageinputtransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/targettransformer/objdettargettransformer.py` & `niceml-0.6.0/niceml/mlcomponents/targettransformer/objdettargettransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/targettransformer/semsegtargettransformer.py` & `niceml-0.6.0/niceml/mlcomponents/targettransformer/semsegtargettransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/targettransformer/targettransformer.py` & `niceml-0.6.0/niceml/mlcomponents/targettransformer/targettransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/mlcomponents/targettransformer/targettransformercls.py` & `niceml-0.6.0/niceml/mlcomponents/targettransformer/targettransformercls.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/scripts/hydraconfreader.py` & `niceml-0.6.0/niceml/scripts/hydraconfreader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/scripts/rundatatests.py` & `niceml-0.6.0/niceml/scripts/rundatatests.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/scripts/splitdatasetindex.py` & `niceml-0.6.0/niceml/scripts/splitdatasetindex.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/storages/abs.py` & `niceml-0.6.0/niceml/storages/abs.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg` & `niceml-0.6.0/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg` & `niceml-0.6.0/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg` & `niceml-0.6.0/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg` & `niceml-0.6.0/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/DMMono-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/DMMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/Dosis-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/Dosis-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/Heebo-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/Heebo-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/Karla-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/OpenSans-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/Oswald-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/Rubik-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/Rubik-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf` & `niceml-0.6.0/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/bboxconversion.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/bboxconversion.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/bboxdrawing.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/bboxdrawing.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/bboxencoding.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/bboxencoding.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/bboxlabeling.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/bboxlabeling.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/boundingbox.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/boundingbox.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/filtering/nmsfilter.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/filtering/nmsfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/filtering/predictionfilter.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/filtering/predictionfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/filtering/thresholdfilter.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/filtering/thresholdfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py` & `niceml-0.6.0/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/chartutils.py` & `niceml-0.6.0/niceml/utilities/chartutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/checksums.py` & `niceml-0.6.0/niceml/utilities/checksums.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/colorutils.py` & `niceml-0.6.0/niceml/utilities/colorutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/commonutils.py` & `niceml-0.6.0/niceml/utilities/commonutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/copyutils.py` & `niceml-0.6.0/niceml/utilities/copyutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/encoding.py` & `niceml-0.6.0/niceml/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/factoryutils.py` & `niceml-0.6.0/niceml/utilities/factoryutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/filtering/probabilityclassselector.py` & `niceml-0.6.0/niceml/utilities/filtering/probabilityclassselector.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/fsspec/locationutils.py` & `niceml-0.6.0/niceml/utilities/fsspec/locationutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/gitutils.py` & `niceml-0.6.0/niceml/utilities/gitutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/hydrautils.py` & `niceml-0.6.0/niceml/utilities/hydrautils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/idutils.py` & `niceml-0.6.0/niceml/utilities/idutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/imagegeneration.py` & `niceml-0.6.0/niceml/utilities/imagegeneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/imageloading.py` & `niceml-0.6.0/niceml/utilities/imageloading.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/imagesize.py` & `niceml-0.6.0/niceml/utilities/imagesize.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/imageutils.py` & `niceml-0.6.0/niceml/utilities/imageutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/instancelabeling.py` & `niceml-0.6.0/niceml/utilities/instancelabeling.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/instancelabelmatching.py` & `niceml-0.6.0/niceml/utilities/instancelabelmatching.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/ioumatrix.py` & `niceml-0.6.0/niceml/utilities/ioumatrix.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/ioutils.py` & `niceml-0.6.0/niceml/utilities/ioutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for helper functions for io operations"""
 import json
-from os.path import dirname, join, relpath
+from os.path import dirname, join, relpath, splitext
 from typing import List, Optional, Any, Tuple
 
 import fastparquet
 import pandas as pd
 import yaml
 from fsspec import AbstractFileSystem
 from fsspec.implementations.local import LocalFileSystem
@@ -14,14 +14,15 @@
 
 
 def list_dir(
     path: str,
     return_full_path: bool = False,
     recursive: bool = False,
     file_system: Optional[AbstractFileSystem] = None,
+    filter_ext: Optional[List[str]] = None,
 ) -> List[str]:
     """
     Returns a list of files in a directory
 
     Args:
         path: path to directory, which should be listed
         return_full_path: Returns full filepaths (True) or relative path (False)
@@ -31,14 +32,16 @@
     Returns:
         A list of files in the specified directory
     """
     cur_fs: AbstractFileSystem = file_system or LocalFileSystem()
     files: List[str] = [
         relpath(cur_file, path) for cur_file in list(cur_fs.listdir(path, detail=False))
     ]
+    if filter_ext is not None:
+        files = [cur_file for cur_file in files if splitext(cur_file)[1] in filter_ext]
     if recursive:
         folders = [
             cur_folder for cur_folder in files if cur_fs.isdir(join(path, cur_folder))
         ]
         for cur_folder in folders:
             files += [
                 join(cur_folder, cur_file)
```

### Comparing `niceml-0.5.0/niceml/utilities/masks/cymaskdownscale.pyx` & `niceml-0.6.0/niceml/utilities/masks/cymaskdownscale.pyx`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/masks/maskdownscale.py` & `niceml-0.6.0/niceml/utilities/masks/maskdownscale.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/matchingresult.py` & `niceml-0.6.0/niceml/utilities/matchingresult.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/omegaconfutils.py` & `niceml-0.6.0/niceml/utilities/omegaconfutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/pytestutils.py` & `niceml-0.6.0/niceml/utilities/pytestutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/readwritelock.py` & `niceml-0.6.0/niceml/utilities/readwritelock.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/regexutils.py` & `niceml-0.6.0/niceml/utilities/regexutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/semseg/semsegdrawing.py` & `niceml-0.6.0/niceml/utilities/semseg/semsegdrawing.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/semseg/semseginstancelabeling.py` & `niceml-0.6.0/niceml/utilities/semseg/semseginstancelabeling.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/sinusgeneration.py` & `niceml-0.6.0/niceml/utilities/sinusgeneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/splitutils.py` & `niceml-0.6.0/niceml/utilities/splitutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/thumbnailshower.py` & `niceml-0.6.0/niceml/utilities/thumbnailshower.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/niceml/utilities/userselection.py` & `niceml-0.6.0/niceml/utilities/userselection.py`

 * *Files identical despite different names*

### Comparing `niceml-0.5.0/pyproject.toml` & `niceml-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "niceml"
-version = "0.5.0"
+version = "0.6.0"
 description = "Welcome to niceML 🍦, a Python-based MLOps framework that uses TensorFlow and Dagster. This framework streamlines the development, and maintenance of machine learning models, providing an end-to-end solution for building efficient and scalable pipelines."
 authors = [
     "Denis Stalz-John <denis.stalz-john@codecentric.de>",
     "Nils Uhrberg <nils.uhrberg@codecentric.de>",
     "Anke Koke <anke.koke@codecentric.de>"
 ]
 readme = "README.md"
@@ -89,15 +89,15 @@
 mkdocs-material = "^9.1.9"
 mkdocstrings = "^0.21.2"
 mdx-include = "^1.4.2"
 mkdocs = "^1.4.3"
 mkdocs-table-reader-plugin = "^2.0"
 
 [tool.ruff]
-select = ["E","F","D100", "D101","D102", "D103", "D104","D105","D106","D107","PT","PL"]
+select = ["E","F","D100", "D101","D102", "D103","D105","D106","D107","PT","PL"]
 fixable = ["E","F","D","PT","PL"]
 exclude = ["./tests/**"]
 line-length = 100
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `niceml-0.5.0/PKG-INFO` & `niceml-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceml
-Version: 0.5.0
+Version: 0.6.0
 Summary: Welcome to niceML 🍦, a Python-based MLOps framework that uses TensorFlow and Dagster. This framework streamlines the development, and maintenance of machine learning models, providing an end-to-end solution for building efficient and scalable pipelines.
 Keywords: tensorflow,scikit-learn,streamlit
 Author: Denis Stalz-John
 Author-email: denis.stalz-john@codecentric.de
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.11.*
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


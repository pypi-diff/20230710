# Comparing `tmp/deepchem-2.7.2.dev20230707051842.tar.gz` & `tmp/deepchem-2.7.2.dev20230710190635.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230707051842.tar", last modified: Fri Jul  7 05:18:42 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230710190635.tar", last modified: Mon Jul 10 19:06:36 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230707051842.tar` & `deepchem-2.7.2.dev20230710190635.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.918686 deepchem-2.7.2.dev20230707051842/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 05:18:42.918686 deepchem-2.7.2.dev20230707051842/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.890700 deepchem-2.7.2.dev20230707051842/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.890700 deepchem-2.7.2.dev20230707051842/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.890700 deepchem-2.7.2.dev20230707051842/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.890700 deepchem-2.7.2.dev20230707051842/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.894698 deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.894698 deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.898696 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.898696 deepchem-2.7.2.dev20230707051842/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.898696 deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.898696 deepchem-2.7.2.dev20230707051842/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.898696 deepchem-2.7.2.dev20230707051842/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.898696 deepchem-2.7.2.dev20230707051842/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.902694 deepchem-2.7.2.dev20230707051842/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.902694 deepchem-2.7.2.dev20230707051842/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.902694 deepchem-2.7.2.dev20230707051842/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.902694 deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.902694 deepchem-2.7.2.dev20230707051842/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.902694 deepchem-2.7.2.dev20230707051842/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.906692 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   146027 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.906692 deepchem-2.7.2.dev20230707051842/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.910690 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.910690 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.910690 deepchem-2.7.2.dev20230707051842/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.910690 deepchem-2.7.2.dev20230707051842/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.910690 deepchem-2.7.2.dev20230707051842/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.910690 deepchem-2.7.2.dev20230707051842/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.914688 deepchem-2.7.2.dev20230707051842/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.918686 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-07 05:18:31.000000 deepchem-2.7.2.dev20230707051842/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 05:18:42.890700 deepchem-2.7.2.dev20230707051842/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 05:18:42.000000 deepchem-2.7.2.dev20230707051842/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-07 05:18:42.000000 deepchem-2.7.2.dev20230707051842/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 05:18:42.000000 deepchem-2.7.2.dev20230707051842/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 05:18:42.000000 deepchem-2.7.2.dev20230707051842/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 05:18:42.000000 deepchem-2.7.2.dev20230707051842/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-07 05:18:42.918686 deepchem-2.7.2.dev20230707051842/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-07 05:18:32.000000 deepchem-2.7.2.dev20230707051842/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.077358 deepchem-2.7.2.dev20230710190635/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 19:06:36.077358 deepchem-2.7.2.dev20230710190635/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.053357 deepchem-2.7.2.dev20230710190635/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.053357 deepchem-2.7.2.dev20230710190635/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.053357 deepchem-2.7.2.dev20230710190635/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.053357 deepchem-2.7.2.dev20230710190635/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.057358 deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.057358 deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.057358 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.057358 deepchem-2.7.2.dev20230710190635/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.057358 deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.057358 deepchem-2.7.2.dev20230710190635/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.061358 deepchem-2.7.2.dev20230710190635/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.061358 deepchem-2.7.2.dev20230710190635/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.061358 deepchem-2.7.2.dev20230710190635/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.061358 deepchem-2.7.2.dev20230710190635/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.061358 deepchem-2.7.2.dev20230710190635/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.065358 deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.065358 deepchem-2.7.2.dev20230710190635/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.065358 deepchem-2.7.2.dev20230710190635/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.065358 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149111 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.069358 deepchem-2.7.2.dev20230710190635/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.073358 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.073358 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.073358 deepchem-2.7.2.dev20230710190635/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.073358 deepchem-2.7.2.dev20230710190635/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.073358 deepchem-2.7.2.dev20230710190635/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.073358 deepchem-2.7.2.dev20230710190635/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.077358 deepchem-2.7.2.dev20230710190635/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.077358 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:06:36.053357 deepchem-2.7.2.dev20230710190635/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 19:06:35.000000 deepchem-2.7.2.dev20230710190635/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-10 19:06:36.000000 deepchem-2.7.2.dev20230710190635/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:06:35.000000 deepchem-2.7.2.dev20230710190635/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-10 19:06:35.000000 deepchem-2.7.2.dev20230710190635/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 19:06:35.000000 deepchem-2.7.2.dev20230710190635/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-10 19:06:36.077358 deepchem-2.7.2.dev20230710190635/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-10 19:06:24.000000 deepchem-2.7.2.dev20230710190635/setup.py
```

### Comparing `deepchem-2.7.2.dev20230707051842/LICENSE` & `deepchem-2.7.2.dev20230710190635/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/PKG-INFO` & `deepchem-2.7.2.dev20230710190635/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230707051842
+Version: 2.7.2.dev20230710190635
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230707051842/README.md` & `deepchem-2.7.2.dev20230710190635/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230710190635/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230710190635/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230710190635/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230710190635/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230710190635/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230710190635/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230710190635/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230710190635/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230710190635/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230710190635/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230710190635/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230710190635/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230710190635/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230710190635/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230710190635/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/models.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from deepchem.models.torch_models.infograph import InfoGraphStar, InfoGraphStarModel, InfoGraphEncoder, GINEncoder, InfoGraph, InfoGraphModel, InfoGraphEncoder
 from deepchem.models.torch_models.mpnn import MPNN, MPNNModel
 from deepchem.models.torch_models.lcnn import LCNN, LCNNModel
 from deepchem.models.torch_models.pagtn import Pagtn, PagtnModel
 from deepchem.models.torch_models.mat import MAT, MATModel
 from deepchem.models.torch_models.megnet import MEGNetModel
 from deepchem.models.torch_models.normalizing_flows_pytorch import NormalizingFlow
-from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, MolGANConvolutionLayer
+from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, MolGANConvolutionLayer, MolGANAggregationLayer
 from deepchem.models.torch_models.cnn import CNN
 from deepchem.models.torch_models.attention import ScaledDotProductAttention, SelfAttention
 from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 try:
     from deepchem.models.torch_models.dmpnn import DMPNN, DMPNNModel
     from deepchem.models.torch_models.gnn import GNN, GNNHead, GNNModular
```

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7461,1667 +7461,1860 @@
 0001d240: 640a 2020 2020 6869 6464 656e 5f6c 6179  d.    hidden_lay
 0001d250: 6572 2061 6e64 2069 7420 686f 6c64 2072  er and it hold r
 0001d260: 6573 756c 7473 206f 6620 7468 6520 636f  esults of the co
 0001d270: 6e76 6f6c 7574 696f 6e20 7768 696c 6520  nvolution while 
 0001d280: 6669 7273 7420 7477 6f20 6172 6520 756e  first two are un
 0001d290: 6368 616e 6765 640a 2020 2020 696e 7075  changed.    inpu
 0001d2a0: 7420 7465 6e73 6f72 732e 0a0a 2020 2020  t tensors...    
-0001d2b0: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
-0001d2c0: 2d2d 2d0a 2020 2020 5365 653a 204d 6f6c  ---.    See: Mol
-0001d2d0: 4741 4e4d 756c 7469 436f 6e76 6f6c 7574  GANMultiConvolut
-0001d2e0: 696f 6e4c 6179 6572 2066 6f72 2075 7369  ionLayer for usi
-0001d2f0: 6e67 2069 6e20 6c61 7965 7273 2e0a 0a20  ng in layers... 
-0001d300: 2020 203e 3e3e 2069 6d70 6f72 7420 746f     >>> import to
-0001d310: 7263 680a 2020 2020 3e3e 3e20 696d 706f  rch.    >>> impo
-0001d320: 7274 2074 6f72 6368 2e6e 6e20 6173 206e  rt torch.nn as n
-0001d330: 6e0a 2020 2020 3e3e 3e20 696d 706f 7274  n.    >>> import
-0001d340: 2074 6f72 6368 2e6e 6e2e 6675 6e63 7469   torch.nn.functi
-0001d350: 6f6e 616c 2061 7320 460a 2020 2020 3e3e  onal as F.    >>
-0001d360: 3e20 7665 7274 6963 6573 203d 2039 0a20  > vertices = 9. 
-0001d370: 2020 203e 3e3e 206e 6f64 6573 203d 2035     >>> nodes = 5
-0001d380: 0a20 2020 203e 3e3e 2065 6467 6573 203d  .    >>> edges =
-0001d390: 2035 0a20 2020 203e 3e3e 2075 6e69 7473   5.    >>> units
-0001d3a0: 203d 2031 3238 0a0a 2020 2020 3e3e 3e20   = 128..    >>> 
-0001d3b0: 6c61 7965 7231 203d 204d 6f6c 4741 4e43  layer1 = MolGANC
-0001d3c0: 6f6e 766f 6c75 7469 6f6e 4c61 7965 7228  onvolutionLayer(
-0001d3d0: 756e 6974 733d 756e 6974 732c 2065 6467  units=units, edg
-0001d3e0: 6573 3d65 6467 6573 2c20 6e6f 6465 733d  es=edges, nodes=
-0001d3f0: 6e6f 6465 732c 206e 616d 653d 276c 6179  nodes, name='lay
-0001d400: 6572 3127 290a 2020 2020 3e3e 3e20 6164  er1').    >>> ad
-0001d410: 6a61 6365 6e63 795f 7465 6e73 6f72 203d  jacency_tensor =
-0001d420: 2074 6f72 6368 2e72 616e 646e 2828 312c   torch.randn((1,
-0001d430: 2076 6572 7469 6365 732c 2076 6572 7469   vertices, verti
-0001d440: 6365 732c 2065 6467 6573 2929 0a20 2020  ces, edges)).   
-0001d450: 203e 3e3e 206e 6f64 655f 7465 6e73 6f72   >>> node_tensor
-0001d460: 203d 2074 6f72 6368 2e72 616e 646e 2828   = torch.randn((
-0001d470: 312c 2076 6572 7469 6365 732c 206e 6f64  1, vertices, nod
-0001d480: 6573 2929 0a20 2020 203e 3e3e 206f 7574  es)).    >>> out
-0001d490: 7075 7420 3d20 6c61 7965 7231 285b 6164  put = layer1([ad
-0001d4a0: 6a61 6365 6e63 795f 7465 6e73 6f72 2c20  jacency_tensor, 
-0001d4b0: 6e6f 6465 5f74 656e 736f 725d 290a 0a20  node_tensor]).. 
-0001d4c0: 2020 2052 6566 6572 656e 6365 730a 2020     References.  
-0001d4d0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001d4e0: 202e 2e20 5b31 5d20 4e69 636f 6c61 2044   .. [1] Nicola D
-0001d4f0: 6520 4361 6f20 6574 2061 6c2e 2022 4d6f  e Cao et al. "Mo
-0001d500: 6c47 414e 3a20 416e 2069 6d70 6c69 6369  lGAN: An implici
-0001d510: 7420 6765 6e65 7261 7469 7665 206d 6f64  t generative mod
-0001d520: 656c 0a20 2020 2020 2020 2066 6f72 2073  el.        for s
-0001d530: 6d61 6c6c 206d 6f6c 6563 756c 6172 2067  mall molecular g
-0001d540: 7261 7068 7322 2c20 6874 7470 733a 2f2f  raphs", https://
-0001d550: 6172 7869 762e 6f72 672f 6162 732f 3138  arxiv.org/abs/18
-0001d560: 3035 2e31 3139 3733 0a20 2020 2022 2222  05.11973.    """
-0001d570: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0001d580: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
-0001d590: 2020 2020 2020 2020 2020 756e 6974 733a            units:
-0001d5a0: 2069 6e74 2c0a 2020 2020 2020 2020 2020   int,.          
-0001d5b0: 2020 2020 2020 206e 6f64 6573 3a20 696e         nodes: in
-0001d5c0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0001d5d0: 2020 2020 6163 7469 7661 7469 6f6e 3d46      activation=F
-0001d5e0: 2e74 616e 682c 0a20 2020 2020 2020 2020  .tanh,.         
-0001d5f0: 2020 2020 2020 2020 6472 6f70 6f75 745f          dropout_
-0001d600: 7261 7465 3a20 666c 6f61 7420 3d20 302e  rate: float = 0.
-0001d610: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0001d620: 2020 2020 6564 6765 733a 2069 6e74 203d      edges: int =
-0001d630: 2035 2c0a 2020 2020 2020 2020 2020 2020   5,.            
-0001d640: 2020 2020 206e 616d 653a 2073 7472 203d       name: str =
-0001d650: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-0001d660: 2020 2020 2020 2a2a 6b77 6172 6773 293a        **kwargs):
-0001d670: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001d680: 2020 2020 2049 6e69 7469 616c 697a 6520       Initialize 
-0001d690: 7468 6973 206c 6179 6572 2e0a 0a20 2020  this layer...   
-0001d6a0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-0001d6b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0001d6c0: 2d0a 2020 2020 2020 2020 756e 6974 733a  -.        units:
-0001d6d0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-0001d6e0: 2044 696d 6573 696f 6e20 6f66 2064 656e   Dimesion of den
-0001d6f0: 7365 206c 6179 6572 7320 7573 6564 2066  se layers used f
-0001d700: 6f72 2063 6f6e 766f 6c75 7469 6f6e 0a20  or convolution. 
-0001d710: 2020 2020 2020 206e 6f64 6573 3a20 696e         nodes: in
-0001d720: 740a 2020 2020 2020 2020 2020 2020 4e75  t.            Nu
-0001d730: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
-0001d740: 2069 6e20 6e6f 6465 2074 656e 736f 720a   in node tensor.
-0001d750: 2020 2020 2020 2020 6163 7469 7661 7469          activati
-0001d760: 6f6e 3a20 6675 6e63 7469 6f6e 2c20 6f70  on: function, op
-0001d770: 7469 6f6e 616c 2028 6465 6661 756c 743d  tional (default=
-0001d780: 5461 6e68 290a 2020 2020 2020 2020 2020  Tanh).          
-0001d790: 2020 6163 7469 7661 7469 6f6e 2066 756e    activation fun
-0001d7a0: 6374 696f 6e20 7573 6564 2061 6372 6f73  ction used acros
-0001d7b0: 7320 6d6f 6465 6c2c 2064 6566 6175 6c74  s model, default
-0001d7c0: 2069 7320 5461 6e68 0a20 2020 2020 2020   is Tanh.       
-0001d7d0: 2064 726f 706f 7574 5f72 6174 653a 2066   dropout_rate: f
-0001d7e0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 2028  loat, optional (
-0001d7f0: 6465 6661 756c 743d 302e 3029 0a20 2020  default=0.0).   
-0001d800: 2020 2020 2020 2020 2044 726f 706f 7574           Dropout
-0001d810: 2072 6174 6520 7573 6564 2062 7920 6472   rate used by dr
-0001d820: 6f70 6f75 7420 6c61 7965 720a 2020 2020  opout layer.    
-0001d830: 2020 2020 6564 6765 733a 2069 6e74 2c20      edges: int, 
-0001d840: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
-0001d850: 743d 3529 0a20 2020 2020 2020 2020 2020  t=5).           
-0001d860: 2048 6f77 206d 616e 7920 6465 6e73 6520   How many dense 
-0001d870: 6c61 7965 7273 2074 6f20 7573 6520 696e  layers to use in
-0001d880: 2063 6f6e 766f 6c75 7469 6f6e 2e0a 2020   convolution..  
-0001d890: 2020 2020 2020 2020 2020 5479 7069 6361            Typica
-0001d8a0: 6c6c 7920 6571 7561 6c20 746f 206e 756d  lly equal to num
-0001d8b0: 6265 7220 6f66 2062 6f6e 6420 7479 7065  ber of bond type
-0001d8c0: 7320 7573 6564 2069 6e20 7468 6520 6d6f  s used in the mo
-0001d8d0: 6465 6c2e 0a20 2020 2020 2020 206e 616d  del..        nam
-0001d8e0: 653a 2073 7472 696e 672c 206f 7074 696f  e: string, optio
-0001d8f0: 6e61 6c20 2864 6566 6175 6c74 3d22 2229  nal (default="")
-0001d900: 0a20 2020 2020 2020 2020 2020 204e 616d  .            Nam
-0001d910: 6520 6f66 2074 6865 206c 6179 6572 0a20  e of the layer. 
-0001d920: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001d930: 2020 2073 7570 6572 284d 6f6c 4741 4e43     super(MolGANC
-0001d940: 6f6e 766f 6c75 7469 6f6e 4c61 7965 722c  onvolutionLayer,
-0001d950: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
-0001d960: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0001d970: 6163 7469 7661 7469 6f6e 203d 2061 6374  activation = act
-0001d980: 6976 6174 696f 6e0a 2020 2020 2020 2020  ivation.        
-0001d990: 7365 6c66 2e64 726f 706f 7574 5f72 6174  self.dropout_rat
-0001d9a0: 653a 2066 6c6f 6174 203d 2064 726f 706f  e: float = dropo
-0001d9b0: 7574 5f72 6174 650a 2020 2020 2020 2020  ut_rate.        
-0001d9c0: 7365 6c66 2e75 6e69 7473 3a20 696e 7420  self.units: int 
-0001d9d0: 3d20 756e 6974 730a 2020 2020 2020 2020  = units.        
-0001d9e0: 7365 6c66 2e65 6467 6573 3a20 696e 7420  self.edges: int 
-0001d9f0: 3d20 6564 6765 730a 2020 2020 2020 2020  = edges.        
-0001da00: 7365 6c66 2e6e 616d 653a 2073 7472 203d  self.name: str =
-0001da10: 206e 616d 650a 2020 2020 2020 2020 7365   name.        se
-0001da20: 6c66 2e6e 6f64 6573 3a20 696e 7420 3d20  lf.nodes: int = 
-0001da30: 6e6f 6465 730a 0a20 2020 2020 2020 2073  nodes..        s
-0001da40: 656c 662e 6465 6e73 6531 3a20 6e6e 2e4d  elf.dense1: nn.M
-0001da50: 6f64 756c 654c 6973 7420 3d20 6e6e 2e4d  oduleList = nn.M
-0001da60: 6f64 756c 654c 6973 7428 0a20 2020 2020  oduleList(.     
-0001da70: 2020 2020 2020 205b 6e6e 2e4c 696e 6561         [nn.Linea
-0001da80: 7228 6e6f 6465 732c 2073 656c 662e 756e  r(nodes, self.un
-0001da90: 6974 7329 2066 6f72 205f 2069 6e20 7261  its) for _ in ra
-0001daa0: 6e67 6528 6564 6765 7320 2d20 3129 5d29  nge(edges - 1)])
-0001dab0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
-0001dac0: 6e73 6532 3a20 6e6e 2e4c 696e 6561 7220  nse2: nn.Linear 
-0001dad0: 3d20 6e6e 2e4c 696e 6561 7228 6e6f 6465  = nn.Linear(node
-0001dae0: 732c 2073 656c 662e 756e 6974 7329 0a20  s, self.units). 
-0001daf0: 2020 2020 2020 2073 656c 662e 6472 6f70         self.drop
-0001db00: 6f75 743a 206e 6e2e 4472 6f70 6f75 7420  out: nn.Dropout 
-0001db10: 3d20 6e6e 2e44 726f 706f 7574 2873 656c  = nn.Dropout(sel
-0001db20: 662e 6472 6f70 6f75 745f 7261 7465 290a  f.dropout_rate).
-0001db30: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-0001db40: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0a  _(self) -> str:.
-0001db50: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0001db60: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-0001db70: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
-0001db80: 5f6e 616d 655f 5f7d 2855 6e69 7473 3d7b  _name__}(Units={
-0001db90: 7365 6c66 2e75 6e69 7473 7d2c 204e 6f64  self.units}, Nod
-0001dba0: 6573 3d7b 7365 6c66 2e6e 6f64 6573 7d2c  es={self.nodes},
-0001dbb0: 2041 6374 6976 6174 696f 6e3d 7b73 656c   Activation={sel
-0001dbc0: 662e 6163 7469 7661 7469 6f6e 7d2c 2044  f.activation}, D
-0001dbd0: 726f 706f 7574 5f72 6174 653d 7b73 656c  ropout_rate={sel
-0001dbe0: 662e 6472 6f70 7574 5f72 6174 657d 2c20  f.droput_rate}, 
-0001dbf0: 4564 6765 733d 7b73 656c 662e 6564 6765  Edges={self.edge
-0001dc00: 737d 2c20 4e61 6d65 3d7b 7365 6c66 2e6e  s}, Name={self.n
-0001dc10: 616d 657d 2927 0a20 2020 2020 2020 2029  ame})'.        )
-0001dc20: 0a0a 2020 2020 6465 6620 666f 7277 6172  ..    def forwar
-0001dc30: 6428 0a20 2020 2020 2020 2020 2020 2073  d(.            s
-0001dc40: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0001dc50: 2069 6e70 7574 733a 204c 6973 7429 202d   inputs: List) -
-0001dc60: 3e20 5475 706c 655b 746f 7263 682e 5465  > Tuple[torch.Te
-0001dc70: 6e73 6f72 2c20 746f 7263 682e 5465 6e73  nsor, torch.Tens
-0001dc80: 6f72 2c20 746f 7263 682e 5465 6e73 6f72  or, torch.Tensor
-0001dc90: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-0001dca0: 2020 2020 2020 2049 6e76 6f6b 6520 7468         Invoke th
-0001dcb0: 6973 206c 6179 6572 0a0a 2020 2020 2020  is layer..      
-0001dcc0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0001dcd0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-0001dce0: 2020 2020 2020 2020 696e 7075 7473 3a20          inputs: 
-0001dcf0: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
-0001dd00: 204c 6973 7420 6f66 2074 776f 2069 6e70   List of two inp
-0001dd10: 7574 206d 6174 7269 6365 732c 2061 646a  ut matrices, adj
-0001dd20: 6163 656e 6379 2074 656e 736f 7220 616e  acency tensor an
-0001dd30: 6420 6e6f 6465 2066 6561 7475 7265 7320  d node features 
-0001dd40: 7465 6e73 6f72 730a 2020 2020 2020 2020  tensors.        
-0001dd50: 2020 2020 696e 206f 6e65 2d68 6f74 2065      in one-hot e
-0001dd60: 6e63 6f64 696e 6720 666f 726d 6174 2e0a  ncoding format..
-0001dd70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0001dd80: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0001dd90: 2d0a 2020 2020 2020 2020 7475 706c 6528  -.        tuple(
-0001dda0: 746f 7263 682e 5465 6e73 6f72 2c74 6f72  torch.Tensor,tor
-0001ddb0: 6368 2e54 656e 736f 722c 746f 7263 682e  ch.Tensor,torch.
-0001ddc0: 5465 6e73 6f72 290a 2020 2020 2020 2020  Tensor).        
-0001ddd0: 2020 2020 4669 7273 7420 616e 6420 7365      First and se
-0001dde0: 636f 6e64 2061 7265 206f 7269 6769 6e61  cond are origina
-0001ddf0: 6c20 696e 7075 7420 7465 6e73 6f72 730a  l input tensors.
-0001de00: 2020 2020 2020 2020 2020 2020 5468 6972              Thir
-0001de10: 6420 6973 2074 6865 2072 6573 756c 7420  d is the result 
-0001de20: 6f66 2063 6f6e 766f 6c75 7469 6f6e 0a20  of convolution. 
-0001de30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001de40: 2020 2069 633a 2069 6e74 203d 206c 656e     ic: int = len
-0001de50: 2869 6e70 7574 7329 0a20 2020 2020 2020  (inputs).       
-0001de60: 2069 6620 6963 203c 2032 3a0a 2020 2020   if ic < 2:.    
-0001de70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0001de80: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-0001de90: 2020 2020 2020 2020 2020 224d 6f6c 4741            "MolGA
-0001dea0: 4e43 6f6e 766f 6c75 7469 6f6e 4c61 7965  NConvolutionLaye
-0001deb0: 7220 7265 7175 6972 6573 2061 7420 6c65  r requires at le
-0001dec0: 6173 7420 7477 6f20 696e 7075 7473 3a20  ast two inputs: 
-0001ded0: 5b61 646a 6163 656e 6379 5f74 656e 736f  [adjacency_tenso
-0001dee0: 722c 206e 6f64 655f 6665 6174 7572 6573  r, node_features
-0001def0: 5f74 656e 736f 725d 220a 2020 2020 2020  _tensor]".      
-0001df00: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001df10: 2061 646a 6163 656e 6379 5f74 656e 736f   adjacency_tenso
-0001df20: 723a 2074 6f72 6368 2e54 656e 736f 7220  r: torch.Tensor 
-0001df30: 3d20 696e 7075 7473 5b30 5d0a 2020 2020  = inputs[0].    
-0001df40: 2020 2020 6e6f 6465 5f74 656e 736f 723a      node_tensor:
-0001df50: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-0001df60: 696e 7075 7473 5b31 5d0a 0a20 2020 2020  inputs[1]..     
-0001df70: 2020 2069 6620 6963 203e 2032 3a0a 2020     if ic > 2:.  
-0001df80: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
-0001df90: 5f74 656e 736f 723a 2074 6f72 6368 2e54  _tensor: torch.T
-0001dfa0: 656e 736f 7220 3d20 696e 7075 7473 5b32  ensor = inputs[2
-0001dfb0: 5d0a 2020 2020 2020 2020 2020 2020 616e  ].            an
-0001dfc0: 6e6f 7461 7469 6f6e 7320 3d20 746f 7263  notations = torc
-0001dfd0: 682e 6361 7428 2868 6964 6465 6e5f 7465  h.cat((hidden_te
-0001dfe0: 6e73 6f72 2c20 6e6f 6465 5f74 656e 736f  nsor, node_tenso
-0001dff0: 7229 2c20 2d31 290a 2020 2020 2020 2020  r), -1).        
-0001e000: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001e010: 2020 616e 6e6f 7461 7469 6f6e 7320 3d20    annotations = 
-0001e020: 6e6f 6465 5f74 656e 736f 720a 0a20 2020  node_tensor..   
-0001e030: 2020 2020 206f 7574 7075 745f 6465 6e73       output_dens
-0001e040: 653a 2074 6f72 6368 2e54 656e 736f 7220  e: torch.Tensor 
-0001e050: 3d20 746f 7263 682e 7374 6163 6b28 0a20  = torch.stack(. 
-0001e060: 2020 2020 2020 2020 2020 205b 6465 6e73             [dens
-0001e070: 6528 616e 6e6f 7461 7469 6f6e 7329 2066  e(annotations) f
-0001e080: 6f72 2064 656e 7365 2069 6e20 7365 6c66  or dense in self
-0001e090: 2e64 656e 7365 315d 2c20 3129 0a0a 2020  .dense1], 1)..  
-0001e0a0: 2020 2020 2020 6164 6a3a 2074 6f72 6368        adj: torch
-0001e0b0: 2e54 656e 736f 7220 3d20 6164 6a61 6365  .Tensor = adjace
-0001e0c0: 6e63 795f 7465 6e73 6f72 2e70 6572 6d75  ncy_tensor.permu
-0001e0d0: 7465 2830 2c20 332c 2031 2c20 3229 5b3a  te(0, 3, 1, 2)[:
-0001e0e0: 2c20 313a 2c20 3a2c 203a 5d0a 0a20 2020  , 1:, :, :]..   
-0001e0f0: 2020 2020 206f 7574 7075 745f 6d75 6c3a       output_mul:
-0001e100: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-0001e110: 746f 7263 682e 6d61 746d 756c 2861 646a  torch.matmul(adj
-0001e120: 2c20 6f75 7470 7574 5f64 656e 7365 290a  , output_dense).
-0001e130: 2020 2020 2020 2020 6f75 7470 7574 5f73          output_s
-0001e140: 756d 3a20 746f 7263 682e 5465 6e73 6f72  um: torch.Tensor
-0001e150: 203d 2074 6f72 6368 2e73 756d 286f 7574   = torch.sum(out
-0001e160: 7075 745f 6d75 6c2c 0a20 2020 2020 2020  put_mul,.       
+0001d2b0: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
+0001d2c0: 2d2d 2d2d 2d0a 2020 2020 5365 653a 204d  -----.    See: M
+0001d2d0: 6f6c 4741 4e4d 756c 7469 436f 6e76 6f6c  olGANMultiConvol
+0001d2e0: 7574 696f 6e4c 6179 6572 2066 6f72 2075  utionLayer for u
+0001d2f0: 7369 6e67 2069 6e20 6c61 7965 7273 2e0a  sing in layers..
+0001d300: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
+0001d310: 746f 7263 680a 2020 2020 3e3e 3e20 696d  torch.    >>> im
+0001d320: 706f 7274 2074 6f72 6368 2e6e 6e20 6173  port torch.nn as
+0001d330: 206e 6e0a 2020 2020 3e3e 3e20 696d 706f   nn.    >>> impo
+0001d340: 7274 2074 6f72 6368 2e6e 6e2e 6675 6e63  rt torch.nn.func
+0001d350: 7469 6f6e 616c 2061 7320 460a 2020 2020  tional as F.    
+0001d360: 3e3e 3e20 7665 7274 6963 6573 203d 2039  >>> vertices = 9
+0001d370: 0a20 2020 203e 3e3e 206e 6f64 6573 203d  .    >>> nodes =
+0001d380: 2035 0a20 2020 203e 3e3e 2065 6467 6573   5.    >>> edges
+0001d390: 203d 2035 0a20 2020 203e 3e3e 2075 6e69   = 5.    >>> uni
+0001d3a0: 7473 203d 2031 3238 0a0a 2020 2020 3e3e  ts = 128..    >>
+0001d3b0: 3e20 6c61 7965 7231 203d 204d 6f6c 4741  > layer1 = MolGA
+0001d3c0: 4e43 6f6e 766f 6c75 7469 6f6e 4c61 7965  NConvolutionLaye
+0001d3d0: 7228 756e 6974 733d 756e 6974 732c 2065  r(units=units, e
+0001d3e0: 6467 6573 3d65 6467 6573 2c20 6e6f 6465  dges=edges, node
+0001d3f0: 733d 6e6f 6465 732c 206e 616d 653d 276c  s=nodes, name='l
+0001d400: 6179 6572 3127 290a 2020 2020 3e3e 3e20  ayer1').    >>> 
+0001d410: 6164 6a61 6365 6e63 795f 7465 6e73 6f72  adjacency_tensor
+0001d420: 203d 2074 6f72 6368 2e72 616e 646e 2828   = torch.randn((
+0001d430: 312c 2076 6572 7469 6365 732c 2076 6572  1, vertices, ver
+0001d440: 7469 6365 732c 2065 6467 6573 2929 0a20  tices, edges)). 
+0001d450: 2020 203e 3e3e 206e 6f64 655f 7465 6e73     >>> node_tens
+0001d460: 6f72 203d 2074 6f72 6368 2e72 616e 646e  or = torch.randn
+0001d470: 2828 312c 2076 6572 7469 6365 732c 206e  ((1, vertices, n
+0001d480: 6f64 6573 2929 0a20 2020 203e 3e3e 206f  odes)).    >>> o
+0001d490: 7574 7075 7420 3d20 6c61 7965 7231 285b  utput = layer1([
+0001d4a0: 6164 6a61 6365 6e63 795f 7465 6e73 6f72  adjacency_tensor
+0001d4b0: 2c20 6e6f 6465 5f74 656e 736f 725d 290a  , node_tensor]).
+0001d4c0: 0a20 2020 2052 6566 6572 656e 6365 730a  .    References.
+0001d4d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001d4e0: 2020 202e 2e20 5b31 5d20 4e69 636f 6c61     .. [1] Nicola
+0001d4f0: 2044 6520 4361 6f20 6574 2061 6c2e 2022   De Cao et al. "
+0001d500: 4d6f 6c47 414e 3a20 416e 2069 6d70 6c69  MolGAN: An impli
+0001d510: 6369 7420 6765 6e65 7261 7469 7665 206d  cit generative m
+0001d520: 6f64 656c 0a20 2020 2020 2020 2066 6f72  odel.        for
+0001d530: 2073 6d61 6c6c 206d 6f6c 6563 756c 6172   small molecular
+0001d540: 2067 7261 7068 7322 2c20 6874 7470 733a   graphs", https:
+0001d550: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+0001d560: 3138 3035 2e31 3139 3733 0a20 2020 2022  1805.11973.    "
+0001d570: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+0001d580: 6974 5f5f 2873 656c 662c 0a20 2020 2020  it__(self,.     
+0001d590: 2020 2020 2020 2020 2020 2020 756e 6974              unit
+0001d5a0: 733a 2069 6e74 2c0a 2020 2020 2020 2020  s: int,.        
+0001d5b0: 2020 2020 2020 2020 206e 6f64 6573 3a20           nodes: 
+0001d5c0: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
+0001d5d0: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
+0001d5e0: 3d74 6f72 6368 2e74 616e 682c 0a20 2020  =torch.tanh,.   
+0001d5f0: 2020 2020 2020 2020 2020 2020 2020 6472                dr
+0001d600: 6f70 6f75 745f 7261 7465 3a20 666c 6f61  opout_rate: floa
+0001d610: 7420 3d20 302e 302c 0a20 2020 2020 2020  t = 0.0,.       
+0001d620: 2020 2020 2020 2020 2020 6564 6765 733a            edges:
+0001d630: 2069 6e74 203d 2035 2c0a 2020 2020 2020   int = 5,.      
+0001d640: 2020 2020 2020 2020 2020 206e 616d 653a             name:
+0001d650: 2073 7472 203d 2022 222c 0a20 2020 2020   str = "",.     
+0001d660: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+0001d670: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
+0001d680: 2222 0a20 2020 2020 2020 2049 6e69 7469  "".        Initi
+0001d690: 616c 697a 6520 7468 6973 206c 6179 6572  alize this layer
+0001d6a0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0001d6b0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0001d6c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0001d6d0: 756e 6974 733a 2069 6e74 0a20 2020 2020  units: int.     
+0001d6e0: 2020 2020 2020 2044 696d 6573 696f 6e20         Dimesion 
+0001d6f0: 6f66 2064 656e 7365 206c 6179 6572 7320  of dense layers 
+0001d700: 7573 6564 2066 6f72 2063 6f6e 766f 6c75  used for convolu
+0001d710: 7469 6f6e 0a20 2020 2020 2020 206e 6f64  tion.        nod
+0001d720: 6573 3a20 696e 740a 2020 2020 2020 2020  es: int.        
+0001d730: 2020 2020 4e75 6d62 6572 206f 6620 6665      Number of fe
+0001d740: 6174 7572 6573 2069 6e20 6e6f 6465 2074  atures in node t
+0001d750: 656e 736f 720a 2020 2020 2020 2020 6163  ensor.        ac
+0001d760: 7469 7661 7469 6f6e 3a20 6675 6e63 7469  tivation: functi
+0001d770: 6f6e 2c20 6f70 7469 6f6e 616c 2028 6465  on, optional (de
+0001d780: 6661 756c 743d 5461 6e68 290a 2020 2020  fault=Tanh).    
+0001d790: 2020 2020 2020 2020 6163 7469 7661 7469          activati
+0001d7a0: 6f6e 2066 756e 6374 696f 6e20 7573 6564  on function used
+0001d7b0: 2061 6372 6f73 7320 6d6f 6465 6c2c 2064   across model, d
+0001d7c0: 6566 6175 6c74 2069 7320 5461 6e68 0a20  efault is Tanh. 
+0001d7d0: 2020 2020 2020 2064 726f 706f 7574 5f72         dropout_r
+0001d7e0: 6174 653a 2066 6c6f 6174 2c20 6f70 7469  ate: float, opti
+0001d7f0: 6f6e 616c 2028 6465 6661 756c 743d 302e  onal (default=0.
+0001d800: 3029 0a20 2020 2020 2020 2020 2020 2044  0).            D
+0001d810: 726f 706f 7574 2072 6174 6520 7573 6564  ropout rate used
+0001d820: 2062 7920 6472 6f70 6f75 7420 6c61 7965   by dropout laye
+0001d830: 720a 2020 2020 2020 2020 6564 6765 733a  r.        edges:
+0001d840: 2069 6e74 2c20 6f70 7469 6f6e 616c 2028   int, optional (
+0001d850: 6465 6661 756c 743d 3529 0a20 2020 2020  default=5).     
+0001d860: 2020 2020 2020 2048 6f77 206d 616e 7920         How many 
+0001d870: 6465 6e73 6520 6c61 7965 7273 2074 6f20  dense layers to 
+0001d880: 7573 6520 696e 2063 6f6e 766f 6c75 7469  use in convoluti
+0001d890: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+0001d8a0: 5479 7069 6361 6c6c 7920 6571 7561 6c20  Typically equal 
+0001d8b0: 746f 206e 756d 6265 7220 6f66 2062 6f6e  to number of bon
+0001d8c0: 6420 7479 7065 7320 7573 6564 2069 6e20  d types used in 
+0001d8d0: 7468 6520 6d6f 6465 6c2e 0a20 2020 2020  the model..     
+0001d8e0: 2020 206e 616d 653a 2073 7472 696e 672c     name: string,
+0001d8f0: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
+0001d900: 6c74 3d22 2229 0a20 2020 2020 2020 2020  lt="").         
+0001d910: 2020 204e 616d 6520 6f66 2074 6865 206c     Name of the l
+0001d920: 6179 6572 0a20 2020 2020 2020 2022 2222  ayer.        """
+0001d930: 0a20 2020 2020 2020 2073 7570 6572 284d  .        super(M
+0001d940: 6f6c 4741 4e43 6f6e 766f 6c75 7469 6f6e  olGANConvolution
+0001d950: 4c61 7965 722c 2073 656c 6629 2e5f 5f69  Layer, self).__i
+0001d960: 6e69 745f 5f28 290a 0a20 2020 2020 2020  nit__()..       
+0001d970: 2073 656c 662e 6163 7469 7661 7469 6f6e   self.activation
+0001d980: 203d 2061 6374 6976 6174 696f 6e0a 2020   = activation.  
+0001d990: 2020 2020 2020 7365 6c66 2e64 726f 706f        self.dropo
+0001d9a0: 7574 5f72 6174 653a 2066 6c6f 6174 203d  ut_rate: float =
+0001d9b0: 2064 726f 706f 7574 5f72 6174 650a 2020   dropout_rate.  
+0001d9c0: 2020 2020 2020 7365 6c66 2e75 6e69 7473        self.units
+0001d9d0: 3a20 696e 7420 3d20 756e 6974 730a 2020  : int = units.  
+0001d9e0: 2020 2020 2020 7365 6c66 2e65 6467 6573        self.edges
+0001d9f0: 3a20 696e 7420 3d20 6564 6765 730a 2020  : int = edges.  
+0001da00: 2020 2020 2020 7365 6c66 2e6e 616d 653a        self.name:
+0001da10: 2073 7472 203d 206e 616d 650a 2020 2020   str = name.    
+0001da20: 2020 2020 7365 6c66 2e6e 6f64 6573 3a20      self.nodes: 
+0001da30: 696e 7420 3d20 6e6f 6465 730a 0a20 2020  int = nodes..   
+0001da40: 2020 2020 2073 656c 662e 6465 6e73 6531       self.dense1
+0001da50: 3a20 6e6e 2e4d 6f64 756c 654c 6973 7420  : nn.ModuleList 
+0001da60: 3d20 6e6e 2e4d 6f64 756c 654c 6973 7428  = nn.ModuleList(
+0001da70: 0a20 2020 2020 2020 2020 2020 205b 6e6e  .            [nn
+0001da80: 2e4c 696e 6561 7228 6e6f 6465 732c 2073  .Linear(nodes, s
+0001da90: 656c 662e 756e 6974 7329 2066 6f72 205f  elf.units) for _
+0001daa0: 2069 6e20 7261 6e67 6528 6564 6765 7320   in range(edges 
+0001dab0: 2d20 3129 5d29 0a20 2020 2020 2020 2073  - 1)]).        s
+0001dac0: 656c 662e 6465 6e73 6532 3a20 6e6e 2e4c  elf.dense2: nn.L
+0001dad0: 696e 6561 7220 3d20 6e6e 2e4c 696e 6561  inear = nn.Linea
+0001dae0: 7228 6e6f 6465 732c 2073 656c 662e 756e  r(nodes, self.un
+0001daf0: 6974 7329 0a20 2020 2020 2020 2073 656c  its).        sel
+0001db00: 662e 6472 6f70 6f75 743a 206e 6e2e 4472  f.dropout: nn.Dr
+0001db10: 6f70 6f75 7420 3d20 6e6e 2e44 726f 706f  opout = nn.Dropo
+0001db20: 7574 2873 656c 662e 6472 6f70 6f75 745f  ut(self.dropout_
+0001db30: 7261 7465 290a 0a20 2020 2064 6566 205f  rate)..    def _
+0001db40: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
+0001db50: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
+0001db60: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
+0001db70: 2020 2066 277b 7365 6c66 2e5f 5f63 6c61     f'{self.__cla
+0001db80: 7373 5f5f 2e5f 5f6e 616d 655f 5f7d 2855  ss__.__name__}(U
+0001db90: 6e69 7473 3d7b 7365 6c66 2e75 6e69 7473  nits={self.units
+0001dba0: 7d2c 204e 6f64 6573 3d7b 7365 6c66 2e6e  }, Nodes={self.n
+0001dbb0: 6f64 6573 7d2c 2041 6374 6976 6174 696f  odes}, Activatio
+0001dbc0: 6e3d 7b73 656c 662e 6163 7469 7661 7469  n={self.activati
+0001dbd0: 6f6e 7d2c 2044 726f 706f 7574 5f72 6174  on}, Dropout_rat
+0001dbe0: 653d 7b73 656c 662e 6472 6f70 7574 5f72  e={self.droput_r
+0001dbf0: 6174 657d 2c20 4564 6765 733d 7b73 656c  ate}, Edges={sel
+0001dc00: 662e 6564 6765 737d 2c20 4e61 6d65 3d7b  f.edges}, Name={
+0001dc10: 7365 6c66 2e6e 616d 657d 2927 0a20 2020  self.name})'.   
+0001dc20: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0001dc30: 666f 7277 6172 6428 0a20 2020 2020 2020  forward(.       
+0001dc40: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0001dc50: 2020 2020 2020 2069 6e70 7574 733a 204c         inputs: L
+0001dc60: 6973 7429 202d 3e20 5475 706c 655b 746f  ist) -> Tuple[to
+0001dc70: 7263 682e 5465 6e73 6f72 2c20 746f 7263  rch.Tensor, torc
+0001dc80: 682e 5465 6e73 6f72 2c20 746f 7263 682e  h.Tensor, torch.
+0001dc90: 5465 6e73 6f72 5d3a 0a20 2020 2020 2020  Tensor]:.       
+0001dca0: 2022 2222 0a20 2020 2020 2020 2049 6e76   """.        Inv
+0001dcb0: 6f6b 6520 7468 6973 206c 6179 6572 0a0a  oke this layer..
+0001dcc0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0001dcd0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0001dce0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 696e  -----.        in
+0001dcf0: 7075 7473 3a20 6c69 7374 0a20 2020 2020  puts: list.     
+0001dd00: 2020 2020 2020 204c 6973 7420 6f66 2074         List of t
+0001dd10: 776f 2069 6e70 7574 206d 6174 7269 6365  wo input matrice
+0001dd20: 732c 2061 646a 6163 656e 6379 2074 656e  s, adjacency ten
+0001dd30: 736f 7220 616e 6420 6e6f 6465 2066 6561  sor and node fea
+0001dd40: 7475 7265 7320 7465 6e73 6f72 730a 2020  tures tensors.  
+0001dd50: 2020 2020 2020 2020 2020 696e 206f 6e65            in one
+0001dd60: 2d68 6f74 2065 6e63 6f64 696e 6720 666f  -hot encoding fo
+0001dd70: 726d 6174 2e0a 0a20 2020 2020 2020 2052  rmat...        R
+0001dd80: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0001dd90: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0001dda0: 7475 706c 6528 746f 7263 682e 5465 6e73  tuple(torch.Tens
+0001ddb0: 6f72 2c74 6f72 6368 2e54 656e 736f 722c  or,torch.Tensor,
+0001ddc0: 746f 7263 682e 5465 6e73 6f72 290a 2020  torch.Tensor).  
+0001ddd0: 2020 2020 2020 2020 2020 4669 7273 7420            First 
+0001dde0: 616e 6420 7365 636f 6e64 2061 7265 206f  and second are o
+0001ddf0: 7269 6769 6e61 6c20 696e 7075 7420 7465  riginal input te
+0001de00: 6e73 6f72 730a 2020 2020 2020 2020 2020  nsors.          
+0001de10: 2020 5468 6972 6420 6973 2074 6865 2072    Third is the r
+0001de20: 6573 756c 7420 6f66 2063 6f6e 766f 6c75  esult of convolu
+0001de30: 7469 6f6e 0a20 2020 2020 2020 2022 2222  tion.        """
+0001de40: 0a20 2020 2020 2020 2069 633a 2069 6e74  .        ic: int
+0001de50: 203d 206c 656e 2869 6e70 7574 7329 0a20   = len(inputs). 
+0001de60: 2020 2020 2020 2069 6620 6963 203c 2032         if ic < 2
+0001de70: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0001de80: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+0001de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dea0: 224d 6f6c 4741 4e43 6f6e 766f 6c75 7469  "MolGANConvoluti
+0001deb0: 6f6e 4c61 7965 7220 7265 7175 6972 6573  onLayer requires
+0001dec0: 2061 7420 6c65 6173 7420 7477 6f20 696e   at least two in
+0001ded0: 7075 7473 3a20 5b61 646a 6163 656e 6379  puts: [adjacency
+0001dee0: 5f74 656e 736f 722c 206e 6f64 655f 6665  _tensor, node_fe
+0001def0: 6174 7572 6573 5f74 656e 736f 725d 220a  atures_tensor]".
+0001df00: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0001df10: 2020 2020 2020 2061 646a 6163 656e 6379         adjacency
+0001df20: 5f74 656e 736f 723a 2074 6f72 6368 2e54  _tensor: torch.T
+0001df30: 656e 736f 7220 3d20 696e 7075 7473 5b30  ensor = inputs[0
+0001df40: 5d0a 2020 2020 2020 2020 6e6f 6465 5f74  ].        node_t
+0001df50: 656e 736f 723a 2074 6f72 6368 2e54 656e  ensor: torch.Ten
+0001df60: 736f 7220 3d20 696e 7075 7473 5b31 5d0a  sor = inputs[1].
+0001df70: 0a20 2020 2020 2020 2069 6620 6963 203e  .        if ic >
+0001df80: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+0001df90: 6869 6464 656e 5f74 656e 736f 723a 2074  hidden_tensor: t
+0001dfa0: 6f72 6368 2e54 656e 736f 7220 3d20 696e  orch.Tensor = in
+0001dfb0: 7075 7473 5b32 5d0a 2020 2020 2020 2020  puts[2].        
+0001dfc0: 2020 2020 616e 6e6f 7461 7469 6f6e 7320      annotations 
+0001dfd0: 3d20 746f 7263 682e 6361 7428 2868 6964  = torch.cat((hid
+0001dfe0: 6465 6e5f 7465 6e73 6f72 2c20 6e6f 6465  den_tensor, node
+0001dff0: 5f74 656e 736f 7229 2c20 2d31 290a 2020  _tensor), -1).  
+0001e000: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001e010: 2020 2020 2020 2020 616e 6e6f 7461 7469          annotati
+0001e020: 6f6e 7320 3d20 6e6f 6465 5f74 656e 736f  ons = node_tenso
+0001e030: 720a 0a20 2020 2020 2020 206f 7574 7075  r..        outpu
+0001e040: 745f 6465 6e73 653a 2074 6f72 6368 2e54  t_dense: torch.T
+0001e050: 656e 736f 7220 3d20 746f 7263 682e 7374  ensor = torch.st
+0001e060: 6163 6b28 0a20 2020 2020 2020 2020 2020  ack(.           
+0001e070: 205b 6465 6e73 6528 616e 6e6f 7461 7469   [dense(annotati
+0001e080: 6f6e 7329 2066 6f72 2064 656e 7365 2069  ons) for dense i
+0001e090: 6e20 7365 6c66 2e64 656e 7365 315d 2c20  n self.dense1], 
+0001e0a0: 3129 0a0a 2020 2020 2020 2020 6164 6a3a  1)..        adj:
+0001e0b0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+0001e0c0: 6164 6a61 6365 6e63 795f 7465 6e73 6f72  adjacency_tensor
+0001e0d0: 2e70 6572 6d75 7465 2830 2c20 332c 2031  .permute(0, 3, 1
+0001e0e0: 2c20 3229 5b3a 2c20 313a 2c20 3a2c 203a  , 2)[:, 1:, :, :
+0001e0f0: 5d0a 0a20 2020 2020 2020 206f 7574 7075  ]..        outpu
+0001e100: 745f 6d75 6c3a 2074 6f72 6368 2e54 656e  t_mul: torch.Ten
+0001e110: 736f 7220 3d20 746f 7263 682e 6d61 746d  sor = torch.matm
+0001e120: 756c 2861 646a 2c20 6f75 7470 7574 5f64  ul(adj, output_d
+0001e130: 656e 7365 290a 2020 2020 2020 2020 6f75  ense).        ou
+0001e140: 7470 7574 5f73 756d 3a20 746f 7263 682e  tput_sum: torch.
+0001e150: 5465 6e73 6f72 203d 2074 6f72 6368 2e73  Tensor = torch.s
+0001e160: 756d 286f 7574 7075 745f 6d75 6c2c 0a20  um(output_mul,. 
 0001e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e190: 2020 2020 2020 6469 6d3d 3129 202b 2073        dim=1) + s
-0001e1a0: 656c 662e 6465 6e73 6532 286e 6f64 655f  elf.dense2(node_
-0001e1b0: 7465 6e73 6f72 290a 2020 2020 2020 2020  tensor).        
-0001e1c0: 6f75 7470 7574 5f61 6374 3a20 746f 7263  output_act: torc
-0001e1d0: 682e 5465 6e73 6f72 203d 2073 656c 662e  h.Tensor = self.
-0001e1e0: 6163 7469 7661 7469 6f6e 286f 7574 7075  activation(outpu
-0001e1f0: 745f 7375 6d29 0a20 2020 2020 2020 206f  t_sum).        o
-0001e200: 7574 7075 7420 3d20 7365 6c66 2e64 726f  utput = self.dro
-0001e210: 706f 7574 286f 7574 7075 745f 6163 7429  pout(output_act)
-0001e220: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001e230: 6164 6a61 6365 6e63 795f 7465 6e73 6f72  adjacency_tensor
-0001e240: 2c20 6e6f 6465 5f74 656e 736f 722c 206f  , node_tensor, o
-0001e250: 7574 7075 740a 0a0a 636c 6173 7320 4454  utput...class DT
-0001e260: 4e4e 5374 6570 286e 6e2e 4d6f 6475 6c65  NNStep(nn.Module
-0001e270: 293a 0a20 2020 2022 2222 4454 4e4e 5374  ):.    """DTNNSt
-0001e280: 6570 204c 6179 6572 2066 6f72 2044 544e  ep Layer for DTN
-0001e290: 4e20 6d6f 6465 6c2e 0a0a 2020 2020 456e  N model...    En
-0001e2a0: 636f 6465 7320 7468 6520 6174 6f6d 2773  codes the atom's
-0001e2b0: 2069 6e74 6572 6163 7469 6f6e 2077 6974   interaction wit
-0001e2c0: 6820 6f74 6865 7220 6174 6f6d 7320 6163  h other atoms ac
-0001e2d0: 636f 7264 696e 6720 746f 2064 6973 7461  cording to dista
-0001e2e0: 6e63 6520 7265 6c61 7469 6f6e 7368 6970  nce relationship
-0001e2f0: 732e 205b 315d 5f0a 0a20 2020 2054 6869  s. [1]_..    Thi
-0001e300: 7320 4c61 7965 7220 696d 706c 656d 656e  s Layer implemen
-0001e310: 7473 2074 6865 2045 7120 2837 2920 6672  ts the Eq (7) fr
-0001e320: 6f6d 2044 544e 4e20 5061 7065 722e 2054  om DTNN Paper. T
-0001e330: 6865 6e20 7375 6d73 2074 6865 6d20 7570  hen sums them up
-0001e340: 2074 6f20 6765 7420 7468 6520 6669 6e61   to get the fina
-0001e350: 6c20 6f75 7470 7574 2075 7369 6e67 2045  l output using E
-0001e360: 7120 2836 2920 6672 6f6d 2044 544e 4e20  q (6) from DTNN 
-0001e370: 5061 7065 722e 0a0a 2020 2020 4571 2028  Paper...    Eq (
-0001e380: 3729 3a20 565f 696a 203d 2074 616e 685b  7): V_ij = tanh[
-0001e390: 575f 6663 202e 2028 2857 5f63 6620 2e20  W_fc . ((W_cf . 
-0001e3a0: 435f 6a20 2b20 625f 6366 2920 2a20 2857  C_j + b_cf) * (W
-0001e3b0: 5f64 6620 2e20 645f 696a 202b 2062 5f64  _df . d_ij + b_d
-0001e3c0: 6629 295d 0a0a 2020 2020 4571 2028 3629  f))]..    Eq (6)
-0001e3d0: 3a20 435f 6920 3d20 435f 6920 2b20 7375  : C_i = C_i + su
-0001e3e0: 6d28 565f 696a 290a 0a20 2020 2048 6572  m(V_ij)..    Her
-0001e3f0: 6520 3a20 272e 273d 4d61 7472 6978 204d  e : '.'=Matrix M
-0001e400: 756c 7469 706c 6963 6174 696f 6e20 2c20  ultiplication , 
-0001e410: 272a 273d 4d75 6c74 6970 6c69 6361 7469  '*'=Multiplicati
-0001e420: 6f6e 0a0a 2020 2020 5265 6665 7265 6e63  on..    Referenc
-0001e430: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  es.    ---------
-0001e440: 2d0a 2020 2020 5b31 5d20 5363 68c3 bc74  -.    [1] Sch..t
-0001e450: 742c 204b 7269 7374 6f66 2054 2e2c 2065  t, Kristof T., e
-0001e460: 7420 616c 2e20 2251 7561 6e74 756d 2d63  t al. "Quantum-c
-0001e470: 6865 6d69 6361 6c20 696e 7369 6768 7473  hemical insights
-0001e480: 2066 726f 6d20 6465 6570 0a20 2020 2020   from deep.     
-0001e490: 2020 2074 656e 736f 7220 6e65 7572 616c     tensor neural
-0001e4a0: 206e 6574 776f 726b 732e 2220 4e61 7475   networks." Natu
-0001e4b0: 7265 2063 6f6d 6d75 6e69 6361 7469 6f6e  re communication
-0001e4c0: 7320 382e 3120 2832 3031 3729 3a20 312d  s 8.1 (2017): 1-
-0001e4d0: 382e 0a0a 2020 2020 4578 616d 706c 6573  8...    Examples
-0001e4e0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001e4f0: 2020 3e3e 3e20 6672 6f6d 2064 6565 7063    >>> from deepc
-0001e500: 6865 6d2e 6d6f 6465 6c73 2e74 6f72 6368  hem.models.torch
-0001e510: 5f6d 6f64 656c 7320 696d 706f 7274 206c  _models import l
-0001e520: 6179 6572 730a 2020 2020 3e3e 3e20 696d  ayers.    >>> im
-0001e530: 706f 7274 2074 6f72 6368 0a20 2020 203e  port torch.    >
-0001e540: 3e3e 2065 6d62 6564 6469 6e67 5f6c 6179  >> embedding_lay
-0001e550: 6572 203d 206c 6179 6572 732e 4454 4e4e  er = layers.DTNN
-0001e560: 456d 6265 6464 696e 6728 342c 2034 290a  Embedding(4, 4).
-0001e570: 2020 2020 3e3e 3e20 656d 6220 3d20 656d      >>> emb = em
-0001e580: 6265 6464 696e 675f 6c61 7965 7228 746f  bedding_layer(to
-0001e590: 7263 682e 5465 6e73 6f72 285b 302c 312c  rch.Tensor([0,1,
-0001e5a0: 322c 335d 292e 746f 2874 6f72 6368 2e69  2,3]).to(torch.i
-0001e5b0: 6e74 3634 2929 0a20 2020 203e 3e3e 2073  nt64)).    >>> s
-0001e5c0: 7465 705f 6c61 7965 7220 3d20 6c61 7965  tep_layer = laye
-0001e5d0: 7273 2e44 544e 4e53 7465 7028 342c 2036  rs.DTNNStep(4, 6
-0001e5e0: 2c20 3829 0a20 2020 203e 3e3e 206f 7574  , 8).    >>> out
-0001e5f0: 7075 745f 746f 7263 6820 3d20 7374 6570  put_torch = step
-0001e600: 5f6c 6179 6572 285b 0a20 2020 202e 2e2e  _layer([.    ...
-0001e610: 2020 2020 2074 6f72 6368 2e54 656e 736f       torch.Tenso
-0001e620: 7228 656d 6229 2c0a 2020 2020 2e2e 2e20  r(emb),.    ... 
-0001e630: 2020 2020 746f 7263 682e 5465 6e73 6f72      torch.Tensor
-0001e640: 285b 302c 2031 2c20 322c 2033 2c20 342c  ([0, 1, 2, 3, 4,
-0001e650: 2035 5d29 2e74 6f28 746f 7263 682e 666c   5]).to(torch.fl
-0001e660: 6f61 7433 3229 2c0a 2020 2020 2e2e 2e20  oat32),.    ... 
-0001e670: 2020 2020 746f 7263 682e 5465 6e73 6f72      torch.Tensor
-0001e680: 285b 315d 292e 746f 2874 6f72 6368 2e69  ([1]).to(torch.i
-0001e690: 6e74 3634 292c 0a20 2020 202e 2e2e 2020  nt64),.    ...  
-0001e6a0: 2020 2074 6f72 6368 2e54 656e 736f 7228     torch.Tensor(
-0001e6b0: 5b5b 315d 5d29 2e74 6f28 746f 7263 682e  [[1]]).to(torch.
-0001e6c0: 696e 7436 3429 0a20 2020 202e 2e2e 205d  int64).    ... ]
-0001e6d0: 290a 2020 2020 3e3e 3e20 6f75 7470 7574  ).    >>> output
-0001e6e0: 5f74 6f72 6368 2e73 6861 7065 0a20 2020  _torch.shape.   
-0001e6f0: 2074 6f72 6368 2e53 697a 6528 5b32 2c20   torch.Size([2, 
-0001e700: 342c 2034 5d29 0a0a 2020 2020 2222 220a  4, 4])..    """.
-0001e710: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0001e720: 5f28 7365 6c66 2c0a 2020 2020 2020 2020  _(self,.        
-0001e730: 2020 2020 2020 2020 206e 5f65 6d62 6564           n_embed
-0001e740: 6469 6e67 3a20 696e 7420 3d20 3330 2c0a  ding: int = 30,.
-0001e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e760: 206e 5f64 6973 7461 6e63 653a 2069 6e74   n_distance: int
-0001e770: 203d 2031 3030 2c0a 2020 2020 2020 2020   = 100,.        
-0001e780: 2020 2020 2020 2020 206e 5f68 6964 6465           n_hidde
-0001e790: 6e3a 2069 6e74 203d 2036 302c 0a20 2020  n: int = 60,.   
-0001e7a0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0001e7b0: 6974 6961 6c69 7a65 723a 2073 7472 203d  itializer: str =
-0001e7c0: 2027 7861 7669 6572 5f75 6e69 666f 726d   'xavier_uniform
-0001e7d0: 5f27 2c0a 2020 2020 2020 2020 2020 2020  _',.            
-0001e7e0: 2020 2020 2061 6374 6976 6174 696f 6e3d       activation=
-0001e7f0: 2774 616e 6827 2c0a 2020 2020 2020 2020  'tanh',.        
-0001e800: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-0001e810: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
-0001e820: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0001e830: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0001e840: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e5f  -----.        n_
-0001e850: 656d 6265 6464 696e 673a 2069 6e74 2c20  embedding: int, 
-0001e860: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0001e870: 2020 2020 204e 756d 6265 7220 6f66 2066       Number of f
-0001e880: 6561 7475 7265 7320 666f 7220 6561 6368  eatures for each
-0001e890: 2061 746f 6d0a 2020 2020 2020 2020 6e5f   atom.        n_
-0001e8a0: 6469 7374 616e 6365 3a20 696e 742c 206f  distance: int, o
-0001e8b0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0001e8c0: 2020 2020 6772 616e 756c 6172 6974 7920      granularity 
-0001e8d0: 6f66 2064 6973 7461 6e63 6520 6d61 7472  of distance matr
-0001e8e0: 6978 0a20 2020 2020 2020 206e 5f68 6964  ix.        n_hid
-0001e8f0: 6465 6e3a 2069 6e74 2c20 6f70 7469 6f6e  den: int, option
-0001e900: 616c 0a20 2020 2020 2020 2020 2020 204e  al.            N
-0001e910: 756d 6265 7220 6f66 206e 6f64 6573 2069  umber of nodes i
-0001e920: 6e20 6869 6464 656e 206c 6179 6572 0a20  n hidden layer. 
-0001e930: 2020 2020 2020 2069 6e69 7469 616c 697a         initializ
-0001e940: 6572 3a20 7374 722c 206f 7074 696f 6e61  er: str, optiona
-0001e950: 6c0a 2020 2020 2020 2020 2020 2020 5765  l.            We
-0001e960: 6967 6874 2069 6e69 7469 616c 697a 6174  ight initializat
-0001e970: 696f 6e20 666f 7220 6669 6c74 6572 732e  ion for filters.
-0001e980: 0a20 2020 2020 2020 2020 2020 204f 7074  .            Opt
-0001e990: 696f 6e73 3a20 7b78 6176 6965 725f 756e  ions: {xavier_un
-0001e9a0: 6966 6f72 6d5f 2c20 7861 7669 6572 5f6e  iform_, xavier_n
-0001e9b0: 6f72 6d61 6c5f 2c20 6b61 696d 696e 675f  ormal_, kaiming_
-0001e9c0: 756e 6966 6f72 6d5f 2c20 6b61 696d 696e  uniform_, kaimin
-0001e9d0: 675f 6e6f 726d 616c 5f2c 2074 7275 6e63  g_normal_, trunc
-0001e9e0: 5f6e 6f72 6d61 6c5f 7d0a 2020 2020 2020  _normal_}.      
-0001e9f0: 2020 6163 7469 7661 7469 6f6e 3a20 7374    activation: st
-0001ea00: 722c 206f 7074 696f 6e61 6c0a 2020 2020  r, optional.    
-0001ea10: 2020 2020 2020 2020 4163 7469 7661 7469          Activati
-0001ea20: 6f6e 2066 756e 6374 696f 6e20 6170 706c  on function appl
-0001ea30: 6965 640a 0a20 2020 2020 2020 2022 2222  ied..        """
-0001ea40: 0a20 2020 2020 2020 2073 7570 6572 2844  .        super(D
-0001ea50: 544e 4e53 7465 702c 2073 656c 6629 2e5f  TNNStep, self)._
-0001ea60: 5f69 6e69 745f 5f28 2a2a 6b77 6172 6773  _init__(**kwargs
-0001ea70: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
-0001ea80: 5f65 6d62 6564 6469 6e67 203d 206e 5f65  _embedding = n_e
-0001ea90: 6d62 6564 6469 6e67 0a20 2020 2020 2020  mbedding.       
-0001eaa0: 2073 656c 662e 6e5f 6469 7374 616e 6365   self.n_distance
-0001eab0: 203d 206e 5f64 6973 7461 6e63 650a 2020   = n_distance.  
-0001eac0: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
-0001ead0: 6465 6e20 3d20 6e5f 6869 6464 656e 0a20  den = n_hidden. 
-0001eae0: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
-0001eaf0: 6961 6c69 7a65 7220 3d20 696e 6974 6961  ializer = initia
-0001eb00: 6c69 7a65 7220 2023 2053 6574 2077 6569  lizer  # Set wei
-0001eb10: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
-0001eb20: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
-0001eb30: 6163 7469 7661 7469 6f6e 203d 2061 6374  activation = act
-0001eb40: 6976 6174 696f 6e20 2023 2047 6574 2061  ivation  # Get a
-0001eb50: 6374 6976 6174 696f 6e73 0a20 2020 2020  ctivations.     
-0001eb60: 2020 2073 656c 662e 6163 7469 7661 7469     self.activati
-0001eb70: 6f6e 5f66 6e20 3d20 6765 745f 6163 7469  on_fn = get_acti
-0001eb80: 7661 7469 6f6e 2873 656c 662e 6163 7469  vation(self.acti
-0001eb90: 7661 7469 6f6e 290a 0a20 2020 2020 2020  vation)..       
-0001eba0: 2069 6e69 745f 6675 6e63 3a20 4361 6c6c   init_func: Call
-0001ebb0: 6162 6c65 203d 2067 6574 6174 7472 2869  able = getattr(i
-0001ebc0: 6e69 7469 616c 697a 6572 732c 2073 656c  nitializers, sel
-0001ebd0: 662e 696e 6974 6961 6c69 7a65 7229 0a0a  f.initializer)..
-0001ebe0: 2020 2020 2020 2020 7365 6c66 2e57 5f63          self.W_c
-0001ebf0: 6620 3d20 6e6e 2e50 6172 616d 6574 6572  f = nn.Parameter
-0001ec00: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-0001ec10: 6974 5f66 756e 6328 746f 7263 682e 656d  it_func(torch.em
-0001ec20: 7074 7928 5b73 656c 662e 6e5f 656d 6265  pty([self.n_embe
-0001ec30: 6464 696e 672c 2073 656c 662e 6e5f 6869  dding, self.n_hi
-0001ec40: 6464 656e 5d29 2929 0a20 2020 2020 2020  dden]))).       
-0001ec50: 2073 656c 662e 575f 6466 203d 206e 6e2e   self.W_df = nn.
-0001ec60: 5061 7261 6d65 7465 7228 0a20 2020 2020  Parameter(.     
-0001ec70: 2020 2020 2020 2069 6e69 745f 6675 6e63         init_func
-0001ec80: 2874 6f72 6368 2e65 6d70 7479 285b 7365  (torch.empty([se
-0001ec90: 6c66 2e6e 5f64 6973 7461 6e63 652c 2073  lf.n_distance, s
-0001eca0: 656c 662e 6e5f 6869 6464 656e 5d29 2929  elf.n_hidden])))
-0001ecb0: 0a20 2020 2020 2020 2073 656c 662e 575f  .        self.W_
-0001ecc0: 6663 203d 206e 6e2e 5061 7261 6d65 7465  fc = nn.Paramete
-0001ecd0: 7228 0a20 2020 2020 2020 2020 2020 2069  r(.            i
-0001ece0: 6e69 745f 6675 6e63 2874 6f72 6368 2e65  nit_func(torch.e
-0001ecf0: 6d70 7479 285b 7365 6c66 2e6e 5f68 6964  mpty([self.n_hid
-0001ed00: 6465 6e2c 2073 656c 662e 6e5f 656d 6265  den, self.n_embe
-0001ed10: 6464 696e 675d 2929 290a 2020 2020 2020  dding]))).      
-0001ed20: 2020 7365 6c66 2e62 5f63 6620 3d20 6e6e    self.b_cf = nn
-0001ed30: 2e50 6172 616d 6574 6572 2874 6f72 6368  .Parameter(torch
-0001ed40: 2e7a 6572 6f73 2873 697a 653d 5b0a 2020  .zeros(size=[.  
-0001ed50: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0001ed60: 5f68 6964 6465 6e2c 0a20 2020 2020 2020  _hidden,.       
-0001ed70: 205d 2929 0a20 2020 2020 2020 2073 656c   ])).        sel
-0001ed80: 662e 625f 6466 203d 206e 6e2e 5061 7261  f.b_df = nn.Para
-0001ed90: 6d65 7465 7228 746f 7263 682e 7a65 726f  meter(torch.zero
-0001eda0: 7328 7369 7a65 3d5b 0a20 2020 2020 2020  s(size=[.       
-0001edb0: 2020 2020 2073 656c 662e 6e5f 6869 6464       self.n_hidd
-0001edc0: 656e 2c0a 2020 2020 2020 2020 5d29 290a  en,.        ])).
-0001edd0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-0001ede0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-0001edf0: 2022 2222 5265 7475 726e 7320 6120 7374   """Returns a st
-0001ee00: 7269 6e67 2072 6570 7265 7365 6e74 696e  ring representin
-0001ee10: 6720 7468 6520 636f 6e66 6967 7572 6174  g the configurat
-0001ee20: 696f 6e20 6f66 2074 6865 206c 6179 6572  ion of the layer
-0001ee30: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0001ee40: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-0001ee50: 2d2d 0a20 2020 2020 2020 206e 5f65 6d62  --.        n_emb
-0001ee60: 6564 6469 6e67 3a20 696e 742c 206f 7074  edding: int, opt
-0001ee70: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0001ee80: 2020 4e75 6d62 6572 206f 6620 6665 6174    Number of feat
-0001ee90: 7572 6573 2066 6f72 2065 6163 6820 6174  ures for each at
-0001eea0: 6f6d 0a20 2020 2020 2020 206e 5f64 6973  om.        n_dis
-0001eeb0: 7461 6e63 653a 2069 6e74 2c20 6f70 7469  tance: int, opti
-0001eec0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-0001eed0: 2067 7261 6e75 6c61 7269 7479 206f 6620   granularity of 
-0001eee0: 6469 7374 616e 6365 206d 6174 7269 780a  distance matrix.
-0001eef0: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
-0001ef00: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
-0001ef10: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
-0001ef20: 6572 206f 6620 6e6f 6465 7320 696e 2068  er of nodes in h
-0001ef30: 6964 6465 6e20 6c61 7965 720a 2020 2020  idden layer.    
-0001ef40: 2020 2020 696e 6974 6961 6c69 7a65 723a      initializer:
-0001ef50: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
-0001ef60: 2020 2020 2020 2020 2020 2057 6569 6768             Weigh
-0001ef70: 7420 696e 6974 6961 6c69 7a61 7469 6f6e  t initialization
-0001ef80: 2066 6f72 2066 696c 7465 7273 2e0a 2020   for filters..  
-0001ef90: 2020 2020 2020 2020 2020 4f70 7469 6f6e            Option
-0001efa0: 733a 207b 7861 7669 6572 5f75 6e69 666f  s: {xavier_unifo
-0001efb0: 726d 5f2c 2078 6176 6965 725f 6e6f 726d  rm_, xavier_norm
-0001efc0: 616c 5f2c 206b 6169 6d69 6e67 5f75 6e69  al_, kaiming_uni
-0001efd0: 666f 726d 5f2c 206b 6169 6d69 6e67 5f6e  form_, kaiming_n
-0001efe0: 6f72 6d61 6c5f 2c20 7472 756e 635f 6e6f  ormal_, trunc_no
-0001eff0: 726d 616c 5f7d 0a20 2020 2020 2020 2061  rmal_}.        a
-0001f000: 6374 6976 6174 696f 6e3a 2073 7472 2c20  ctivation: str, 
-0001f010: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0001f020: 2020 2020 2041 6374 6976 6174 696f 6e20       Activation 
-0001f030: 6675 6e63 7469 6f6e 2061 7070 6c69 6564  function applied
-0001f040: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0001f050: 2020 2020 2020 7265 7475 726e 2066 277b        return f'{
-0001f060: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
-0001f070: 5f6e 616d 655f 5f7d 286e 5f65 6d62 6564  _name__}(n_embed
-0001f080: 6469 6e67 3d7b 7365 6c66 2e6e 5f65 6d62  ding={self.n_emb
-0001f090: 6564 6469 6e67 7d2c 206e 5f64 6973 7461  edding}, n_dista
-0001f0a0: 6e63 653d 7b73 656c 662e 6e5f 6469 7374  nce={self.n_dist
-0001f0b0: 616e 6365 7d2c 206e 5f68 6964 6465 6e3d  ance}, n_hidden=
-0001f0c0: 7b73 656c 662e 6e5f 6869 6464 656e 7d2c  {self.n_hidden},
-0001f0d0: 2069 6e69 7469 616c 697a 6572 3d7b 7365   initializer={se
-0001f0e0: 6c66 2e69 6e69 7469 616c 697a 6572 7d2c  lf.initializer},
-0001f0f0: 2061 6374 6976 6174 696f 6e3d 7b73 656c   activation={sel
-0001f100: 662e 6163 7469 7661 7469 6f6e 7d29 270a  f.activation})'.
-0001f110: 0a20 2020 2064 6566 2066 6f72 7761 7264  .    def forward
-0001f120: 2873 656c 662c 2069 6e70 7574 7329 3a0a  (self, inputs):.
-0001f130: 2020 2020 2020 2020 2222 2245 7865 6375          """Execu
-0001f140: 7465 7320 7468 6520 6571 7561 7469 6f6e  tes the equation
-0001f150: 7320 616e 6420 5265 7475 726e 7320 7468  s and Returns th
-0001f160: 6520 696e 7472 6163 7469 6f6e 2076 6563  e intraction vec
-0001f170: 746f 7220 6f66 2074 6865 2061 746f 6d20  tor of the atom 
-0001f180: 7769 7468 206f 7468 6572 2061 746f 6d73  with other atoms
-0001f190: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0001f1a0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0001f1b0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0001f1c0: 2069 6e70 7574 733a 2074 6f72 6368 2e54   inputs: torch.T
-0001f1d0: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
-0001f1e0: 2020 4c69 7374 206f 6620 5465 6e73 6f72    List of Tensor
-0001f1f0: 7320 6861 7669 6e67 2061 746f 6d5f 6665  s having atom_fe
-0001f200: 6174 7572 6573 2c20 6469 7374 616e 6365  atures, distance
-0001f210: 2c20 6469 7374 616e 6365 5f6d 656d 6265  , distance_membe
-0001f220: 7273 6869 705f 692c 2064 6973 7461 6e63  rship_i, distanc
-0001f230: 655f 6d65 6d62 6572 7368 6970 5f6a 2e0a  e_membership_j..
-0001f240: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0001f250: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0001f260: 0a20 2020 2020 2020 2069 6e74 6572 6163  .        interac
-0001f270: 7469 6f6e 5f76 6563 746f 723a 2074 6f72  tion_vector: tor
-0001f280: 6368 2e54 656e 736f 720a 2020 2020 2020  ch.Tensor.      
-0001f290: 2020 2020 2020 696e 7465 7261 6374 696f        interactio
-0001f2a0: 6e20 6f66 2074 6865 2061 746f 6d20 7769  n of the atom wi
-0001f2b0: 7468 206f 7468 6572 2061 746f 6d73 2062  th other atoms b
-0001f2c0: 6173 6564 206f 6e20 6469 7374 616e 6365  ased on distance
-0001f2d0: 2061 6e64 2064 6973 7461 6e63 655f 6d65   and distance_me
-0001f2e0: 6d62 6572 7368 6970 2e0a 0a20 2020 2020  mbership...     
-0001f2f0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
-0001f300: 746f 6d5f 6665 6174 7572 6573 203d 2069  tom_features = i
-0001f310: 6e70 7574 735b 305d 0a20 2020 2020 2020  nputs[0].       
-0001f320: 2064 6973 7461 6e63 6520 3d20 696e 7075   distance = inpu
-0001f330: 7473 5b31 5d0a 2020 2020 2020 2020 6469  ts[1].        di
-0001f340: 7374 616e 6365 5f6d 656d 6265 7273 6869  stance_membershi
-0001f350: 705f 6920 3d20 696e 7075 7473 5b32 5d0a  p_i = inputs[2].
-0001f360: 2020 2020 2020 2020 6469 7374 616e 6365          distance
-0001f370: 5f6d 656d 6265 7273 6869 705f 6a20 3d20  _membership_j = 
-0001f380: 696e 7075 7473 5b33 5d0a 2020 2020 2020  inputs[3].      
-0001f390: 2020 6469 7374 616e 6365 5f68 6964 6465    distance_hidde
-0001f3a0: 6e20 3d20 746f 7263 682e 6d61 746d 756c  n = torch.matmul
-0001f3b0: 2864 6973 7461 6e63 652c 2073 656c 662e  (distance, self.
-0001f3c0: 575f 6466 2920 2b20 7365 6c66 2e62 5f64  W_df) + self.b_d
-0001f3d0: 660a 2020 2020 2020 2020 6174 6f6d 5f66  f.        atom_f
-0001f3e0: 6561 7475 7265 735f 6869 6464 656e 203d  eatures_hidden =
-0001f3f0: 2074 6f72 6368 2e6d 6174 6d75 6c28 6174   torch.matmul(at
-0001f400: 6f6d 5f66 6561 7475 7265 732c 0a20 2020  om_features,.   
-0001f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f430: 2020 2020 2020 2020 2073 656c 662e 575f           self.W_
-0001f440: 6366 2920 2b20 7365 6c66 2e62 5f63 660a  cf) + self.b_cf.
-0001f450: 2020 2020 2020 2020 6f75 7470 7574 7320          outputs 
-0001f460: 3d20 746f 7263 682e 6d75 6c28 0a20 2020  = torch.mul(.   
-0001f470: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
-0001f480: 655f 6869 6464 656e 2c0a 2020 2020 2020  e_hidden,.      
-0001f490: 2020 2020 2020 746f 7263 682e 656d 6265        torch.embe
-0001f4a0: 6464 696e 6728 6174 6f6d 5f66 6561 7475  dding(atom_featu
-0001f4b0: 7265 735f 6869 6464 656e 2c20 6469 7374  res_hidden, dist
-0001f4c0: 616e 6365 5f6d 656d 6265 7273 6869 705f  ance_membership_
-0001f4d0: 6a29 290a 0a20 2020 2020 2020 2023 2066  j))..        # f
-0001f4e0: 6f72 2061 746f 6d20 6920 696e 2061 206d  or atom i in a m
-0001f4f0: 6f6c 6563 756c 6520 6d2c 2074 6869 7320  olecule m, this 
-0001f500: 7374 6570 206d 756c 7469 706c 6965 7320  step multiplies 
-0001f510: 746f 6765 7468 6572 2064 6973 7461 6e63  together distanc
-0001f520: 6520 696e 666f 206f 6620 6174 6f6d 2070  e info of atom p
-0001f530: 6169 7228 692c 6a29 0a20 2020 2020 2020  air(i,j).       
-0001f540: 2023 2061 6e64 2065 6d62 6564 6469 6e67   # and embedding
-0001f550: 7320 6f66 2061 746f 6d20 6a28 626f 7468  s of atom j(both
-0001f560: 2067 6f6e 6520 7468 726f 7567 6820 6120   gone through a 
-0001f570: 6869 6464 656e 206c 6179 6572 290a 2020  hidden layer).  
-0001f580: 2020 2020 2020 6f75 7470 7574 7320 3d20        outputs = 
-0001f590: 746f 7263 682e 6d61 746d 756c 286f 7574  torch.matmul(out
-0001f5a0: 7075 7473 2c20 7365 6c66 2e57 5f66 6329  puts, self.W_fc)
-0001f5b0: 0a20 2020 2020 2020 206f 7574 7075 7473  .        outputs
-0001f5c0: 203d 2073 656c 662e 6163 7469 7661 7469   = self.activati
-0001f5d0: 6f6e 5f66 6e28 6f75 7470 7574 7329 0a0a  on_fn(outputs)..
-0001f5e0: 2020 2020 2020 2020 6f75 7470 7574 5f69          output_i
-0001f5f0: 6920 3d20 746f 7263 682e 6d75 6c28 7365  i = torch.mul(se
-0001f600: 6c66 2e62 5f64 662c 2061 746f 6d5f 6665  lf.b_df, atom_fe
-0001f610: 6174 7572 6573 5f68 6964 6465 6e29 0a20  atures_hidden). 
-0001f620: 2020 2020 2020 206f 7574 7075 745f 6969         output_ii
-0001f630: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
-0001f640: 6f75 7470 7574 5f69 692c 2073 656c 662e  output_ii, self.
-0001f650: 575f 6663 290a 2020 2020 2020 2020 6f75  W_fc).        ou
-0001f660: 7470 7574 5f69 6920 3d20 7365 6c66 2e61  tput_ii = self.a
-0001f670: 6374 6976 6174 696f 6e5f 666e 286f 7574  ctivation_fn(out
-0001f680: 7075 745f 6969 290a 0a20 2020 2020 2020  put_ii)..       
-0001f690: 2023 2066 6f72 2061 746f 6d20 692c 2073   # for atom i, s
-0001f6a0: 756d 2074 6865 2069 6e66 6c75 656e 6365  um the influence
-0001f6b0: 2066 726f 6d20 616c 6c20 6f74 6865 7220   from all other 
-0001f6c0: 6174 6f6d 206a 2069 6e20 7468 6520 6d6f  atom j in the mo
-0001f6d0: 6c65 6375 6c65 0a20 2020 2020 2020 2069  lecule.        i
-0001f6e0: 6e74 7261 6374 696f 6e5f 7665 6374 6f72  ntraction_vector
-0001f6f0: 203d 2073 6361 7474 6572 286f 7574 7075   = scatter(outpu
-0001f700: 7473 2c20 6469 7374 616e 6365 5f6d 656d  ts, distance_mem
-0001f710: 6265 7273 6869 705f 692c 0a20 2020 2020  bership_i,.     
-0001f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f730: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001f740: 696d 3d30 2920 2d20 6f75 7470 7574 5f69  im=0) - output_i
-0001f750: 6920 2b20 6174 6f6d 5f66 6561 7475 7265  i + atom_feature
-0001f760: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-0001f770: 2069 6e74 7261 6374 696f 6e5f 7665 6374   intraction_vect
-0001f780: 6f72 0a0a 0a63 6c61 7373 2045 6467 654e  or...class EdgeN
-0001f790: 6574 776f 726b 286e 6e2e 4d6f 6475 6c65  etwork(nn.Module
-0001f7a0: 293a 0a20 2020 2022 2222 5468 6520 4564  ):.    """The Ed
-0001f7b0: 6765 4e65 7477 6f72 6b20 6d6f 6475 6c65  geNetwork module
-0001f7c0: 2069 7320 6120 5079 546f 7263 6820 7375   is a PyTorch su
-0001f7d0: 626d 6f64 756c 6520 6465 7369 676e 6564  bmodule designed
-0001f7e0: 2066 6f72 206d 6573 7361 6765 2070 6173   for message pas
-0001f7f0: 7369 6e67 2069 6e20 6772 6170 6820 6e65  sing in graph ne
-0001f800: 7572 616c 206e 6574 776f 726b 732e 0a0a  ural networks...
-0001f810: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-0001f820: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
-0001f830: 3e20 7061 6972 5f66 6561 7475 7265 7320  > pair_features 
-0001f840: 3d20 746f 7263 682e 7261 6e64 2828 342c  = torch.rand((4,
-0001f850: 2032 292c 2064 7479 7065 3d74 6f72 6368   2), dtype=torch
-0001f860: 2e66 6c6f 6174 3332 290a 2020 2020 3e3e  .float32).    >>
-0001f870: 3e20 6174 6f6d 5f66 6561 7475 7265 7320  > atom_features 
-0001f880: 3d20 746f 7263 682e 7261 6e64 2828 352c  = torch.rand((5,
-0001f890: 2032 292c 2064 7479 7065 3d74 6f72 6368   2), dtype=torch
-0001f8a0: 2e66 6c6f 6174 3332 290a 2020 2020 3e3e  .float32).    >>
-0001f8b0: 3e20 6174 6f6d 5f74 6f5f 7061 6972 203d  > atom_to_pair =
-0001f8c0: 205b 5d0a 2020 2020 3e3e 3e20 6e5f 6174   [].    >>> n_at
-0001f8d0: 6f6d 7320 3d20 320a 2020 2020 3e3e 3e20  oms = 2.    >>> 
-0001f8e0: 7374 6172 7420 3d20 300a 2020 2020 3e3e  start = 0.    >>
-0001f8f0: 3e20 4330 2c20 4331 203d 206e 702e 6d65  > C0, C1 = np.me
-0001f900: 7368 6772 6964 286e 702e 6172 616e 6765  shgrid(np.arange
-0001f910: 286e 5f61 746f 6d73 292c 206e 702e 6172  (n_atoms), np.ar
-0001f920: 616e 6765 286e 5f61 746f 6d73 2929 0a20  ange(n_atoms)). 
-0001f930: 2020 203e 3e3e 2061 746f 6d5f 746f 5f70     >>> atom_to_p
-0001f940: 6169 722e 6170 7065 6e64 286e 702e 7472  air.append(np.tr
-0001f950: 616e 7370 6f73 6528 6e70 2e61 7272 6179  anspose(np.array
-0001f960: 285b 4331 2e66 6c61 7474 656e 2829 202b  ([C1.flatten() +
-0001f970: 2073 7461 7274 2c20 4330 2e66 6c61 7474   start, C0.flatt
-0001f980: 656e 2829 202b 2073 7461 7274 5d29 2929  en() + start])))
-0001f990: 0a20 2020 203e 3e3e 2061 746f 6d5f 746f  .    >>> atom_to
-0001f9a0: 5f70 6169 7220 3d20 746f 7263 682e 5465  _pair = torch.Te
-0001f9b0: 6e73 6f72 2861 746f 6d5f 746f 5f70 6169  nsor(atom_to_pai
-0001f9c0: 7229 0a20 2020 203e 3e3e 2061 746f 6d5f  r).    >>> atom_
-0001f9d0: 746f 5f70 6169 7220 3d20 746f 7263 682e  to_pair = torch.
-0001f9e0: 7371 7565 657a 6528 6174 6f6d 5f74 6f5f  squeeze(atom_to_
-0001f9f0: 7061 6972 2e74 6f28 746f 7263 682e 696e  pair.to(torch.in
-0001fa00: 7436 3429 2c20 6469 6d3d 3029 0a20 2020  t64), dim=0).   
-0001fa10: 203e 3e3e 2069 6e70 7574 7320 3d20 5b70   >>> inputs = [p
-0001fa20: 6169 725f 6665 6174 7572 6573 2c20 6174  air_features, at
-0001fa30: 6f6d 5f66 6561 7475 7265 732c 2061 746f  om_features, ato
-0001fa40: 6d5f 746f 5f70 6169 725d 0a20 2020 203e  m_to_pair].    >
-0001fa50: 3e3e 206e 5f70 6169 725f 6665 6174 7572  >> n_pair_featur
-0001fa60: 6573 203d 2032 0a20 2020 203e 3e3e 206e  es = 2.    >>> n
-0001fa70: 5f68 6964 6465 6e20 3d20 320a 2020 2020  _hidden = 2.    
-0001fa80: 3e3e 3e20 696e 6974 203d 2027 7861 7669  >>> init = 'xavi
-0001fa90: 6572 5f75 6e69 666f 726d 5f27 0a20 2020  er_uniform_'.   
-0001faa0: 203e 3e3e 206c 6179 6572 203d 2045 6467   >>> layer = Edg
-0001fab0: 654e 6574 776f 726b 286e 5f70 6169 725f  eNetwork(n_pair_
-0001fac0: 6665 6174 7572 6573 2c20 6e5f 6869 6464  features, n_hidd
-0001fad0: 656e 2c20 696e 6974 290a 2020 2020 3e3e  en, init).    >>
-0001fae0: 3e20 7265 7375 6c74 203d 206c 6179 6572  > result = layer
-0001faf0: 2869 6e70 7574 7329 0a20 2020 203e 3e3e  (inputs).    >>>
-0001fb00: 2072 6573 756c 742e 7368 6170 655b 315d   result.shape[1]
-0001fb10: 0a20 2020 2032 0a20 2020 2022 2222 0a0a  .    2.    """..
-0001fb20: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0001fb30: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-0001fb40: 2020 2020 2020 2020 6e5f 7061 6972 5f66          n_pair_f
-0001fb50: 6561 7475 7265 733a 2069 6e74 203d 2038  eatures: int = 8
-0001fb60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001fb70: 2020 206e 5f68 6964 6465 6e3a 2069 6e74     n_hidden: int
-0001fb80: 203d 2031 3030 2c0a 2020 2020 2020 2020   = 100,.        
-0001fb90: 2020 2020 2020 2020 2069 6e69 743a 2073           init: s
-0001fba0: 7472 203d 2027 7861 7669 6572 5f75 6e69  tr = 'xavier_uni
-0001fbb0: 666f 726d 5f27 2c0a 2020 2020 2020 2020  form_',.        
-0001fbc0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-0001fbd0: 7329 3a0a 2020 2020 2020 2020 2222 2249  s):.        """I
-0001fbe0: 6e69 7461 6c69 7365 7320 6120 4564 6765  nitalises a Edge
-0001fbf0: 4e65 7477 6f72 6b20 4c61 7965 720a 0a20  Network Layer.. 
-0001fc00: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0001fc10: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0001fc20: 2d2d 2d2d 0a20 2020 2020 2020 206e 5f70  ----.        n_p
-0001fc30: 6169 725f 6665 6174 7572 6573 3a20 696e  air_features: in
-0001fc40: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-0001fc50: 2020 2020 2020 2020 5468 6520 6c65 6e67          The leng
-0001fc60: 7468 206f 6620 7468 6520 7061 6972 2066  th of the pair f
-0001fc70: 6561 7475 7265 7320 7665 6374 6f72 2e0a  eatures vector..
-0001fc80: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
-0001fc90: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
-0001fca0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-0001fcb0: 6572 206f 6620 6869 6464 656e 2075 6e69  er of hidden uni
-0001fcc0: 7473 2069 6e20 7468 6520 7061 7373 696e  ts in the passin
-0001fcd0: 6720 7068 6173 650a 2020 2020 2020 2020  g phase.        
-0001fce0: 696e 6974 3a20 7374 722c 206f 7074 696f  init: str, optio
-0001fcf0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0001fd00: 496e 6974 6961 6c69 7a61 7469 6f6e 2066  Initialization f
-0001fd10: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
-0001fd20: 6564 2069 6e20 7468 6520 6d65 7373 6167  ed in the messag
-0001fd30: 6520 7061 7373 696e 6720 6c61 7965 722e  e passing layer.
-0001fd40: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0001fd50: 2020 2020 2020 7375 7065 7228 4564 6765        super(Edge
-0001fd60: 4e65 7477 6f72 6b2c 2073 656c 6629 2e5f  Network, self)._
-0001fd70: 5f69 6e69 745f 5f28 2a2a 6b77 6172 6773  _init__(**kwargs
-0001fd80: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
-0001fd90: 5f70 6169 725f 6665 6174 7572 6573 3a20  _pair_features: 
-0001fda0: 696e 7420 3d20 6e5f 7061 6972 5f66 6561  int = n_pair_fea
-0001fdb0: 7475 7265 730a 2020 2020 2020 2020 7365  tures.        se
-0001fdc0: 6c66 2e6e 5f68 6964 6465 6e3a 2069 6e74  lf.n_hidden: int
-0001fdd0: 203d 206e 5f68 6964 6465 6e0a 2020 2020   = n_hidden.    
-0001fde0: 2020 2020 7365 6c66 2e69 6e69 743a 2073      self.init: s
-0001fdf0: 7472 203d 2069 6e69 740a 0a20 2020 2020  tr = init..     
-0001fe00: 2020 2069 6e69 745f 6675 6e63 3a20 4361     init_func: Ca
-0001fe10: 6c6c 6162 6c65 203d 2067 6574 6174 7472  llable = getattr
-0001fe20: 2869 6e69 7469 616c 697a 6572 732c 2073  (initializers, s
-0001fe30: 656c 662e 696e 6974 290a 2020 2020 2020  elf.init).      
-0001fe40: 2020 7365 6c66 2e57 3a20 746f 7263 682e    self.W: torch.
-0001fe50: 5465 6e73 6f72 203d 2069 6e69 745f 6675  Tensor = init_fu
-0001fe60: 6e63 280a 2020 2020 2020 2020 2020 2020  nc(.            
-0001fe70: 746f 7263 682e 656d 7074 7928 5b73 656c  torch.empty([sel
-0001fe80: 662e 6e5f 7061 6972 5f66 6561 7475 7265  f.n_pair_feature
-0001fe90: 732c 2073 656c 662e 6e5f 6869 6464 656e  s, self.n_hidden
-0001fea0: 202a 2073 656c 662e 6e5f 6869 6464 656e   * self.n_hidden
-0001feb0: 5d29 290a 2020 2020 2020 2020 7365 6c66  ])).        self
-0001fec0: 2e62 3a20 746f 7263 682e 5465 6e73 6f72  .b: torch.Tensor
-0001fed0: 203d 2074 6f72 6368 2e7a 6572 6f73 2828   = torch.zeros((
-0001fee0: 7365 6c66 2e6e 5f68 6964 6465 6e20 2a20  self.n_hidden * 
-0001fef0: 7365 6c66 2e6e 5f68 6964 6465 6e2c 2929  self.n_hidden,))
-0001ff00: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
-0001ff10: 696c 743a 2062 6f6f 6c20 3d20 5472 7565  ilt: bool = True
-0001ff20: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-0001ff30: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
-0001ff40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001ff50: 280a 2020 2020 2020 2020 2020 2020 6627  (.            f'
-0001ff60: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
-0001ff70: 5f5f 6e61 6d65 5f5f 7d28 6e5f 7061 6972  __name__}(n_pair
-0001ff80: 5f66 6561 7475 7265 733a 7b73 656c 662e  _features:{self.
-0001ff90: 6e5f 7061 6972 5f66 6561 7475 7265 737d  n_pair_features}
-0001ffa0: 2c6e 5f68 6964 6465 6e3a 7b73 656c 662e  ,n_hidden:{self.
-0001ffb0: 6e5f 6869 6464 656e 7d2c 696e 6974 3a7b  n_hidden},init:{
-0001ffc0: 7365 6c66 2e69 6e69 747d 2927 0a20 2020  self.init})'.   
-0001ffd0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0001ffe0: 666f 7277 6172 6428 7365 6c66 2c20 696e  forward(self, in
-0001fff0: 7075 7473 3a20 4c69 7374 5b74 6f72 6368  puts: List[torch
-00020000: 2e54 656e 736f 725d 2920 2d3e 2074 6f72  .Tensor]) -> tor
-00020010: 6368 2e54 656e 736f 723a 0a20 2020 2020  ch.Tensor:.     
-00020020: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
-00020030: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00020040: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00020050: 2020 2020 2069 6e70 7574 733a 204c 6973       inputs: Lis
-00020060: 745b 746f 7263 682e 5465 6e73 6f72 5d0a  t[torch.Tensor].
-00020070: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00020080: 6c65 6e67 7468 206f 6620 6174 6f6d 5f74  length of atom_t
-00020090: 6f5f 7061 6972 2073 686f 756c 6420 6265  o_pair should be
-000200a0: 2073 616d 6520 6173 206e 5f70 6169 725f   same as n_pair_
-000200b0: 6665 6174 7572 6573 2e0a 2020 2020 2020  features..      
-000200c0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-000200d0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-000200e0: 2020 7265 7375 6c74 3a20 746f 7263 682e    result: torch.
-000200f0: 5465 6e73 6f72 0a20 2020 2020 2020 2020  Tensor.         
-00020100: 2020 2054 656e 736f 7220 636f 6e74 6169     Tensor contai
-00020110: 6e69 6e67 2074 6865 206d 6170 7069 6e67  ning the mapping
-00020120: 206f 6620 7468 6520 6564 6765 2076 6563   of the edge vec
-00020130: 746f 7220 746f 2061 2064 20c3 9720 6420  tor to a d .. d 
-00020140: 6d61 7472 6978 2c20 7768 6572 6520 6420  matrix, where d 
-00020150: 6465 6e6f 7465 7320 7468 6520 6469 6d65  denotes the dime
-00020160: 6e73 696f 6e20 6f66 2074 6865 2069 6e74  nsion of the int
-00020170: 6572 6e61 6c20 6869 6464 656e 2072 6570  ernal hidden rep
-00020180: 7265 7365 6e74 6174 696f 6e20 6f66 2065  resentation of e
-00020190: 6163 6820 6e6f 6465 2069 6e20 7468 6520  ach node in the 
-000201a0: 6772 6170 682e 0a20 2020 2020 2020 2022  graph..        "
-000201b0: 2222 0a20 2020 2020 2020 2070 6169 725f  "".        pair_
-000201c0: 6665 6174 7572 6573 3a20 746f 7263 682e  features: torch.
-000201d0: 5465 6e73 6f72 0a20 2020 2020 2020 2061  Tensor.        a
-000201e0: 746f 6d5f 6665 6174 7572 6573 3a20 746f  tom_features: to
-000201f0: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
-00020200: 2020 2061 746f 6d5f 746f 5f70 6169 723a     atom_to_pair:
-00020210: 2074 6f72 6368 2e54 656e 736f 720a 2020   torch.Tensor.  
-00020220: 2020 2020 2020 7061 6972 5f66 6561 7475        pair_featu
-00020230: 7265 732c 2061 746f 6d5f 6665 6174 7572  res, atom_featur
-00020240: 6573 2c20 6174 6f6d 5f74 6f5f 7061 6972  es, atom_to_pair
-00020250: 203d 2069 6e70 7574 730a 0a20 2020 2020   = inputs..     
-00020260: 2020 2041 3a20 746f 7263 682e 5465 6e73     A: torch.Tens
-00020270: 6f72 203d 2074 6f72 6368 2e61 6464 2874  or = torch.add(t
-00020280: 6f72 6368 2e6d 6174 6d75 6c28 7061 6972  orch.matmul(pair
-00020290: 5f66 6561 7475 7265 732c 2073 656c 662e  _features, self.
-000202a0: 5729 2c20 7365 6c66 2e62 290a 2020 2020  W), self.b).    
-000202b0: 2020 2020 4120 3d20 746f 7263 682e 7265      A = torch.re
-000202c0: 7368 6170 6528 412c 2028 2d31 2c20 7365  shape(A, (-1, se
-000202d0: 6c66 2e6e 5f68 6964 6465 6e2c 2073 656c  lf.n_hidden, sel
-000202e0: 662e 6e5f 6869 6464 656e 2929 0a20 2020  f.n_hidden)).   
-000202f0: 2020 2020 206f 7574 3a20 746f 7263 682e       out: torch.
-00020300: 5465 6e73 6f72 203d 2074 6f72 6368 2e75  Tensor = torch.u
-00020310: 6e73 7175 6565 7a65 2861 746f 6d5f 6665  nsqueeze(atom_fe
-00020320: 6174 7572 6573 5b61 746f 6d5f 746f 5f70  atures[atom_to_p
-00020330: 6169 725b 3a2c 2031 5d5d 2c0a 2020 2020  air[:, 1]],.    
-00020340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020360: 2020 2020 2020 2020 6469 6d3d 3229 0a20          dim=2). 
-00020370: 2020 2020 2020 206f 7574 5f73 7175 6565         out_squee
-00020380: 7a65 3a20 746f 7263 682e 5465 6e73 6f72  ze: torch.Tensor
-00020390: 203d 2074 6f72 6368 2e73 7175 6565 7a65   = torch.squeeze
-000203a0: 2874 6f72 6368 2e6d 6174 6d75 6c28 412c  (torch.matmul(A,
-000203b0: 206f 7574 292c 2064 696d 3d32 290a 2020   out), dim=2).  
-000203c0: 2020 2020 2020 696e 643a 2074 6f72 6368        ind: torch
-000203d0: 2e54 656e 736f 7220 3d20 6174 6f6d 5f74  .Tensor = atom_t
-000203e0: 6f5f 7061 6972 5b3a 2c20 305d 0a0a 2020  o_pair[:, 0]..  
-000203f0: 2020 2020 2020 7265 7375 6c74 3a20 746f        result: to
-00020400: 7263 682e 5465 6e73 6f72 203d 2073 6567  rch.Tensor = seg
-00020410: 6d65 6e74 5f73 756d 286f 7574 5f73 7175  ment_sum(out_squ
-00020420: 6565 7a65 2c20 696e 6429 0a0a 2020 2020  eeze, ind)..    
-00020430: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00020440: 740a 0a0a 636c 6173 7320 5765 6176 654c  t...class WeaveL
-00020450: 6179 6572 286e 6e2e 4d6f 6475 6c65 293a  ayer(nn.Module):
-00020460: 0a20 2020 2022 2222 5468 6973 2063 6c61  .    """This cla
-00020470: 7373 2069 6d70 6c65 6d65 6e74 7320 7468  ss implements th
-00020480: 6520 636f 7265 2057 6561 7665 2063 6f6e  e core Weave con
-00020490: 766f 6c75 7469 6f6e 2066 726f 6d20 7468  volution from th
-000204a0: 6520 476f 6f67 6c65 2067 7261 7068 2063  e Google graph c
-000204b0: 6f6e 766f 6c75 7469 6f6e 2070 6170 6572  onvolution paper
-000204c0: 205b 315d 5f0a 2020 5468 6973 2069 7320   [1]_.  This is 
-000204d0: 7468 6520 546f 7263 6820 6571 7569 7661  the Torch equiva
-000204e0: 6c65 6e74 206f 6620 7468 6520 6f72 6967  lent of the orig
-000204f0: 696e 616c 2069 6d70 6c65 6d65 6e74 6174  inal implementat
-00020500: 696f 6e20 7573 696e 6720 4b65 7261 732e  ion using Keras.
-00020510: 0a0a 2020 5468 6973 206d 6f64 656c 2063  ..  This model c
-00020520: 6f6e 7461 696e 7320 6174 6f6d 2066 6561  ontains atom fea
-00020530: 7475 7265 7320 616e 6420 626f 6e64 2066  tures and bond f
-00020540: 6561 7475 7265 730a 2020 7365 7061 7261  eatures.  separa
-00020550: 7465 6c79 2e48 6572 652c 2062 6f6e 6420  tely.Here, bond 
-00020560: 6665 6174 7572 6573 2061 7265 2061 6c73  features are als
-00020570: 6f20 6361 6c6c 6564 2070 6169 7220 6665  o called pair fe
-00020580: 6174 7572 6573 2e0a 2020 5468 6572 6520  atures..  There 
-00020590: 6172 6520 3220 7479 7065 7320 6f66 2074  are 2 types of t
-000205a0: 7261 6e73 666f 726d 6174 696f 6e2c 2061  ransformation, a
-000205b0: 746f 6d2d 3e61 746f 6d2c 2061 746f 6d2d  tom->atom, atom-
-000205c0: 3e70 6169 722c 2070 6169 722d 3e61 746f  >pair, pair->ato
-000205d0: 6d2c 2070 6169 722d 3e70 6169 7220 7468  m, pair->pair th
-000205e0: 6174 2074 6869 7320 6d6f 6465 6c20 696d  at this model im
-000205f0: 706c 656d 656e 7473 2e0a 0a20 2045 7861  plements...  Exa
-00020600: 6d70 6c65 730a 2020 2d2d 2d2d 2d2d 2d2d  mples.  --------
-00020610: 0a20 2054 6869 7320 6c61 7965 7220 6578  .  This layer ex
-00020620: 7065 6374 7320 3420 696e 7075 7473 2069  pects 4 inputs i
-00020630: 6e20 6120 6c69 7374 206f 6620 7468 6520  n a list of the 
-00020640: 666f 726d 2060 5b61 746f 6d5f 6665 6174  form `[atom_feat
-00020650: 7572 6573 2c0a 2020 7061 6972 5f66 6561  ures,.  pair_fea
-00020660: 7475 7265 732c 2070 6169 725f 7370 6c69  tures, pair_spli
-00020670: 742c 2061 746f 6d5f 746f 5f70 6169 725d  t, atom_to_pair]
-00020680: 602e 2057 6527 6c6c 2077 616c 6b20 7468  `. We'll walk th
-00020690: 726f 7567 6820 7468 6520 7374 7275 6374  rough the struct
-000206a0: 7572 6520 6f66 2074 6865 7365 2069 6e70  ure of these inp
-000206b0: 7574 732e 204c 6574 2773 2073 7461 7274  uts. Let's start
-000206c0: 2077 6974 6820 736f 6d65 2062 6173 6963   with some basic
-000206d0: 2064 6566 696e 6974 696f 6e73 2e0a 2020   definitions..  
-000206e0: 3e3e 3e20 696d 706f 7274 2064 6565 7063  >>> import deepc
-000206f0: 6865 6d20 6173 2064 630a 2020 3e3e 3e20  hem as dc.  >>> 
-00020700: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-00020710: 6e70 0a20 203e 3e3e 2073 6d69 6c65 7320  np.  >>> smiles 
-00020720: 3d20 5b22 4343 4322 2c20 2243 225d 0a0a  = ["CCC", "C"]..
-00020730: 2020 4e6f 7465 2074 6861 7420 7468 6572    Note that ther
-00020740: 6520 6172 6520 3420 6174 6f6d 7320 696e  e are 4 atoms in
-00020750: 2074 6f74 616c 2069 6e20 7468 6973 2073   total in this s
-00020760: 7973 7465 6d2e 2054 6869 7320 6c61 7965  ystem. This laye
-00020770: 7220 6578 7065 6374 7320 6974 7320 696e  r expects its in
-00020780: 7075 7420 6d6f 6c65 6375 6c65 7320 746f  put molecules to
-00020790: 2062 6520 6261 7463 6865 6420 746f 6765   be batched toge
-000207a0: 7468 6572 2e0a 0a20 203e 3e3e 2074 6f74  ther...  >>> tot
-000207b0: 616c 5f6e 5f61 746f 6d73 203d 2034 0a0a  al_n_atoms = 4..
-000207c0: 2020 4c65 7427 7320 7375 7070 6f73 6520    Let's suppose 
-000207d0: 7468 6174 2077 6520 6861 7665 2061 2066  that we have a f
-000207e0: 6561 7475 7269 7a65 7220 7468 6174 2063  eaturizer that c
-000207f0: 6f6d 7075 7465 7320 606e 5f61 746f 6d5f  omputes `n_atom_
-00020800: 6665 6174 6020 6665 6174 7572 6573 2070  feat` features p
-00020810: 6572 2061 746f 6d2e 0a0a 2020 3e3e 3e20  er atom...  >>> 
-00020820: 6e5f 6174 6f6d 5f66 6561 7420 3d20 3735  n_atom_feat = 75
-00020830: 0a0a 2020 5468 656e 2063 6f6e 6365 7074  ..  Then concept
-00020840: 7561 6c6c 792c 2060 6174 6f6d 5f66 6561  ually, `atom_fea
-00020850: 7460 2069 7320 7468 6520 6172 7261 7920  t` is the array 
-00020860: 6f66 2073 6861 7065 2060 2874 6f74 616c  of shape `(total
-00020870: 5f6e 5f61 746f 6d73 2c0a 2020 6e5f 6174  _n_atoms,.  n_at
-00020880: 6f6d 5f66 6561 7429 6020 6f66 2061 746f  om_feat)` of ato
-00020890: 6d69 6320 6665 6174 7572 6573 2e20 466f  mic features. Fo
-000208a0: 7220 7369 6d70 6c69 6369 7479 2c20 6c65  r simplicity, le
-000208b0: 7427 7320 6a75 7374 2067 6f20 7769 7468  t's just go with
-000208c0: 2061 0a20 2072 616e 646f 6d20 7375 6368   a.  random such
-000208d0: 206d 6174 7269 782e 0a0a 2020 3e3e 3e20   matrix...  >>> 
-000208e0: 6174 6f6d 5f66 6561 7420 3d20 6e70 2e72  atom_feat = np.r
-000208f0: 616e 646f 6d2e 7261 6e64 2874 6f74 616c  andom.rand(total
-00020900: 5f6e 5f61 746f 6d73 2c20 6e5f 6174 6f6d  _n_atoms, n_atom
-00020910: 5f66 6561 7429 0a0a 2020 4c65 7427 7320  _feat)..  Let's 
-00020920: 7375 7070 6f73 6520 7765 2068 6176 6520  suppose we have 
-00020930: 606e 5f70 6169 725f 6665 6174 6020 7061  `n_pair_feat` pa
-00020940: 6972 7769 7365 2066 6561 7475 7265 730a  irwise features.
-00020950: 0a20 203e 3e3e 206e 5f70 6169 725f 6665  .  >>> n_pair_fe
-00020960: 6174 203d 2031 340a 0a20 2046 6f72 2065  at = 14..  For e
-00020970: 6163 6820 6d6f 6c65 6375 6c65 2c20 7765  ach molecule, we
-00020980: 2063 6f6d 7075 7465 2061 206d 6174 7269   compute a matri
-00020990: 7820 6f66 2073 6861 7065 2060 286e 5f61  x of shape `(n_a
-000209a0: 746f 6d73 2a6e 5f61 746f 6d73 2c0a 2020  toms*n_atoms,.  
-000209b0: 6e5f 7061 6972 5f66 6561 7429 6020 6f66  n_pair_feat)` of
-000209c0: 2070 6169 7277 6973 6520 6665 6174 7572   pairwise featur
-000209d0: 6573 2066 6f72 2065 6163 6820 7061 6972  es for each pair
-000209e0: 206f 6620 6174 6f6d 7320 696e 2074 6865   of atoms in the
-000209f0: 206d 6f6c 6563 756c 652e 0a20 204c 6574   molecule..  Let
-00020a00: 2773 2063 6f6e 7374 7275 6374 2074 6869  's construct thi
-00020a10: 7320 636f 6e63 6570 7475 616c 6c79 2066  s conceptually f
-00020a20: 6f72 206f 7572 2065 7861 6d70 6c65 2e0a  or our example..
-00020a30: 0a20 203e 3e3e 2070 6169 725f 6665 6174  .  >>> pair_feat
-00020a40: 203d 205b 6e70 2e72 616e 646f 6d2e 7261   = [np.random.ra
-00020a50: 6e64 2833 2a33 2c20 6e5f 7061 6972 5f66  nd(3*3, n_pair_f
-00020a60: 6561 7429 2c20 6e70 2e72 616e 646f 6d2e  eat), np.random.
-00020a70: 7261 6e64 2831 2a31 2c6e 5f70 6169 725f  rand(1*1,n_pair_
-00020a80: 6665 6174 295d 0a20 203e 3e3e 2070 6169  feat)].  >>> pai
-00020a90: 725f 6665 6174 203d 206e 702e 636f 6e63  r_feat = np.conc
-00020aa0: 6174 656e 6174 6528 7061 6972 5f66 6561  atenate(pair_fea
-00020ab0: 742c 2061 7869 733d 3029 0a20 203e 3e3e  t, axis=0).  >>>
-00020ac0: 2070 6169 725f 6665 6174 2e73 6861 7065   pair_feat.shape
-00020ad0: 0a20 2028 3130 2c20 3134 290a 0a20 2060  .  (10, 14)..  `
-00020ae0: 7061 6972 5f73 706c 6974 6020 6973 2061  pair_split` is a
-00020af0: 6e20 696e 6465 7820 696e 746f 2060 7061  n index into `pa
-00020b00: 6972 5f66 6561 7460 2077 6869 6368 2074  ir_feat` which t
-00020b10: 656c 6c73 2075 7320 7768 6963 6820 6174  ells us which at
-00020b20: 6f6d 2065 6163 6820 726f 7720 6265 6c6f  om each row belo
-00020b30: 6e67 7320 746f 2e20 496e 206f 7572 2063  ngs to. In our c
-00020b40: 6173 652c 2077 6520 6876 650a 0a20 203e  ase, we hve..  >
-00020b50: 3e3e 2070 6169 725f 7370 6c69 7420 3d20  >> pair_split = 
-00020b60: 6e70 2e61 7272 6179 285b 302c 2030 2c20  np.array([0, 0, 
-00020b70: 302c 2031 2c20 312c 2031 2c20 322c 2032  0, 1, 1, 1, 2, 2
-00020b80: 2c20 322c 2033 5d29 0a0a 2020 5468 6174  , 2, 3])..  That
-00020b90: 2069 732c 2074 6865 2066 6972 7374 2039   is, the first 9
-00020ba0: 2065 6e74 7269 6573 2062 656c 6f6e 6720   entries belong 
-00020bb0: 746f 2022 4343 4322 2061 6e64 2074 6865  to "CCC" and the
-00020bc0: 206c 6173 7420 656e 7472 7920 746f 2022   last entry to "
-00020bd0: 4322 2e20 5468 650a 2020 6669 6e61 6c20  C". The.  final 
-00020be0: 656e 7472 7920 6061 746f 6d5f 746f 5f70  entry `atom_to_p
-00020bf0: 6169 7260 2067 6f65 7320 696e 2061 206c  air` goes in a l
-00020c00: 6974 746c 6520 6d6f 7265 2069 6e2d 6465  ittle more in-de
-00020c10: 7074 6820 7468 616e 2060 7061 6972 5f73  pth than `pair_s
-00020c20: 706c 6974 600a 2020 616e 6420 7465 6c6c  plit`.  and tell
-00020c30: 7320 7573 2074 6865 2070 7265 6369 7365  s us the precise
-00020c40: 2070 6169 7220 6561 6368 2070 6169 7220   pair each pair 
-00020c50: 6665 6174 7572 6520 6265 6c6f 6e67 7320  feature belongs 
-00020c60: 746f 2e20 496e 206f 7572 2063 6173 650a  to. In our case.
-00020c70: 0a20 203e 3e3e 2061 746f 6d5f 746f 5f70  .  >>> atom_to_p
-00020c80: 6169 7220 3d20 6e70 2e61 7272 6179 285b  air = np.array([
-00020c90: 5b30 2c20 305d 2c0a 2020 2e2e 2e20 2020  [0, 0],.  ...   
-00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cb0: 2020 2020 2020 205b 302c 2031 5d2c 0a20         [0, 1],. 
-00020cc0: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
-00020cd0: 2020 2020 2020 2020 2020 2020 2020 5b30                [0
-00020ce0: 2c20 325d 2c0a 2020 2e2e 2e20 2020 2020  , 2],.  ...     
-00020cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d00: 2020 2020 205b 312c 2030 5d2c 0a20 202e       [1, 0],.  .
-00020d10: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
-00020d20: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
-00020d30: 315d 2c0a 2020 2e2e 2e20 2020 2020 2020  1],.  ...       
-00020d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d50: 2020 205b 312c 2032 5d2c 0a20 202e 2e2e     [1, 2],.  ...
-00020d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d70: 2020 2020 2020 2020 2020 5b32 2c20 305d            [2, 0]
-00020d80: 2c0a 2020 2e2e 2e20 2020 2020 2020 2020  ,.  ...         
-00020d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020da0: 205b 322c 2031 5d2c 0a20 202e 2e2e 2020   [2, 1],.  ...  
-00020db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020dc0: 2020 2020 2020 2020 5b32 2c20 325d 2c0a          [2, 2],.
-00020dd0: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
-00020de0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00020df0: 332c 2033 5d5d 290a 0a20 204c 6574 2773  3, 3]])..  Let's
-00020e00: 206e 6f77 2064 6566 696e 6520 7468 6520   now define the 
-00020e10: 6163 7475 616c 206c 6179 6572 0a0a 2020  actual layer..  
-00020e20: 3e3e 3e20 6c61 7965 7220 3d20 5765 6176  >>> layer = Weav
-00020e30: 654c 6179 6572 2829 0a0a 2020 416e 6420  eLayer()..  And 
-00020e40: 696e 766f 6b65 2069 740a 0a20 203e 3e3e  invoke it..  >>>
-00020e50: 205b 412c 2050 5d20 3d20 6c61 7965 7228   [A, P] = layer(
-00020e60: 5b61 746f 6d5f 6665 6174 2c20 7061 6972  [atom_feat, pair
-00020e70: 5f66 6561 742c 2070 6169 725f 7370 6c69  _feat, pair_spli
-00020e80: 742c 2061 746f 6d5f 746f 5f70 6169 725d  t, atom_to_pair]
-00020e90: 290a 0a20 2054 6865 2077 6561 7665 206c  )..  The weave l
-00020ea0: 6179 6572 2070 726f 6475 6365 7320 6e65  ayer produces ne
-00020eb0: 7720 6174 6f6d 2f70 6169 7220 6665 6174  w atom/pair feat
-00020ec0: 7572 6573 2e20 4c65 7427 7320 6368 6563  ures. Let's chec
-00020ed0: 6b20 7468 6569 7220 7368 6170 6573 0a0a  k their shapes..
-00020ee0: 2020 3e3e 3e20 4120 3d20 412e 6465 7461    >>> A = A.deta
-00020ef0: 6368 2829 2e6e 756d 7079 2829 0a20 203e  ch().numpy().  >
-00020f00: 3e3e 2041 2e73 6861 7065 0a20 2028 342c  >> A.shape.  (4,
-00020f10: 2035 3029 0a20 203e 3e3e 2050 203d 2050   50).  >>> P = P
-00020f20: 2e64 6574 6163 6828 292e 6e75 6d70 7928  .detach().numpy(
-00020f30: 290a 2020 3e3e 3e20 502e 7368 6170 650a  ).  >>> P.shape.
-00020f40: 2020 2831 302c 2035 3029 0a0a 2020 5468    (10, 50)..  Th
-00020f50: 6520 3420 6973 2060 746f 7461 6c5f 6e75  e 4 is `total_nu
-00020f60: 6d5f 6174 6f6d 7360 2061 6e64 2074 6865  m_atoms` and the
-00020f70: 2031 3020 6973 2074 6865 2074 6f74 616c   10 is the total
-00020f80: 206e 756d 6265 7220 6f66 2070 6169 7273   number of pairs
-00020f90: 2e20 5768 6572 650a 2020 646f 6573 2060  . Where.  does `
-00020fa0: 3530 6020 636f 6d65 2066 726f 6d3f 2049  50` come from? I
-00020fb0: 7427 7320 6672 6f6d 2074 6865 2064 6566  t's from the def
-00020fc0: 6175 6c74 2061 7267 756d 656e 7473 2060  ault arguments `
-00020fd0: 6e5f 6174 6f6d 5f69 6e70 7574 5f66 6561  n_atom_input_fea
-00020fe0: 7460 2061 6e64 0a20 2060 6e5f 7061 6972  t` and.  `n_pair
-00020ff0: 5f69 6e70 7574 5f66 6561 7460 2e0a 0a20  _input_feat`... 
-00021000: 2052 6566 6572 656e 6365 730a 2020 2d2d   References.  --
-00021010: 2d2d 2d2d 2d2d 2d2d 0a20 202e 2e20 5b31  --------.  .. [1
-00021020: 5d20 4b65 6172 6e65 732c 2053 7465 7665  ] Kearnes, Steve
-00021030: 6e2c 2065 7420 616c 2e20 224d 6f6c 6563  n, et al. "Molec
-00021040: 756c 6172 2067 7261 7068 2063 6f6e 766f  ular graph convo
-00021050: 6c75 7469 6f6e 733a 206d 6f76 696e 6720  lutions: moving 
-00021060: 6265 796f 6e64 0a20 2020 2020 2020 2066  beyond.        f
-00021070: 696e 6765 7270 7269 6e74 732e 2220 4a6f  ingerprints." Jo
-00021080: 7572 6e61 6c20 6f66 2063 6f6d 7075 7465  urnal of compute
-00021090: 722d 6169 6465 6420 6d6f 6c65 6375 6c61  r-aided molecula
-000210a0: 7220 6465 7369 676e 2033 302e 3820 2832  r design 30.8 (2
-000210b0: 3031 3629 3a0a 2020 2020 2020 2020 3539  016):.        59
-000210c0: 352d 3630 382e 0a20 2022 2222 0a0a 2020  5-608..  """..  
-000210d0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-000210e0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-000210f0: 2020 2020 2020 6e5f 6174 6f6d 5f69 6e70        n_atom_inp
-00021100: 7574 5f66 6561 743a 2069 6e74 203d 2037  ut_feat: int = 7
-00021110: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00021120: 2020 2020 6e5f 7061 6972 5f69 6e70 7574      n_pair_input
-00021130: 5f66 6561 743a 2069 6e74 203d 2031 342c  _feat: int = 14,
-00021140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021150: 2020 6e5f 6174 6f6d 5f6f 7574 7075 745f    n_atom_output_
-00021160: 6665 6174 3a20 696e 7420 3d20 3530 2c0a  feat: int = 50,.
-00021170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021180: 206e 5f70 6169 725f 6f75 7470 7574 5f66   n_pair_output_f
-00021190: 6561 743a 2069 6e74 203d 2035 302c 0a20  eat: int = 50,. 
-000211a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211b0: 6e5f 6869 6464 656e 5f41 413a 2069 6e74  n_hidden_AA: int
-000211c0: 203d 2035 302c 0a20 2020 2020 2020 2020   = 50,.         
-000211d0: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
-000211e0: 5f50 413a 2069 6e74 203d 2035 302c 0a20  _PA: int = 50,. 
-000211f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021200: 6e5f 6869 6464 656e 5f41 503a 2069 6e74  n_hidden_AP: int
-00021210: 203d 2035 302c 0a20 2020 2020 2020 2020   = 50,.         
-00021220: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
-00021230: 5f50 503a 2069 6e74 203d 2035 302c 0a20  _PP: int = 50,. 
-00021240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021250: 7570 6461 7465 5f70 6169 723a 2062 6f6f  update_pair: boo
-00021260: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
-00021270: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
-00021280: 3a20 7374 7220 3d20 2778 6176 6965 725f  : str = 'xavier_
-00021290: 756e 6966 6f72 6d5f 272c 0a20 2020 2020  uniform_',.     
-000212a0: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-000212b0: 7661 7469 6f6e 3a20 7374 7220 3d20 2772  vation: str = 'r
-000212c0: 656c 7527 2c0a 2020 2020 2020 2020 2020  elu',.          
-000212d0: 2020 2020 2020 2062 6174 6368 5f6e 6f72         batch_nor
-000212e0: 6d61 6c69 7a65 3a20 626f 6f6c 203d 2054  malize: bool = T
-000212f0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00021300: 2020 2020 2020 2a2a 6b77 6172 6773 293a        **kwargs):
-00021310: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00021320: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00021330: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
-00021340: 5f61 746f 6d5f 696e 7075 745f 6665 6174  _atom_input_feat
-00021350: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
-00021360: 2864 6566 6175 6c74 2037 3529 0a20 2020  (default 75).   
-00021370: 2020 204e 756d 6265 7220 6f66 2066 6561     Number of fea
-00021380: 7475 7265 7320 666f 7220 6561 6368 2061  tures for each a
-00021390: 746f 6d20 696e 2069 6e70 7574 2e0a 2020  tom in input..  
-000213a0: 2020 6e5f 7061 6972 5f69 6e70 7574 5f66    n_pair_input_f
-000213b0: 6561 743a 2069 6e74 2c20 6f70 7469 6f6e  eat: int, option
-000213c0: 616c 2028 6465 6661 756c 7420 3134 290a  al (default 14).
-000213d0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
-000213e0: 6665 6174 7572 6573 2066 6f72 2065 6163  features for eac
-000213f0: 6820 7061 6972 206f 6620 6174 6f6d 7320  h pair of atoms 
-00021400: 696e 2069 6e70 7574 2e0a 2020 2020 6e5f  in input..    n_
-00021410: 6174 6f6d 5f6f 7574 7075 745f 6665 6174  atom_output_feat
-00021420: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
-00021430: 2864 6566 6175 6c74 2035 3029 0a20 2020  (default 50).   
-00021440: 2020 204e 756d 6265 7220 6f66 2066 6561     Number of fea
-00021450: 7475 7265 7320 666f 7220 6561 6368 2061  tures for each a
-00021460: 746f 6d20 696e 206f 7574 7075 742e 0a20  tom in output.. 
-00021470: 2020 206e 5f70 6169 725f 6f75 7470 7574     n_pair_output
-00021480: 5f66 6561 743a 2069 6e74 2c20 6f70 7469  _feat: int, opti
-00021490: 6f6e 616c 2028 6465 6661 756c 7420 3530  onal (default 50
-000214a0: 290a 2020 2020 2020 4e75 6d62 6572 206f  ).      Number o
-000214b0: 6620 6665 6174 7572 6573 2066 6f72 2065  f features for e
-000214c0: 6163 6820 7061 6972 206f 6620 6174 6f6d  ach pair of atom
-000214d0: 7320 696e 206f 7574 7075 742e 0a20 2020  s in output..   
-000214e0: 206e 5f68 6964 6465 6e5f 4141 3a20 696e   n_hidden_AA: in
-000214f0: 742c 206f 7074 696f 6e61 6c20 2864 6566  t, optional (def
-00021500: 6175 6c74 2035 3029 0a20 2020 2020 204e  ault 50).      N
-00021510: 756d 6265 7220 6f66 2075 6e69 7473 2863  umber of units(c
-00021520: 6f6e 766f 6c75 7469 6f6e 2064 6570 7468  onvolution depth
-00021530: 7329 2069 6e20 636f 7272 6573 706f 6e64  s) in correspond
-00021540: 696e 6720 6869 6464 656e 206c 6179 6572  ing hidden layer
-00021550: 0a20 2020 206e 5f68 6964 6465 6e5f 5041  .    n_hidden_PA
-00021560: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
-00021570: 2864 6566 6175 6c74 2035 3029 0a20 2020  (default 50).   
-00021580: 2020 204e 756d 6265 7220 6f66 2075 6e69     Number of uni
-00021590: 7473 2863 6f6e 766f 6c75 7469 6f6e 2064  ts(convolution d
-000215a0: 6570 7468 7329 2069 6e20 636f 7272 6573  epths) in corres
-000215b0: 706f 6e64 696e 6720 6869 6464 656e 206c  ponding hidden l
-000215c0: 6179 6572 0a20 2020 206e 5f68 6964 6465  ayer.    n_hidde
-000215d0: 6e5f 4150 3a20 696e 742c 206f 7074 696f  n_AP: int, optio
-000215e0: 6e61 6c20 2864 6566 6175 6c74 2035 3029  nal (default 50)
-000215f0: 0a20 2020 2020 204e 756d 6265 7220 6f66  .      Number of
-00021600: 2075 6e69 7473 2863 6f6e 766f 6c75 7469   units(convoluti
-00021610: 6f6e 2064 6570 7468 7329 2069 6e20 636f  on depths) in co
-00021620: 7272 6573 706f 6e64 696e 6720 6869 6464  rresponding hidd
-00021630: 656e 206c 6179 6572 0a20 2020 206e 5f68  en layer.    n_h
-00021640: 6964 6465 6e5f 5050 3a20 696e 742c 206f  idden_PP: int, o
-00021650: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
-00021660: 2035 3029 0a20 2020 2020 204e 756d 6265   50).      Numbe
-00021670: 7220 6f66 2075 6e69 7473 2863 6f6e 766f  r of units(convo
-00021680: 6c75 7469 6f6e 2064 6570 7468 7329 2069  lution depths) i
-00021690: 6e20 636f 7272 6573 706f 6e64 696e 6720  n corresponding 
-000216a0: 6869 6464 656e 206c 6179 6572 0a20 2020  hidden layer.   
-000216b0: 2075 7064 6174 655f 7061 6972 3a20 626f   update_pair: bo
-000216c0: 6f6c 2c20 6f70 7469 6f6e 616c 2028 6465  ol, optional (de
-000216d0: 6661 756c 7420 5472 7565 290a 2020 2020  fault True).    
-000216e0: 2020 5768 6574 6865 7220 746f 2063 616c    Whether to cal
-000216f0: 6375 6c61 7465 2066 6f72 2070 6169 7220  culate for pair 
-00021700: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
-00021710: 636f 756c 6420 6265 2074 7572 6e65 6420  could be turned 
-00021720: 6f66 6620 666f 7220 6c61 7374 206c 6179  off for last lay
-00021730: 6572 0a20 2020 2069 6e69 743a 2073 7472  er.    init: str
-00021740: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
-00021750: 756c 7420 2778 6176 6965 725f 756e 6966  ult 'xavier_unif
-00021760: 6f72 6d5f 2729 0a20 2020 2020 2057 6569  orm_').      Wei
-00021770: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
-00021780: 6f6e 2066 6f72 2066 696c 7465 7273 2e0a  on for filters..
-00021790: 2020 2020 6163 7469 7661 7469 6f6e 3a20      activation: 
-000217a0: 7374 722c 206f 7074 696f 6e61 6c20 2864  str, optional (d
-000217b0: 6566 6175 6c74 2027 7265 6c75 2729 0a20  efault 'relu'). 
-000217c0: 2020 2020 2041 6374 6976 6174 696f 6e20       Activation 
-000217d0: 6675 6e63 7469 6f6e 2061 7070 6c69 6564  function applied
-000217e0: 0a20 2020 2062 6174 6368 5f6e 6f72 6d61  .    batch_norma
-000217f0: 6c69 7a65 3a20 626f 6f6c 2c20 6f70 7469  lize: bool, opti
-00021800: 6f6e 616c 2028 6465 6661 756c 7420 5472  onal (default Tr
-00021810: 7565 290a 2020 2020 2020 4966 2074 6869  ue).      If thi
-00021820: 7320 6973 2074 7572 6e65 6420 6f6e 2c20  s is turned on, 
-00021830: 6170 706c 7920 6261 7463 6820 6e6f 726d  apply batch norm
-00021840: 616c 697a 6174 696f 6e20 6265 666f 7265  alization before
-00021850: 2061 7070 6c79 696e 670a 2020 2020 2020   applying.      
-00021860: 6163 7469 7661 7469 6f6e 2066 756e 6374  activation funct
-00021870: 696f 6e73 206f 6e20 636f 6e76 6f6c 7574  ions on convolut
-00021880: 696f 6e61 6c20 6c61 7965 7273 2e0a 2020  ional layers..  
-00021890: 2020 2222 220a 2020 2020 2020 2020 7375    """.        su
-000218a0: 7065 7228 5765 6176 654c 6179 6572 2c20  per(WeaveLayer, 
-000218b0: 7365 6c66 292e 5f5f 696e 6974 5f5f 282a  self).__init__(*
-000218c0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
-000218d0: 2073 656c 662e 696e 6974 3a20 7374 7220   self.init: str 
-000218e0: 3d20 696e 6974 5f20 2023 2053 6574 2077  = init_  # Set w
-000218f0: 6569 6768 7420 696e 6974 6961 6c69 7a61  eight initializa
-00021900: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
-00021910: 662e 6163 7469 7661 7469 6f6e 3a20 7374  f.activation: st
-00021920: 7220 3d20 6163 7469 7661 7469 6f6e 2020  r = activation  
-00021930: 2320 4765 7420 6163 7469 7661 7469 6f6e  # Get activation
-00021940: 730a 2020 2020 2020 2020 7365 6c66 2e61  s.        self.a
-00021950: 6374 6976 6174 696f 6e5f 666e 3a20 746f  ctivation_fn: to
-00021960: 7263 682e 6e6e 2e4d 6f64 756c 6520 3d20  rch.nn.Module = 
-00021970: 6765 745f 6163 7469 7661 7469 6f6e 2861  get_activation(a
-00021980: 6374 6976 6174 696f 6e29 0a20 2020 2020  ctivation).     
-00021990: 2020 2073 656c 662e 7570 6461 7465 5f70     self.update_p
-000219a0: 6169 723a 2062 6f6f 6c20 3d20 7570 6461  air: bool = upda
-000219b0: 7465 5f70 6169 7220 2023 206c 6173 7420  te_pair  # last 
-000219c0: 7765 6176 6520 6c61 7965 7220 646f 6573  weave layer does
-000219d0: 206e 6f74 206e 6565 6420 746f 2075 7064   not need to upd
-000219e0: 6174 650a 2020 2020 2020 2020 7365 6c66  ate.        self
-000219f0: 2e6e 5f68 6964 6465 6e5f 4141 3a20 696e  .n_hidden_AA: in
-00021a00: 7420 3d20 6e5f 6869 6464 656e 5f41 410a  t = n_hidden_AA.
-00021a10: 2020 2020 2020 2020 7365 6c66 2e6e 5f68          self.n_h
-00021a20: 6964 6465 6e5f 5041 3a20 696e 7420 3d20  idden_PA: int = 
-00021a30: 6e5f 6869 6464 656e 5f50 410a 2020 2020  n_hidden_PA.    
-00021a40: 2020 2020 7365 6c66 2e6e 5f68 6964 6465      self.n_hidde
-00021a50: 6e5f 4150 3a20 696e 7420 3d20 6e5f 6869  n_AP: int = n_hi
-00021a60: 6464 656e 5f41 500a 2020 2020 2020 2020  dden_AP.        
-00021a70: 7365 6c66 2e6e 5f68 6964 6465 6e5f 5050  self.n_hidden_PP
-00021a80: 3a20 696e 7420 3d20 6e5f 6869 6464 656e  : int = n_hidden
-00021a90: 5f50 500a 2020 2020 2020 2020 7365 6c66  _PP.        self
-00021aa0: 2e6e 5f68 6964 6465 6e5f 413a 2069 6e74  .n_hidden_A: int
-00021ab0: 203d 206e 5f68 6964 6465 6e5f 4141 202b   = n_hidden_AA +
-00021ac0: 206e 5f68 6964 6465 6e5f 5041 0a20 2020   n_hidden_PA.   
-00021ad0: 2020 2020 2073 656c 662e 6e5f 6869 6464       self.n_hidd
-00021ae0: 656e 5f50 3a20 696e 7420 3d20 6e5f 6869  en_P: int = n_hi
-00021af0: 6464 656e 5f41 5020 2b20 6e5f 6869 6464  dden_AP + n_hidd
-00021b00: 656e 5f50 500a 2020 2020 2020 2020 7365  en_PP.        se
-00021b10: 6c66 2e62 6174 6368 5f6e 6f72 6d61 6c69  lf.batch_normali
-00021b20: 7a65 3a20 626f 6f6c 203d 2062 6174 6368  ze: bool = batch
-00021b30: 5f6e 6f72 6d61 6c69 7a65 0a0a 2020 2020  _normalize..    
-00021b40: 2020 2020 7365 6c66 2e6e 5f61 746f 6d5f      self.n_atom_
-00021b50: 696e 7075 745f 6665 6174 3a20 696e 7420  input_feat: int 
-00021b60: 3d20 6e5f 6174 6f6d 5f69 6e70 7574 5f66  = n_atom_input_f
-00021b70: 6561 740a 2020 2020 2020 2020 7365 6c66  eat.        self
-00021b80: 2e6e 5f70 6169 725f 696e 7075 745f 6665  .n_pair_input_fe
-00021b90: 6174 3a20 696e 7420 3d20 6e5f 7061 6972  at: int = n_pair
-00021ba0: 5f69 6e70 7574 5f66 6561 740a 2020 2020  _input_feat.    
-00021bb0: 2020 2020 7365 6c66 2e6e 5f61 746f 6d5f      self.n_atom_
-00021bc0: 6f75 7470 7574 5f66 6561 743a 2069 6e74  output_feat: int
-00021bd0: 203d 206e 5f61 746f 6d5f 6f75 7470 7574   = n_atom_output
-00021be0: 5f66 6561 740a 2020 2020 2020 2020 7365  _feat.        se
-00021bf0: 6c66 2e6e 5f70 6169 725f 6f75 7470 7574  lf.n_pair_output
-00021c00: 5f66 6561 743a 2069 6e74 203d 206e 5f70  _feat: int = n_p
-00021c10: 6169 725f 6f75 7470 7574 5f66 6561 740a  air_output_feat.
-00021c20: 0a20 2020 2020 2020 2023 2043 6f6e 7374  .        # Const
-00021c30: 7275 6374 2069 6e74 6572 6e61 6c20 7472  ruct internal tr
-00021c40: 6169 6e61 626c 6520 7765 6967 6874 730a  ainable weights.
-00021c50: 2020 2020 2020 2020 696e 6974 203d 2067          init = g
-00021c60: 6574 6174 7472 2869 6e69 7469 616c 697a  etattr(initializ
-00021c70: 6572 732c 2073 656c 662e 696e 6974 290a  ers, self.init).
-00021c80: 2020 2020 2020 2020 2320 5765 6967 6874          # Weight
-00021c90: 206d 6174 7269 7820 616e 6420 6269 6173   matrix and bias
-00021ca0: 206d 6174 7269 7820 7265 7175 6972 6564   matrix required
-00021cb0: 2074 6f20 636f 6d70 7574 6520 6e65 7720   to compute new 
-00021cc0: 6174 6f6d 206c 6179 6572 2066 726f 6d20  atom layer from 
-00021cd0: 7468 6520 7072 6576 696f 7573 2061 746f  the previous ato
-00021ce0: 6d20 6c61 7965 720a 2020 2020 2020 2020  m layer.        
-00021cf0: 7365 6c66 2e57 5f41 413a 2074 6f72 6368  self.W_AA: torch
-00021d00: 2e54 656e 736f 7220 3d20 696e 6974 280a  .Tensor = init(.
-00021d10: 2020 2020 2020 2020 2020 2020 746f 7263              torc
-00021d20: 682e 656d 7074 7928 7365 6c66 2e6e 5f61  h.empty(self.n_a
-00021d30: 746f 6d5f 696e 7075 745f 6665 6174 2c20  tom_input_feat, 
-00021d40: 7365 6c66 2e6e 5f68 6964 6465 6e5f 4141  self.n_hidden_AA
-00021d50: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00021d60: 625f 4141 3a20 746f 7263 682e 5465 6e73  b_AA: torch.Tens
-00021d70: 6f72 203d 2074 6f72 6368 2e7a 6572 6f73  or = torch.zeros
-00021d80: 2828 7365 6c66 2e6e 5f68 6964 6465 6e5f  ((self.n_hidden_
-00021d90: 4141 2c29 290a 2020 2020 2020 2020 7365  AA,)).        se
-00021da0: 6c66 2e41 415f 626e 3a20 6e6e 2e42 6174  lf.AA_bn: nn.Bat
-00021db0: 6368 4e6f 726d 3164 203d 206e 6e2e 4261  chNorm1d = nn.Ba
-00021dc0: 7463 684e 6f72 6d31 6428 0a20 2020 2020  tchNorm1d(.     
-00021dd0: 2020 2020 2020 206e 756d 5f66 6561 7475         num_featu
-00021de0: 7265 733d 7365 6c66 2e6e 5f68 6964 6465  res=self.n_hidde
-00021df0: 6e5f 4141 2c0a 2020 2020 2020 2020 2020  n_AA,.          
-00021e00: 2020 6570 733d 3165 2d33 2c0a 2020 2020    eps=1e-3,.    
-00021e10: 2020 2020 2020 2020 6d6f 6d65 6e74 756d          momentum
-00021e20: 3d30 2e39 392c 0a20 2020 2020 2020 2020  =0.99,.         
-00021e30: 2020 2061 6666 696e 653d 5472 7565 2c0a     affine=True,.
-00021e40: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00021e50: 6b5f 7275 6e6e 696e 675f 7374 6174 733d  k_running_stats=
-00021e60: 5472 7565 290a 0a20 2020 2020 2020 2023  True)..        #
-00021e70: 2057 6569 6768 7420 6d61 7472 6978 2061   Weight matrix a
-00021e80: 6e64 2062 6961 7320 6d61 7472 6978 2072  nd bias matrix r
-00021e90: 6571 7569 7265 6420 746f 2063 6f6d 7075  equired to compu
-00021ea0: 7465 206e 6577 2061 746f 6d20 6c61 7965  te new atom laye
-00021eb0: 7220 6672 6f6d 2074 6865 2070 7265 7669  r from the previ
-00021ec0: 6f75 7320 7061 6972 206c 6179 6572 0a20  ous pair layer. 
-00021ed0: 2020 2020 2020 2073 656c 662e 575f 5041         self.W_PA
-00021ee0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00021ef0: 2069 6e69 7428 0a20 2020 2020 2020 2020   init(.         
-00021f00: 2020 2074 6f72 6368 2e65 6d70 7479 2873     torch.empty(s
-00021f10: 656c 662e 6e5f 7061 6972 5f69 6e70 7574  elf.n_pair_input
-00021f20: 5f66 6561 742c 2073 656c 662e 6e5f 6869  _feat, self.n_hi
-00021f30: 6464 656e 5f50 4129 290a 2020 2020 2020  dden_PA)).      
-00021f40: 2020 7365 6c66 2e62 5f50 413a 2074 6f72    self.b_PA: tor
-00021f50: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
-00021f60: 682e 7a65 726f 7328 2873 656c 662e 6e5f  h.zeros((self.n_
-00021f70: 6869 6464 656e 5f50 412c 2929 0a20 2020  hidden_PA,)).   
-00021f80: 2020 2020 2073 656c 662e 5041 5f62 6e3a       self.PA_bn:
-00021f90: 206e 6e2e 4261 7463 684e 6f72 6d31 6420   nn.BatchNorm1d 
-00021fa0: 3d20 6e6e 2e42 6174 6368 4e6f 726d 3164  = nn.BatchNorm1d
-00021fb0: 280a 2020 2020 2020 2020 2020 2020 6e75  (.            nu
-00021fc0: 6d5f 6665 6174 7572 6573 3d73 656c 662e  m_features=self.
-00021fd0: 6e5f 6869 6464 656e 5f50 412c 0a20 2020  n_hidden_PA,.   
-00021fe0: 2020 2020 2020 2020 2065 7073 3d31 652d           eps=1e-
-00021ff0: 332c 0a20 2020 2020 2020 2020 2020 206d  3,.            m
-00022000: 6f6d 656e 7475 6d3d 302e 3939 2c0a 2020  omentum=0.99,.  
-00022010: 2020 2020 2020 2020 2020 6166 6669 6e65            affine
-00022020: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00022030: 2020 2074 7261 636b 5f72 756e 6e69 6e67     track_running
-00022040: 5f73 7461 7473 3d54 7275 6529 0a0a 2020  _stats=True)..  
-00022050: 2020 2020 2020 7365 6c66 2e57 5f41 3a20        self.W_A: 
-00022060: 746f 7263 682e 5465 6e73 6f72 203d 2069  torch.Tensor = i
-00022070: 6e69 7428 0a20 2020 2020 2020 2020 2020  nit(.           
-00022080: 2074 6f72 6368 2e65 6d70 7479 2873 656c   torch.empty(sel
-00022090: 662e 6e5f 6869 6464 656e 5f41 2c20 7365  f.n_hidden_A, se
-000220a0: 6c66 2e6e 5f61 746f 6d5f 6f75 7470 7574  lf.n_atom_output
-000220b0: 5f66 6561 7429 290a 2020 2020 2020 2020  _feat)).        
-000220c0: 7365 6c66 2e62 5f41 3a20 746f 7263 682e  self.b_A: torch.
-000220d0: 5465 6e73 6f72 203d 2074 6f72 6368 2e7a  Tensor = torch.z
-000220e0: 6572 6f73 2828 7365 6c66 2e6e 5f61 746f  eros((self.n_ato
-000220f0: 6d5f 6f75 7470 7574 5f66 6561 742c 2929  m_output_feat,))
-00022100: 0a20 2020 2020 2020 2073 656c 662e 415f  .        self.A_
-00022110: 626e 3a20 6e6e 2e42 6174 6368 4e6f 726d  bn: nn.BatchNorm
-00022120: 3164 203d 206e 6e2e 4261 7463 684e 6f72  1d = nn.BatchNor
-00022130: 6d31 6428 0a20 2020 2020 2020 2020 2020  m1d(.           
-00022140: 206e 756d 5f66 6561 7475 7265 733d 7365   num_features=se
-00022150: 6c66 2e6e 5f61 746f 6d5f 6f75 7470 7574  lf.n_atom_output
-00022160: 5f66 6561 742c 0a20 2020 2020 2020 2020  _feat,.         
-00022170: 2020 2065 7073 3d31 652d 332c 0a20 2020     eps=1e-3,.   
-00022180: 2020 2020 2020 2020 206d 6f6d 656e 7475           momentu
-00022190: 6d3d 302e 3939 2c0a 2020 2020 2020 2020  m=0.99,.        
-000221a0: 2020 2020 6166 6669 6e65 3d54 7275 652c      affine=True,
-000221b0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-000221c0: 636b 5f72 756e 6e69 6e67 5f73 7461 7473  ck_running_stats
-000221d0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-000221e0: 6966 2073 656c 662e 7570 6461 7465 5f70  if self.update_p
-000221f0: 6169 723a 0a20 2020 2020 2020 2020 2020  air:.           
-00022200: 2023 2057 6569 6768 7420 6d61 7472 6978   # Weight matrix
-00022210: 2061 6e64 2062 6961 7320 6d61 7472 6978   and bias matrix
-00022220: 2072 6571 7569 7265 6420 746f 2063 6f6d   required to com
-00022230: 7075 7465 206e 6577 2070 6169 7220 6c61  pute new pair la
-00022240: 7965 7220 6672 6f6d 2074 6865 2070 7265  yer from the pre
-00022250: 7669 6f75 7320 6174 6f6d 206c 6179 6572  vious atom layer
-00022260: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00022270: 662e 575f 4150 3a20 746f 7263 682e 5465  f.W_AP: torch.Te
-00022280: 6e73 6f72 203d 2069 6e69 7428 0a20 2020  nsor = init(.   
-00022290: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
-000222a0: 6368 2e65 6d70 7479 2873 656c 662e 6e5f  ch.empty(self.n_
-000222b0: 6174 6f6d 5f69 6e70 7574 5f66 6561 7420  atom_input_feat 
-000222c0: 2a20 322c 2073 656c 662e 6e5f 6869 6464  * 2, self.n_hidd
-000222d0: 656e 5f41 5029 290a 2020 2020 2020 2020  en_AP)).        
-000222e0: 2020 2020 7365 6c66 2e62 5f41 503a 2074      self.b_AP: t
-000222f0: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
-00022300: 7263 682e 7a65 726f 7328 2873 656c 662e  rch.zeros((self.
-00022310: 6e5f 6869 6464 656e 5f41 502c 2929 0a20  n_hidden_AP,)). 
-00022320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00022330: 4150 5f62 6e3a 206e 6e2e 4261 7463 684e  AP_bn: nn.BatchN
-00022340: 6f72 6d31 6420 3d20 6e6e 2e42 6174 6368  orm1d = nn.Batch
-00022350: 4e6f 726d 3164 280a 2020 2020 2020 2020  Norm1d(.        
-00022360: 2020 2020 2020 2020 6e75 6d5f 6665 6174          num_feat
-00022370: 7572 6573 3d73 656c 662e 6e5f 6869 6464  ures=self.n_hidd
-00022380: 656e 5f41 502c 0a20 2020 2020 2020 2020  en_AP,.         
-00022390: 2020 2020 2020 2065 7073 3d31 652d 332c         eps=1e-3,
-000223a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000223b0: 206d 6f6d 656e 7475 6d3d 302e 3939 2c0a   momentum=0.99,.
-000223c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000223d0: 6166 6669 6e65 3d54 7275 652c 0a20 2020  affine=True,.   
-000223e0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-000223f0: 636b 5f72 756e 6e69 6e67 5f73 7461 7473  ck_running_stats
-00022400: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00022410: 2020 2023 2057 6569 6768 7420 6d61 7472     # Weight matr
-00022420: 6978 2061 6e64 2062 6961 7320 6d61 7472  ix and bias matr
-00022430: 6978 2072 6571 7569 7265 6420 746f 2063  ix required to c
-00022440: 6f6d 7075 7465 206e 6577 2070 6169 7220  ompute new pair 
-00022450: 6c61 7965 7220 6672 6f6d 2074 6865 2070  layer from the p
-00022460: 7265 7669 6f75 7320 7061 6972 206c 6179  revious pair lay
-00022470: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
-00022480: 656c 662e 575f 5050 3a20 746f 7263 682e  elf.W_PP: torch.
-00022490: 5465 6e73 6f72 203d 2069 6e69 7428 0a20  Tensor = init(. 
-000224a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000224b0: 6f72 6368 2e65 6d70 7479 2873 656c 662e  orch.empty(self.
-000224c0: 6e5f 7061 6972 5f69 6e70 7574 5f66 6561  n_pair_input_fea
-000224d0: 742c 2073 656c 662e 6e5f 6869 6464 656e  t, self.n_hidden
-000224e0: 5f50 5029 290a 2020 2020 2020 2020 2020  _PP)).          
-000224f0: 2020 7365 6c66 2e62 5f50 503a 2074 6f72    self.b_PP: tor
-00022500: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
-00022510: 682e 7a65 726f 7328 2873 656c 662e 6e5f  h.zeros((self.n_
-00022520: 6869 6464 656e 5f50 502c 2929 0a20 2020  hidden_PP,)).   
-00022530: 2020 2020 2020 2020 2073 656c 662e 5050           self.PP
-00022540: 5f62 6e3a 206e 6e2e 4261 7463 684e 6f72  _bn: nn.BatchNor
-00022550: 6d31 6420 3d20 6e6e 2e42 6174 6368 4e6f  m1d = nn.BatchNo
-00022560: 726d 3164 280a 2020 2020 2020 2020 2020  rm1d(.          
-00022570: 2020 2020 2020 6e75 6d5f 6665 6174 7572        num_featur
-00022580: 6573 3d73 656c 662e 6e5f 6869 6464 656e  es=self.n_hidden
-00022590: 5f50 502c 0a20 2020 2020 2020 2020 2020  _PP,.           
-000225a0: 2020 2020 2065 7073 3d31 652d 332c 0a20       eps=1e-3,. 
-000225b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000225c0: 6f6d 656e 7475 6d3d 302e 3939 2c0a 2020  omentum=0.99,.  
-000225d0: 2020 2020 2020 2020 2020 2020 2020 6166                af
-000225e0: 6669 6e65 3d54 7275 652c 0a20 2020 2020  fine=True,.     
-000225f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00022600: 5f72 756e 6e69 6e67 5f73 7461 7473 3d54  _running_stats=T
-00022610: 7275 6529 0a0a 2020 2020 2020 2020 2020  rue)..          
-00022620: 2020 7365 6c66 2e57 5f50 3a20 746f 7263    self.W_P: torc
-00022630: 682e 5465 6e73 6f72 203d 2069 6e69 7428  h.Tensor = init(
-00022640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022650: 2074 6f72 6368 2e65 6d70 7479 2873 656c   torch.empty(sel
-00022660: 662e 6e5f 6869 6464 656e 5f50 2c20 7365  f.n_hidden_P, se
-00022670: 6c66 2e6e 5f70 6169 725f 6f75 7470 7574  lf.n_pair_output
-00022680: 5f66 6561 7429 290a 2020 2020 2020 2020  _feat)).        
-00022690: 2020 2020 7365 6c66 2e62 5f50 3a20 746f      self.b_P: to
-000226a0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
-000226b0: 6368 2e7a 6572 6f73 2828 7365 6c66 2e6e  ch.zeros((self.n
-000226c0: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
-000226d0: 742c 2929 0a20 2020 2020 2020 2020 2020  t,)).           
-000226e0: 2073 656c 662e 505f 626e 3a20 6e6e 2e42   self.P_bn: nn.B
-000226f0: 6174 6368 4e6f 726d 3164 203d 206e 6e2e  atchNorm1d = nn.
-00022700: 4261 7463 684e 6f72 6d31 6428 0a20 2020  BatchNorm1d(.   
-00022710: 2020 2020 2020 2020 2020 2020 206e 756d               num
-00022720: 5f66 6561 7475 7265 733d 7365 6c66 2e6e  _features=self.n
-00022730: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
-00022740: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00022750: 2020 2065 7073 3d31 652d 332c 0a20 2020     eps=1e-3,.   
-00022760: 2020 2020 2020 2020 2020 2020 206d 6f6d               mom
-00022770: 656e 7475 6d3d 302e 3939 2c0a 2020 2020  entum=0.99,.    
-00022780: 2020 2020 2020 2020 2020 2020 6166 6669              affi
-00022790: 6e65 3d54 7275 652c 0a20 2020 2020 2020  ne=True,.       
-000227a0: 2020 2020 2020 2020 2074 7261 636b 5f72           track_r
-000227b0: 756e 6e69 6e67 5f73 7461 7473 3d54 7275  unning_stats=Tru
-000227c0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-000227d0: 6275 696c 7420 3d20 5472 7565 0a0a 2020  built = True..  
-000227e0: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-000227f0: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-00022800: 2020 2020 2022 2222 0a20 2020 2052 6574       """.    Ret
-00022810: 7572 6e73 2061 2073 7472 696e 6720 7265  urns a string re
-00022820: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-00022830: 7468 6520 6f62 6a65 6374 2e0a 0a20 2020  the object...   
-00022840: 2052 6574 7572 6e73 3a0a 2020 2020 2d2d   Returns:.    --
-00022850: 2d2d 2d2d 2d0a 2020 2020 7374 723a 2041  -----.    str: A
-00022860: 2073 7472 696e 6720 7468 6174 2063 6f6e   string that con
-00022870: 7461 696e 7320 7468 6520 636c 6173 7320  tains the class 
-00022880: 6e61 6d65 2066 6f6c 6c6f 7765 6420 6279  name followed by
-00022890: 2074 6865 2076 616c 7565 7320 6f66 2069   the values of i
-000228a0: 7473 2069 6e73 7461 6e63 6520 7661 7269  ts instance vari
-000228b0: 6162 6c65 2e0a 2020 2020 2222 220a 2020  able..    """.  
-000228c0: 2020 2020 2020 2320 666c 616b 6538 3a20        # flake8: 
-000228d0: 6e6f 7161 0a20 2020 2020 2020 2072 6574  noqa.        ret
-000228e0: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
-000228f0: 2020 6627 7b73 656c 662e 5f5f 636c 6173    f'{self.__clas
-00022900: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d28 6e5f  s__.__name__}(n_
-00022910: 6174 6f6d 5f69 6e70 7574 5f66 6561 743a  atom_input_feat:
-00022920: 7b73 656c 662e 6e5f 6174 6f6d 5f69 6e70  {self.n_atom_inp
-00022930: 7574 5f66 6561 747d 2c6e 5f70 6169 725f  ut_feat},n_pair_
-00022940: 696e 7075 745f 6665 6174 3a7b 7365 6c66  input_feat:{self
-00022950: 2e6e 5f70 6169 725f 696e 7075 745f 6665  .n_pair_input_fe
-00022960: 6174 7d2c 6e5f 6174 6f6d 5f6f 7574 7075  at},n_atom_outpu
-00022970: 745f 6665 6174 3a7b 7365 6c66 2e6e 5f61  t_feat:{self.n_a
-00022980: 746f 6d5f 6f75 7470 7574 5f66 6561 747d  tom_output_feat}
-00022990: 2c6e 5f70 6169 725f 6f75 7470 7574 5f66  ,n_pair_output_f
-000229a0: 6561 743a 7b73 656c 662e 6e5f 7061 6972  eat:{self.n_pair
-000229b0: 5f6f 7574 7075 745f 6665 6174 7d2c 6e5f  _output_feat},n_
-000229c0: 6869 6464 656e 5f41 413a 7b73 656c 662e  hidden_AA:{self.
-000229d0: 6e5f 6869 6464 656e 5f41 417d 2c6e 5f68  n_hidden_AA},n_h
-000229e0: 6964 6465 6e5f 5041 3a7b 7365 6c66 2e6e  idden_PA:{self.n
-000229f0: 5f68 6964 6465 6e5f 5041 7d2c 6e5f 6869  _hidden_PA},n_hi
-00022a00: 6464 656e 5f41 503a 7b73 656c 662e 6e5f  dden_AP:{self.n_
-00022a10: 6869 6464 656e 5f41 507d 2c6e 5f68 6964  hidden_AP},n_hid
-00022a20: 6465 6e5f 5050 3a7b 7365 6c66 2e6e 5f68  den_PP:{self.n_h
-00022a30: 6964 6465 6e5f 5050 7d2c 6261 7463 685f  idden_PP},batch_
-00022a40: 6e6f 726d 616c 697a 653a 7b73 656c 662e  normalize:{self.
-00022a50: 6261 7463 685f 6e6f 726d 616c 697a 657d  batch_normalize}
-00022a60: 2c75 7064 6174 655f 7061 6972 3a7b 7365  ,update_pair:{se
-00022a70: 6c66 2e75 7064 6174 655f 7061 6972 7d2c  lf.update_pair},
-00022a80: 696e 6974 3a7b 7365 6c66 2e69 6e69 747d  init:{self.init}
-00022a90: 2c61 6374 6976 6174 696f 6e3a 7b73 656c  ,activation:{sel
-00022aa0: 662e 6163 7469 7661 7469 6f6e 7d29 270a  f.activation})'.
-00022ab0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00022ac0: 6566 2066 6f72 7761 7264 280a 2020 2020  ef forward(.    
-00022ad0: 2020 2020 7365 6c66 2c20 696e 7075 7473      self, inputs
-00022ae0: 3a20 4c69 7374 5b55 6e69 6f6e 5b6e 702e  : List[Union[np.
-00022af0: 6e64 6172 7261 792c 206e 702e 6e64 6172  ndarray, np.ndar
-00022b00: 7261 792c 206e 702e 6e64 6172 7261 792c  ray, np.ndarray,
-00022b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b30: 2020 6e70 2e6e 6461 7272 6179 5d5d 0a20    np.ndarray]]. 
-00022b40: 2020 2029 202d 3e20 4c69 7374 5b55 6e69     ) -> List[Uni
-00022b50: 6f6e 5b74 6f72 6368 2e54 656e 736f 722c  on[torch.Tensor,
-00022b60: 2074 6f72 6368 2e54 656e 736f 725d 5d3a   torch.Tensor]]:
-00022b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00022b80: 2043 7265 6174 6573 2077 6561 7665 2074   Creates weave t
-00022b90: 656e 736f 7273 2e0a 0a20 2020 2050 6172  ensors...    Par
-00022ba0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00022bb0: 2d2d 2d2d 2d2d 0a20 2020 2069 6e70 7574  ------.    input
-00022bc0: 733a 204c 6973 745b 556e 696f 6e5b 6e70  s: List[Union[np
-00022bd0: 2e6e 6461 7272 6179 2c20 6e70 2e6e 6461  .ndarray, np.nda
-00022be0: 7272 6179 2c20 6e70 2e6e 6461 7272 6179  rray, np.ndarray
-00022bf0: 2c20 6e70 2e6e 6461 7272 6179 5d5d 0a20  , np.ndarray]]. 
-00022c00: 2020 2053 686f 756c 6420 636f 6e74 6169     Should contai
-00022c10: 6e20 3420 7465 6e73 6f72 7320 5b61 746f  n 4 tensors [ato
-00022c20: 6d5f 6665 6174 7572 6573 2c20 7061 6972  m_features, pair
-00022c30: 5f66 6561 7475 7265 732c 2070 6169 725f  _features, pair_
-00022c40: 7370 6c69 742c 0a20 2020 2061 746f 6d5f  split,.    atom_
-00022c50: 746f 5f70 6169 725d 0a0a 2020 2020 5265  to_pair]..    Re
-00022c60: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
-00022c70: 2d2d 0a20 2020 204c 6973 745b 556e 696f  --.    List[Unio
-00022c80: 6e5b 746f 7263 682e 5465 6e73 6f72 2c20  n[torch.Tensor, 
-00022c90: 746f 7263 682e 5465 6e73 6f72 5d5d 0a20  torch.Tensor]]. 
-00022ca0: 2020 2020 2041 3a20 4174 6f6d 2066 6561       A: Atom fea
-00022cb0: 7475 7265 7320 7465 6e73 6f72 2077 6974  tures tensor wit
-00022cc0: 6820 7368 6170 655b 746f 7461 6c5f 6e75  h shape[total_nu
-00022cd0: 6d5f 6174 6f6d 732c 6174 6f6d 2066 6561  m_atoms,atom fea
-00022ce0: 7475 7265 2073 697a 655d 0a20 2020 2020  ture size].     
-00022cf0: 2050 3a20 5061 6972 2066 6561 7475 7265   P: Pair feature
-00022d00: 7320 7465 6e73 6f72 2077 6974 6820 7368  s tensor with sh
-00022d10: 6170 655b 746f 7461 6c20 6e75 6d20 6f66  ape[total num of
-00022d20: 2070 6169 7273 2c62 6f6e 6420 6665 6174   pairs,bond feat
-00022d30: 7572 6520 7369 7a65 5d0a 2020 2020 2222  ure size].    ""
-00022d40: 220a 2020 2020 2020 2020 2320 436f 6e76  ".        # Conv
-00022d50: 6572 7469 6e67 2074 6865 2069 6e70 7574  erting the input
-00022d60: 2074 6f20 746f 7263 6820 7465 6e73 6f72   to torch tensor
-00022d70: 730a 2020 2020 2020 2020 6174 6f6d 5f66  s.        atom_f
-00022d80: 6561 7475 7265 733a 2074 6f72 6368 2e54  eatures: torch.T
-00022d90: 656e 736f 7220 3d20 746f 7263 682e 7465  ensor = torch.te
-00022da0: 6e73 6f72 2869 6e70 7574 735b 305d 290a  nsor(inputs[0]).
-00022db0: 2020 2020 2020 2020 7061 6972 5f66 6561          pair_fea
-00022dc0: 7475 7265 733a 2074 6f72 6368 2e54 656e  tures: torch.Ten
-00022dd0: 736f 7220 3d20 746f 7263 682e 7465 6e73  sor = torch.tens
-00022de0: 6f72 2869 6e70 7574 735b 315d 290a 0a20  or(inputs[1]).. 
-00022df0: 2020 2020 2020 2070 6169 725f 7370 6c69         pair_spli
-00022e00: 743a 2074 6f72 6368 2e54 656e 736f 7220  t: torch.Tensor 
-00022e10: 3d20 746f 7263 682e 7465 6e73 6f72 2869  = torch.tensor(i
-00022e20: 6e70 7574 735b 325d 290a 2020 2020 2020  nputs[2]).      
-00022e30: 2020 6174 6f6d 5f74 6f5f 7061 6972 3a20    atom_to_pair: 
-00022e40: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
-00022e50: 6f72 6368 2e74 656e 736f 7228 696e 7075  orch.tensor(inpu
-00022e60: 7473 5b33 5d29 0a0a 2020 2020 2020 2020  ts[3])..        
-00022e70: 6163 7469 7661 7469 6f6e 203d 2073 656c  activation = sel
-00022e80: 662e 6163 7469 7661 7469 6f6e 5f66 6e0a  f.activation_fn.
-00022e90: 0a20 2020 2020 2020 2023 2041 4120 6973  .        # AA is
-00022ea0: 2061 2074 656e 736f 7220 7769 7468 2073   a tensor with s
-00022eb0: 6861 7065 5b74 6f74 616c 5f6e 756d 5f61  hape[total_num_a
-00022ec0: 746f 6d73 2c6e 5f68 6964 6465 6e5f 4141  toms,n_hidden_AA
-00022ed0: 5d0a 2020 2020 2020 2020 4141 3a20 746f  ].        AA: to
-00022ee0: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
-00022ef0: 6368 2e6d 6174 6d75 6c28 6174 6f6d 5f66  ch.matmul(atom_f
-00022f00: 6561 7475 7265 732e 7479 7065 2874 6f72  eatures.type(tor
-00022f10: 6368 2e66 6c6f 6174 3332 292c 0a20 2020  ch.float32),.   
-00022f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f40: 2020 2020 2073 656c 662e 575f 4141 2920       self.W_AA) 
-00022f50: 2b20 7365 6c66 2e62 5f41 410a 2020 2020  + self.b_AA.    
-00022f60: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
-00022f70: 685f 6e6f 726d 616c 697a 653a 0a20 2020  h_normalize:.   
-00022f80: 2020 2020 2020 2020 2073 656c 662e 4141           self.AA
-00022f90: 5f62 6e2e 6576 616c 2829 0a20 2020 2020  _bn.eval().     
-00022fa0: 2020 2020 2020 2041 4120 3d20 7365 6c66         AA = self
-00022fb0: 2e41 415f 626e 2841 4129 0a20 2020 2020  .AA_bn(AA).     
-00022fc0: 2020 2041 4120 3d20 6163 7469 7661 7469     AA = activati
-00022fd0: 6f6e 2841 4129 0a20 2020 2020 2020 2023  on(AA).        #
-00022fe0: 2050 4120 6973 2061 2074 656e 736f 7220   PA is a tensor 
-00022ff0: 7769 7468 2073 6861 7065 5b74 6f74 616c  with shape[total
-00023000: 206e 756d 6265 7220 6f66 2070 6169 7273   number of pairs
-00023010: 2c6e 5f68 6964 6465 6e5f 5041 5d0a 2020  ,n_hidden_PA].  
-00023020: 2020 2020 2020 5041 3a20 746f 7263 682e        PA: torch.
-00023030: 5465 6e73 6f72 203d 2074 6f72 6368 2e6d  Tensor = torch.m
-00023040: 6174 6d75 6c28 7061 6972 5f66 6561 7475  atmul(pair_featu
-00023050: 7265 732e 7479 7065 2874 6f72 6368 2e66  res.type(torch.f
-00023060: 6c6f 6174 3332 292c 0a20 2020 2020 2020  loat32),.       
-00023070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023090: 2073 656c 662e 575f 5041 2920 2b20 7365   self.W_PA) + se
-000230a0: 6c66 2e62 5f50 410a 2020 2020 2020 2020  lf.b_PA.        
-000230b0: 6966 2073 656c 662e 6261 7463 685f 6e6f  if self.batch_no
-000230c0: 726d 616c 697a 653a 0a20 2020 2020 2020  rmalize:.       
-000230d0: 2020 2020 2073 656c 662e 5041 5f62 6e2e       self.PA_bn.
-000230e0: 6576 616c 2829 0a20 2020 2020 2020 2020  eval().         
-000230f0: 2020 2050 4120 3d20 7365 6c66 2e50 415f     PA = self.PA_
-00023100: 626e 2850 4129 0a20 2020 2020 2020 2050  bn(PA).        P
-00023110: 4120 3d20 6163 7469 7661 7469 6f6e 2850  A = activation(P
-00023120: 4129 0a0a 2020 2020 2020 2020 2320 5370  A)..        # Sp
-00023130: 6c69 7420 7468 6520 5041 2074 656e 736f  lit the PA tenso
-00023140: 7220 6163 636f 7264 696e 6720 746f 2074  r according to t
-00023150: 6865 2027 7061 6972 5f73 706c 6974 2720  he 'pair_split' 
-00023160: 7465 6e73 6f72 0a20 2020 2020 2020 2074  tensor.        t
-00023170: 5f67 7270 3a20 4469 6374 5b54 656e 736f  _grp: Dict[Tenso
-00023180: 722c 2054 656e 736f 725d 203d 207b 7d0a  r, Tensor] = {}.
-00023190: 2020 2020 2020 2020 6964 783a 2069 6e74          idx: int
-000231a0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
-000231b0: 2069 2c20 735f 6964 2069 6e20 656e 756d   i, s_id in enum
-000231c0: 6572 6174 6528 7061 6972 5f73 706c 6974  erate(pair_split
-000231d0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000231e0: 5f69 6420 3d20 735f 6964 2e69 7465 6d28  _id = s_id.item(
-000231f0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00023200: 2073 5f69 6420 696e 2074 5f67 7270 3a0a   s_id in t_grp:.
-00023210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023220: 745f 6772 705b 735f 6964 5d20 3d20 745f  t_grp[s_id] = t_
-00023230: 6772 705b 735f 6964 5d20 2b20 5041 5b69  grp[s_id] + PA[i
-00023240: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
-00023250: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00023260: 2020 2020 2020 745f 6772 705b 735f 6964        t_grp[s_id
-00023270: 5d20 3d20 5041 5b69 6478 5d0a 2020 2020  ] = PA[idx].    
-00023280: 2020 2020 2020 2020 6964 7820 3d20 6920          idx = i 
-00023290: 2b20 310a 0a20 2020 2020 2020 2020 2020  + 1..           
-000232a0: 206c 7374 203d 206c 6973 7428 745f 6772   lst = list(t_gr
-000232b0: 702e 7661 6c75 6573 2829 290a 2020 2020  p.values()).    
-000232c0: 2020 2020 2020 2020 7465 6e73 6f72 203d          tensor =
-000232d0: 2074 6f72 6368 2e73 7461 636b 286c 7374   torch.stack(lst
-000232e0: 290a 2020 2020 2020 2020 5041 203d 2074  ).        PA = t
-000232f0: 656e 736f 720a 0a20 2020 2020 2020 2041  ensor..        A
-00023300: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00023310: 2074 6f72 6368 2e6d 6174 6d75 6c28 746f   torch.matmul(to
-00023320: 7263 682e 636f 6e63 6174 285b 4141 2c20  rch.concat([AA, 
-00023330: 5041 5d2c 2031 292c 0a20 2020 2020 2020  PA], 1),.       
-00023340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023360: 7365 6c66 2e57 5f41 2920 2b20 7365 6c66  self.W_A) + self
-00023370: 2e62 5f41 0a20 2020 2020 2020 2069 6620  .b_A.        if 
-00023380: 7365 6c66 2e62 6174 6368 5f6e 6f72 6d61  self.batch_norma
-00023390: 6c69 7a65 3a0a 2020 2020 2020 2020 2020  lize:.          
-000233a0: 2020 7365 6c66 2e41 5f62 6e2e 6576 616c    self.A_bn.eval
-000233b0: 2829 0a20 2020 2020 2020 2020 2020 2041  ().            A
-000233c0: 203d 2073 656c 662e 415f 626e 2841 290a   = self.A_bn(A).
-000233d0: 2020 2020 2020 2020 4120 3d20 6163 7469          A = acti
-000233e0: 7661 7469 6f6e 2841 290a 0a20 2020 2020  vation(A)..     
-000233f0: 2020 2069 6620 7365 6c66 2e75 7064 6174     if self.updat
-00023400: 655f 7061 6972 3a0a 2020 2020 2020 2020  e_pair:.        
-00023410: 2020 2020 2320 4e6f 7465 2074 6861 7420      # Note that 
-00023420: 4150 5f69 6a20 616e 6420 4150 5f6a 6920  AP_ij and AP_ji 
-00023430: 7368 6172 6520 7468 6520 7361 6d65 2073  share the same s
-00023440: 656c 662e 4150 5f62 6e20 6261 7463 680a  elf.AP_bn batch.
-00023450: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
-00023460: 726d 616c 697a 6174 696f 6e0a 2020 2020  rmalization.    
-00023470: 2020 2020 2020 2020 4150 5f69 6a3a 2074          AP_ij: t
-00023480: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
-00023490: 7263 682e 6d61 746d 756c 280a 2020 2020  rch.matmul(.    
-000234a0: 2020 2020 2020 2020 2020 2020 746f 7263              torc
-000234b0: 682e 7265 7368 6170 6528 6174 6f6d 5f66  h.reshape(atom_f
-000234c0: 6561 7475 7265 735b 6174 6f6d 5f74 6f5f  eatures[atom_to_
-000234d0: 7061 6972 5d2c 0a20 2020 2020 2020 2020  pair],.         
-000234e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000234f0: 2020 2020 205b 2d31 2c20 3220 2a20 7365       [-1, 2 * se
-00023500: 6c66 2e6e 5f61 746f 6d5f 696e 7075 745f  lf.n_atom_input_
-00023510: 6665 6174 5d29 2e74 7970 6528 0a20 2020  feat]).type(.   
-00023520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023530: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00023540: 6f72 6368 2e66 6c6f 6174 3332 292c 2073  orch.float32), s
-00023550: 656c 662e 575f 4150 2920 2b20 7365 6c66  elf.W_AP) + self
-00023560: 2e62 5f41 500a 2020 2020 2020 2020 2020  .b_AP.          
-00023570: 2020 6966 2073 656c 662e 6261 7463 685f    if self.batch_
-00023580: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
-00023590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000235a0: 4150 5f62 6e2e 6576 616c 2829 0a20 2020  AP_bn.eval().   
-000235b0: 2020 2020 2020 2020 2020 2020 2041 505f               AP_
-000235c0: 696a 203d 2073 656c 662e 4150 5f62 6e28  ij = self.AP_bn(
-000235d0: 4150 5f69 6a29 0a20 2020 2020 2020 2020  AP_ij).         
-000235e0: 2020 2041 505f 696a 203d 2061 6374 6976     AP_ij = activ
-000235f0: 6174 696f 6e28 4150 5f69 6a29 0a20 2020  ation(AP_ij).   
-00023600: 2020 2020 2020 2020 2041 505f 6a69 3a20           AP_ji: 
-00023610: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
-00023620: 6f72 6368 2e6d 6174 6d75 6c28 0a20 2020  orch.matmul(.   
-00023630: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
-00023640: 6368 2e72 6573 6861 7065 2861 746f 6d5f  ch.reshape(atom_
-00023650: 6665 6174 7572 6573 5b74 6f72 6368 2e66  features[torch.f
-00023660: 6c69 7028 6174 6f6d 5f74 6f5f 7061 6972  lip(atom_to_pair
-00023670: 2c20 5b31 5d29 5d2c 0a20 2020 2020 2020  , [1])],.       
-00023680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023690: 2020 2020 2020 205b 2d31 2c20 3220 2a20         [-1, 2 * 
-000236a0: 7365 6c66 2e6e 5f61 746f 6d5f 696e 7075  self.n_atom_inpu
-000236b0: 745f 6665 6174 5d29 2e74 7970 6528 0a20  t_feat]).type(. 
-000236c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000236d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000236e0: 2074 6f72 6368 2e66 6c6f 6174 3332 292c   torch.float32),
-000236f0: 2073 656c 662e 575f 4150 2920 2b20 7365   self.W_AP) + se
-00023700: 6c66 2e62 5f41 500a 2020 2020 2020 2020  lf.b_AP.        
-00023710: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
-00023720: 685f 6e6f 726d 616c 697a 653a 0a20 2020  h_normalize:.   
-00023730: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00023740: 662e 4150 5f62 6e2e 6576 616c 2829 0a20  f.AP_bn.eval(). 
-00023750: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-00023760: 505f 6a69 203d 2073 656c 662e 4150 5f62  P_ji = self.AP_b
-00023770: 6e28 4150 5f6a 6929 0a20 2020 2020 2020  n(AP_ji).       
-00023780: 2020 2020 2041 505f 6a69 203d 2061 6374       AP_ji = act
-00023790: 6976 6174 696f 6e28 4150 5f6a 6929 0a20  ivation(AP_ji). 
-000237a0: 2020 2020 2020 2020 2020 2023 2050 5020             # PP 
-000237b0: 6973 2061 2074 656e 736f 7220 7769 7468  is a tensor with
-000237c0: 2073 6861 7065 205b 746f 7461 6c20 6e75   shape [total nu
-000237d0: 6d62 6572 206f 6620 7061 6972 732c 6e5f  mber of pairs,n_
-000237e0: 6869 6464 656e 5f50 505d 0a20 2020 2020  hidden_PP].     
-000237f0: 2020 2020 2020 2050 503a 2074 6f72 6368         PP: torch
-00023800: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
-00023810: 6d61 746d 756c 2870 6169 725f 6665 6174  matmul(pair_feat
-00023820: 7572 6573 2e74 7970 6528 746f 7263 682e  ures.type(torch.
-00023830: 666c 6f61 7433 3229 2c0a 2020 2020 2020  float32),.      
-00023840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023860: 2020 2020 2020 7365 6c66 2e57 5f50 5029        self.W_PP)
-00023870: 202b 2073 656c 662e 625f 5050 0a20 2020   + self.b_PP.   
-00023880: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00023890: 2e62 6174 6368 5f6e 6f72 6d61 6c69 7a65  .batch_normalize
-000238a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000238b0: 2020 7365 6c66 2e50 505f 626e 2e65 7661    self.PP_bn.eva
-000238c0: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
-000238d0: 2020 2020 5050 203d 2073 656c 662e 5050      PP = self.PP
-000238e0: 5f62 6e28 5050 290a 2020 2020 2020 2020  _bn(PP).        
-000238f0: 2020 2020 5050 203d 2061 6374 6976 6174      PP = activat
-00023900: 696f 6e28 5050 290a 2020 2020 2020 2020  ion(PP).        
-00023910: 2020 2020 503a 2074 6f72 6368 2e54 656e      P: torch.Ten
-00023920: 736f 7220 3d20 746f 7263 682e 6d61 746d  sor = torch.matm
-00023930: 756c 280a 2020 2020 2020 2020 2020 2020  ul(.            
-00023940: 2020 2020 746f 7263 682e 636f 6e63 6174      torch.concat
-00023950: 285b 4150 5f69 6a20 2b20 4150 5f6a 692c  ([AP_ij + AP_ji,
-00023960: 2050 505d 2c20 3129 2e74 7970 6528 746f   PP], 1).type(to
-00023970: 7263 682e 666c 6f61 7433 3229 2c0a 2020  rch.float32),.  
-00023980: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00023990: 6c66 2e57 5f50 2920 2b20 7365 6c66 2e62  lf.W_P) + self.b
-000239a0: 5f50 0a20 2020 2020 2020 2020 2020 2069  _P.            i
-000239b0: 6620 7365 6c66 2e62 6174 6368 5f6e 6f72  f self.batch_nor
-000239c0: 6d61 6c69 7a65 3a0a 2020 2020 2020 2020  malize:.        
-000239d0: 2020 2020 2020 2020 7365 6c66 2e50 5f62          self.P_b
-000239e0: 6e2e 6576 616c 2829 0a20 2020 2020 2020  n.eval().       
-000239f0: 2020 2020 2020 2020 2050 203d 2073 656c           P = sel
-00023a00: 662e 505f 626e 2850 290a 2020 2020 2020  f.P_bn(P).      
-00023a10: 2020 2020 2020 5020 3d20 6163 7469 7661        P = activa
-00023a20: 7469 6f6e 2850 290a 2020 2020 2020 2020  tion(P).        
-00023a30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00023a40: 2020 5020 3d20 7061 6972 5f66 6561 7475    P = pair_featu
-00023a50: 7265 730a 0a20 2020 2020 2020 2072 6574  res..        ret
-00023a60: 7572 6e20 5b41 2c20 505d 0a              urn [A, P].
+0001e190: 2020 2020 2020 2020 2020 2020 6469 6d3d              dim=
+0001e1a0: 3129 202b 2073 656c 662e 6465 6e73 6532  1) + self.dense2
+0001e1b0: 286e 6f64 655f 7465 6e73 6f72 290a 2020  (node_tensor).  
+0001e1c0: 2020 2020 2020 6f75 7470 7574 5f61 6374        output_act
+0001e1d0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+0001e1e0: 2073 656c 662e 6163 7469 7661 7469 6f6e   self.activation
+0001e1f0: 286f 7574 7075 745f 7375 6d29 0a20 2020  (output_sum).   
+0001e200: 2020 2020 206f 7574 7075 7420 3d20 7365       output = se
+0001e210: 6c66 2e64 726f 706f 7574 286f 7574 7075  lf.dropout(outpu
+0001e220: 745f 6163 7429 0a20 2020 2020 2020 2072  t_act).        r
+0001e230: 6574 7572 6e20 6164 6a61 6365 6e63 795f  eturn adjacency_
+0001e240: 7465 6e73 6f72 2c20 6e6f 6465 5f74 656e  tensor, node_ten
+0001e250: 736f 722c 206f 7574 7075 740a 0a0a 636c  sor, output...cl
+0001e260: 6173 7320 4d6f 6c47 414e 4167 6772 6567  ass MolGANAggreg
+0001e270: 6174 696f 6e4c 6179 6572 286e 6e2e 4d6f  ationLayer(nn.Mo
+0001e280: 6475 6c65 293a 0a20 2020 2022 2222 0a20  dule):.    """. 
+0001e290: 2020 2047 7261 7068 2041 6767 7265 6761     Graph Aggrega
+0001e2a0: 7469 6f6e 206c 6179 6572 2075 7365 6420  tion layer used 
+0001e2b0: 696e 204d 6f6c 4741 4e20 6d6f 6465 6c2e  in MolGAN model.
+0001e2c0: 0a20 2020 204d 6f6c 4741 4e20 6973 2061  .    MolGAN is a
+0001e2d0: 2057 4741 4e20 7479 7065 206d 6f64 656c   WGAN type model
+0001e2e0: 2066 6f72 2067 656e 6572 6174 696f 6e20   for generation 
+0001e2f0: 6f66 2073 6d61 6c6c 206d 6f6c 6563 756c  of small molecul
+0001e300: 6573 2e0a 2020 2020 5065 7266 6f72 6d73  es..    Performs
+0001e310: 2061 6767 7265 6761 7469 6f6e 206f 6e20   aggregation on 
+0001e320: 7465 6e73 6f72 2072 6573 756c 7469 6e67  tensor resulting
+0001e330: 2066 726f 6d20 636f 6e76 6f6c 7574 696f   from convolutio
+0001e340: 6e20 6c61 7965 7273 2e0a 2020 2020 4769  n layers..    Gi
+0001e350: 7665 6e20 6974 7320 7369 6d70 6c65 206e  ven its simple n
+0001e360: 6174 7572 6520 6974 206d 6967 6874 2062  ature it might b
+0001e370: 6520 7265 6d6f 7665 6420 696e 2066 7574  e removed in fut
+0001e380: 7572 6520 616e 6420 6d6f 7665 6420 746f  ure and moved to
+0001e390: 0a20 2020 204d 6f6c 4741 4e45 6e63 6f64  .    MolGANEncod
+0001e3a0: 6572 4c61 7965 722e 0a0a 0a20 2020 2045  erLayer....    E
+0001e3b0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+0001e3c0: 2d2d 2d2d 0a20 2020 203e 3e3e 2069 6d70  ----.    >>> imp
+0001e3d0: 6f72 7420 746f 7263 680a 2020 2020 3e3e  ort torch.    >>
+0001e3e0: 3e20 696d 706f 7274 2074 6f72 6368 2e6e  > import torch.n
+0001e3f0: 6e20 6173 206e 6e0a 2020 2020 3e3e 3e20  n as nn.    >>> 
+0001e400: 696d 706f 7274 2074 6f72 6368 2e6e 6e2e  import torch.nn.
+0001e410: 6675 6e63 7469 6f6e 616c 2061 7320 460a  functional as F.
+0001e420: 2020 2020 3e3e 3e20 7665 7274 6963 6573      >>> vertices
+0001e430: 203d 2039 0a20 2020 203e 3e3e 206e 6f64   = 9.    >>> nod
+0001e440: 6573 203d 2035 0a20 2020 203e 3e3e 2065  es = 5.    >>> e
+0001e450: 6467 6573 203d 2035 0a20 2020 203e 3e3e  dges = 5.    >>>
+0001e460: 2075 6e69 7473 203d 2031 3238 0a0a 2020   units = 128..  
+0001e470: 2020 3e3e 3e20 6c61 7965 725f 3120 3d20    >>> layer_1 = 
+0001e480: 4d6f 6c47 414e 436f 6e76 6f6c 7574 696f  MolGANConvolutio
+0001e490: 6e4c 6179 6572 2875 6e69 7473 3d75 6e69  nLayer(units=uni
+0001e4a0: 7473 2c6e 6f64 6573 3d6e 6f64 6573 2c65  ts,nodes=nodes,e
+0001e4b0: 6467 6573 3d65 6467 6573 2c20 6e61 6d65  dges=edges, name
+0001e4c0: 3d27 6c61 7965 7231 2729 0a20 2020 203e  ='layer1').    >
+0001e4d0: 3e3e 206c 6179 6572 5f32 203d 204d 6f6c  >> layer_2 = Mol
+0001e4e0: 4741 4e41 6767 7265 6761 7469 6f6e 4c61  GANAggregationLa
+0001e4f0: 7965 7228 756e 6974 733d 3132 382c 206e  yer(units=128, n
+0001e500: 616d 653d 276c 6179 6572 3227 290a 2020  ame='layer2').  
+0001e510: 2020 3e3e 3e20 6164 6a61 6365 6e63 795f    >>> adjacency_
+0001e520: 7465 6e73 6f72 203d 2074 6f72 6368 2e72  tensor = torch.r
+0001e530: 616e 646e 2828 312c 2076 6572 7469 6365  andn((1, vertice
+0001e540: 732c 2076 6572 7469 6365 732c 2065 6467  s, vertices, edg
+0001e550: 6573 2929 0a20 2020 203e 3e3e 206e 6f64  es)).    >>> nod
+0001e560: 655f 7465 6e73 6f72 203d 2074 6f72 6368  e_tensor = torch
+0001e570: 2e72 616e 646e 2828 312c 2076 6572 7469  .randn((1, verti
+0001e580: 6365 732c 206e 6f64 6573 2929 0a20 2020  ces, nodes)).   
+0001e590: 203e 3e3e 2068 6964 6465 6e5f 3120 3d20   >>> hidden_1 = 
+0001e5a0: 6c61 7965 725f 3128 5b61 646a 6163 656e  layer_1([adjacen
+0001e5b0: 6379 5f74 656e 736f 722c 206e 6f64 655f  cy_tensor, node_
+0001e5c0: 7465 6e73 6f72 5d29 0a20 2020 203e 3e3e  tensor]).    >>>
+0001e5d0: 206f 7574 7075 7420 3d20 6c61 7965 725f   output = layer_
+0001e5e0: 3228 6869 6464 656e 5f31 5b32 5d29 0a0a  2(hidden_1[2])..
+0001e5f0: 2020 2020 5265 6665 7265 6e63 6573 0a20      References. 
+0001e600: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001e610: 2020 2e2e 205b 315d 204e 6963 6f6c 6120    .. [1] Nicola 
+0001e620: 4465 2043 616f 2065 7420 616c 2e20 224d  De Cao et al. "M
+0001e630: 6f6c 4741 4e3a 2041 6e20 696d 706c 6963  olGAN: An implic
+0001e640: 6974 2067 656e 6572 6174 6976 6520 6d6f  it generative mo
+0001e650: 6465 6c0a 2020 2020 2020 2020 666f 7220  del.        for 
+0001e660: 736d 616c 6c20 6d6f 6c65 6375 6c61 7220  small molecular 
+0001e670: 6772 6170 6873 222c 2068 7474 7073 3a2f  graphs", https:/
+0001e680: 2f61 7278 6976 2e6f 7267 2f61 6273 2f31  /arxiv.org/abs/1
+0001e690: 3830 352e 3131 3937 330a 2020 2020 2222  805.11973.    ""
+0001e6a0: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+0001e6b0: 745f 5f28 7365 6c66 2c0a 2020 2020 2020  t__(self,.      
+0001e6c0: 2020 2020 2020 2020 2020 2075 6e69 7473             units
+0001e6d0: 3a20 696e 7420 3d20 3132 382c 0a20 2020  : int = 128,.   
+0001e6e0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
+0001e6f0: 7469 7661 7469 6f6e 3d74 6f72 6368 2e74  tivation=torch.t
+0001e700: 616e 682c 0a20 2020 2020 2020 2020 2020  anh,.           
+0001e710: 2020 2020 2020 6472 6f70 6f75 745f 7261        dropout_ra
+0001e720: 7465 3a20 666c 6f61 7420 3d20 302e 302c  te: float = 0.0,
+0001e730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e740: 2020 6e61 6d65 3a20 7374 7220 3d20 2222    name: str = ""
+0001e750: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001e760: 2020 202a 2a6b 7761 7267 7329 3a0a 2020     **kwargs):.  
+0001e770: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001e780: 2020 496e 6974 6961 6c69 7a65 2074 6865    Initialize the
+0001e790: 206c 6179 6572 0a0a 2020 2020 2020 2020   layer..        
+0001e7a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0001e7b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 0a20 2020     ---------.   
+0001e7c0: 2020 2020 2075 6e69 7473 3a20 696e 742c       units: int,
+0001e7d0: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
+0001e7e0: 6c74 3d31 3238 290a 2020 2020 2020 2020  lt=128).        
+0001e7f0: 2020 2020 4469 6d65 7369 6f6e 206f 6620      Dimesion of 
+0001e800: 6465 6e73 6520 6c61 7965 7273 2075 7365  dense layers use
+0001e810: 6420 666f 7220 6167 6772 6567 6174 696f  d for aggregatio
+0001e820: 6e0a 2020 2020 2020 2020 6163 7469 7661  n.        activa
+0001e830: 7469 6f6e 3a20 6675 6e63 7469 6f6e 2c20  tion: function, 
+0001e840: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+0001e850: 743d 5461 6e68 290a 2020 2020 2020 2020  t=Tanh).        
+0001e860: 2020 2020 6163 7469 7661 7469 6f6e 2066      activation f
+0001e870: 756e 6374 696f 6e20 7573 6564 2061 6372  unction used acr
+0001e880: 6f73 7320 6d6f 6465 6c2c 2064 6566 6175  oss model, defau
+0001e890: 6c74 2069 7320 5461 6e68 0a20 2020 2020  lt is Tanh.     
+0001e8a0: 2020 2064 726f 706f 7574 5f72 6174 653a     dropout_rate:
+0001e8b0: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+0001e8c0: 2028 6465 6661 756c 743d 302e 3029 0a20   (default=0.0). 
+0001e8d0: 2020 2020 2020 2020 2020 2055 7365 6420             Used 
+0001e8e0: 6279 2064 726f 706f 7574 206c 6179 6572  by dropout layer
+0001e8f0: 0a20 2020 2020 2020 206e 616d 653a 2073  .        name: s
+0001e900: 7472 696e 672c 206f 7074 696f 6e61 6c20  tring, optional 
+0001e910: 2864 6566 6175 6c74 3d22 2229 0a20 2020  (default="").   
+0001e920: 2020 2020 2020 2020 204e 616d 6520 6f66           Name of
+0001e930: 2074 6865 206c 6179 6572 0a20 2020 2020   the layer.     
+0001e940: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0001e950: 7375 7065 7228 4d6f 6c47 414e 4167 6772  super(MolGANAggr
+0001e960: 6567 6174 696f 6e4c 6179 6572 2c20 7365  egationLayer, se
+0001e970: 6c66 292e 5f5f 696e 6974 5f5f 2829 0a20  lf).__init__(). 
+0001e980: 2020 2020 2020 2073 656c 662e 756e 6974         self.unit
+0001e990: 733a 2069 6e74 203d 2075 6e69 7473 0a20  s: int = units. 
+0001e9a0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+0001e9b0: 7661 7469 6f6e 203d 2061 6374 6976 6174  vation = activat
+0001e9c0: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
+0001e9d0: 2e64 726f 706f 7574 5f72 6174 653a 2066  .dropout_rate: f
+0001e9e0: 6c6f 6174 203d 2064 726f 706f 7574 5f72  loat = dropout_r
+0001e9f0: 6174 650a 2020 2020 2020 2020 7365 6c66  ate.        self
+0001ea00: 2e6e 616d 653a 2073 7472 203d 206e 616d  .name: str = nam
+0001ea10: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+0001ea20: 6431 203d 206e 6e2e 4c69 6e65 6172 2873  d1 = nn.Linear(s
+0001ea30: 656c 662e 756e 6974 732c 2073 656c 662e  elf.units, self.
+0001ea40: 756e 6974 7329 0a20 2020 2020 2020 2073  units).        s
+0001ea50: 656c 662e 6432 203d 206e 6e2e 4c69 6e65  elf.d2 = nn.Line
+0001ea60: 6172 2873 656c 662e 756e 6974 732c 2073  ar(self.units, s
+0001ea70: 656c 662e 756e 6974 7329 0a20 2020 2020  elf.units).     
+0001ea80: 2020 2073 656c 662e 6472 6f70 6f75 745f     self.dropout_
+0001ea90: 6c61 7965 7220 3d20 6e6e 2e44 726f 706f  layer = nn.Dropo
+0001eaa0: 7574 2864 726f 706f 7574 5f72 6174 6529  ut(dropout_rate)
+0001eab0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+0001eac0: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
+0001ead0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001eae0: 2020 2020 2053 7472 696e 6720 7265 7072       String repr
+0001eaf0: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
+0001eb00: 6520 6c61 7965 720a 2020 2020 2020 2020  e layer.        
+0001eb10: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0001eb20: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0001eb30: 0a20 2020 2020 2020 2073 7472 696e 670a  .        string.
+0001eb40: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
+0001eb50: 6e67 2072 6570 7265 7365 6e74 6174 696f  ng representatio
+0001eb60: 6e20 6f66 2074 6865 206c 6179 6572 2020  n of the layer  
+0001eb70: 2020 0a20 2020 2020 2020 2022 2222 0a20    .        """. 
+0001eb80: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+0001eb90: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
+0001eba0: 5f5f 6e61 6d65 5f5f 7d28 756e 6974 733d  __name__}(units=
+0001ebb0: 7b73 656c 662e 756e 6974 737d 2c20 6163  {self.units}, ac
+0001ebc0: 7469 7661 7469 6f6e 3d7b 7365 6c66 2e61  tivation={self.a
+0001ebd0: 6374 6976 6174 696f 6e7d 2c20 6472 6f70  ctivation}, drop
+0001ebe0: 6f75 745f 7261 7465 3d7b 7365 6c66 2e64  out_rate={self.d
+0001ebf0: 726f 706f 7574 5f72 6174 657d 2922 0a0a  ropout_rate})"..
+0001ec00: 2020 2020 6465 6620 666f 7277 6172 6428      def forward(
+0001ec10: 7365 6c66 2c20 696e 7075 7473 3a20 4c69  self, inputs: Li
+0001ec20: 7374 2920 2d3e 2074 6f72 6368 2e54 656e  st) -> torch.Ten
+0001ec30: 736f 723a 0a20 2020 2020 2020 2022 2222  sor:.        """
+0001ec40: 0a20 2020 2020 2020 2049 6e76 6f6b 6520  .        Invoke 
+0001ec50: 7468 6973 206c 6179 6572 0a0a 2020 2020  this layer..    
+0001ec60: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001ec70: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0001ec80: 2d0a 2020 2020 2020 2020 696e 7075 7473  -.        inputs
+0001ec90: 3a20 4c69 7374 0a20 2020 2020 2020 2020  : List.         
+0001eca0: 2020 2053 696e 676c 6520 7465 6e73 6f72     Single tensor
+0001ecb0: 2072 6573 756c 7469 6e67 2066 726f 6d20   resulting from 
+0001ecc0: 6772 6170 6820 636f 6e76 6f6c 7574 696f  graph convolutio
+0001ecd0: 6e20 6c61 7965 720a 0a20 2020 2020 2020  n layer..       
+0001ece0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0001ecf0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+0001ed00: 2020 6167 6772 6567 6174 696f 6e20 7465    aggregation te
+0001ed10: 6e73 6f72 3a20 746f 7263 682e 5465 6e73  nsor: torch.Tens
+0001ed20: 6f72 0a20 2020 2020 2020 2020 2052 6573  or.          Res
+0001ed30: 756c 7420 6f66 2061 6767 7265 6761 7469  ult of aggregati
+0001ed40: 6f6e 2066 756e 6374 696f 6e20 6f6e 2069  on function on i
+0001ed50: 6e70 7574 2063 6f6e 766f 6c75 7469 6f6e  nput convolution
+0001ed60: 2074 656e 736f 722e 0a20 2020 2020 2020   tensor..       
+0001ed70: 2022 2222 0a0a 2020 2020 2020 2020 6920   """..        i 
+0001ed80: 3d20 746f 7263 682e 7369 676d 6f69 6428  = torch.sigmoid(
+0001ed90: 7365 6c66 2e64 3128 696e 7075 7473 2929  self.d1(inputs))
+0001eda0: 0a20 2020 2020 2020 206a 203d 2073 656c  .        j = sel
+0001edb0: 662e 6163 7469 7661 7469 6f6e 2873 656c  f.activation(sel
+0001edc0: 662e 6432 2869 6e70 7574 7329 290a 2020  f.d2(inputs)).  
+0001edd0: 2020 2020 2020 6f75 7470 7574 203d 2074        output = t
+0001ede0: 6f72 6368 2e73 756d 2869 202a 206a 2c20  orch.sum(i * j, 
+0001edf0: 6469 6d3d 3129 0a20 2020 2020 2020 206f  dim=1).        o
+0001ee00: 7574 7075 7420 3d20 7365 6c66 2e61 6374  utput = self.act
+0001ee10: 6976 6174 696f 6e28 6f75 7470 7574 290a  ivation(output).
+0001ee20: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+0001ee30: 2073 656c 662e 6472 6f70 6f75 745f 6c61   self.dropout_la
+0001ee40: 7965 7228 6f75 7470 7574 290a 2020 2020  yer(output).    
+0001ee50: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
+0001ee60: 740a 0a0a 636c 6173 7320 4454 4e4e 5374  t...class DTNNSt
+0001ee70: 6570 286e 6e2e 4d6f 6475 6c65 293a 0a20  ep(nn.Module):. 
+0001ee80: 2020 2022 2222 4454 4e4e 5374 6570 204c     """DTNNStep L
+0001ee90: 6179 6572 2066 6f72 2044 544e 4e20 6d6f  ayer for DTNN mo
+0001eea0: 6465 6c2e 0a0a 2020 2020 456e 636f 6465  del...    Encode
+0001eeb0: 7320 7468 6520 6174 6f6d 2773 2069 6e74  s the atom's int
+0001eec0: 6572 6163 7469 6f6e 2077 6974 6820 6f74  eraction with ot
+0001eed0: 6865 7220 6174 6f6d 7320 6163 636f 7264  her atoms accord
+0001eee0: 696e 6720 746f 2064 6973 7461 6e63 6520  ing to distance 
+0001eef0: 7265 6c61 7469 6f6e 7368 6970 732e 205b  relationships. [
+0001ef00: 315d 5f0a 0a20 2020 2054 6869 7320 4c61  1]_..    This La
+0001ef10: 7965 7220 696d 706c 656d 656e 7473 2074  yer implements t
+0001ef20: 6865 2045 7120 2837 2920 6672 6f6d 2044  he Eq (7) from D
+0001ef30: 544e 4e20 5061 7065 722e 2054 6865 6e20  TNN Paper. Then 
+0001ef40: 7375 6d73 2074 6865 6d20 7570 2074 6f20  sums them up to 
+0001ef50: 6765 7420 7468 6520 6669 6e61 6c20 6f75  get the final ou
+0001ef60: 7470 7574 2075 7369 6e67 2045 7120 2836  tput using Eq (6
+0001ef70: 2920 6672 6f6d 2044 544e 4e20 5061 7065  ) from DTNN Pape
+0001ef80: 722e 0a0a 2020 2020 4571 2028 3729 3a20  r...    Eq (7): 
+0001ef90: 565f 696a 203d 2074 616e 685b 575f 6663  V_ij = tanh[W_fc
+0001efa0: 202e 2028 2857 5f63 6620 2e20 435f 6a20   . ((W_cf . C_j 
+0001efb0: 2b20 625f 6366 2920 2a20 2857 5f64 6620  + b_cf) * (W_df 
+0001efc0: 2e20 645f 696a 202b 2062 5f64 6629 295d  . d_ij + b_df))]
+0001efd0: 0a0a 2020 2020 4571 2028 3629 3a20 435f  ..    Eq (6): C_
+0001efe0: 6920 3d20 435f 6920 2b20 7375 6d28 565f  i = C_i + sum(V_
+0001eff0: 696a 290a 0a20 2020 2048 6572 6520 3a20  ij)..    Here : 
+0001f000: 272e 273d 4d61 7472 6978 204d 756c 7469  '.'=Matrix Multi
+0001f010: 706c 6963 6174 696f 6e20 2c20 272a 273d  plication , '*'=
+0001f020: 4d75 6c74 6970 6c69 6361 7469 6f6e 0a0a  Multiplication..
+0001f030: 2020 2020 5265 6665 7265 6e63 6573 0a20      References. 
+0001f040: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001f050: 2020 5b31 5d20 5363 68c3 bc74 742c 204b    [1] Sch..tt, K
+0001f060: 7269 7374 6f66 2054 2e2c 2065 7420 616c  ristof T., et al
+0001f070: 2e20 2251 7561 6e74 756d 2d63 6865 6d69  . "Quantum-chemi
+0001f080: 6361 6c20 696e 7369 6768 7473 2066 726f  cal insights fro
+0001f090: 6d20 6465 6570 0a20 2020 2020 2020 2074  m deep.        t
+0001f0a0: 656e 736f 7220 6e65 7572 616c 206e 6574  ensor neural net
+0001f0b0: 776f 726b 732e 2220 4e61 7475 7265 2063  works." Nature c
+0001f0c0: 6f6d 6d75 6e69 6361 7469 6f6e 7320 382e  ommunications 8.
+0001f0d0: 3120 2832 3031 3729 3a20 312d 382e 0a0a  1 (2017): 1-8...
+0001f0e0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+0001f0f0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
+0001f100: 3e20 6672 6f6d 2064 6565 7063 6865 6d2e  > from deepchem.
+0001f110: 6d6f 6465 6c73 2e74 6f72 6368 5f6d 6f64  models.torch_mod
+0001f120: 656c 7320 696d 706f 7274 206c 6179 6572  els import layer
+0001f130: 730a 2020 2020 3e3e 3e20 696d 706f 7274  s.    >>> import
+0001f140: 2074 6f72 6368 0a20 2020 203e 3e3e 2065   torch.    >>> e
+0001f150: 6d62 6564 6469 6e67 5f6c 6179 6572 203d  mbedding_layer =
+0001f160: 206c 6179 6572 732e 4454 4e4e 456d 6265   layers.DTNNEmbe
+0001f170: 6464 696e 6728 342c 2034 290a 2020 2020  dding(4, 4).    
+0001f180: 3e3e 3e20 656d 6220 3d20 656d 6265 6464  >>> emb = embedd
+0001f190: 696e 675f 6c61 7965 7228 746f 7263 682e  ing_layer(torch.
+0001f1a0: 5465 6e73 6f72 285b 302c 312c 322c 335d  Tensor([0,1,2,3]
+0001f1b0: 292e 746f 2874 6f72 6368 2e69 6e74 3634  ).to(torch.int64
+0001f1c0: 2929 0a20 2020 203e 3e3e 2073 7465 705f  )).    >>> step_
+0001f1d0: 6c61 7965 7220 3d20 6c61 7965 7273 2e44  layer = layers.D
+0001f1e0: 544e 4e53 7465 7028 342c 2036 2c20 3829  TNNStep(4, 6, 8)
+0001f1f0: 0a20 2020 203e 3e3e 206f 7574 7075 745f  .    >>> output_
+0001f200: 746f 7263 6820 3d20 7374 6570 5f6c 6179  torch = step_lay
+0001f210: 6572 285b 0a20 2020 202e 2e2e 2020 2020  er([.    ...    
+0001f220: 2074 6f72 6368 2e54 656e 736f 7228 656d   torch.Tensor(em
+0001f230: 6229 2c0a 2020 2020 2e2e 2e20 2020 2020  b),.    ...     
+0001f240: 746f 7263 682e 5465 6e73 6f72 285b 302c  torch.Tensor([0,
+0001f250: 2031 2c20 322c 2033 2c20 342c 2035 5d29   1, 2, 3, 4, 5])
+0001f260: 2e74 6f28 746f 7263 682e 666c 6f61 7433  .to(torch.float3
+0001f270: 3229 2c0a 2020 2020 2e2e 2e20 2020 2020  2),.    ...     
+0001f280: 746f 7263 682e 5465 6e73 6f72 285b 315d  torch.Tensor([1]
+0001f290: 292e 746f 2874 6f72 6368 2e69 6e74 3634  ).to(torch.int64
+0001f2a0: 292c 0a20 2020 202e 2e2e 2020 2020 2074  ),.    ...     t
+0001f2b0: 6f72 6368 2e54 656e 736f 7228 5b5b 315d  orch.Tensor([[1]
+0001f2c0: 5d29 2e74 6f28 746f 7263 682e 696e 7436  ]).to(torch.int6
+0001f2d0: 3429 0a20 2020 202e 2e2e 205d 290a 2020  4).    ... ]).  
+0001f2e0: 2020 3e3e 3e20 6f75 7470 7574 5f74 6f72    >>> output_tor
+0001f2f0: 6368 2e73 6861 7065 0a20 2020 2074 6f72  ch.shape.    tor
+0001f300: 6368 2e53 697a 6528 5b32 2c20 342c 2034  ch.Size([2, 4, 4
+0001f310: 5d29 0a0a 2020 2020 2222 220a 0a20 2020  ])..    """..   
+0001f320: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0001f330: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0001f340: 2020 2020 206e 5f65 6d62 6564 6469 6e67       n_embedding
+0001f350: 3a20 696e 7420 3d20 3330 2c0a 2020 2020  : int = 30,.    
+0001f360: 2020 2020 2020 2020 2020 2020 206e 5f64               n_d
+0001f370: 6973 7461 6e63 653a 2069 6e74 203d 2031  istance: int = 1
+0001f380: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+0001f390: 2020 2020 206e 5f68 6964 6465 6e3a 2069       n_hidden: i
+0001f3a0: 6e74 203d 2036 302c 0a20 2020 2020 2020  nt = 60,.       
+0001f3b0: 2020 2020 2020 2020 2020 696e 6974 6961            initia
+0001f3c0: 6c69 7a65 723a 2073 7472 203d 2027 7861  lizer: str = 'xa
+0001f3d0: 7669 6572 5f75 6e69 666f 726d 5f27 2c0a  vier_uniform_',.
+0001f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3f0: 2061 6374 6976 6174 696f 6e3d 2774 616e   activation='tan
+0001f400: 6827 2c0a 2020 2020 2020 2020 2020 2020  h',.            
+0001f410: 2020 2020 202a 2a6b 7761 7267 7329 3a0a       **kwargs):.
+0001f420: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001f430: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001f440: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0001f450: 2d0a 2020 2020 2020 2020 6e5f 656d 6265  -.        n_embe
+0001f460: 6464 696e 673a 2069 6e74 2c20 6f70 7469  dding: int, opti
+0001f470: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0001f480: 204e 756d 6265 7220 6f66 2066 6561 7475   Number of featu
+0001f490: 7265 7320 666f 7220 6561 6368 2061 746f  res for each ato
+0001f4a0: 6d0a 2020 2020 2020 2020 6e5f 6469 7374  m.        n_dist
+0001f4b0: 616e 6365 3a20 696e 742c 206f 7074 696f  ance: int, optio
+0001f4c0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+0001f4d0: 6772 616e 756c 6172 6974 7920 6f66 2064  granularity of d
+0001f4e0: 6973 7461 6e63 6520 6d61 7472 6978 0a20  istance matrix. 
+0001f4f0: 2020 2020 2020 206e 5f68 6964 6465 6e3a         n_hidden:
+0001f500: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
+0001f510: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
+0001f520: 7220 6f66 206e 6f64 6573 2069 6e20 6869  r of nodes in hi
+0001f530: 6464 656e 206c 6179 6572 0a20 2020 2020  dden layer.     
+0001f540: 2020 2069 6e69 7469 616c 697a 6572 3a20     initializer: 
+0001f550: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
+0001f560: 2020 2020 2020 2020 2020 5765 6967 6874            Weight
+0001f570: 2069 6e69 7469 616c 697a 6174 696f 6e20   initialization 
+0001f580: 666f 7220 6669 6c74 6572 732e 0a20 2020  for filters..   
+0001f590: 2020 2020 2020 2020 204f 7074 696f 6e73           Options
+0001f5a0: 3a20 7b78 6176 6965 725f 756e 6966 6f72  : {xavier_unifor
+0001f5b0: 6d5f 2c20 7861 7669 6572 5f6e 6f72 6d61  m_, xavier_norma
+0001f5c0: 6c5f 2c20 6b61 696d 696e 675f 756e 6966  l_, kaiming_unif
+0001f5d0: 6f72 6d5f 2c20 6b61 696d 696e 675f 6e6f  orm_, kaiming_no
+0001f5e0: 726d 616c 5f2c 2074 7275 6e63 5f6e 6f72  rmal_, trunc_nor
+0001f5f0: 6d61 6c5f 7d0a 2020 2020 2020 2020 6163  mal_}.        ac
+0001f600: 7469 7661 7469 6f6e 3a20 7374 722c 206f  tivation: str, o
+0001f610: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0001f620: 2020 2020 4163 7469 7661 7469 6f6e 2066      Activation f
+0001f630: 756e 6374 696f 6e20 6170 706c 6965 640a  unction applied.
+0001f640: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001f650: 2020 2020 2073 7570 6572 2844 544e 4e53       super(DTNNS
+0001f660: 7465 702c 2073 656c 6629 2e5f 5f69 6e69  tep, self).__ini
+0001f670: 745f 5f28 2a2a 6b77 6172 6773 290a 2020  t__(**kwargs).  
+0001f680: 2020 2020 2020 7365 6c66 2e6e 5f65 6d62        self.n_emb
+0001f690: 6564 6469 6e67 203d 206e 5f65 6d62 6564  edding = n_embed
+0001f6a0: 6469 6e67 0a20 2020 2020 2020 2073 656c  ding.        sel
+0001f6b0: 662e 6e5f 6469 7374 616e 6365 203d 206e  f.n_distance = n
+0001f6c0: 5f64 6973 7461 6e63 650a 2020 2020 2020  _distance.      
+0001f6d0: 2020 7365 6c66 2e6e 5f68 6964 6465 6e20    self.n_hidden 
+0001f6e0: 3d20 6e5f 6869 6464 656e 0a20 2020 2020  = n_hidden.     
+0001f6f0: 2020 2073 656c 662e 696e 6974 6961 6c69     self.initiali
+0001f700: 7a65 7220 3d20 696e 6974 6961 6c69 7a65  zer = initialize
+0001f710: 7220 2023 2053 6574 2077 6569 6768 7420  r  # Set weight 
+0001f720: 696e 6974 6961 6c69 7a61 7469 6f6e 0a20  initialization. 
+0001f730: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+0001f740: 7661 7469 6f6e 203d 2061 6374 6976 6174  vation = activat
+0001f750: 696f 6e20 2023 2047 6574 2061 6374 6976  ion  # Get activ
+0001f760: 6174 696f 6e73 0a20 2020 2020 2020 2073  ations.        s
+0001f770: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
+0001f780: 6e20 3d20 6765 745f 6163 7469 7661 7469  n = get_activati
+0001f790: 6f6e 2873 656c 662e 6163 7469 7661 7469  on(self.activati
+0001f7a0: 6f6e 290a 0a20 2020 2020 2020 2069 6e69  on)..        ini
+0001f7b0: 745f 6675 6e63 3a20 4361 6c6c 6162 6c65  t_func: Callable
+0001f7c0: 203d 2067 6574 6174 7472 2869 6e69 7469   = getattr(initi
+0001f7d0: 616c 697a 6572 732c 2073 656c 662e 696e  alizers, self.in
+0001f7e0: 6974 6961 6c69 7a65 7229 0a0a 2020 2020  itializer)..    
+0001f7f0: 2020 2020 7365 6c66 2e57 5f63 6620 3d20      self.W_cf = 
+0001f800: 6e6e 2e50 6172 616d 6574 6572 280a 2020  nn.Parameter(.  
+0001f810: 2020 2020 2020 2020 2020 696e 6974 5f66            init_f
+0001f820: 756e 6328 746f 7263 682e 656d 7074 7928  unc(torch.empty(
+0001f830: 5b73 656c 662e 6e5f 656d 6265 6464 696e  [self.n_embeddin
+0001f840: 672c 2073 656c 662e 6e5f 6869 6464 656e  g, self.n_hidden
+0001f850: 5d29 2929 0a20 2020 2020 2020 2073 656c  ]))).        sel
+0001f860: 662e 575f 6466 203d 206e 6e2e 5061 7261  f.W_df = nn.Para
+0001f870: 6d65 7465 7228 0a20 2020 2020 2020 2020  meter(.         
+0001f880: 2020 2069 6e69 745f 6675 6e63 2874 6f72     init_func(tor
+0001f890: 6368 2e65 6d70 7479 285b 7365 6c66 2e6e  ch.empty([self.n
+0001f8a0: 5f64 6973 7461 6e63 652c 2073 656c 662e  _distance, self.
+0001f8b0: 6e5f 6869 6464 656e 5d29 2929 0a20 2020  n_hidden]))).   
+0001f8c0: 2020 2020 2073 656c 662e 575f 6663 203d       self.W_fc =
+0001f8d0: 206e 6e2e 5061 7261 6d65 7465 7228 0a20   nn.Parameter(. 
+0001f8e0: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
+0001f8f0: 6675 6e63 2874 6f72 6368 2e65 6d70 7479  func(torch.empty
+0001f900: 285b 7365 6c66 2e6e 5f68 6964 6465 6e2c  ([self.n_hidden,
+0001f910: 2073 656c 662e 6e5f 656d 6265 6464 696e   self.n_embeddin
+0001f920: 675d 2929 290a 2020 2020 2020 2020 7365  g]))).        se
+0001f930: 6c66 2e62 5f63 6620 3d20 6e6e 2e50 6172  lf.b_cf = nn.Par
+0001f940: 616d 6574 6572 2874 6f72 6368 2e7a 6572  ameter(torch.zer
+0001f950: 6f73 2873 697a 653d 5b0a 2020 2020 2020  os(size=[.      
+0001f960: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
+0001f970: 6465 6e2c 0a20 2020 2020 2020 205d 2929  den,.        ]))
+0001f980: 0a20 2020 2020 2020 2073 656c 662e 625f  .        self.b_
+0001f990: 6466 203d 206e 6e2e 5061 7261 6d65 7465  df = nn.Paramete
+0001f9a0: 7228 746f 7263 682e 7a65 726f 7328 7369  r(torch.zeros(si
+0001f9b0: 7a65 3d5b 0a20 2020 2020 2020 2020 2020  ze=[.           
+0001f9c0: 2073 656c 662e 6e5f 6869 6464 656e 2c0a   self.n_hidden,.
+0001f9d0: 2020 2020 2020 2020 5d29 290a 0a20 2020          ]))..   
+0001f9e0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+0001f9f0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0001fa00: 5265 7475 726e 7320 6120 7374 7269 6e67  Returns a string
+0001fa10: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+0001fa20: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+0001fa30: 6f66 2074 6865 206c 6179 6572 2e0a 0a20  of the layer... 
+0001fa40: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0001fa50: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+0001fa60: 2020 2020 2020 206e 5f65 6d62 6564 6469         n_embeddi
+0001fa70: 6e67 3a20 696e 742c 206f 7074 696f 6e61  ng: int, optiona
+0001fa80: 6c0a 2020 2020 2020 2020 2020 2020 4e75  l.            Nu
+0001fa90: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
+0001faa0: 2066 6f72 2065 6163 6820 6174 6f6d 0a20   for each atom. 
+0001fab0: 2020 2020 2020 206e 5f64 6973 7461 6e63         n_distanc
+0001fac0: 653a 2069 6e74 2c20 6f70 7469 6f6e 616c  e: int, optional
+0001fad0: 0a20 2020 2020 2020 2020 2020 2067 7261  .            gra
+0001fae0: 6e75 6c61 7269 7479 206f 6620 6469 7374  nularity of dist
+0001faf0: 616e 6365 206d 6174 7269 780a 2020 2020  ance matrix.    
+0001fb00: 2020 2020 6e5f 6869 6464 656e 3a20 696e      n_hidden: in
+0001fb10: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0001fb20: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+0001fb30: 6620 6e6f 6465 7320 696e 2068 6964 6465  f nodes in hidde
+0001fb40: 6e20 6c61 7965 720a 2020 2020 2020 2020  n layer.        
+0001fb50: 696e 6974 6961 6c69 7a65 723a 2073 7472  initializer: str
+0001fb60: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0001fb70: 2020 2020 2020 2057 6569 6768 7420 696e         Weight in
+0001fb80: 6974 6961 6c69 7a61 7469 6f6e 2066 6f72  itialization for
+0001fb90: 2066 696c 7465 7273 2e0a 2020 2020 2020   filters..      
+0001fba0: 2020 2020 2020 4f70 7469 6f6e 733a 207b        Options: {
+0001fbb0: 7861 7669 6572 5f75 6e69 666f 726d 5f2c  xavier_uniform_,
+0001fbc0: 2078 6176 6965 725f 6e6f 726d 616c 5f2c   xavier_normal_,
+0001fbd0: 206b 6169 6d69 6e67 5f75 6e69 666f 726d   kaiming_uniform
+0001fbe0: 5f2c 206b 6169 6d69 6e67 5f6e 6f72 6d61  _, kaiming_norma
+0001fbf0: 6c5f 2c20 7472 756e 635f 6e6f 726d 616c  l_, trunc_normal
+0001fc00: 5f7d 0a20 2020 2020 2020 2061 6374 6976  _}.        activ
+0001fc10: 6174 696f 6e3a 2073 7472 2c20 6f70 7469  ation: str, opti
+0001fc20: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0001fc30: 2041 6374 6976 6174 696f 6e20 6675 6e63   Activation func
+0001fc40: 7469 6f6e 2061 7070 6c69 6564 0a0a 2020  tion applied..  
+0001fc50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001fc60: 2020 7265 7475 726e 2066 277b 7365 6c66    return f'{self
+0001fc70: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+0001fc80: 655f 5f7d 286e 5f65 6d62 6564 6469 6e67  e__}(n_embedding
+0001fc90: 3d7b 7365 6c66 2e6e 5f65 6d62 6564 6469  ={self.n_embeddi
+0001fca0: 6e67 7d2c 206e 5f64 6973 7461 6e63 653d  ng}, n_distance=
+0001fcb0: 7b73 656c 662e 6e5f 6469 7374 616e 6365  {self.n_distance
+0001fcc0: 7d2c 206e 5f68 6964 6465 6e3d 7b73 656c  }, n_hidden={sel
+0001fcd0: 662e 6e5f 6869 6464 656e 7d2c 2069 6e69  f.n_hidden}, ini
+0001fce0: 7469 616c 697a 6572 3d7b 7365 6c66 2e69  tializer={self.i
+0001fcf0: 6e69 7469 616c 697a 6572 7d2c 2061 6374  nitializer}, act
+0001fd00: 6976 6174 696f 6e3d 7b73 656c 662e 6163  ivation={self.ac
+0001fd10: 7469 7661 7469 6f6e 7d29 270a 0a20 2020  tivation})'..   
+0001fd20: 2064 6566 2066 6f72 7761 7264 2873 656c   def forward(sel
+0001fd30: 662c 2069 6e70 7574 7329 3a0a 2020 2020  f, inputs):.    
+0001fd40: 2020 2020 2222 2245 7865 6375 7465 7320      """Executes 
+0001fd50: 7468 6520 6571 7561 7469 6f6e 7320 616e  the equations an
+0001fd60: 6420 5265 7475 726e 7320 7468 6520 696e  d Returns the in
+0001fd70: 7472 6163 7469 6f6e 2076 6563 746f 7220  traction vector 
+0001fd80: 6f66 2074 6865 2061 746f 6d20 7769 7468  of the atom with
+0001fd90: 206f 7468 6572 2061 746f 6d73 2e0a 0a20   other atoms... 
+0001fda0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001fdb0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0001fdc0: 2d2d 2d2d 0a20 2020 2020 2020 2069 6e70  ----.        inp
+0001fdd0: 7574 733a 2074 6f72 6368 2e54 656e 736f  uts: torch.Tenso
+0001fde0: 720a 2020 2020 2020 2020 2020 2020 4c69  r.            Li
+0001fdf0: 7374 206f 6620 5465 6e73 6f72 7320 6861  st of Tensors ha
+0001fe00: 7669 6e67 2061 746f 6d5f 6665 6174 7572  ving atom_featur
+0001fe10: 6573 2c20 6469 7374 616e 6365 2c20 6469  es, distance, di
+0001fe20: 7374 616e 6365 5f6d 656d 6265 7273 6869  stance_membershi
+0001fe30: 705f 692c 2064 6973 7461 6e63 655f 6d65  p_i, distance_me
+0001fe40: 6d62 6572 7368 6970 5f6a 2e0a 0a20 2020  mbership_j...   
+0001fe50: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0001fe60: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0001fe70: 2020 2020 2069 6e74 6572 6163 7469 6f6e       interaction
+0001fe80: 5f76 6563 746f 723a 2074 6f72 6368 2e54  _vector: torch.T
+0001fe90: 656e 736f 720a 2020 2020 2020 2020 2020  ensor.          
+0001fea0: 2020 696e 7465 7261 6374 696f 6e20 6f66    interaction of
+0001feb0: 2074 6865 2061 746f 6d20 7769 7468 206f   the atom with o
+0001fec0: 7468 6572 2061 746f 6d73 2062 6173 6564  ther atoms based
+0001fed0: 206f 6e20 6469 7374 616e 6365 2061 6e64   on distance and
+0001fee0: 2064 6973 7461 6e63 655f 6d65 6d62 6572   distance_member
+0001fef0: 7368 6970 2e0a 0a20 2020 2020 2020 2022  ship...        "
+0001ff00: 2222 0a20 2020 2020 2020 2061 746f 6d5f  "".        atom_
+0001ff10: 6665 6174 7572 6573 203d 2069 6e70 7574  features = input
+0001ff20: 735b 305d 0a20 2020 2020 2020 2064 6973  s[0].        dis
+0001ff30: 7461 6e63 6520 3d20 696e 7075 7473 5b31  tance = inputs[1
+0001ff40: 5d0a 2020 2020 2020 2020 6469 7374 616e  ].        distan
+0001ff50: 6365 5f6d 656d 6265 7273 6869 705f 6920  ce_membership_i 
+0001ff60: 3d20 696e 7075 7473 5b32 5d0a 2020 2020  = inputs[2].    
+0001ff70: 2020 2020 6469 7374 616e 6365 5f6d 656d      distance_mem
+0001ff80: 6265 7273 6869 705f 6a20 3d20 696e 7075  bership_j = inpu
+0001ff90: 7473 5b33 5d0a 2020 2020 2020 2020 6469  ts[3].        di
+0001ffa0: 7374 616e 6365 5f68 6964 6465 6e20 3d20  stance_hidden = 
+0001ffb0: 746f 7263 682e 6d61 746d 756c 2864 6973  torch.matmul(dis
+0001ffc0: 7461 6e63 652c 2073 656c 662e 575f 6466  tance, self.W_df
+0001ffd0: 2920 2b20 7365 6c66 2e62 5f64 660a 2020  ) + self.b_df.  
+0001ffe0: 2020 2020 2020 6174 6f6d 5f66 6561 7475        atom_featu
+0001fff0: 7265 735f 6869 6464 656e 203d 2074 6f72  res_hidden = tor
+00020000: 6368 2e6d 6174 6d75 6c28 6174 6f6d 5f66  ch.matmul(atom_f
+00020010: 6561 7475 7265 732c 0a20 2020 2020 2020  eatures,.       
+00020020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020040: 2020 2020 2073 656c 662e 575f 6366 2920       self.W_cf) 
+00020050: 2b20 7365 6c66 2e62 5f63 660a 2020 2020  + self.b_cf.    
+00020060: 2020 2020 6f75 7470 7574 7320 3d20 746f      outputs = to
+00020070: 7263 682e 6d75 6c28 0a20 2020 2020 2020  rch.mul(.       
+00020080: 2020 2020 2064 6973 7461 6e63 655f 6869       distance_hi
+00020090: 6464 656e 2c0a 2020 2020 2020 2020 2020  dden,.          
+000200a0: 2020 746f 7263 682e 656d 6265 6464 696e    torch.embeddin
+000200b0: 6728 6174 6f6d 5f66 6561 7475 7265 735f  g(atom_features_
+000200c0: 6869 6464 656e 2c20 6469 7374 616e 6365  hidden, distance
+000200d0: 5f6d 656d 6265 7273 6869 705f 6a29 290a  _membership_j)).
+000200e0: 0a20 2020 2020 2020 2023 2066 6f72 2061  .        # for a
+000200f0: 746f 6d20 6920 696e 2061 206d 6f6c 6563  tom i in a molec
+00020100: 756c 6520 6d2c 2074 6869 7320 7374 6570  ule m, this step
+00020110: 206d 756c 7469 706c 6965 7320 746f 6765   multiplies toge
+00020120: 7468 6572 2064 6973 7461 6e63 6520 696e  ther distance in
+00020130: 666f 206f 6620 6174 6f6d 2070 6169 7228  fo of atom pair(
+00020140: 692c 6a29 0a20 2020 2020 2020 2023 2061  i,j).        # a
+00020150: 6e64 2065 6d62 6564 6469 6e67 7320 6f66  nd embeddings of
+00020160: 2061 746f 6d20 6a28 626f 7468 2067 6f6e   atom j(both gon
+00020170: 6520 7468 726f 7567 6820 6120 6869 6464  e through a hidd
+00020180: 656e 206c 6179 6572 290a 2020 2020 2020  en layer).      
+00020190: 2020 6f75 7470 7574 7320 3d20 746f 7263    outputs = torc
+000201a0: 682e 6d61 746d 756c 286f 7574 7075 7473  h.matmul(outputs
+000201b0: 2c20 7365 6c66 2e57 5f66 6329 0a20 2020  , self.W_fc).   
+000201c0: 2020 2020 206f 7574 7075 7473 203d 2073       outputs = s
+000201d0: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
+000201e0: 6e28 6f75 7470 7574 7329 0a0a 2020 2020  n(outputs)..    
+000201f0: 2020 2020 6f75 7470 7574 5f69 6920 3d20      output_ii = 
+00020200: 746f 7263 682e 6d75 6c28 7365 6c66 2e62  torch.mul(self.b
+00020210: 5f64 662c 2061 746f 6d5f 6665 6174 7572  _df, atom_featur
+00020220: 6573 5f68 6964 6465 6e29 0a20 2020 2020  es_hidden).     
+00020230: 2020 206f 7574 7075 745f 6969 203d 2074     output_ii = t
+00020240: 6f72 6368 2e6d 6174 6d75 6c28 6f75 7470  orch.matmul(outp
+00020250: 7574 5f69 692c 2073 656c 662e 575f 6663  ut_ii, self.W_fc
+00020260: 290a 2020 2020 2020 2020 6f75 7470 7574  ).        output
+00020270: 5f69 6920 3d20 7365 6c66 2e61 6374 6976  _ii = self.activ
+00020280: 6174 696f 6e5f 666e 286f 7574 7075 745f  ation_fn(output_
+00020290: 6969 290a 0a20 2020 2020 2020 2023 2066  ii)..        # f
+000202a0: 6f72 2061 746f 6d20 692c 2073 756d 2074  or atom i, sum t
+000202b0: 6865 2069 6e66 6c75 656e 6365 2066 726f  he influence fro
+000202c0: 6d20 616c 6c20 6f74 6865 7220 6174 6f6d  m all other atom
+000202d0: 206a 2069 6e20 7468 6520 6d6f 6c65 6375   j in the molecu
+000202e0: 6c65 0a20 2020 2020 2020 2069 6e74 7261  le.        intra
+000202f0: 6374 696f 6e5f 7665 6374 6f72 203d 2073  ction_vector = s
+00020300: 6361 7474 6572 286f 7574 7075 7473 2c20  catter(outputs, 
+00020310: 6469 7374 616e 6365 5f6d 656d 6265 7273  distance_members
+00020320: 6869 705f 692c 0a20 2020 2020 2020 2020  hip_i,.         
+00020330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020340: 2020 2020 2020 2020 2020 2064 696d 3d30             dim=0
+00020350: 2920 2d20 6f75 7470 7574 5f69 6920 2b20  ) - output_ii + 
+00020360: 6174 6f6d 5f66 6561 7475 7265 730a 2020  atom_features.  
+00020370: 2020 2020 2020 7265 7475 726e 2069 6e74        return int
+00020380: 7261 6374 696f 6e5f 7665 6374 6f72 0a0a  raction_vector..
+00020390: 0a63 6c61 7373 2045 6467 654e 6574 776f  .class EdgeNetwo
+000203a0: 726b 286e 6e2e 4d6f 6475 6c65 293a 0a20  rk(nn.Module):. 
+000203b0: 2020 2022 2222 5468 6520 4564 6765 4e65     """The EdgeNe
+000203c0: 7477 6f72 6b20 6d6f 6475 6c65 2069 7320  twork module is 
+000203d0: 6120 5079 546f 7263 6820 7375 626d 6f64  a PyTorch submod
+000203e0: 756c 6520 6465 7369 676e 6564 2066 6f72  ule designed for
+000203f0: 206d 6573 7361 6765 2070 6173 7369 6e67   message passing
+00020400: 2069 6e20 6772 6170 6820 6e65 7572 616c   in graph neural
+00020410: 206e 6574 776f 726b 732e 0a0a 2020 2020   networks...    
+00020420: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
+00020430: 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20 7061  -----.    >>> pa
+00020440: 6972 5f66 6561 7475 7265 7320 3d20 746f  ir_features = to
+00020450: 7263 682e 7261 6e64 2828 342c 2032 292c  rch.rand((4, 2),
+00020460: 2064 7479 7065 3d74 6f72 6368 2e66 6c6f   dtype=torch.flo
+00020470: 6174 3332 290a 2020 2020 3e3e 3e20 6174  at32).    >>> at
+00020480: 6f6d 5f66 6561 7475 7265 7320 3d20 746f  om_features = to
+00020490: 7263 682e 7261 6e64 2828 352c 2032 292c  rch.rand((5, 2),
+000204a0: 2064 7479 7065 3d74 6f72 6368 2e66 6c6f   dtype=torch.flo
+000204b0: 6174 3332 290a 2020 2020 3e3e 3e20 6174  at32).    >>> at
+000204c0: 6f6d 5f74 6f5f 7061 6972 203d 205b 5d0a  om_to_pair = [].
+000204d0: 2020 2020 3e3e 3e20 6e5f 6174 6f6d 7320      >>> n_atoms 
+000204e0: 3d20 320a 2020 2020 3e3e 3e20 7374 6172  = 2.    >>> star
+000204f0: 7420 3d20 300a 2020 2020 3e3e 3e20 4330  t = 0.    >>> C0
+00020500: 2c20 4331 203d 206e 702e 6d65 7368 6772  , C1 = np.meshgr
+00020510: 6964 286e 702e 6172 616e 6765 286e 5f61  id(np.arange(n_a
+00020520: 746f 6d73 292c 206e 702e 6172 616e 6765  toms), np.arange
+00020530: 286e 5f61 746f 6d73 2929 0a20 2020 203e  (n_atoms)).    >
+00020540: 3e3e 2061 746f 6d5f 746f 5f70 6169 722e  >> atom_to_pair.
+00020550: 6170 7065 6e64 286e 702e 7472 616e 7370  append(np.transp
+00020560: 6f73 6528 6e70 2e61 7272 6179 285b 4331  ose(np.array([C1
+00020570: 2e66 6c61 7474 656e 2829 202b 2073 7461  .flatten() + sta
+00020580: 7274 2c20 4330 2e66 6c61 7474 656e 2829  rt, C0.flatten()
+00020590: 202b 2073 7461 7274 5d29 2929 0a20 2020   + start]))).   
+000205a0: 203e 3e3e 2061 746f 6d5f 746f 5f70 6169   >>> atom_to_pai
+000205b0: 7220 3d20 746f 7263 682e 5465 6e73 6f72  r = torch.Tensor
+000205c0: 2861 746f 6d5f 746f 5f70 6169 7229 0a20  (atom_to_pair). 
+000205d0: 2020 203e 3e3e 2061 746f 6d5f 746f 5f70     >>> atom_to_p
+000205e0: 6169 7220 3d20 746f 7263 682e 7371 7565  air = torch.sque
+000205f0: 657a 6528 6174 6f6d 5f74 6f5f 7061 6972  eze(atom_to_pair
+00020600: 2e74 6f28 746f 7263 682e 696e 7436 3429  .to(torch.int64)
+00020610: 2c20 6469 6d3d 3029 0a20 2020 203e 3e3e  , dim=0).    >>>
+00020620: 2069 6e70 7574 7320 3d20 5b70 6169 725f   inputs = [pair_
+00020630: 6665 6174 7572 6573 2c20 6174 6f6d 5f66  features, atom_f
+00020640: 6561 7475 7265 732c 2061 746f 6d5f 746f  eatures, atom_to
+00020650: 5f70 6169 725d 0a20 2020 203e 3e3e 206e  _pair].    >>> n
+00020660: 5f70 6169 725f 6665 6174 7572 6573 203d  _pair_features =
+00020670: 2032 0a20 2020 203e 3e3e 206e 5f68 6964   2.    >>> n_hid
+00020680: 6465 6e20 3d20 320a 2020 2020 3e3e 3e20  den = 2.    >>> 
+00020690: 696e 6974 203d 2027 7861 7669 6572 5f75  init = 'xavier_u
+000206a0: 6e69 666f 726d 5f27 0a20 2020 203e 3e3e  niform_'.    >>>
+000206b0: 206c 6179 6572 203d 2045 6467 654e 6574   layer = EdgeNet
+000206c0: 776f 726b 286e 5f70 6169 725f 6665 6174  work(n_pair_feat
+000206d0: 7572 6573 2c20 6e5f 6869 6464 656e 2c20  ures, n_hidden, 
+000206e0: 696e 6974 290a 2020 2020 3e3e 3e20 7265  init).    >>> re
+000206f0: 7375 6c74 203d 206c 6179 6572 2869 6e70  sult = layer(inp
+00020700: 7574 7329 0a20 2020 203e 3e3e 2072 6573  uts).    >>> res
+00020710: 756c 742e 7368 6170 655b 315d 0a20 2020  ult.shape[1].   
+00020720: 2032 0a20 2020 2022 2222 0a0a 2020 2020   2.    """..    
+00020730: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00020740: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00020750: 2020 2020 6e5f 7061 6972 5f66 6561 7475      n_pair_featu
+00020760: 7265 733a 2069 6e74 203d 2038 2c0a 2020  res: int = 8,.  
+00020770: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00020780: 5f68 6964 6465 6e3a 2069 6e74 203d 2031  _hidden: int = 1
+00020790: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+000207a0: 2020 2020 2069 6e69 743a 2073 7472 203d       init: str =
+000207b0: 2027 7861 7669 6572 5f75 6e69 666f 726d   'xavier_uniform
+000207c0: 5f27 2c0a 2020 2020 2020 2020 2020 2020  _',.            
+000207d0: 2020 2020 202a 2a6b 7761 7267 7329 3a0a       **kwargs):.
+000207e0: 2020 2020 2020 2020 2222 2249 6e69 7461          """Inita
+000207f0: 6c69 7365 7320 6120 4564 6765 4e65 7477  lises a EdgeNetw
+00020800: 6f72 6b20 4c61 7965 720a 0a20 2020 2020  ork Layer..     
+00020810: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00020820: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00020830: 0a20 2020 2020 2020 206e 5f70 6169 725f  .        n_pair_
+00020840: 6665 6174 7572 6573 3a20 696e 742c 206f  features: int, o
+00020850: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00020860: 2020 2020 5468 6520 6c65 6e67 7468 206f      The length o
+00020870: 6620 7468 6520 7061 6972 2066 6561 7475  f the pair featu
+00020880: 7265 7320 7665 6374 6f72 2e0a 2020 2020  res vector..    
+00020890: 2020 2020 6e5f 6869 6464 656e 3a20 696e      n_hidden: in
+000208a0: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+000208b0: 2020 2020 2020 2020 6e75 6d62 6572 206f          number o
+000208c0: 6620 6869 6464 656e 2075 6e69 7473 2069  f hidden units i
+000208d0: 6e20 7468 6520 7061 7373 696e 6720 7068  n the passing ph
+000208e0: 6173 650a 2020 2020 2020 2020 696e 6974  ase.        init
+000208f0: 3a20 7374 722c 206f 7074 696f 6e61 6c0a  : str, optional.
+00020900: 2020 2020 2020 2020 2020 2020 496e 6974              Init
+00020910: 6961 6c69 7a61 7469 6f6e 2066 756e 6374  ialization funct
+00020920: 696f 6e20 746f 2062 6520 7573 6564 2069  ion to be used i
+00020930: 6e20 7468 6520 6d65 7373 6167 6520 7061  n the message pa
+00020940: 7373 696e 6720 6c61 7965 722e 0a20 2020  ssing layer..   
+00020950: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00020960: 2020 7375 7065 7228 4564 6765 4e65 7477    super(EdgeNetw
+00020970: 6f72 6b2c 2073 656c 6629 2e5f 5f69 6e69  ork, self).__ini
+00020980: 745f 5f28 2a2a 6b77 6172 6773 290a 2020  t__(**kwargs).  
+00020990: 2020 2020 2020 7365 6c66 2e6e 5f70 6169        self.n_pai
+000209a0: 725f 6665 6174 7572 6573 3a20 696e 7420  r_features: int 
+000209b0: 3d20 6e5f 7061 6972 5f66 6561 7475 7265  = n_pair_feature
+000209c0: 730a 2020 2020 2020 2020 7365 6c66 2e6e  s.        self.n
+000209d0: 5f68 6964 6465 6e3a 2069 6e74 203d 206e  _hidden: int = n
+000209e0: 5f68 6964 6465 6e0a 2020 2020 2020 2020  _hidden.        
+000209f0: 7365 6c66 2e69 6e69 743a 2073 7472 203d  self.init: str =
+00020a00: 2069 6e69 740a 0a20 2020 2020 2020 2069   init..        i
+00020a10: 6e69 745f 6675 6e63 3a20 4361 6c6c 6162  nit_func: Callab
+00020a20: 6c65 203d 2067 6574 6174 7472 2869 6e69  le = getattr(ini
+00020a30: 7469 616c 697a 6572 732c 2073 656c 662e  tializers, self.
+00020a40: 696e 6974 290a 2020 2020 2020 2020 7365  init).        se
+00020a50: 6c66 2e57 3a20 746f 7263 682e 5465 6e73  lf.W: torch.Tens
+00020a60: 6f72 203d 2069 6e69 745f 6675 6e63 280a  or = init_func(.
+00020a70: 2020 2020 2020 2020 2020 2020 746f 7263              torc
+00020a80: 682e 656d 7074 7928 5b73 656c 662e 6e5f  h.empty([self.n_
+00020a90: 7061 6972 5f66 6561 7475 7265 732c 2073  pair_features, s
+00020aa0: 656c 662e 6e5f 6869 6464 656e 202a 2073  elf.n_hidden * s
+00020ab0: 656c 662e 6e5f 6869 6464 656e 5d29 290a  elf.n_hidden])).
+00020ac0: 2020 2020 2020 2020 7365 6c66 2e62 3a20          self.b: 
+00020ad0: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00020ae0: 6f72 6368 2e7a 6572 6f73 2828 7365 6c66  orch.zeros((self
+00020af0: 2e6e 5f68 6964 6465 6e20 2a20 7365 6c66  .n_hidden * self
+00020b00: 2e6e 5f68 6964 6465 6e2c 2929 0a20 2020  .n_hidden,)).   
+00020b10: 2020 2020 2073 656c 662e 6275 696c 743a       self.built:
+00020b20: 2062 6f6f 6c20 3d20 5472 7565 0a0a 2020   bool = True..  
+00020b30: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
+00020b40: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+00020b50: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
+00020b60: 2020 2020 2020 2020 2020 6627 7b73 656c            f'{sel
+00020b70: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
+00020b80: 6d65 5f5f 7d28 6e5f 7061 6972 5f66 6561  me__}(n_pair_fea
+00020b90: 7475 7265 733a 7b73 656c 662e 6e5f 7061  tures:{self.n_pa
+00020ba0: 6972 5f66 6561 7475 7265 737d 2c6e 5f68  ir_features},n_h
+00020bb0: 6964 6465 6e3a 7b73 656c 662e 6e5f 6869  idden:{self.n_hi
+00020bc0: 6464 656e 7d2c 696e 6974 3a7b 7365 6c66  dden},init:{self
+00020bd0: 2e69 6e69 747d 2927 0a20 2020 2020 2020  .init})'.       
+00020be0: 2029 0a0a 2020 2020 6465 6620 666f 7277   )..    def forw
+00020bf0: 6172 6428 7365 6c66 2c20 696e 7075 7473  ard(self, inputs
+00020c00: 3a20 4c69 7374 5b74 6f72 6368 2e54 656e  : List[torch.Ten
+00020c10: 736f 725d 2920 2d3e 2074 6f72 6368 2e54  sor]) -> torch.T
+00020c20: 656e 736f 723a 0a20 2020 2020 2020 2022  ensor:.        "
+00020c30: 2222 0a20 2020 2020 2020 2050 6172 616d  "".        Param
+00020c40: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00020c50: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00020c60: 2069 6e70 7574 733a 204c 6973 745b 746f   inputs: List[to
+00020c70: 7263 682e 5465 6e73 6f72 5d0a 2020 2020  rch.Tensor].    
+00020c80: 2020 2020 2020 2020 5468 6520 6c65 6e67          The leng
+00020c90: 7468 206f 6620 6174 6f6d 5f74 6f5f 7061  th of atom_to_pa
+00020ca0: 6972 2073 686f 756c 6420 6265 2073 616d  ir should be sam
+00020cb0: 6520 6173 206e 5f70 6169 725f 6665 6174  e as n_pair_feat
+00020cc0: 7572 6573 2e0a 2020 2020 2020 2020 5265  ures..        Re
+00020cd0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00020ce0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7265  -----.        re
+00020cf0: 7375 6c74 3a20 746f 7263 682e 5465 6e73  sult: torch.Tens
+00020d00: 6f72 0a20 2020 2020 2020 2020 2020 2054  or.            T
+00020d10: 656e 736f 7220 636f 6e74 6169 6e69 6e67  ensor containing
+00020d20: 2074 6865 206d 6170 7069 6e67 206f 6620   the mapping of 
+00020d30: 7468 6520 6564 6765 2076 6563 746f 7220  the edge vector 
+00020d40: 746f 2061 2064 20c3 9720 6420 6d61 7472  to a d .. d matr
+00020d50: 6978 2c20 7768 6572 6520 6420 6465 6e6f  ix, where d deno
+00020d60: 7465 7320 7468 6520 6469 6d65 6e73 696f  tes the dimensio
+00020d70: 6e20 6f66 2074 6865 2069 6e74 6572 6e61  n of the interna
+00020d80: 6c20 6869 6464 656e 2072 6570 7265 7365  l hidden represe
+00020d90: 6e74 6174 696f 6e20 6f66 2065 6163 6820  ntation of each 
+00020da0: 6e6f 6465 2069 6e20 7468 6520 6772 6170  node in the grap
+00020db0: 682e 0a20 2020 2020 2020 2022 2222 0a20  h..        """. 
+00020dc0: 2020 2020 2020 2070 6169 725f 6665 6174         pair_feat
+00020dd0: 7572 6573 3a20 746f 7263 682e 5465 6e73  ures: torch.Tens
+00020de0: 6f72 0a20 2020 2020 2020 2061 746f 6d5f  or.        atom_
+00020df0: 6665 6174 7572 6573 3a20 746f 7263 682e  features: torch.
+00020e00: 5465 6e73 6f72 0a20 2020 2020 2020 2061  Tensor.        a
+00020e10: 746f 6d5f 746f 5f70 6169 723a 2074 6f72  tom_to_pair: tor
+00020e20: 6368 2e54 656e 736f 720a 2020 2020 2020  ch.Tensor.      
+00020e30: 2020 7061 6972 5f66 6561 7475 7265 732c    pair_features,
+00020e40: 2061 746f 6d5f 6665 6174 7572 6573 2c20   atom_features, 
+00020e50: 6174 6f6d 5f74 6f5f 7061 6972 203d 2069  atom_to_pair = i
+00020e60: 6e70 7574 730a 0a20 2020 2020 2020 2041  nputs..        A
+00020e70: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+00020e80: 2074 6f72 6368 2e61 6464 2874 6f72 6368   torch.add(torch
+00020e90: 2e6d 6174 6d75 6c28 7061 6972 5f66 6561  .matmul(pair_fea
+00020ea0: 7475 7265 732c 2073 656c 662e 5729 2c20  tures, self.W), 
+00020eb0: 7365 6c66 2e62 290a 2020 2020 2020 2020  self.b).        
+00020ec0: 4120 3d20 746f 7263 682e 7265 7368 6170  A = torch.reshap
+00020ed0: 6528 412c 2028 2d31 2c20 7365 6c66 2e6e  e(A, (-1, self.n
+00020ee0: 5f68 6964 6465 6e2c 2073 656c 662e 6e5f  _hidden, self.n_
+00020ef0: 6869 6464 656e 2929 0a20 2020 2020 2020  hidden)).       
+00020f00: 206f 7574 3a20 746f 7263 682e 5465 6e73   out: torch.Tens
+00020f10: 6f72 203d 2074 6f72 6368 2e75 6e73 7175  or = torch.unsqu
+00020f20: 6565 7a65 2861 746f 6d5f 6665 6174 7572  eeze(atom_featur
+00020f30: 6573 5b61 746f 6d5f 746f 5f70 6169 725b  es[atom_to_pair[
+00020f40: 3a2c 2031 5d5d 2c0a 2020 2020 2020 2020  :, 1]],.        
+00020f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f70: 2020 2020 6469 6d3d 3229 0a20 2020 2020      dim=2).     
+00020f80: 2020 206f 7574 5f73 7175 6565 7a65 3a20     out_squeeze: 
+00020f90: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00020fa0: 6f72 6368 2e73 7175 6565 7a65 2874 6f72  orch.squeeze(tor
+00020fb0: 6368 2e6d 6174 6d75 6c28 412c 206f 7574  ch.matmul(A, out
+00020fc0: 292c 2064 696d 3d32 290a 2020 2020 2020  ), dim=2).      
+00020fd0: 2020 696e 643a 2074 6f72 6368 2e54 656e    ind: torch.Ten
+00020fe0: 736f 7220 3d20 6174 6f6d 5f74 6f5f 7061  sor = atom_to_pa
+00020ff0: 6972 5b3a 2c20 305d 0a0a 2020 2020 2020  ir[:, 0]..      
+00021000: 2020 7265 7375 6c74 3a20 746f 7263 682e    result: torch.
+00021010: 5465 6e73 6f72 203d 2073 6567 6d65 6e74  Tensor = segment
+00021020: 5f73 756d 286f 7574 5f73 7175 6565 7a65  _sum(out_squeeze
+00021030: 2c20 696e 6429 0a0a 2020 2020 2020 2020  , ind)..        
+00021040: 7265 7475 726e 2072 6573 756c 740a 0a0a  return result...
+00021050: 636c 6173 7320 5765 6176 654c 6179 6572  class WeaveLayer
+00021060: 286e 6e2e 4d6f 6475 6c65 293a 0a20 2020  (nn.Module):.   
+00021070: 2022 2222 5468 6973 2063 6c61 7373 2069   """This class i
+00021080: 6d70 6c65 6d65 6e74 7320 7468 6520 636f  mplements the co
+00021090: 7265 2057 6561 7665 2063 6f6e 766f 6c75  re Weave convolu
+000210a0: 7469 6f6e 2066 726f 6d20 7468 6520 476f  tion from the Go
+000210b0: 6f67 6c65 2067 7261 7068 2063 6f6e 766f  ogle graph convo
+000210c0: 6c75 7469 6f6e 2070 6170 6572 205b 315d  lution paper [1]
+000210d0: 5f0a 2020 5468 6973 2069 7320 7468 6520  _.  This is the 
+000210e0: 546f 7263 6820 6571 7569 7661 6c65 6e74  Torch equivalent
+000210f0: 206f 6620 7468 6520 6f72 6967 696e 616c   of the original
+00021100: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00021110: 7573 696e 6720 4b65 7261 732e 0a0a 2020  using Keras...  
+00021120: 5468 6973 206d 6f64 656c 2063 6f6e 7461  This model conta
+00021130: 696e 7320 6174 6f6d 2066 6561 7475 7265  ins atom feature
+00021140: 7320 616e 6420 626f 6e64 2066 6561 7475  s and bond featu
+00021150: 7265 730a 2020 7365 7061 7261 7465 6c79  res.  separately
+00021160: 2e48 6572 652c 2062 6f6e 6420 6665 6174  .Here, bond feat
+00021170: 7572 6573 2061 7265 2061 6c73 6f20 6361  ures are also ca
+00021180: 6c6c 6564 2070 6169 7220 6665 6174 7572  lled pair featur
+00021190: 6573 2e0a 2020 5468 6572 6520 6172 6520  es..  There are 
+000211a0: 3220 7479 7065 7320 6f66 2074 7261 6e73  2 types of trans
+000211b0: 666f 726d 6174 696f 6e2c 2061 746f 6d2d  formation, atom-
+000211c0: 3e61 746f 6d2c 2061 746f 6d2d 3e70 6169  >atom, atom->pai
+000211d0: 722c 2070 6169 722d 3e61 746f 6d2c 2070  r, pair->atom, p
+000211e0: 6169 722d 3e70 6169 7220 7468 6174 2074  air->pair that t
+000211f0: 6869 7320 6d6f 6465 6c20 696d 706c 656d  his model implem
+00021200: 656e 7473 2e0a 0a20 2045 7861 6d70 6c65  ents...  Example
+00021210: 730a 2020 2d2d 2d2d 2d2d 2d2d 0a20 2054  s.  --------.  T
+00021220: 6869 7320 6c61 7965 7220 6578 7065 6374  his layer expect
+00021230: 7320 3420 696e 7075 7473 2069 6e20 6120  s 4 inputs in a 
+00021240: 6c69 7374 206f 6620 7468 6520 666f 726d  list of the form
+00021250: 2060 5b61 746f 6d5f 6665 6174 7572 6573   `[atom_features
+00021260: 2c0a 2020 7061 6972 5f66 6561 7475 7265  ,.  pair_feature
+00021270: 732c 2070 6169 725f 7370 6c69 742c 2061  s, pair_split, a
+00021280: 746f 6d5f 746f 5f70 6169 725d 602e 2057  tom_to_pair]`. W
+00021290: 6527 6c6c 2077 616c 6b20 7468 726f 7567  e'll walk throug
+000212a0: 6820 7468 6520 7374 7275 6374 7572 6520  h the structure 
+000212b0: 6f66 2074 6865 7365 2069 6e70 7574 732e  of these inputs.
+000212c0: 204c 6574 2773 2073 7461 7274 2077 6974   Let's start wit
+000212d0: 6820 736f 6d65 2062 6173 6963 2064 6566  h some basic def
+000212e0: 696e 6974 696f 6e73 2e0a 2020 3e3e 3e20  initions..  >>> 
+000212f0: 696d 706f 7274 2064 6565 7063 6865 6d20  import deepchem 
+00021300: 6173 2064 630a 2020 3e3e 3e20 696d 706f  as dc.  >>> impo
+00021310: 7274 206e 756d 7079 2061 7320 6e70 0a20  rt numpy as np. 
+00021320: 203e 3e3e 2073 6d69 6c65 7320 3d20 5b22   >>> smiles = ["
+00021330: 4343 4322 2c20 2243 225d 0a0a 2020 4e6f  CCC", "C"]..  No
+00021340: 7465 2074 6861 7420 7468 6572 6520 6172  te that there ar
+00021350: 6520 3420 6174 6f6d 7320 696e 2074 6f74  e 4 atoms in tot
+00021360: 616c 2069 6e20 7468 6973 2073 7973 7465  al in this syste
+00021370: 6d2e 2054 6869 7320 6c61 7965 7220 6578  m. This layer ex
+00021380: 7065 6374 7320 6974 7320 696e 7075 7420  pects its input 
+00021390: 6d6f 6c65 6375 6c65 7320 746f 2062 6520  molecules to be 
+000213a0: 6261 7463 6865 6420 746f 6765 7468 6572  batched together
+000213b0: 2e0a 0a20 203e 3e3e 2074 6f74 616c 5f6e  ...  >>> total_n
+000213c0: 5f61 746f 6d73 203d 2034 0a0a 2020 4c65  _atoms = 4..  Le
+000213d0: 7427 7320 7375 7070 6f73 6520 7468 6174  t's suppose that
+000213e0: 2077 6520 6861 7665 2061 2066 6561 7475   we have a featu
+000213f0: 7269 7a65 7220 7468 6174 2063 6f6d 7075  rizer that compu
+00021400: 7465 7320 606e 5f61 746f 6d5f 6665 6174  tes `n_atom_feat
+00021410: 6020 6665 6174 7572 6573 2070 6572 2061  ` features per a
+00021420: 746f 6d2e 0a0a 2020 3e3e 3e20 6e5f 6174  tom...  >>> n_at
+00021430: 6f6d 5f66 6561 7420 3d20 3735 0a0a 2020  om_feat = 75..  
+00021440: 5468 656e 2063 6f6e 6365 7074 7561 6c6c  Then conceptuall
+00021450: 792c 2060 6174 6f6d 5f66 6561 7460 2069  y, `atom_feat` i
+00021460: 7320 7468 6520 6172 7261 7920 6f66 2073  s the array of s
+00021470: 6861 7065 2060 2874 6f74 616c 5f6e 5f61  hape `(total_n_a
+00021480: 746f 6d73 2c0a 2020 6e5f 6174 6f6d 5f66  toms,.  n_atom_f
+00021490: 6561 7429 6020 6f66 2061 746f 6d69 6320  eat)` of atomic 
+000214a0: 6665 6174 7572 6573 2e20 466f 7220 7369  features. For si
+000214b0: 6d70 6c69 6369 7479 2c20 6c65 7427 7320  mplicity, let's 
+000214c0: 6a75 7374 2067 6f20 7769 7468 2061 0a20  just go with a. 
+000214d0: 2072 616e 646f 6d20 7375 6368 206d 6174   random such mat
+000214e0: 7269 782e 0a0a 2020 3e3e 3e20 6174 6f6d  rix...  >>> atom
+000214f0: 5f66 6561 7420 3d20 6e70 2e72 616e 646f  _feat = np.rando
+00021500: 6d2e 7261 6e64 2874 6f74 616c 5f6e 5f61  m.rand(total_n_a
+00021510: 746f 6d73 2c20 6e5f 6174 6f6d 5f66 6561  toms, n_atom_fea
+00021520: 7429 0a0a 2020 4c65 7427 7320 7375 7070  t)..  Let's supp
+00021530: 6f73 6520 7765 2068 6176 6520 606e 5f70  ose we have `n_p
+00021540: 6169 725f 6665 6174 6020 7061 6972 7769  air_feat` pairwi
+00021550: 7365 2066 6561 7475 7265 730a 0a20 203e  se features..  >
+00021560: 3e3e 206e 5f70 6169 725f 6665 6174 203d  >> n_pair_feat =
+00021570: 2031 340a 0a20 2046 6f72 2065 6163 6820   14..  For each 
+00021580: 6d6f 6c65 6375 6c65 2c20 7765 2063 6f6d  molecule, we com
+00021590: 7075 7465 2061 206d 6174 7269 7820 6f66  pute a matrix of
+000215a0: 2073 6861 7065 2060 286e 5f61 746f 6d73   shape `(n_atoms
+000215b0: 2a6e 5f61 746f 6d73 2c0a 2020 6e5f 7061  *n_atoms,.  n_pa
+000215c0: 6972 5f66 6561 7429 6020 6f66 2070 6169  ir_feat)` of pai
+000215d0: 7277 6973 6520 6665 6174 7572 6573 2066  rwise features f
+000215e0: 6f72 2065 6163 6820 7061 6972 206f 6620  or each pair of 
+000215f0: 6174 6f6d 7320 696e 2074 6865 206d 6f6c  atoms in the mol
+00021600: 6563 756c 652e 0a20 204c 6574 2773 2063  ecule..  Let's c
+00021610: 6f6e 7374 7275 6374 2074 6869 7320 636f  onstruct this co
+00021620: 6e63 6570 7475 616c 6c79 2066 6f72 206f  nceptually for o
+00021630: 7572 2065 7861 6d70 6c65 2e0a 0a20 203e  ur example...  >
+00021640: 3e3e 2070 6169 725f 6665 6174 203d 205b  >> pair_feat = [
+00021650: 6e70 2e72 616e 646f 6d2e 7261 6e64 2833  np.random.rand(3
+00021660: 2a33 2c20 6e5f 7061 6972 5f66 6561 7429  *3, n_pair_feat)
+00021670: 2c20 6e70 2e72 616e 646f 6d2e 7261 6e64  , np.random.rand
+00021680: 2831 2a31 2c6e 5f70 6169 725f 6665 6174  (1*1,n_pair_feat
+00021690: 295d 0a20 203e 3e3e 2070 6169 725f 6665  )].  >>> pair_fe
+000216a0: 6174 203d 206e 702e 636f 6e63 6174 656e  at = np.concaten
+000216b0: 6174 6528 7061 6972 5f66 6561 742c 2061  ate(pair_feat, a
+000216c0: 7869 733d 3029 0a20 203e 3e3e 2070 6169  xis=0).  >>> pai
+000216d0: 725f 6665 6174 2e73 6861 7065 0a20 2028  r_feat.shape.  (
+000216e0: 3130 2c20 3134 290a 0a20 2060 7061 6972  10, 14)..  `pair
+000216f0: 5f73 706c 6974 6020 6973 2061 6e20 696e  _split` is an in
+00021700: 6465 7820 696e 746f 2060 7061 6972 5f66  dex into `pair_f
+00021710: 6561 7460 2077 6869 6368 2074 656c 6c73  eat` which tells
+00021720: 2075 7320 7768 6963 6820 6174 6f6d 2065   us which atom e
+00021730: 6163 6820 726f 7720 6265 6c6f 6e67 7320  ach row belongs 
+00021740: 746f 2e20 496e 206f 7572 2063 6173 652c  to. In our case,
+00021750: 2077 6520 6876 650a 0a20 203e 3e3e 2070   we hve..  >>> p
+00021760: 6169 725f 7370 6c69 7420 3d20 6e70 2e61  air_split = np.a
+00021770: 7272 6179 285b 302c 2030 2c20 302c 2031  rray([0, 0, 0, 1
+00021780: 2c20 312c 2031 2c20 322c 2032 2c20 322c  , 1, 1, 2, 2, 2,
+00021790: 2033 5d29 0a0a 2020 5468 6174 2069 732c   3])..  That is,
+000217a0: 2074 6865 2066 6972 7374 2039 2065 6e74   the first 9 ent
+000217b0: 7269 6573 2062 656c 6f6e 6720 746f 2022  ries belong to "
+000217c0: 4343 4322 2061 6e64 2074 6865 206c 6173  CCC" and the las
+000217d0: 7420 656e 7472 7920 746f 2022 4322 2e20  t entry to "C". 
+000217e0: 5468 650a 2020 6669 6e61 6c20 656e 7472  The.  final entr
+000217f0: 7920 6061 746f 6d5f 746f 5f70 6169 7260  y `atom_to_pair`
+00021800: 2067 6f65 7320 696e 2061 206c 6974 746c   goes in a littl
+00021810: 6520 6d6f 7265 2069 6e2d 6465 7074 6820  e more in-depth 
+00021820: 7468 616e 2060 7061 6972 5f73 706c 6974  than `pair_split
+00021830: 600a 2020 616e 6420 7465 6c6c 7320 7573  `.  and tells us
+00021840: 2074 6865 2070 7265 6369 7365 2070 6169   the precise pai
+00021850: 7220 6561 6368 2070 6169 7220 6665 6174  r each pair feat
+00021860: 7572 6520 6265 6c6f 6e67 7320 746f 2e20  ure belongs to. 
+00021870: 496e 206f 7572 2063 6173 650a 0a20 203e  In our case..  >
+00021880: 3e3e 2061 746f 6d5f 746f 5f70 6169 7220  >> atom_to_pair 
+00021890: 3d20 6e70 2e61 7272 6179 285b 5b30 2c20  = np.array([[0, 
+000218a0: 305d 2c0a 2020 2e2e 2e20 2020 2020 2020  0],.  ...       
+000218b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000218c0: 2020 205b 302c 2031 5d2c 0a20 202e 2e2e     [0, 1],.  ...
+000218d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000218e0: 2020 2020 2020 2020 2020 5b30 2c20 325d            [0, 2]
+000218f0: 2c0a 2020 2e2e 2e20 2020 2020 2020 2020  ,.  ...         
+00021900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021910: 205b 312c 2030 5d2c 0a20 202e 2e2e 2020   [1, 0],.  ...  
+00021920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021930: 2020 2020 2020 2020 5b31 2c20 315d 2c0a          [1, 1],.
+00021940: 2020 2e2e 2e20 2020 2020 2020 2020 2020    ...           
+00021950: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00021960: 312c 2032 5d2c 0a20 202e 2e2e 2020 2020  1, 2],.  ...    
+00021970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021980: 2020 2020 2020 5b32 2c20 305d 2c0a 2020        [2, 0],.  
+00021990: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+000219a0: 2020 2020 2020 2020 2020 2020 205b 322c               [2,
+000219b0: 2031 5d2c 0a20 202e 2e2e 2020 2020 2020   1],.  ...      
+000219c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000219d0: 2020 2020 5b32 2c20 325d 2c0a 2020 2e2e      [2, 2],.  ..
+000219e0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+000219f0: 2020 2020 2020 2020 2020 205b 332c 2033             [3, 3
+00021a00: 5d5d 290a 0a20 204c 6574 2773 206e 6f77  ]])..  Let's now
+00021a10: 2064 6566 696e 6520 7468 6520 6163 7475   define the actu
+00021a20: 616c 206c 6179 6572 0a0a 2020 3e3e 3e20  al layer..  >>> 
+00021a30: 6c61 7965 7220 3d20 5765 6176 654c 6179  layer = WeaveLay
+00021a40: 6572 2829 0a0a 2020 416e 6420 696e 766f  er()..  And invo
+00021a50: 6b65 2069 740a 0a20 203e 3e3e 205b 412c  ke it..  >>> [A,
+00021a60: 2050 5d20 3d20 6c61 7965 7228 5b61 746f   P] = layer([ato
+00021a70: 6d5f 6665 6174 2c20 7061 6972 5f66 6561  m_feat, pair_fea
+00021a80: 742c 2070 6169 725f 7370 6c69 742c 2061  t, pair_split, a
+00021a90: 746f 6d5f 746f 5f70 6169 725d 290a 0a20  tom_to_pair]).. 
+00021aa0: 2054 6865 2077 6561 7665 206c 6179 6572   The weave layer
+00021ab0: 2070 726f 6475 6365 7320 6e65 7720 6174   produces new at
+00021ac0: 6f6d 2f70 6169 7220 6665 6174 7572 6573  om/pair features
+00021ad0: 2e20 4c65 7427 7320 6368 6563 6b20 7468  . Let's check th
+00021ae0: 6569 7220 7368 6170 6573 0a0a 2020 3e3e  eir shapes..  >>
+00021af0: 3e20 4120 3d20 412e 6465 7461 6368 2829  > A = A.detach()
+00021b00: 2e6e 756d 7079 2829 0a20 203e 3e3e 2041  .numpy().  >>> A
+00021b10: 2e73 6861 7065 0a20 2028 342c 2035 3029  .shape.  (4, 50)
+00021b20: 0a20 203e 3e3e 2050 203d 2050 2e64 6574  .  >>> P = P.det
+00021b30: 6163 6828 292e 6e75 6d70 7928 290a 2020  ach().numpy().  
+00021b40: 3e3e 3e20 502e 7368 6170 650a 2020 2831  >>> P.shape.  (1
+00021b50: 302c 2035 3029 0a0a 2020 5468 6520 3420  0, 50)..  The 4 
+00021b60: 6973 2060 746f 7461 6c5f 6e75 6d5f 6174  is `total_num_at
+00021b70: 6f6d 7360 2061 6e64 2074 6865 2031 3020  oms` and the 10 
+00021b80: 6973 2074 6865 2074 6f74 616c 206e 756d  is the total num
+00021b90: 6265 7220 6f66 2070 6169 7273 2e20 5768  ber of pairs. Wh
+00021ba0: 6572 650a 2020 646f 6573 2060 3530 6020  ere.  does `50` 
+00021bb0: 636f 6d65 2066 726f 6d3f 2049 7427 7320  come from? It's 
+00021bc0: 6672 6f6d 2074 6865 2064 6566 6175 6c74  from the default
+00021bd0: 2061 7267 756d 656e 7473 2060 6e5f 6174   arguments `n_at
+00021be0: 6f6d 5f69 6e70 7574 5f66 6561 7460 2061  om_input_feat` a
+00021bf0: 6e64 0a20 2060 6e5f 7061 6972 5f69 6e70  nd.  `n_pair_inp
+00021c00: 7574 5f66 6561 7460 2e0a 0a20 2052 6566  ut_feat`...  Ref
+00021c10: 6572 656e 6365 730a 2020 2d2d 2d2d 2d2d  erences.  ------
+00021c20: 2d2d 2d2d 0a20 202e 2e20 5b31 5d20 4b65  ----.  .. [1] Ke
+00021c30: 6172 6e65 732c 2053 7465 7665 6e2c 2065  arnes, Steven, e
+00021c40: 7420 616c 2e20 224d 6f6c 6563 756c 6172  t al. "Molecular
+00021c50: 2067 7261 7068 2063 6f6e 766f 6c75 7469   graph convoluti
+00021c60: 6f6e 733a 206d 6f76 696e 6720 6265 796f  ons: moving beyo
+00021c70: 6e64 0a20 2020 2020 2020 2066 696e 6765  nd.        finge
+00021c80: 7270 7269 6e74 732e 2220 4a6f 7572 6e61  rprints." Journa
+00021c90: 6c20 6f66 2063 6f6d 7075 7465 722d 6169  l of computer-ai
+00021ca0: 6465 6420 6d6f 6c65 6375 6c61 7220 6465  ded molecular de
+00021cb0: 7369 676e 2033 302e 3820 2832 3031 3629  sign 30.8 (2016)
+00021cc0: 3a0a 2020 2020 2020 2020 3539 352d 3630  :.        595-60
+00021cd0: 382e 0a20 2022 2222 0a0a 2020 2020 6465  8..  """..    de
+00021ce0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00021cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021d00: 2020 6e5f 6174 6f6d 5f69 6e70 7574 5f66    n_atom_input_f
+00021d10: 6561 743a 2069 6e74 203d 2037 352c 0a20  eat: int = 75,. 
+00021d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021d30: 6e5f 7061 6972 5f69 6e70 7574 5f66 6561  n_pair_input_fea
+00021d40: 743a 2069 6e74 203d 2031 342c 0a20 2020  t: int = 14,.   
+00021d50: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+00021d60: 6174 6f6d 5f6f 7574 7075 745f 6665 6174  atom_output_feat
+00021d70: 3a20 696e 7420 3d20 3530 2c0a 2020 2020  : int = 50,.    
+00021d80: 2020 2020 2020 2020 2020 2020 206e 5f70               n_p
+00021d90: 6169 725f 6f75 7470 7574 5f66 6561 743a  air_output_feat:
+00021da0: 2069 6e74 203d 2035 302c 0a20 2020 2020   int = 50,.     
+00021db0: 2020 2020 2020 2020 2020 2020 6e5f 6869              n_hi
+00021dc0: 6464 656e 5f41 413a 2069 6e74 203d 2035  dden_AA: int = 5
+00021dd0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00021de0: 2020 2020 6e5f 6869 6464 656e 5f50 413a      n_hidden_PA:
+00021df0: 2069 6e74 203d 2035 302c 0a20 2020 2020   int = 50,.     
+00021e00: 2020 2020 2020 2020 2020 2020 6e5f 6869              n_hi
+00021e10: 6464 656e 5f41 503a 2069 6e74 203d 2035  dden_AP: int = 5
+00021e20: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00021e30: 2020 2020 6e5f 6869 6464 656e 5f50 503a      n_hidden_PP:
+00021e40: 2069 6e74 203d 2035 302c 0a20 2020 2020   int = 50,.     
+00021e50: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+00021e60: 7465 5f70 6169 723a 2062 6f6f 6c20 3d20  te_pair: bool = 
+00021e70: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00021e80: 2020 2020 2020 2069 6e69 745f 3a20 7374         init_: st
+00021e90: 7220 3d20 2778 6176 6965 725f 756e 6966  r = 'xavier_unif
+00021ea0: 6f72 6d5f 272c 0a20 2020 2020 2020 2020  orm_',.         
+00021eb0: 2020 2020 2020 2020 6163 7469 7661 7469          activati
+00021ec0: 6f6e 3a20 7374 7220 3d20 2772 656c 7527  on: str = 'relu'
+00021ed0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021ee0: 2020 2062 6174 6368 5f6e 6f72 6d61 6c69     batch_normali
+00021ef0: 7a65 3a20 626f 6f6c 203d 2054 7275 652c  ze: bool = True,
+00021f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021f10: 2020 2a2a 6b77 6172 6773 293a 0a20 2020    **kwargs):.   
+00021f20: 2020 2020 2022 2222 0a20 2020 2050 6172       """.    Par
+00021f30: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00021f40: 2d2d 2d2d 2d2d 0a20 2020 206e 5f61 746f  ------.    n_ato
+00021f50: 6d5f 696e 7075 745f 6665 6174 3a20 696e  m_input_feat: in
+00021f60: 742c 206f 7074 696f 6e61 6c20 2864 6566  t, optional (def
+00021f70: 6175 6c74 2037 3529 0a20 2020 2020 204e  ault 75).      N
+00021f80: 756d 6265 7220 6f66 2066 6561 7475 7265  umber of feature
+00021f90: 7320 666f 7220 6561 6368 2061 746f 6d20  s for each atom 
+00021fa0: 696e 2069 6e70 7574 2e0a 2020 2020 6e5f  in input..    n_
+00021fb0: 7061 6972 5f69 6e70 7574 5f66 6561 743a  pair_input_feat:
+00021fc0: 2069 6e74 2c20 6f70 7469 6f6e 616c 2028   int, optional (
+00021fd0: 6465 6661 756c 7420 3134 290a 2020 2020  default 14).    
+00021fe0: 2020 4e75 6d62 6572 206f 6620 6665 6174    Number of feat
+00021ff0: 7572 6573 2066 6f72 2065 6163 6820 7061  ures for each pa
+00022000: 6972 206f 6620 6174 6f6d 7320 696e 2069  ir of atoms in i
+00022010: 6e70 7574 2e0a 2020 2020 6e5f 6174 6f6d  nput..    n_atom
+00022020: 5f6f 7574 7075 745f 6665 6174 3a20 696e  _output_feat: in
+00022030: 742c 206f 7074 696f 6e61 6c20 2864 6566  t, optional (def
+00022040: 6175 6c74 2035 3029 0a20 2020 2020 204e  ault 50).      N
+00022050: 756d 6265 7220 6f66 2066 6561 7475 7265  umber of feature
+00022060: 7320 666f 7220 6561 6368 2061 746f 6d20  s for each atom 
+00022070: 696e 206f 7574 7075 742e 0a20 2020 206e  in output..    n
+00022080: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
+00022090: 743a 2069 6e74 2c20 6f70 7469 6f6e 616c  t: int, optional
+000220a0: 2028 6465 6661 756c 7420 3530 290a 2020   (default 50).  
+000220b0: 2020 2020 4e75 6d62 6572 206f 6620 6665      Number of fe
+000220c0: 6174 7572 6573 2066 6f72 2065 6163 6820  atures for each 
+000220d0: 7061 6972 206f 6620 6174 6f6d 7320 696e  pair of atoms in
+000220e0: 206f 7574 7075 742e 0a20 2020 206e 5f68   output..    n_h
+000220f0: 6964 6465 6e5f 4141 3a20 696e 742c 206f  idden_AA: int, o
+00022100: 7074 696f 6e61 6c20 2864 6566 6175 6c74  ptional (default
+00022110: 2035 3029 0a20 2020 2020 204e 756d 6265   50).      Numbe
+00022120: 7220 6f66 2075 6e69 7473 2863 6f6e 766f  r of units(convo
+00022130: 6c75 7469 6f6e 2064 6570 7468 7329 2069  lution depths) i
+00022140: 6e20 636f 7272 6573 706f 6e64 696e 6720  n corresponding 
+00022150: 6869 6464 656e 206c 6179 6572 0a20 2020  hidden layer.   
+00022160: 206e 5f68 6964 6465 6e5f 5041 3a20 696e   n_hidden_PA: in
+00022170: 742c 206f 7074 696f 6e61 6c20 2864 6566  t, optional (def
+00022180: 6175 6c74 2035 3029 0a20 2020 2020 204e  ault 50).      N
+00022190: 756d 6265 7220 6f66 2075 6e69 7473 2863  umber of units(c
+000221a0: 6f6e 766f 6c75 7469 6f6e 2064 6570 7468  onvolution depth
+000221b0: 7329 2069 6e20 636f 7272 6573 706f 6e64  s) in correspond
+000221c0: 696e 6720 6869 6464 656e 206c 6179 6572  ing hidden layer
+000221d0: 0a20 2020 206e 5f68 6964 6465 6e5f 4150  .    n_hidden_AP
+000221e0: 3a20 696e 742c 206f 7074 696f 6e61 6c20  : int, optional 
+000221f0: 2864 6566 6175 6c74 2035 3029 0a20 2020  (default 50).   
+00022200: 2020 204e 756d 6265 7220 6f66 2075 6e69     Number of uni
+00022210: 7473 2863 6f6e 766f 6c75 7469 6f6e 2064  ts(convolution d
+00022220: 6570 7468 7329 2069 6e20 636f 7272 6573  epths) in corres
+00022230: 706f 6e64 696e 6720 6869 6464 656e 206c  ponding hidden l
+00022240: 6179 6572 0a20 2020 206e 5f68 6964 6465  ayer.    n_hidde
+00022250: 6e5f 5050 3a20 696e 742c 206f 7074 696f  n_PP: int, optio
+00022260: 6e61 6c20 2864 6566 6175 6c74 2035 3029  nal (default 50)
+00022270: 0a20 2020 2020 204e 756d 6265 7220 6f66  .      Number of
+00022280: 2075 6e69 7473 2863 6f6e 766f 6c75 7469   units(convoluti
+00022290: 6f6e 2064 6570 7468 7329 2069 6e20 636f  on depths) in co
+000222a0: 7272 6573 706f 6e64 696e 6720 6869 6464  rresponding hidd
+000222b0: 656e 206c 6179 6572 0a20 2020 2075 7064  en layer.    upd
+000222c0: 6174 655f 7061 6972 3a20 626f 6f6c 2c20  ate_pair: bool, 
+000222d0: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+000222e0: 7420 5472 7565 290a 2020 2020 2020 5768  t True).      Wh
+000222f0: 6574 6865 7220 746f 2063 616c 6375 6c61  ether to calcula
+00022300: 7465 2066 6f72 2070 6169 7220 6665 6174  te for pair feat
+00022310: 7572 6573 2c0a 2020 2020 2020 636f 756c  ures,.      coul
+00022320: 6420 6265 2074 7572 6e65 6420 6f66 6620  d be turned off 
+00022330: 666f 7220 6c61 7374 206c 6179 6572 0a20  for last layer. 
+00022340: 2020 2069 6e69 743a 2073 7472 2c20 6f70     init: str, op
+00022350: 7469 6f6e 616c 2028 6465 6661 756c 7420  tional (default 
+00022360: 2778 6176 6965 725f 756e 6966 6f72 6d5f  'xavier_uniform_
+00022370: 2729 0a20 2020 2020 2057 6569 6768 7420  ').      Weight 
+00022380: 696e 6974 6961 6c69 7a61 7469 6f6e 2066  initialization f
+00022390: 6f72 2066 696c 7465 7273 2e0a 2020 2020  or filters..    
+000223a0: 6163 7469 7661 7469 6f6e 3a20 7374 722c  activation: str,
+000223b0: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
+000223c0: 6c74 2027 7265 6c75 2729 0a20 2020 2020  lt 'relu').     
+000223d0: 2041 6374 6976 6174 696f 6e20 6675 6e63   Activation func
+000223e0: 7469 6f6e 2061 7070 6c69 6564 0a20 2020  tion applied.   
+000223f0: 2062 6174 6368 5f6e 6f72 6d61 6c69 7a65   batch_normalize
+00022400: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00022410: 2028 6465 6661 756c 7420 5472 7565 290a   (default True).
+00022420: 2020 2020 2020 4966 2074 6869 7320 6973        If this is
+00022430: 2074 7572 6e65 6420 6f6e 2c20 6170 706c   turned on, appl
+00022440: 7920 6261 7463 6820 6e6f 726d 616c 697a  y batch normaliz
+00022450: 6174 696f 6e20 6265 666f 7265 2061 7070  ation before app
+00022460: 6c79 696e 670a 2020 2020 2020 6163 7469  lying.      acti
+00022470: 7661 7469 6f6e 2066 756e 6374 696f 6e73  vation functions
+00022480: 206f 6e20 636f 6e76 6f6c 7574 696f 6e61   on convolutiona
+00022490: 6c20 6c61 7965 7273 2e0a 2020 2020 2222  l layers..    ""
+000224a0: 220a 2020 2020 2020 2020 7375 7065 7228  ".        super(
+000224b0: 5765 6176 654c 6179 6572 2c20 7365 6c66  WeaveLayer, self
+000224c0: 292e 5f5f 696e 6974 5f5f 282a 2a6b 7761  ).__init__(**kwa
+000224d0: 7267 7329 0a20 2020 2020 2020 2073 656c  rgs).        sel
+000224e0: 662e 696e 6974 3a20 7374 7220 3d20 696e  f.init: str = in
+000224f0: 6974 5f20 2023 2053 6574 2077 6569 6768  it_  # Set weigh
+00022500: 7420 696e 6974 6961 6c69 7a61 7469 6f6e  t initialization
+00022510: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+00022520: 7469 7661 7469 6f6e 3a20 7374 7220 3d20  tivation: str = 
+00022530: 6163 7469 7661 7469 6f6e 2020 2320 4765  activation  # Ge
+00022540: 7420 6163 7469 7661 7469 6f6e 730a 2020  t activations.  
+00022550: 2020 2020 2020 7365 6c66 2e61 6374 6976        self.activ
+00022560: 6174 696f 6e5f 666e 3a20 746f 7263 682e  ation_fn: torch.
+00022570: 6e6e 2e4d 6f64 756c 6520 3d20 6765 745f  nn.Module = get_
+00022580: 6163 7469 7661 7469 6f6e 2861 6374 6976  activation(activ
+00022590: 6174 696f 6e29 0a20 2020 2020 2020 2073  ation).        s
+000225a0: 656c 662e 7570 6461 7465 5f70 6169 723a  elf.update_pair:
+000225b0: 2062 6f6f 6c20 3d20 7570 6461 7465 5f70   bool = update_p
+000225c0: 6169 7220 2023 206c 6173 7420 7765 6176  air  # last weav
+000225d0: 6520 6c61 7965 7220 646f 6573 206e 6f74  e layer does not
+000225e0: 206e 6565 6420 746f 2075 7064 6174 650a   need to update.
+000225f0: 2020 2020 2020 2020 7365 6c66 2e6e 5f68          self.n_h
+00022600: 6964 6465 6e5f 4141 3a20 696e 7420 3d20  idden_AA: int = 
+00022610: 6e5f 6869 6464 656e 5f41 410a 2020 2020  n_hidden_AA.    
+00022620: 2020 2020 7365 6c66 2e6e 5f68 6964 6465      self.n_hidde
+00022630: 6e5f 5041 3a20 696e 7420 3d20 6e5f 6869  n_PA: int = n_hi
+00022640: 6464 656e 5f50 410a 2020 2020 2020 2020  dden_PA.        
+00022650: 7365 6c66 2e6e 5f68 6964 6465 6e5f 4150  self.n_hidden_AP
+00022660: 3a20 696e 7420 3d20 6e5f 6869 6464 656e  : int = n_hidden
+00022670: 5f41 500a 2020 2020 2020 2020 7365 6c66  _AP.        self
+00022680: 2e6e 5f68 6964 6465 6e5f 5050 3a20 696e  .n_hidden_PP: in
+00022690: 7420 3d20 6e5f 6869 6464 656e 5f50 500a  t = n_hidden_PP.
+000226a0: 2020 2020 2020 2020 7365 6c66 2e6e 5f68          self.n_h
+000226b0: 6964 6465 6e5f 413a 2069 6e74 203d 206e  idden_A: int = n
+000226c0: 5f68 6964 6465 6e5f 4141 202b 206e 5f68  _hidden_AA + n_h
+000226d0: 6964 6465 6e5f 5041 0a20 2020 2020 2020  idden_PA.       
+000226e0: 2073 656c 662e 6e5f 6869 6464 656e 5f50   self.n_hidden_P
+000226f0: 3a20 696e 7420 3d20 6e5f 6869 6464 656e  : int = n_hidden
+00022700: 5f41 5020 2b20 6e5f 6869 6464 656e 5f50  _AP + n_hidden_P
+00022710: 500a 2020 2020 2020 2020 7365 6c66 2e62  P.        self.b
+00022720: 6174 6368 5f6e 6f72 6d61 6c69 7a65 3a20  atch_normalize: 
+00022730: 626f 6f6c 203d 2062 6174 6368 5f6e 6f72  bool = batch_nor
+00022740: 6d61 6c69 7a65 0a0a 2020 2020 2020 2020  malize..        
+00022750: 7365 6c66 2e6e 5f61 746f 6d5f 696e 7075  self.n_atom_inpu
+00022760: 745f 6665 6174 3a20 696e 7420 3d20 6e5f  t_feat: int = n_
+00022770: 6174 6f6d 5f69 6e70 7574 5f66 6561 740a  atom_input_feat.
+00022780: 2020 2020 2020 2020 7365 6c66 2e6e 5f70          self.n_p
+00022790: 6169 725f 696e 7075 745f 6665 6174 3a20  air_input_feat: 
+000227a0: 696e 7420 3d20 6e5f 7061 6972 5f69 6e70  int = n_pair_inp
+000227b0: 7574 5f66 6561 740a 2020 2020 2020 2020  ut_feat.        
+000227c0: 7365 6c66 2e6e 5f61 746f 6d5f 6f75 7470  self.n_atom_outp
+000227d0: 7574 5f66 6561 743a 2069 6e74 203d 206e  ut_feat: int = n
+000227e0: 5f61 746f 6d5f 6f75 7470 7574 5f66 6561  _atom_output_fea
+000227f0: 740a 2020 2020 2020 2020 7365 6c66 2e6e  t.        self.n
+00022800: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
+00022810: 743a 2069 6e74 203d 206e 5f70 6169 725f  t: int = n_pair_
+00022820: 6f75 7470 7574 5f66 6561 740a 0a20 2020  output_feat..   
+00022830: 2020 2020 2023 2043 6f6e 7374 7275 6374       # Construct
+00022840: 2069 6e74 6572 6e61 6c20 7472 6169 6e61   internal traina
+00022850: 626c 6520 7765 6967 6874 730a 2020 2020  ble weights.    
+00022860: 2020 2020 696e 6974 203d 2067 6574 6174      init = getat
+00022870: 7472 2869 6e69 7469 616c 697a 6572 732c  tr(initializers,
+00022880: 2073 656c 662e 696e 6974 290a 2020 2020   self.init).    
+00022890: 2020 2020 2320 5765 6967 6874 206d 6174      # Weight mat
+000228a0: 7269 7820 616e 6420 6269 6173 206d 6174  rix and bias mat
+000228b0: 7269 7820 7265 7175 6972 6564 2074 6f20  rix required to 
+000228c0: 636f 6d70 7574 6520 6e65 7720 6174 6f6d  compute new atom
+000228d0: 206c 6179 6572 2066 726f 6d20 7468 6520   layer from the 
+000228e0: 7072 6576 696f 7573 2061 746f 6d20 6c61  previous atom la
+000228f0: 7965 720a 2020 2020 2020 2020 7365 6c66  yer.        self
+00022900: 2e57 5f41 413a 2074 6f72 6368 2e54 656e  .W_AA: torch.Ten
+00022910: 736f 7220 3d20 696e 6974 280a 2020 2020  sor = init(.    
+00022920: 2020 2020 2020 2020 746f 7263 682e 656d          torch.em
+00022930: 7074 7928 7365 6c66 2e6e 5f61 746f 6d5f  pty(self.n_atom_
+00022940: 696e 7075 745f 6665 6174 2c20 7365 6c66  input_feat, self
+00022950: 2e6e 5f68 6964 6465 6e5f 4141 2929 0a20  .n_hidden_AA)). 
+00022960: 2020 2020 2020 2073 656c 662e 625f 4141         self.b_AA
+00022970: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+00022980: 2074 6f72 6368 2e7a 6572 6f73 2828 7365   torch.zeros((se
+00022990: 6c66 2e6e 5f68 6964 6465 6e5f 4141 2c29  lf.n_hidden_AA,)
+000229a0: 290a 2020 2020 2020 2020 7365 6c66 2e41  ).        self.A
+000229b0: 415f 626e 3a20 6e6e 2e42 6174 6368 4e6f  A_bn: nn.BatchNo
+000229c0: 726d 3164 203d 206e 6e2e 4261 7463 684e  rm1d = nn.BatchN
+000229d0: 6f72 6d31 6428 0a20 2020 2020 2020 2020  orm1d(.         
+000229e0: 2020 206e 756d 5f66 6561 7475 7265 733d     num_features=
+000229f0: 7365 6c66 2e6e 5f68 6964 6465 6e5f 4141  self.n_hidden_AA
+00022a00: 2c0a 2020 2020 2020 2020 2020 2020 6570  ,.            ep
+00022a10: 733d 3165 2d33 2c0a 2020 2020 2020 2020  s=1e-3,.        
+00022a20: 2020 2020 6d6f 6d65 6e74 756d 3d30 2e39      momentum=0.9
+00022a30: 392c 0a20 2020 2020 2020 2020 2020 2061  9,.            a
+00022a40: 6666 696e 653d 5472 7565 2c0a 2020 2020  ffine=True,.    
+00022a50: 2020 2020 2020 2020 7472 6163 6b5f 7275          track_ru
+00022a60: 6e6e 696e 675f 7374 6174 733d 5472 7565  nning_stats=True
+00022a70: 290a 0a20 2020 2020 2020 2023 2057 6569  )..        # Wei
+00022a80: 6768 7420 6d61 7472 6978 2061 6e64 2062  ght matrix and b
+00022a90: 6961 7320 6d61 7472 6978 2072 6571 7569  ias matrix requi
+00022aa0: 7265 6420 746f 2063 6f6d 7075 7465 206e  red to compute n
+00022ab0: 6577 2061 746f 6d20 6c61 7965 7220 6672  ew atom layer fr
+00022ac0: 6f6d 2074 6865 2070 7265 7669 6f75 7320  om the previous 
+00022ad0: 7061 6972 206c 6179 6572 0a20 2020 2020  pair layer.     
+00022ae0: 2020 2073 656c 662e 575f 5041 3a20 746f     self.W_PA: to
+00022af0: 7263 682e 5465 6e73 6f72 203d 2069 6e69  rch.Tensor = ini
+00022b00: 7428 0a20 2020 2020 2020 2020 2020 2074  t(.            t
+00022b10: 6f72 6368 2e65 6d70 7479 2873 656c 662e  orch.empty(self.
+00022b20: 6e5f 7061 6972 5f69 6e70 7574 5f66 6561  n_pair_input_fea
+00022b30: 742c 2073 656c 662e 6e5f 6869 6464 656e  t, self.n_hidden
+00022b40: 5f50 4129 290a 2020 2020 2020 2020 7365  _PA)).        se
+00022b50: 6c66 2e62 5f50 413a 2074 6f72 6368 2e54  lf.b_PA: torch.T
+00022b60: 656e 736f 7220 3d20 746f 7263 682e 7a65  ensor = torch.ze
+00022b70: 726f 7328 2873 656c 662e 6e5f 6869 6464  ros((self.n_hidd
+00022b80: 656e 5f50 412c 2929 0a20 2020 2020 2020  en_PA,)).       
+00022b90: 2073 656c 662e 5041 5f62 6e3a 206e 6e2e   self.PA_bn: nn.
+00022ba0: 4261 7463 684e 6f72 6d31 6420 3d20 6e6e  BatchNorm1d = nn
+00022bb0: 2e42 6174 6368 4e6f 726d 3164 280a 2020  .BatchNorm1d(.  
+00022bc0: 2020 2020 2020 2020 2020 6e75 6d5f 6665            num_fe
+00022bd0: 6174 7572 6573 3d73 656c 662e 6e5f 6869  atures=self.n_hi
+00022be0: 6464 656e 5f50 412c 0a20 2020 2020 2020  dden_PA,.       
+00022bf0: 2020 2020 2065 7073 3d31 652d 332c 0a20       eps=1e-3,. 
+00022c00: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
+00022c10: 7475 6d3d 302e 3939 2c0a 2020 2020 2020  tum=0.99,.      
+00022c20: 2020 2020 2020 6166 6669 6e65 3d54 7275        affine=Tru
+00022c30: 652c 0a20 2020 2020 2020 2020 2020 2074  e,.            t
+00022c40: 7261 636b 5f72 756e 6e69 6e67 5f73 7461  rack_running_sta
+00022c50: 7473 3d54 7275 6529 0a0a 2020 2020 2020  ts=True)..      
+00022c60: 2020 7365 6c66 2e57 5f41 3a20 746f 7263    self.W_A: torc
+00022c70: 682e 5465 6e73 6f72 203d 2069 6e69 7428  h.Tensor = init(
+00022c80: 0a20 2020 2020 2020 2020 2020 2074 6f72  .            tor
+00022c90: 6368 2e65 6d70 7479 2873 656c 662e 6e5f  ch.empty(self.n_
+00022ca0: 6869 6464 656e 5f41 2c20 7365 6c66 2e6e  hidden_A, self.n
+00022cb0: 5f61 746f 6d5f 6f75 7470 7574 5f66 6561  _atom_output_fea
+00022cc0: 7429 290a 2020 2020 2020 2020 7365 6c66  t)).        self
+00022cd0: 2e62 5f41 3a20 746f 7263 682e 5465 6e73  .b_A: torch.Tens
+00022ce0: 6f72 203d 2074 6f72 6368 2e7a 6572 6f73  or = torch.zeros
+00022cf0: 2828 7365 6c66 2e6e 5f61 746f 6d5f 6f75  ((self.n_atom_ou
+00022d00: 7470 7574 5f66 6561 742c 2929 0a20 2020  tput_feat,)).   
+00022d10: 2020 2020 2073 656c 662e 415f 626e 3a20       self.A_bn: 
+00022d20: 6e6e 2e42 6174 6368 4e6f 726d 3164 203d  nn.BatchNorm1d =
+00022d30: 206e 6e2e 4261 7463 684e 6f72 6d31 6428   nn.BatchNorm1d(
+00022d40: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00022d50: 5f66 6561 7475 7265 733d 7365 6c66 2e6e  _features=self.n
+00022d60: 5f61 746f 6d5f 6f75 7470 7574 5f66 6561  _atom_output_fea
+00022d70: 742c 0a20 2020 2020 2020 2020 2020 2065  t,.            e
+00022d80: 7073 3d31 652d 332c 0a20 2020 2020 2020  ps=1e-3,.       
+00022d90: 2020 2020 206d 6f6d 656e 7475 6d3d 302e       momentum=0.
+00022da0: 3939 2c0a 2020 2020 2020 2020 2020 2020  99,.            
+00022db0: 6166 6669 6e65 3d54 7275 652c 0a20 2020  affine=True,.   
+00022dc0: 2020 2020 2020 2020 2074 7261 636b 5f72           track_r
+00022dd0: 756e 6e69 6e67 5f73 7461 7473 3d54 7275  unning_stats=Tru
+00022de0: 6529 0a0a 2020 2020 2020 2020 6966 2073  e)..        if s
+00022df0: 656c 662e 7570 6461 7465 5f70 6169 723a  elf.update_pair:
+00022e00: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+00022e10: 6569 6768 7420 6d61 7472 6978 2061 6e64  eight matrix and
+00022e20: 2062 6961 7320 6d61 7472 6978 2072 6571   bias matrix req
+00022e30: 7569 7265 6420 746f 2063 6f6d 7075 7465  uired to compute
+00022e40: 206e 6577 2070 6169 7220 6c61 7965 7220   new pair layer 
+00022e50: 6672 6f6d 2074 6865 2070 7265 7669 6f75  from the previou
+00022e60: 7320 6174 6f6d 206c 6179 6572 0a20 2020  s atom layer.   
+00022e70: 2020 2020 2020 2020 2073 656c 662e 575f           self.W_
+00022e80: 4150 3a20 746f 7263 682e 5465 6e73 6f72  AP: torch.Tensor
+00022e90: 203d 2069 6e69 7428 0a20 2020 2020 2020   = init(.       
+00022ea0: 2020 2020 2020 2020 2074 6f72 6368 2e65           torch.e
+00022eb0: 6d70 7479 2873 656c 662e 6e5f 6174 6f6d  mpty(self.n_atom
+00022ec0: 5f69 6e70 7574 5f66 6561 7420 2a20 322c  _input_feat * 2,
+00022ed0: 2073 656c 662e 6e5f 6869 6464 656e 5f41   self.n_hidden_A
+00022ee0: 5029 290a 2020 2020 2020 2020 2020 2020  P)).            
+00022ef0: 7365 6c66 2e62 5f41 503a 2074 6f72 6368  self.b_AP: torch
+00022f00: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+00022f10: 7a65 726f 7328 2873 656c 662e 6e5f 6869  zeros((self.n_hi
+00022f20: 6464 656e 5f41 502c 2929 0a20 2020 2020  dden_AP,)).     
+00022f30: 2020 2020 2020 2073 656c 662e 4150 5f62         self.AP_b
+00022f40: 6e3a 206e 6e2e 4261 7463 684e 6f72 6d31  n: nn.BatchNorm1
+00022f50: 6420 3d20 6e6e 2e42 6174 6368 4e6f 726d  d = nn.BatchNorm
+00022f60: 3164 280a 2020 2020 2020 2020 2020 2020  1d(.            
+00022f70: 2020 2020 6e75 6d5f 6665 6174 7572 6573      num_features
+00022f80: 3d73 656c 662e 6e5f 6869 6464 656e 5f41  =self.n_hidden_A
+00022f90: 502c 0a20 2020 2020 2020 2020 2020 2020  P,.             
+00022fa0: 2020 2065 7073 3d31 652d 332c 0a20 2020     eps=1e-3,.   
+00022fb0: 2020 2020 2020 2020 2020 2020 206d 6f6d               mom
+00022fc0: 656e 7475 6d3d 302e 3939 2c0a 2020 2020  entum=0.99,.    
+00022fd0: 2020 2020 2020 2020 2020 2020 6166 6669              affi
+00022fe0: 6e65 3d54 7275 652c 0a20 2020 2020 2020  ne=True,.       
+00022ff0: 2020 2020 2020 2020 2074 7261 636b 5f72           track_r
+00023000: 756e 6e69 6e67 5f73 7461 7473 3d54 7275  unning_stats=Tru
+00023010: 6529 0a20 2020 2020 2020 2020 2020 2023  e).            #
+00023020: 2057 6569 6768 7420 6d61 7472 6978 2061   Weight matrix a
+00023030: 6e64 2062 6961 7320 6d61 7472 6978 2072  nd bias matrix r
+00023040: 6571 7569 7265 6420 746f 2063 6f6d 7075  equired to compu
+00023050: 7465 206e 6577 2070 6169 7220 6c61 7965  te new pair laye
+00023060: 7220 6672 6f6d 2074 6865 2070 7265 7669  r from the previ
+00023070: 6f75 7320 7061 6972 206c 6179 6572 0a20  ous pair layer. 
+00023080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00023090: 575f 5050 3a20 746f 7263 682e 5465 6e73  W_PP: torch.Tens
+000230a0: 6f72 203d 2069 6e69 7428 0a20 2020 2020  or = init(.     
+000230b0: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
+000230c0: 2e65 6d70 7479 2873 656c 662e 6e5f 7061  .empty(self.n_pa
+000230d0: 6972 5f69 6e70 7574 5f66 6561 742c 2073  ir_input_feat, s
+000230e0: 656c 662e 6e5f 6869 6464 656e 5f50 5029  elf.n_hidden_PP)
+000230f0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00023100: 6c66 2e62 5f50 503a 2074 6f72 6368 2e54  lf.b_PP: torch.T
+00023110: 656e 736f 7220 3d20 746f 7263 682e 7a65  ensor = torch.ze
+00023120: 726f 7328 2873 656c 662e 6e5f 6869 6464  ros((self.n_hidd
+00023130: 656e 5f50 502c 2929 0a20 2020 2020 2020  en_PP,)).       
+00023140: 2020 2020 2073 656c 662e 5050 5f62 6e3a       self.PP_bn:
+00023150: 206e 6e2e 4261 7463 684e 6f72 6d31 6420   nn.BatchNorm1d 
+00023160: 3d20 6e6e 2e42 6174 6368 4e6f 726d 3164  = nn.BatchNorm1d
+00023170: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00023180: 2020 6e75 6d5f 6665 6174 7572 6573 3d73    num_features=s
+00023190: 656c 662e 6e5f 6869 6464 656e 5f50 502c  elf.n_hidden_PP,
+000231a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000231b0: 2065 7073 3d31 652d 332c 0a20 2020 2020   eps=1e-3,.     
+000231c0: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
+000231d0: 7475 6d3d 302e 3939 2c0a 2020 2020 2020  tum=0.99,.      
+000231e0: 2020 2020 2020 2020 2020 6166 6669 6e65            affine
+000231f0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00023200: 2020 2020 2020 2074 7261 636b 5f72 756e         track_run
+00023210: 6e69 6e67 5f73 7461 7473 3d54 7275 6529  ning_stats=True)
+00023220: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00023230: 6c66 2e57 5f50 3a20 746f 7263 682e 5465  lf.W_P: torch.Te
+00023240: 6e73 6f72 203d 2069 6e69 7428 0a20 2020  nsor = init(.   
+00023250: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
+00023260: 6368 2e65 6d70 7479 2873 656c 662e 6e5f  ch.empty(self.n_
+00023270: 6869 6464 656e 5f50 2c20 7365 6c66 2e6e  hidden_P, self.n
+00023280: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
+00023290: 7429 290a 2020 2020 2020 2020 2020 2020  t)).            
+000232a0: 7365 6c66 2e62 5f50 3a20 746f 7263 682e  self.b_P: torch.
+000232b0: 5465 6e73 6f72 203d 2074 6f72 6368 2e7a  Tensor = torch.z
+000232c0: 6572 6f73 2828 7365 6c66 2e6e 5f70 6169  eros((self.n_pai
+000232d0: 725f 6f75 7470 7574 5f66 6561 742c 2929  r_output_feat,))
+000232e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000232f0: 662e 505f 626e 3a20 6e6e 2e42 6174 6368  f.P_bn: nn.Batch
+00023300: 4e6f 726d 3164 203d 206e 6e2e 4261 7463  Norm1d = nn.Batc
+00023310: 684e 6f72 6d31 6428 0a20 2020 2020 2020  hNorm1d(.       
+00023320: 2020 2020 2020 2020 206e 756d 5f66 6561           num_fea
+00023330: 7475 7265 733d 7365 6c66 2e6e 5f70 6169  tures=self.n_pai
+00023340: 725f 6f75 7470 7574 5f66 6561 742c 0a20  r_output_feat,. 
+00023350: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00023360: 7073 3d31 652d 332c 0a20 2020 2020 2020  ps=1e-3,.       
+00023370: 2020 2020 2020 2020 206d 6f6d 656e 7475           momentu
+00023380: 6d3d 302e 3939 2c0a 2020 2020 2020 2020  m=0.99,.        
+00023390: 2020 2020 2020 2020 6166 6669 6e65 3d54          affine=T
+000233a0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000233b0: 2020 2020 2074 7261 636b 5f72 756e 6e69       track_runni
+000233c0: 6e67 5f73 7461 7473 3d54 7275 6529 0a20  ng_stats=True). 
+000233d0: 2020 2020 2020 2073 656c 662e 6275 696c         self.buil
+000233e0: 7420 3d20 5472 7565 0a0a 2020 2020 6465  t = True..    de
+000233f0: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
+00023400: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00023410: 2022 2222 0a20 2020 2052 6574 7572 6e73   """.    Returns
+00023420: 2061 2073 7472 696e 6720 7265 7072 6573   a string repres
+00023430: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
+00023440: 6f62 6a65 6374 2e0a 0a20 2020 2052 6574  object...    Ret
+00023450: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
+00023460: 2d0a 2020 2020 7374 723a 2041 2073 7472  -.    str: A str
+00023470: 696e 6720 7468 6174 2063 6f6e 7461 696e  ing that contain
+00023480: 7320 7468 6520 636c 6173 7320 6e61 6d65  s the class name
+00023490: 2066 6f6c 6c6f 7765 6420 6279 2074 6865   followed by the
+000234a0: 2076 616c 7565 7320 6f66 2069 7473 2069   values of its i
+000234b0: 6e73 7461 6e63 6520 7661 7269 6162 6c65  nstance variable
+000234c0: 2e0a 2020 2020 2222 220a 2020 2020 2020  ..    """.      
+000234d0: 2020 2320 666c 616b 6538 3a20 6e6f 7161    # flake8: noqa
+000234e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000234f0: 280a 2020 2020 2020 2020 2020 2020 6627  (.            f'
+00023500: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
+00023510: 5f5f 6e61 6d65 5f5f 7d28 6e5f 6174 6f6d  __name__}(n_atom
+00023520: 5f69 6e70 7574 5f66 6561 743a 7b73 656c  _input_feat:{sel
+00023530: 662e 6e5f 6174 6f6d 5f69 6e70 7574 5f66  f.n_atom_input_f
+00023540: 6561 747d 2c6e 5f70 6169 725f 696e 7075  eat},n_pair_inpu
+00023550: 745f 6665 6174 3a7b 7365 6c66 2e6e 5f70  t_feat:{self.n_p
+00023560: 6169 725f 696e 7075 745f 6665 6174 7d2c  air_input_feat},
+00023570: 6e5f 6174 6f6d 5f6f 7574 7075 745f 6665  n_atom_output_fe
+00023580: 6174 3a7b 7365 6c66 2e6e 5f61 746f 6d5f  at:{self.n_atom_
+00023590: 6f75 7470 7574 5f66 6561 747d 2c6e 5f70  output_feat},n_p
+000235a0: 6169 725f 6f75 7470 7574 5f66 6561 743a  air_output_feat:
+000235b0: 7b73 656c 662e 6e5f 7061 6972 5f6f 7574  {self.n_pair_out
+000235c0: 7075 745f 6665 6174 7d2c 6e5f 6869 6464  put_feat},n_hidd
+000235d0: 656e 5f41 413a 7b73 656c 662e 6e5f 6869  en_AA:{self.n_hi
+000235e0: 6464 656e 5f41 417d 2c6e 5f68 6964 6465  dden_AA},n_hidde
+000235f0: 6e5f 5041 3a7b 7365 6c66 2e6e 5f68 6964  n_PA:{self.n_hid
+00023600: 6465 6e5f 5041 7d2c 6e5f 6869 6464 656e  den_PA},n_hidden
+00023610: 5f41 503a 7b73 656c 662e 6e5f 6869 6464  _AP:{self.n_hidd
+00023620: 656e 5f41 507d 2c6e 5f68 6964 6465 6e5f  en_AP},n_hidden_
+00023630: 5050 3a7b 7365 6c66 2e6e 5f68 6964 6465  PP:{self.n_hidde
+00023640: 6e5f 5050 7d2c 6261 7463 685f 6e6f 726d  n_PP},batch_norm
+00023650: 616c 697a 653a 7b73 656c 662e 6261 7463  alize:{self.batc
+00023660: 685f 6e6f 726d 616c 697a 657d 2c75 7064  h_normalize},upd
+00023670: 6174 655f 7061 6972 3a7b 7365 6c66 2e75  ate_pair:{self.u
+00023680: 7064 6174 655f 7061 6972 7d2c 696e 6974  pdate_pair},init
+00023690: 3a7b 7365 6c66 2e69 6e69 747d 2c61 6374  :{self.init},act
+000236a0: 6976 6174 696f 6e3a 7b73 656c 662e 6163  ivation:{self.ac
+000236b0: 7469 7661 7469 6f6e 7d29 270a 2020 2020  tivation})'.    
+000236c0: 2020 2020 290a 0a20 2020 2064 6566 2066      )..    def f
+000236d0: 6f72 7761 7264 280a 2020 2020 2020 2020  orward(.        
+000236e0: 7365 6c66 2c20 696e 7075 7473 3a20 4c69  self, inputs: Li
+000236f0: 7374 5b55 6e69 6f6e 5b6e 702e 6e64 6172  st[Union[np.ndar
+00023700: 7261 792c 206e 702e 6e64 6172 7261 792c  ray, np.ndarray,
+00023710: 206e 702e 6e64 6172 7261 792c 0a20 2020   np.ndarray,.   
+00023720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023730: 2020 2020 2020 2020 2020 2020 2020 6e70                np
+00023740: 2e6e 6461 7272 6179 5d5d 0a20 2020 2029  .ndarray]].    )
+00023750: 202d 3e20 4c69 7374 5b55 6e69 6f6e 5b74   -> List[Union[t
+00023760: 6f72 6368 2e54 656e 736f 722c 2074 6f72  orch.Tensor, tor
+00023770: 6368 2e54 656e 736f 725d 5d3a 0a20 2020  ch.Tensor]]:.   
+00023780: 2020 2020 2022 2222 0a20 2020 2043 7265       """.    Cre
+00023790: 6174 6573 2077 6561 7665 2074 656e 736f  ates weave tenso
+000237a0: 7273 2e0a 0a20 2020 2050 6172 616d 6574  rs...    Paramet
+000237b0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000237c0: 2d2d 0a20 2020 2069 6e70 7574 733a 204c  --.    inputs: L
+000237d0: 6973 745b 556e 696f 6e5b 6e70 2e6e 6461  ist[Union[np.nda
+000237e0: 7272 6179 2c20 6e70 2e6e 6461 7272 6179  rray, np.ndarray
+000237f0: 2c20 6e70 2e6e 6461 7272 6179 2c20 6e70  , np.ndarray, np
+00023800: 2e6e 6461 7272 6179 5d5d 0a20 2020 2053  .ndarray]].    S
+00023810: 686f 756c 6420 636f 6e74 6169 6e20 3420  hould contain 4 
+00023820: 7465 6e73 6f72 7320 5b61 746f 6d5f 6665  tensors [atom_fe
+00023830: 6174 7572 6573 2c20 7061 6972 5f66 6561  atures, pair_fea
+00023840: 7475 7265 732c 2070 6169 725f 7370 6c69  tures, pair_spli
+00023850: 742c 0a20 2020 2061 746f 6d5f 746f 5f70  t,.    atom_to_p
+00023860: 6169 725d 0a0a 2020 2020 5265 7475 726e  air]..    Return
+00023870: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  s:.    -------. 
+00023880: 2020 204c 6973 745b 556e 696f 6e5b 746f     List[Union[to
+00023890: 7263 682e 5465 6e73 6f72 2c20 746f 7263  rch.Tensor, torc
+000238a0: 682e 5465 6e73 6f72 5d5d 0a20 2020 2020  h.Tensor]].     
+000238b0: 2041 3a20 4174 6f6d 2066 6561 7475 7265   A: Atom feature
+000238c0: 7320 7465 6e73 6f72 2077 6974 6820 7368  s tensor with sh
+000238d0: 6170 655b 746f 7461 6c5f 6e75 6d5f 6174  ape[total_num_at
+000238e0: 6f6d 732c 6174 6f6d 2066 6561 7475 7265  oms,atom feature
+000238f0: 2073 697a 655d 0a20 2020 2020 2050 3a20   size].      P: 
+00023900: 5061 6972 2066 6561 7475 7265 7320 7465  Pair features te
+00023910: 6e73 6f72 2077 6974 6820 7368 6170 655b  nsor with shape[
+00023920: 746f 7461 6c20 6e75 6d20 6f66 2070 6169  total num of pai
+00023930: 7273 2c62 6f6e 6420 6665 6174 7572 6520  rs,bond feature 
+00023940: 7369 7a65 5d0a 2020 2020 2222 220a 2020  size].    """.  
+00023950: 2020 2020 2020 2320 436f 6e76 6572 7469        # Converti
+00023960: 6e67 2074 6865 2069 6e70 7574 2074 6f20  ng the input to 
+00023970: 746f 7263 6820 7465 6e73 6f72 730a 2020  torch tensors.  
+00023980: 2020 2020 2020 6174 6f6d 5f66 6561 7475        atom_featu
+00023990: 7265 733a 2074 6f72 6368 2e54 656e 736f  res: torch.Tenso
+000239a0: 7220 3d20 746f 7263 682e 7465 6e73 6f72  r = torch.tensor
+000239b0: 2869 6e70 7574 735b 305d 290a 2020 2020  (inputs[0]).    
+000239c0: 2020 2020 7061 6972 5f66 6561 7475 7265      pair_feature
+000239d0: 733a 2074 6f72 6368 2e54 656e 736f 7220  s: torch.Tensor 
+000239e0: 3d20 746f 7263 682e 7465 6e73 6f72 2869  = torch.tensor(i
+000239f0: 6e70 7574 735b 315d 290a 0a20 2020 2020  nputs[1])..     
+00023a00: 2020 2070 6169 725f 7370 6c69 743a 2074     pair_split: t
+00023a10: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+00023a20: 7263 682e 7465 6e73 6f72 2869 6e70 7574  rch.tensor(input
+00023a30: 735b 325d 290a 2020 2020 2020 2020 6174  s[2]).        at
+00023a40: 6f6d 5f74 6f5f 7061 6972 3a20 746f 7263  om_to_pair: torc
+00023a50: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
+00023a60: 2e74 656e 736f 7228 696e 7075 7473 5b33  .tensor(inputs[3
+00023a70: 5d29 0a0a 2020 2020 2020 2020 6163 7469  ])..        acti
+00023a80: 7661 7469 6f6e 203d 2073 656c 662e 6163  vation = self.ac
+00023a90: 7469 7661 7469 6f6e 5f66 6e0a 0a20 2020  tivation_fn..   
+00023aa0: 2020 2020 2023 2041 4120 6973 2061 2074       # AA is a t
+00023ab0: 656e 736f 7220 7769 7468 2073 6861 7065  ensor with shape
+00023ac0: 5b74 6f74 616c 5f6e 756d 5f61 746f 6d73  [total_num_atoms
+00023ad0: 2c6e 5f68 6964 6465 6e5f 4141 5d0a 2020  ,n_hidden_AA].  
+00023ae0: 2020 2020 2020 4141 3a20 746f 7263 682e        AA: torch.
+00023af0: 5465 6e73 6f72 203d 2074 6f72 6368 2e6d  Tensor = torch.m
+00023b00: 6174 6d75 6c28 6174 6f6d 5f66 6561 7475  atmul(atom_featu
+00023b10: 7265 732e 7479 7065 2874 6f72 6368 2e66  res.type(torch.f
+00023b20: 6c6f 6174 3332 292c 0a20 2020 2020 2020  loat32),.       
+00023b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b50: 2073 656c 662e 575f 4141 2920 2b20 7365   self.W_AA) + se
+00023b60: 6c66 2e62 5f41 410a 2020 2020 2020 2020  lf.b_AA.        
+00023b70: 6966 2073 656c 662e 6261 7463 685f 6e6f  if self.batch_no
+00023b80: 726d 616c 697a 653a 0a20 2020 2020 2020  rmalize:.       
+00023b90: 2020 2020 2073 656c 662e 4141 5f62 6e2e       self.AA_bn.
+00023ba0: 6576 616c 2829 0a20 2020 2020 2020 2020  eval().         
+00023bb0: 2020 2041 4120 3d20 7365 6c66 2e41 415f     AA = self.AA_
+00023bc0: 626e 2841 4129 0a20 2020 2020 2020 2041  bn(AA).        A
+00023bd0: 4120 3d20 6163 7469 7661 7469 6f6e 2841  A = activation(A
+00023be0: 4129 0a20 2020 2020 2020 2023 2050 4120  A).        # PA 
+00023bf0: 6973 2061 2074 656e 736f 7220 7769 7468  is a tensor with
+00023c00: 2073 6861 7065 5b74 6f74 616c 206e 756d   shape[total num
+00023c10: 6265 7220 6f66 2070 6169 7273 2c6e 5f68  ber of pairs,n_h
+00023c20: 6964 6465 6e5f 5041 5d0a 2020 2020 2020  idden_PA].      
+00023c30: 2020 5041 3a20 746f 7263 682e 5465 6e73    PA: torch.Tens
+00023c40: 6f72 203d 2074 6f72 6368 2e6d 6174 6d75  or = torch.matmu
+00023c50: 6c28 7061 6972 5f66 6561 7475 7265 732e  l(pair_features.
+00023c60: 7479 7065 2874 6f72 6368 2e66 6c6f 6174  type(torch.float
+00023c70: 3332 292c 0a20 2020 2020 2020 2020 2020  32),.           
+00023c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023c90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00023ca0: 662e 575f 5041 2920 2b20 7365 6c66 2e62  f.W_PA) + self.b
+00023cb0: 5f50 410a 2020 2020 2020 2020 6966 2073  _PA.        if s
+00023cc0: 656c 662e 6261 7463 685f 6e6f 726d 616c  elf.batch_normal
+00023cd0: 697a 653a 0a20 2020 2020 2020 2020 2020  ize:.           
+00023ce0: 2073 656c 662e 5041 5f62 6e2e 6576 616c   self.PA_bn.eval
+00023cf0: 2829 0a20 2020 2020 2020 2020 2020 2050  ().            P
+00023d00: 4120 3d20 7365 6c66 2e50 415f 626e 2850  A = self.PA_bn(P
+00023d10: 4129 0a20 2020 2020 2020 2050 4120 3d20  A).        PA = 
+00023d20: 6163 7469 7661 7469 6f6e 2850 4129 0a0a  activation(PA)..
+00023d30: 2020 2020 2020 2020 2320 5370 6c69 7420          # Split 
+00023d40: 7468 6520 5041 2074 656e 736f 7220 6163  the PA tensor ac
+00023d50: 636f 7264 696e 6720 746f 2074 6865 2027  cording to the '
+00023d60: 7061 6972 5f73 706c 6974 2720 7465 6e73  pair_split' tens
+00023d70: 6f72 0a20 2020 2020 2020 2074 5f67 7270  or.        t_grp
+00023d80: 3a20 4469 6374 5b54 656e 736f 722c 2054  : Dict[Tensor, T
+00023d90: 656e 736f 725d 203d 207b 7d0a 2020 2020  ensor] = {}.    
+00023da0: 2020 2020 6964 783a 2069 6e74 203d 2030      idx: int = 0
+00023db0: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
+00023dc0: 735f 6964 2069 6e20 656e 756d 6572 6174  s_id in enumerat
+00023dd0: 6528 7061 6972 5f73 706c 6974 293a 0a20  e(pair_split):. 
+00023de0: 2020 2020 2020 2020 2020 2073 5f69 6420             s_id 
+00023df0: 3d20 735f 6964 2e69 7465 6d28 290a 2020  = s_id.item().  
+00023e00: 2020 2020 2020 2020 2020 6966 2073 5f69            if s_i
+00023e10: 6420 696e 2074 5f67 7270 3a0a 2020 2020  d in t_grp:.    
+00023e20: 2020 2020 2020 2020 2020 2020 745f 6772              t_gr
+00023e30: 705b 735f 6964 5d20 3d20 745f 6772 705b  p[s_id] = t_grp[
+00023e40: 735f 6964 5d20 2b20 5041 5b69 6478 5d0a  s_id] + PA[idx].
+00023e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00023e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023e70: 2020 745f 6772 705b 735f 6964 5d20 3d20    t_grp[s_id] = 
+00023e80: 5041 5b69 6478 5d0a 2020 2020 2020 2020  PA[idx].        
+00023e90: 2020 2020 6964 7820 3d20 6920 2b20 310a      idx = i + 1.
+00023ea0: 0a20 2020 2020 2020 2020 2020 206c 7374  .            lst
+00023eb0: 203d 206c 6973 7428 745f 6772 702e 7661   = list(t_grp.va
+00023ec0: 6c75 6573 2829 290a 2020 2020 2020 2020  lues()).        
+00023ed0: 2020 2020 7465 6e73 6f72 203d 2074 6f72      tensor = tor
+00023ee0: 6368 2e73 7461 636b 286c 7374 290a 2020  ch.stack(lst).  
+00023ef0: 2020 2020 2020 5041 203d 2074 656e 736f        PA = tenso
+00023f00: 720a 0a20 2020 2020 2020 2041 3a20 746f  r..        A: to
+00023f10: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
+00023f20: 6368 2e6d 6174 6d75 6c28 746f 7263 682e  ch.matmul(torch.
+00023f30: 636f 6e63 6174 285b 4141 2c20 5041 5d2c  concat([AA, PA],
+00023f40: 2031 292c 0a20 2020 2020 2020 2020 2020   1),.           
+00023f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023f60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00023f70: 2e57 5f41 2920 2b20 7365 6c66 2e62 5f41  .W_A) + self.b_A
+00023f80: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00023f90: 2e62 6174 6368 5f6e 6f72 6d61 6c69 7a65  .batch_normalize
+00023fa0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00023fb0: 6c66 2e41 5f62 6e2e 6576 616c 2829 0a20  lf.A_bn.eval(). 
+00023fc0: 2020 2020 2020 2020 2020 2041 203d 2073             A = s
+00023fd0: 656c 662e 415f 626e 2841 290a 2020 2020  elf.A_bn(A).    
+00023fe0: 2020 2020 4120 3d20 6163 7469 7661 7469      A = activati
+00023ff0: 6f6e 2841 290a 0a20 2020 2020 2020 2069  on(A)..        i
+00024000: 6620 7365 6c66 2e75 7064 6174 655f 7061  f self.update_pa
+00024010: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
+00024020: 2320 4e6f 7465 2074 6861 7420 4150 5f69  # Note that AP_i
+00024030: 6a20 616e 6420 4150 5f6a 6920 7368 6172  j and AP_ji shar
+00024040: 6520 7468 6520 7361 6d65 2073 656c 662e  e the same self.
+00024050: 4150 5f62 6e20 6261 7463 680a 2020 2020  AP_bn batch.    
+00024060: 2020 2020 2020 2020 2320 6e6f 726d 616c          # normal
+00024070: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
+00024080: 2020 2020 4150 5f69 6a3a 2074 6f72 6368      AP_ij: torch
+00024090: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
+000240a0: 6d61 746d 756c 280a 2020 2020 2020 2020  matmul(.        
+000240b0: 2020 2020 2020 2020 746f 7263 682e 7265          torch.re
+000240c0: 7368 6170 6528 6174 6f6d 5f66 6561 7475  shape(atom_featu
+000240d0: 7265 735b 6174 6f6d 5f74 6f5f 7061 6972  res[atom_to_pair
+000240e0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+000240f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024100: 205b 2d31 2c20 3220 2a20 7365 6c66 2e6e   [-1, 2 * self.n
+00024110: 5f61 746f 6d5f 696e 7075 745f 6665 6174  _atom_input_feat
+00024120: 5d29 2e74 7970 6528 0a20 2020 2020 2020  ]).type(.       
+00024130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024140: 2020 2020 2020 2020 2020 2074 6f72 6368             torch
+00024150: 2e66 6c6f 6174 3332 292c 2073 656c 662e  .float32), self.
+00024160: 575f 4150 2920 2b20 7365 6c66 2e62 5f41  W_AP) + self.b_A
+00024170: 500a 2020 2020 2020 2020 2020 2020 6966  P.            if
+00024180: 2073 656c 662e 6261 7463 685f 6e6f 726d   self.batch_norm
+00024190: 616c 697a 653a 0a20 2020 2020 2020 2020  alize:.         
+000241a0: 2020 2020 2020 2073 656c 662e 4150 5f62         self.AP_b
+000241b0: 6e2e 6576 616c 2829 0a20 2020 2020 2020  n.eval().       
+000241c0: 2020 2020 2020 2020 2041 505f 696a 203d           AP_ij =
+000241d0: 2073 656c 662e 4150 5f62 6e28 4150 5f69   self.AP_bn(AP_i
+000241e0: 6a29 0a20 2020 2020 2020 2020 2020 2041  j).            A
+000241f0: 505f 696a 203d 2061 6374 6976 6174 696f  P_ij = activatio
+00024200: 6e28 4150 5f69 6a29 0a20 2020 2020 2020  n(AP_ij).       
+00024210: 2020 2020 2041 505f 6a69 3a20 746f 7263       AP_ji: torc
+00024220: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
+00024230: 2e6d 6174 6d75 6c28 0a20 2020 2020 2020  .matmul(.       
+00024240: 2020 2020 2020 2020 2074 6f72 6368 2e72           torch.r
+00024250: 6573 6861 7065 2861 746f 6d5f 6665 6174  eshape(atom_feat
+00024260: 7572 6573 5b74 6f72 6368 2e66 6c69 7028  ures[torch.flip(
+00024270: 6174 6f6d 5f74 6f5f 7061 6972 2c20 5b31  atom_to_pair, [1
+00024280: 5d29 5d2c 0a20 2020 2020 2020 2020 2020  ])],.           
+00024290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000242a0: 2020 205b 2d31 2c20 3220 2a20 7365 6c66     [-1, 2 * self
+000242b0: 2e6e 5f61 746f 6d5f 696e 7075 745f 6665  .n_atom_input_fe
+000242c0: 6174 5d29 2e74 7970 6528 0a20 2020 2020  at]).type(.     
+000242d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000242e0: 2020 2020 2020 2020 2020 2020 2074 6f72               tor
+000242f0: 6368 2e66 6c6f 6174 3332 292c 2073 656c  ch.float32), sel
+00024300: 662e 575f 4150 2920 2b20 7365 6c66 2e62  f.W_AP) + self.b
+00024310: 5f41 500a 2020 2020 2020 2020 2020 2020  _AP.            
+00024320: 6966 2073 656c 662e 6261 7463 685f 6e6f  if self.batch_no
+00024330: 726d 616c 697a 653a 0a20 2020 2020 2020  rmalize:.       
+00024340: 2020 2020 2020 2020 2073 656c 662e 4150           self.AP
+00024350: 5f62 6e2e 6576 616c 2829 0a20 2020 2020  _bn.eval().     
+00024360: 2020 2020 2020 2020 2020 2041 505f 6a69             AP_ji
+00024370: 203d 2073 656c 662e 4150 5f62 6e28 4150   = self.AP_bn(AP
+00024380: 5f6a 6929 0a20 2020 2020 2020 2020 2020  _ji).           
+00024390: 2041 505f 6a69 203d 2061 6374 6976 6174   AP_ji = activat
+000243a0: 696f 6e28 4150 5f6a 6929 0a20 2020 2020  ion(AP_ji).     
+000243b0: 2020 2020 2020 2023 2050 5020 6973 2061         # PP is a
+000243c0: 2074 656e 736f 7220 7769 7468 2073 6861   tensor with sha
+000243d0: 7065 205b 746f 7461 6c20 6e75 6d62 6572  pe [total number
+000243e0: 206f 6620 7061 6972 732c 6e5f 6869 6464   of pairs,n_hidd
+000243f0: 656e 5f50 505d 0a20 2020 2020 2020 2020  en_PP].         
+00024400: 2020 2050 503a 2074 6f72 6368 2e54 656e     PP: torch.Ten
+00024410: 736f 7220 3d20 746f 7263 682e 6d61 746d  sor = torch.matm
+00024420: 756c 2870 6169 725f 6665 6174 7572 6573  ul(pair_features
+00024430: 2e74 7970 6528 746f 7263 682e 666c 6f61  .type(torch.floa
+00024440: 7433 3229 2c0a 2020 2020 2020 2020 2020  t32),.          
+00024450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024470: 2020 7365 6c66 2e57 5f50 5029 202b 2073    self.W_PP) + s
+00024480: 656c 662e 625f 5050 0a20 2020 2020 2020  elf.b_PP.       
+00024490: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+000244a0: 6368 5f6e 6f72 6d61 6c69 7a65 3a0a 2020  ch_normalize:.  
+000244b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000244c0: 6c66 2e50 505f 626e 2e65 7661 6c28 290a  lf.PP_bn.eval().
+000244d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244e0: 5050 203d 2073 656c 662e 5050 5f62 6e28  PP = self.PP_bn(
+000244f0: 5050 290a 2020 2020 2020 2020 2020 2020  PP).            
+00024500: 5050 203d 2061 6374 6976 6174 696f 6e28  PP = activation(
+00024510: 5050 290a 2020 2020 2020 2020 2020 2020  PP).            
+00024520: 503a 2074 6f72 6368 2e54 656e 736f 7220  P: torch.Tensor 
+00024530: 3d20 746f 7263 682e 6d61 746d 756c 280a  = torch.matmul(.
+00024540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024550: 746f 7263 682e 636f 6e63 6174 285b 4150  torch.concat([AP
+00024560: 5f69 6a20 2b20 4150 5f6a 692c 2050 505d  _ij + AP_ji, PP]
+00024570: 2c20 3129 2e74 7970 6528 746f 7263 682e  , 1).type(torch.
+00024580: 666c 6f61 7433 3229 2c0a 2020 2020 2020  float32),.      
+00024590: 2020 2020 2020 2020 2020 7365 6c66 2e57            self.W
+000245a0: 5f50 2920 2b20 7365 6c66 2e62 5f50 0a20  _P) + self.b_P. 
+000245b0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000245c0: 6c66 2e62 6174 6368 5f6e 6f72 6d61 6c69  lf.batch_normali
+000245d0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+000245e0: 2020 2020 7365 6c66 2e50 5f62 6e2e 6576      self.P_bn.ev
+000245f0: 616c 2829 0a20 2020 2020 2020 2020 2020  al().           
+00024600: 2020 2020 2050 203d 2073 656c 662e 505f       P = self.P_
+00024610: 626e 2850 290a 2020 2020 2020 2020 2020  bn(P).          
+00024620: 2020 5020 3d20 6163 7469 7661 7469 6f6e    P = activation
+00024630: 2850 290a 2020 2020 2020 2020 656c 7365  (P).        else
+00024640: 3a0a 2020 2020 2020 2020 2020 2020 5020  :.            P 
+00024650: 3d20 7061 6972 5f66 6561 7475 7265 730a  = pair_features.
+00024660: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00024670: 5b41 2c20 505d 0a                        [A, P].
```

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230710190635/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230710190635/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230710190635/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230710190635/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230710190635/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230710190635/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230710190635/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230710190635/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230710190635/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230710190635/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230710190635/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230707051842
+Version: 2.7.2.dev20230710190635
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230707051842/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230710190635/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/setup.cfg` & `deepchem-2.7.2.dev20230710190635/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230707051842/setup.py` & `deepchem-2.7.2.dev20230710190635/setup.py`

 * *Files identical despite different names*


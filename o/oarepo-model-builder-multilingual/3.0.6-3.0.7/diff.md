# Comparing `tmp/oarepo-model-builder-multilingual-3.0.6.tar.gz` & `tmp/oarepo-model-builder-multilingual-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-multilingual-3.0.6.tar", last modified: Mon Jun 19 12:40:12 2023, max compression
+gzip compressed data, was "oarepo-model-builder-multilingual-3.0.7.tar", last modified: Mon Jul 10 13:55:12 2023, max compression
```

## Comparing `oarepo-model-builder-multilingual-3.0.6.tar` & `oarepo-model-builder-multilingual-3.0.7.tar`

### file list

```diff
@@ -1,73 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.702549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/builtin_models/i18n.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.706549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/multilings.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/faker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/supported_langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.710549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.702549 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-19 12:40:12.000000 oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:40:12.714549 oarepo-model-builder-multilingual-3.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/mock_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/model.json5
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_build_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_marshmallow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_multi_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-19 12:39:31.000000 oarepo-model-builder-multilingual-3.0.6/tests/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.900027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.900027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/builtin_models/i18n.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/faker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.904027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:55:12.900027 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 13:55:12.000000 oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-10 13:55:12.908027 oarepo-model-builder-multilingual-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:54:40.000000 oarepo-model-builder-multilingual-3.0.7/setup.py
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/LICENSE` & `oarepo-model-builder-multilingual-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.6
+Version: 3.0.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/README.md` & `oarepo-model-builder-multilingual-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/__init__.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/facets/i18n.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class I18nStrFacetsComponent(NestedFacetsComponent, RegularFacetsComponent):
     eligible_datatypes = [I18nDataType]
 
     def process_facets(self, datatype, section, **__kwargs):
         facet_section = section.config
         facets = []
-        for l in datatype.schema.settings["supported_langs"]:
+        for l in datatype.schema.settings["supported-langs"]:
             path = self.facet_path(datatype, facet_section)
             facet_definition = FacetDefinition(
                 path=facet_name(datatype.path + "_" + l),
                 dot_path=datatype.path + "." + l,
                 searchable=facet_section.get("searchable"),
                 imports=[
                     {
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/field.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def generate_alternative(datatype):
     if not datatype.key:
         key = datatype.parent.key
         node = datatype.parent.parent
     else:
         key = datatype.key
         node = datatype.parent
-    alternative = alternative_gen(datatype.schema.settings["supported_langs"], key)
+    alternative = alternative_gen(datatype.schema.settings["supported-langs"], key)
     if "properties" in node.section_mapping.config:
         deepmerge(node.section_mapping.config["properties"], alternative)
     else:
         node.section_mapping.config["properties"] = alternative
 
 
 class RegularMultilingualMappingComponent(DataTypeComponent):
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/mapping/multi.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/marshmallow/ui_i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/model/multilingual_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/components/multilingual/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/datatypes/multilings.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/faker.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/faker.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     if type == "i18nStr" or type == "multilingual":
         if hasattr(stack.stack[-1], "multilingual"):
             definition = stack.stack[-1]["multilingual"]
         else:
             definition = {}
         lang_name = definition.get("lang-field", "lang")
         if stack.key == lang_name:
-            return random.choice(list(settings["supported_langs"].keys()))
+            return random.choice(list(settings["supported-langs"].keys()))
 
     return SKIP
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     TYPE = "invenio_multilingual_dumper"
     section = "multilingual-dumper"
     template = "multilingual-record-dumper"
     paths = []
 
     def finish(self, **extra_kwargs):
         langs = []
-        for lang in self.settings["supported_langs"]:
+        for lang in self.settings["supported-langs"]:
             langs.append(lang)
 
         self.get_paths(self.current_model.children)
         extra_kwargs["langs"] = langs
         extra_kwargs["paths"] = sorted(set(self.paths))
         super().finish(**extra_kwargs)
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/utils/supported_langs.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual/validation/__init__.py` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual/validation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     def validate_schema(self, data, **kwargs):
         for lang in data:
             if not langcodes.Language.get(lang).is_valid():
                 raise ValidationError("Invalid language code")
 
 
 class LanguagesSettingsSchema(ExtendablePartSchema):
-    supported_langs = fields.Raw(data_key="supported-langs", required=False)
+    supported_langs = fields.Raw(data_key="supported-langs",attribute="supported-langs", required=False)
 
 
 validators = {
     "settings": LanguagesSettingsSchema,
 }
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/PKG-INFO` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 3.0.6
+Version: 3.0.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/SOURCES.txt` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_model_builder_multilingual/__init__.py
 oarepo_model_builder_multilingual/faker.py
 oarepo_model_builder_multilingual.egg-info/PKG-INFO
@@ -36,20 +37,8 @@
 oarepo_model_builder_multilingual/invenio/invenio_record_multilingual.py
 oarepo_model_builder_multilingual/invenio/templates/__init__.py
 oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
 oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
 oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
 oarepo_model_builder_multilingual/utils/__init__.py
 oarepo_model_builder_multilingual/utils/supported_langs.py
-oarepo_model_builder_multilingual/validation/__init__.py
-tests/__init__.py
-tests/mock_filesystem.py
-tests/model.json5
-tests/multilingual_schema.py
-tests/test_build_from_entrypoints.py
-tests/test_cfg.py
-tests/test_helper.py
-tests/test_i18nStr.py
-tests/test_marshmallow_ui.py
-tests/test_multi_facets.py
-tests/test_schema.py
-tests/test_ui.py
+oarepo_model_builder_multilingual/validation/__init__.py
```

### Comparing `oarepo-model-builder-multilingual-3.0.6/oarepo_model_builder_multilingual.egg-info/entry_points.txt` & `oarepo-model-builder-multilingual-3.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-3.0.6/setup.cfg` & `oarepo-model-builder-multilingual-3.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-multilingual
-version = 3.0.6
+version = 3.0.7
 description = 
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```


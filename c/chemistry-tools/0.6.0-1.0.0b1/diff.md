# Comparing `tmp/chemistry_tools-0.6.0.tar.gz` & `tmp/chemistry_tools-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemistry_tools-0.6.0.tar", last modified: Fri Jul  7 11:12:19 2023, max compression
+gzip compressed data, was "chemistry_tools-1.0.0b1.tar", last modified: Mon Jul 10 12:58:02 2023, max compression
```

## Comparing `chemistry_tools-0.6.0.tar` & `chemistry_tools-1.0.0b1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-07-07 11:12:19.529570 chemistry_tools-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-07 11:12:19.529570 chemistry_tools-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-07-07 11:12:19.537571 chemistry_tools-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-07 11:12:19.521571 chemistry_tools-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6893 2023-07-07 11:12:19.529570 chemistry_tools-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/_memoized_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/toxnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/cas.py
--rw-r--r--   0 runner    (1001) docker     (122)    11278 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/spectrum_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     7922 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/units.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/_memoized_property.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     8842 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/names.py
--rw-r--r--   0 runner    (1001) docker     (122)     7731 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-07 11:11:46.769527 chemistry_tools-0.6.0/chemistry_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/property_format.py
--rw-r--r--   0 runner    (1001) docker     (122)    33686 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/lanthanides.py
--rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/_isotope_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12747 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/chalcogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    12879 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/pnictogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    19500 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/alkaline_earth_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)    14102 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/noble_gases.py
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14069 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/alkali_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)    64225 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/transition_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/_elements.py
--rw-r--r--   0 runner    (1001) docker     (122)    12668 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/halogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    13191 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/triels.py
--rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/tetrels.py
--rw-r--r--   0 runner    (1001) docker     (122)    25825 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/elements/actinides.py
--rw-r--r--   0 runner    (1001) docker     (122)    10097 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/html.py
--rw-r--r--   0 runner    (1001) docker     (122)    10201 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/species.py
--rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/dataarray.py
--rw-r--r--   0 runner    (1001) docker     (122)    12457 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/iso_dist.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5771 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/latex.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/composition.py
--rw-r--r--   0 runner    (1001) docker     (122)     9673 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/_parser_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    27097 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/formulae/unicode.py
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/lookup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/full_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3915 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/description.py
--rw-r--r--   0 runner    (1001) docker     (122)     5750 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4864 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/bond.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    14717 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     5660 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/atom.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/pug_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3871 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/synonyms.py
--rw-r--r--   0 runner    (1001) docker     (122)    19223 2023-07-07 11:11:46.773527 chemistry_tools-0.6.0/chemistry_tools/pubchem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6033 2023-07-10 12:58:02.768788 chemistry_tools-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-10 12:58:02.768788 chemistry_tools-1.0.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9971 2023-07-10 12:58:02.772788 chemistry_tools-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-10 12:58:02.760788 chemistry_tools-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6895 2023-07-10 12:58:02.768788 chemistry_tools-1.0.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/_memoized_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/toxnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/cas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17733 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/spectrum_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     8040 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/units.py
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/_memoized_property.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7739 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/property_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33686 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/lanthanides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/_isotope_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12747 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/chalcogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12879 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/pnictogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/alkaline_earth_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14102 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/noble_gases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14069 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/alkali_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64225 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/transition_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12668 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/halogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13191 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/triels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/tetrels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25825 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/actinides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10097 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/species.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/iso_dist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6979 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5771 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/latex.py
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/composition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9673 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/_parser_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27405 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/full_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5840 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4880 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/bond.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    14771 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5676 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/atom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/pug_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3911 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/synonyms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19312 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/properties.py
```

### Comparing `chemistry_tools-0.6.0/LICENSE` & `chemistry_tools-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/README.rst` & `chemistry_tools-1.0.0b1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/chemistry_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v0.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.0b1
 	:target: https://github.com/domdfcoding/chemistry_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/toxnet.py` & `chemistry_tools-1.0.0b1/chemistry_tools/toxnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 
 # stdlib
 from decimal import Decimal
 from typing import Any, Dict
 
 # 3rd party
 import requests
-from bs4 import BeautifulSoup  # type: ignore  # nodep
+from bs4 import BeautifulSoup  # type: ignore[import]  # nodep
 
 # this package
 from .property_format import *
 
 __all__ = ["toxnet"]
 
 
-def toxnet(cas: str):
+def toxnet(cas: str) -> Dict[str, Any]:
 	"""
 	Obtain physical properties for the compound with the given CAS number from the ToxNet database.
 
 	:param cas:
 	"""
 
 	try:
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/cas.py` & `chemistry_tools-1.0.0b1/chemistry_tools/cas.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/spectrum_similarity.py` & `chemistry_tools-1.0.0b1/chemistry_tools/spectrum_similarity.py`

 * *Files 27% similar despite different names*

```diff
@@ -46,56 +46,224 @@
 #  |  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 #  |  ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  |  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 #  |  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 # stdlib
-from typing import Mapping, Optional, Sequence, Tuple, Union, overload
+from typing import Mapping, Optional, Sequence, Tuple, Union
 
 # 3rd party
 import numpy
-import pandas  # type: ignore
-from typing_extensions import Literal
+import pandas  # type: ignore[import]
 
 __all__ = ["spectrum_similarity", "normalize", "create_array"]
 
 
-@overload
-def spectrum_similarity(
-		spec_top: numpy.ndarray,
-		spec_bottom: numpy.ndarray,
-		t: float = ...,
-		b: float = ...,
-		top_label: Optional[str] = ...,
-		bottom_label: Optional[str] = ...,
-		xlim: Tuple[int, int] = ...,
-		x_threshold: float = ...,
-		print_alignment: bool = ...,
-		print_graphic: bool = ...,
-		output_list: Literal[True] = True,
-		) -> Tuple[float, float, pandas.DataFrame]: ...
+class SpectrumSimilarity:
+	"""
+	Calculate the similarity score for two mass spectra.
 
+	:param spec_top: Array containing the experimental spectrum's peak list with the m/z values in the
+		first column and corresponding intensities in the second
+	:param spec_bottom: Array containing the reference spectrum's peak list with the m/z values in the
+		first column and corresponding intensities in the second
+	:param b: numeric value specifying the baseline threshold for peak identification.
+		Expressed as a percent of the maximum intensity.
+	:param x_threshold: numeric value specifying
+	:param xlim: tuple of length 2, defining the beginning and ending values of the x-axis.
 
-@overload
-def spectrum_similarity(
-		spec_top: numpy.ndarray,
-		spec_bottom: numpy.ndarray,
-		t: float,
-		b: float,
-		top_label: Optional[str],
-		bottom_label: Optional[str],
-		xlim: Tuple[int, int],
-		x_threshold: float,
-		print_alignment: bool,
-		print_graphic: bool,
-		output_list: Literal[False],
-		) -> Tuple[float, float]: ...
+	.. versionadded:: 1.0.0
+
+	.. TODO: t: numeric value specifying the tolerance used to align the m/z values of the two spectra.
+	"""
 
+	top_df: pandas.DataFrame
+	_top_df_plot: pandas.DataFrame  # includes peaks below ``b``
+	bottom_df: pandas.DataFrame
+	_bottom_df_plot: pandas.DataFrame  # includes peaks below ``b``
+	b: float
+	alignment: pandas.DataFrame
+
+	def __init__(
+			self,
+			spec_top: numpy.ndarray,
+			spec_bottom: numpy.ndarray,
+			# t: float = 0.25,
+			b: float = 1,
+			xlim: Tuple[int, int] = (50, 1200),  # x_threshold: float = 0,
+			):
+
+		# if x_threshold < 0:
+		# 	raise ValueError("x_threshold argument must be zero or a positive number")
+
+		self.b = b
+		self.xlim = xlim
+
+		# format spectra and normalize intensitites
+		self.top_df, self._top_df_plot = self._build_dataframe(spec_top)
+		self.bottom_df, self._bottom_df_plot = self._build_dataframe(spec_bottom)
+
+		# align the m/z axis of the two spectra, the bottom spectrum is used as the reference
+
+		# Unimplemented R code
+		#   for(i in 1:nrow(bottom))
+		# 	top["mz"][bottom["mz"][i] >= top["mz"] - t & bottom["mz"][i] <= top["mz"] + t] = bottom["mz"][i]
+		# 	top[,1][bottom[,1][i] >= top[,1] - t & bottom[,1][i] <= top[,1] + t] <- bottom[,1][i]
+		#   alignment <- merge(top, bottom, by = 1, all = TRUE)
+		#   if(length(unique(alignment[,1])) != length(alignment[,1])) warning("the m/z tolerance is set too high")
+		# alignment[,c(2,3)][is.na(alignment[,c(2,3)])] <- 0   # convert NAs to zero (R-Help, Sept. 15, 2004, John Fox)
+		# names(alignment) <- c("mz", "intensity.top", "intensity.bottom")
+
+		alignment = pandas.merge(self.top_df, self.bottom_df, on="mz", how="outer")
+		self.alignment = alignment.fillna(value=0)  # Convert NaN to 0
+		self.alignment.columns = ["mz", "intensity_top", "intensity_bottom"]
+
+		reverse_alignment = pandas.merge(self.top_df, self.bottom_df, on="mz", how="right")
+		self.reverse_alignment = reverse_alignment.dropna()  # Remove rows containing NaN
+		self.reverse_alignment.columns = ["mz", "intensity_top", "intensity_bottom"]
+
+	def _calculate_score(self, alignment: pandas.DataFrame) -> float:
+		u = numpy.array(alignment.iloc[:, 1])
+		v = numpy.array(alignment.iloc[:, 2])
+
+		return numpy.dot(u, v) / (numpy.sqrt(numpy.sum(numpy.square(u))) * numpy.sqrt(numpy.sum(numpy.square(v))))
+
+	def score(self) -> Tuple[float, float]:
+		# similarity score calculation
+
+		# Unimplemented R code
+		# alignment <- alignment[alignment[,1] >= x.threshold, ]
+
+		similarity_score = self._calculate_score(self.alignment)
+		reverse_similarity_score = self._calculate_score(self.reverse_alignment)
+
+		return similarity_score, reverse_similarity_score
 
+	def plot(
+			self,
+			top_label: Optional[str] = None,
+			bottom_label: Optional[str] = None,
+			filter: bool = False,  # Whether peaks below b should be filtered  # noqa: A002  # pylint: disable=redefined-builtin
+			) -> None:
+		"""
+		Plot the mass spectra head to tail.
+
+		:param top_label: string to label the top spectrum.
+		:param bottom_label: string to label the bottom spectrum.
+		"""
+
+		# 3rd party
+		import matplotlib.pyplot as plt  # type: ignore[import]  # nodep
+
+		_, ax = plt.subplots()
+		# fig.scatter(top_plot["mz"],top_plot["intensity"], s=0)
+
+		if filter:
+			ax.vlines(self.top_df["mz"], 0, self.top_df["intensity"], color="blue")
+			ax.vlines(self.bottom_df["mz"], 0, -self.bottom_df["intensity"], color="red")
+		else:
+			ax.vlines(self._top_df_plot["mz"], 0, self._top_df_plot["intensity"], color="blue")
+			ax.vlines(self._bottom_df_plot["mz"], 0, -self._bottom_df_plot["intensity"], color="red")
+
+		ax.set_ylim(-125, 125)
+		ax.set_xlim(self.xlim[0], self.xlim[1])
+		ax.axhline(color="black", linewidth=0.5)
+		ax.set_ylabel("Intensity (%)")
+		ax.set_xlabel("m/z", style="italic", family="serif")
+
+		h_centre = self.xlim[0] + (self.xlim[1] - self.xlim[0]) // 2
+
+		ax.text(h_centre, 110, top_label, horizontalalignment="center", verticalalignment="center")
+		ax.text(h_centre, -110, bottom_label, horizontalalignment="center", verticalalignment="center")
+		return ax
+
+		# Unimplemented R code
+		# 	ticks <- c(-100, -50, 0, 50, 100)
+		# 	plot.window(xlim = c(0, 20), ylim = c(-10, 10))
+		#
+		#
+		#   if(output.list == TRUE) {
+		#
+		# 	# Grid graphics head to tail plot
+		#
+		# 	headTailPlot <- function() {
+		#
+		# 	  pushViewport(plotViewport(c(5, 5, 2, 2)))
+		# 	  pushViewport(dataViewport(xscale = xlim, yscale = c(-125, 125)))
+		#
+		# 	  grid.rect()
+		# 	  tmp <- pretty(xlim)
+		# 	  xlabels <- tmp[tmp >= xlim[1] & tmp <= xlim[2]]
+		# 	  grid.xaxis(at = xlabels)
+		# 	  grid.yaxis(at = c(-100, -50, 0, 50, 100))
+		#
+		# 	  grid.segments(top_plot$mz,
+		# 					top_plot$intensity,
+		# 					top_plot$mz,
+		# 					rep(0, length(top_plot$intensity)),
+		# 					default.units = "native",
+		# 					gp = gpar(lwd = 0.75, col = "blue"))
+		#
+		# 	  grid.segments(bottom_plot$mz,
+		# 					-bottom_plot$intensity,
+		# 					bottom_plot$mz,
+		# 					rep(0, length(bottom_plot$intensity)),
+		# 					default.units = "native",
+		# 					gp = gpar(lwd = 0.75, col = "red"))
+		#
+		# 	  grid.abline(intercept = 0, slope = 0)
+		#
+		# 	  grid.text("intensity (%)", x = unit(-3.5, "lines"), rot = 90)
+		# 	  grid.text("m/z", y = unit(-3.5, "lines"))
+		#
+		# 	  popViewport(1)
+		# 	  pushViewport(dataViewport(xscale = c(0, 20), yscale = c(-10, 10)))
+		# 	  grid.text(top.label, unit(10, "native"), unit(9, "native"))
+		# 	  grid.text(bottom.label, unit(10, "native"), unit(-9, "native"))
+		#
+		# 	  popViewport(2)
+		#
+		# 	}
+		#
+		# 	p <- grid.grabExpr(headTailPlot())
+		#
+		#   }
+		#
+		# with pandas.option_context('display.max_rows', None, 'display.max_columns', None):
+		# 	print(similarity_score)
+
+		# Unimplemented R code
+		#
+		# return(list(similarity.score = similarity_score,
+		# 	alignment = alignment,
+		# 	plot = p))
+		#
+
+	def print_alignment(self) -> None:
+		"""
+		Print the dataframe giving aligned peaks in the top and bottom spectra.
+		"""
+
+		with pandas.option_context("display.max_rows", None, "display.max_columns", None):
+			print(self.alignment)
+
+	def _build_dataframe(self, spectrum: numpy.ndarray) -> Tuple[pandas.DataFrame, pandas.DataFrame]:
+		# format spectra and normalize intensitites
+		tmp = pandas.DataFrame(data=spectrum, columns=["mz", "intensity"])
+		tmp["normalized"] = tmp.apply(normalize, args=(max(tmp["intensity"]), ), axis=1)
+		tmp = tmp[tmp["mz"].between(self.xlim[0], self.xlim[1])]
+		plot = tmp[["mz", "normalized"]].copy()  # data frame for plotting spectrum
+		plot.columns = ["mz", "intensity"]
+		out = plot[plot["intensity"] >= self.b]  # data frame for similarity score calculation
+
+		return out, plot
+
+
+# Deprecated
 def spectrum_similarity(
 		spec_top: numpy.ndarray,
 		spec_bottom: numpy.ndarray,
 		t: float = 0.25,
 		b: float = 10,
 		top_label: Optional[str] = None,
 		bottom_label: Optional[str] = None,
@@ -114,15 +282,15 @@
 		first column and corresponding intensities in the second
 	:param t: numeric value specifying the tolerance used to align the m/z values of the two spectra.
 	:param b: numeric value specifying the baseline threshold for peak identification.
 		Expressed as a percent of the maximum intensity.
 	:param top_label: string to label the top spectrum.
 	:param bottom_label: string to label the bottom spectrum.
 	:param xlim: tuple of length 2, defining the beginning and ending values of the x-axis.
-	:param x_threshold: numeric value specifying
+	:param x_threshold:
 	:param print_alignment:  whether the intensities should be printed
 	:param print_graphic:
 	:param output_list: whether the intensities should be returned as a third element of the tuple.
 	"""
 
 	# format spectra and normalize intensitites
 	top_tmp = pandas.DataFrame(data=spec_top, columns=["mz", "intensity"])
@@ -183,15 +351,15 @@
 			numpy.sqrt(numpy.sum(numpy.square(u))) * numpy.sqrt(numpy.sum(numpy.square(v)))
 			)
 
 	# generate plot
 
 	if print_graphic:
 		# 3rd party
-		import matplotlib.pyplot as plt  # type: ignore  # nodep
+		import matplotlib.pyplot as plt  # nodep
 
 		fig, ax = plt.subplots()
 		# fig.scatter(top_plot["mz"],top_plot["intensity"], s=0)
 		ax.vlines(top_plot["mz"], 0, top_plot["intensity"], color="blue")
 		ax.vlines(bottom["mz"], 0, -bottom["intensity"], color="red")
 		ax.set_ylim(-125, 125)
 		ax.set_xlim(xlim[0], xlim[1])
@@ -270,15 +438,15 @@
 	#
 	else:
 		return similarity_score, reverse_similarity_score
 
 
 # simscore <- as.vector((u %*% v)^2 / (sum(u^2) * sum(v^2)))   # cos squared
 
-SpectrumSimilarity = spectrum_similarity
+# SpectrumSimilarity = spectrum_similarity
 
 
 def normalize(row: Union[Mapping, pandas.Series], max_val: Union[float, str]) -> float:
 	"""
 	Returns the normalised intensity for each rows of a :class:`pandas.DataFrame`.
 
 	:param row:
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/units.py` & `chemistry_tools-1.0.0b1/chemistry_tools/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,20 +45,20 @@
 #  |  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 #  |  ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  |  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 #  |  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 # stdlib
-from typing import Union
+from typing import Tuple, Union
 
 # 3rd party
 import numpy
-import quantities  # type: ignore
-import quantities.markup  # type: ignore
+import quantities  # type: ignore[import]
+import quantities.markup  # type: ignore[import]
 
 __all__ = [
 		"as_latex",
 		"compare_equality",
 		"allclose",
 		"format_string",
 		"per100eV",
@@ -77,15 +77,15 @@
 		"SI_base_registry",
 		"dimension_codes",
 		"m_math_space",
 		"format_si_units",
 		]
 
 
-def as_latex(quant: quantities.quantity.Quantity):
+def as_latex(quant: quantities.quantity.Quantity) -> str:
 	r"""
 	Returns the LaTeX reperesentation of the unit of a quantity.
 
 	:bold-title:`Example:`
 
 	.. code-block:: python
 
@@ -125,22 +125,22 @@
 
 	# Workaround for https://github.com/python-quantities/python-quantities/issues/146
 	try:
 		a + b
 	except TypeError:
 		# We might be dealing with e.g. None (None + None raises TypeError)
 		try:
-			len(a)  # type: ignore
+			len(a)  # type: ignore[arg-type]
 		except TypeError:
 			# Assumed scalar
 			return a == b
 		else:
-			if len(a) != len(b):  # type: ignore
+			if len(a) != len(b):  # type: ignore[arg-type]
 				return False
-			return all(compare_equality(_a, _b) for _a, _b in zip(a, b))  # type: ignore
+			return all(compare_equality(_a, _b) for _a, _b in zip(a, b))  # type: ignore[arg-type]
 	except ValueError:
 		return False
 	else:
 		return a == b
 
 
 def allclose(a, b, rtol=1e-8, atol=None) -> bool:
@@ -171,21 +171,25 @@
 		len(d)
 	except TypeError:
 		return d <= lim
 	else:
 		try:
 			len(lim)
 		except TypeError:
-			return numpy.all([_d <= lim for _d in d])  # type: ignore
+			return numpy.all([_d <= lim for _d in d])  # type: ignore[return-value]
 		else:
-			return numpy.all([_d <= _lim for _d, _lim in zip(d, lim)])  # type: ignore
+			return numpy.all([_d <= _lim for _d, _lim in zip(d, lim)])  # type: ignore[return-value]
 
 
 # TODO: decide whether to deprecate in favor of "number_to_scientific_latex"?
-def format_string(value: quantities.quantity.Quantity, precision: str = "%.5g", tex: bool = False):
+def format_string(
+		value: quantities.quantity.Quantity,
+		precision: str = "%.5g",
+		tex: bool = False,
+		) -> Tuple[str, str]:
 	r"""
 	Formats a scalar with unit as two strings.
 
 	:bold-title:`Examples:`
 
 	.. code-block:: python
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/cache.py` & `chemistry_tools-1.0.0b1/chemistry_tools/cache.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/names.py` & `chemistry_tools-1.0.0b1/chemistry_tools/names.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 
 # stdlib
 import re
 from typing import Any, Dict, List, Pattern, Sequence, Tuple
 
 # 3rd party
-from pandas import DataFrame  # type: ignore
+from pandas import DataFrame  # type: ignore[import]
 
 # this package
 from chemistry_tools import cached_requests
 from chemistry_tools.constants import prefixes
 from chemistry_tools.pubchem.errors import HTTP_ERROR_CODES
 
 __all__ = [
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/constants.py` & `chemistry_tools-1.0.0b1/chemistry_tools/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 #  |  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 # stdlib
 from typing import Dict, NamedTuple, Optional
 
 # 3rd party
-import quantities  # type: ignore
+import quantities  # type: ignore[import]
 
 __all__ = [
 		"Constant",
 		"avogadro_number",
 		"plancks_constant",
 		"speed_of_light",
 		"electron_radius",
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/__init__.py` & `chemistry_tools-1.0.0b1/chemistry_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/property_format.py` & `chemistry_tools-1.0.0b1/chemistry_tools/property_format.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/lanthanides.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/lanthanides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/_table.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/_table.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/_isotope_data.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/_isotope_data.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/chalcogens.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/chalcogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/pnictogens.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/pnictogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/classes.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 			for massnumber, isotope in isotopes.items():
 				if isinstance(isotope, Isotope):
 					self._isotopes[int(massnumber)] = isotope
 				elif isinstance(isotope, (list, tuple)):
 					self._isotopes[int(massnumber)] = Isotope(*isotope, massnumber)
 
 	@property
-	def __dict__(self):
+	def __dict__(self):  # noqa: MAN002
 		return dict(
 				number=self._number,
 				symbol=self._symbol,
 				name=self._name,
 				group=self._group,
 				period=self._period,
 				block=self._block,
@@ -588,15 +588,15 @@
 	def __str__(self) -> str:
 		return f"{self.massnumber}, {self.mass:.4f}, {self.abundance * 100:.6f}%"
 
 	def __repr__(self) -> str:
 		return f"Isotope({repr(self.mass)}, {repr(self.abundance)}, {repr(self.massnumber)})"
 
 	@property
-	def __dict__(self):
+	def __dict__(self):  # noqa: MAN002
 		return dict(
 				mass=self.mass,
 				abundance=self.abundance,
 				massnumber=self.massnumber,
 				)
 
 
@@ -638,15 +638,15 @@
 	def __repr__(self) -> str:
 		elements = ",\n    ".join(
 				"\n    ".join(line for line in repr(element).splitlines()) for element in self._list
 				)
 		elements = f"Elements(\n    {elements},\n)"
 		return elements
 
-	def __contains__(self, item) -> bool:
+	def __contains__(self, item) -> bool:  # noqa: MAN001
 		return item in self._dict
 
 	def __iter__(self) -> Iterator[Element]:
 		"""
 		Returns an iterator over the elements, in order.
 		"""
 
@@ -661,15 +661,15 @@
 
 	@overload
 	def __getitem__(self, key: slice) -> List[Element]: ...
 
 	@overload
 	def __getitem__(self, key: Union[str, int, float]) -> Element: ...
 
-	def __getitem__(self, key):
+	def __getitem__(self, key):  # noqa: MAN001,MAN002
 		"""
 		Return ``self[key]``.
 
 		:param key: If a string, return the :class:`~.Element` with that name or symbol.
 			If a number, return the element with that atomic number.
 		"""
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/alkaline_earth_metals.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/alkaline_earth_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/noble_gases.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/noble_gases.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/__init__.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/alkali_metals.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/alkali_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/transition_metals.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/transition_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/_elements.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/_elements.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/halogens.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/halogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/triels.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/triels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/tetrels.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/tetrels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/elements/actinides.py` & `chemistry_tools-1.0.0b1/chemistry_tools/elements/actinides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/utils.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/utils.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/html.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/html.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/species.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/species.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
 		return self.__class__(
 				self,
 				charge=self.charge,
 				phase=cast(Optional[Literal['s', 'l', 'g', "aq"]], self.phase),
 				)
 
-	def __eq__(self, other) -> bool:
+	def __eq__(self, other) -> bool:  # noqa: MAN001
 		"""
 		Returns ``self == other``.
 		"""
 
 		if isinstance(other, Species):
 			if super().__eq__(other):
 				return self.phase == other.phase
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/dataarray.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/dataarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # stdlib
 from abc import abstractmethod
 #  3rd party
 from typing import Any, Dict, List, Optional, Set
 
 # 3rd party
-import pandas  # type: ignore
+import pandas  # type: ignore[import]
 import tabulate  # nodep
 from cawdrey import FrozenOrderedDict  # nodep
 from domdf_python_tools.doctools import prettify_docstrings
 
 __all__ = ["DataArray"]
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/parser.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 #
 
 # stdlib
 import re
 from collections import defaultdict
 from functools import lru_cache
 from string import ascii_lowercase, ascii_uppercase
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Union
+from typing import Dict, Iterable, List, Mapping, Optional, Sequence, Union
 
 # 3rd party
 import pyparsing  # nodep
 
 # this package
 from chemistry_tools.elements import ELEMENTS
 
@@ -164,15 +164,15 @@
 for elem in element_re:
 	isotopes_re.append(rf"\b{elem}\[[0-9]+\]")
 	isotopes_re.append(rf"\[{elem}[0-9]+\]")
 	isotopes_re.append(rf"\[[0-9]+{elem}\]")
 
 
 @lru_cache()
-def _get_formula_parser():
+def _get_formula_parser() -> pyparsing.Forward:
 	"""
 	Create a forward pyparsing parser for chemical formulae.
 
 	BNF for simple chemical formula (no nesting)
 
 		integer :: '0'..'9'+
 		element :: 'A'..'Z' 'a'..'z'*
@@ -191,15 +191,14 @@
 	-----
 	Based on http://stackoverflow.com/a/18555142/790973
 	Copyright 2013 Paul McGuire (http://stackoverflow.com/users/165216/paul-mcguire)
 	Licensed under CC-BY-SA 3.0.
 	"""
 
 	Forward, Group, OneOrMore = pyparsing.Forward, pyparsing.Group, pyparsing.OneOrMore
-	ParseResults = pyparsing.ParseResults
 	Suppress, Word, nums = pyparsing.Suppress, pyparsing.Word, pyparsing.nums
 
 	LPAR, RPAR = map(Suppress, "()")
 	integer = Word(nums)
 
 	# add parse action to convert integers to ints, to support doing addition
 	# and multiplication at parse time
@@ -217,58 +216,58 @@
 
 	_term_subgroup = (element | Group(LPAR + formula + RPAR)("subgroup"))
 	term = Group(_term_subgroup + pyparsing.Optional(integer, default=1)("mult"))
 
 	# add parse actions for parse-time processing
 
 	# parse action to multiply out subgroups
-	def multiplyContents(tokens):
+	def multiplyContents(tokens):  # noqa: MAN001,MAN002
 		t = tokens[0]
 		# if these tokens contain a subgroup, then use multiplier to
 		# extend counts of all elements in the subgroup
 		if t.subgroup:
 			mult = t.mult
 			for term in t.subgroup:
 				term[1] *= mult
 			return t.subgroup
 
 	term.setParseAction(multiplyContents)
 
 	# add parse action to sum up multiple references to the same element
-	def sum_by_element(tokens):
+	def sum_by_element(tokens) -> Optional[pyparsing.ParseResults]:  # noqa: MAN001
 		elementsList = [t[0] for t in tokens]
 
 		# construct set to see if there are duplicates
 		duplicates = len(elementsList) > len(set(elementsList))
 
 		# if there are duplicate element names, sum up by element and
-		# return a new nested ParseResults
+		# return a new nested pyparsing.ParseResults
 		if duplicates:
 			ctr: Dict = defaultdict(int)
 			for t in tokens:
 				ctr[t[0]] += t[1]
-			return ParseResults([ParseResults([k, v]) for k, v in ctr.items()])
+			return pyparsing.ParseResults([pyparsing.ParseResults([k, v]) for k, v in ctr.items()])
+		return None
 
 	# define contents of a formula as one or more terms
 	formula << OneOrMore(term)  # pylint: disable=expression-not-assigned
 	formula.setParseAction(sum_by_element)
-
 	return formula
 
 
-def _parse_stoich(stoich) -> Dict[int, Any]:
-	if stoich == 'e':  # special case, the electron is not an element
-		return {}
+# def _parse_stoich(stoich) -> Dict[int, Any]:
+# 	if stoich == 'e':  # special case, the electron is not an element
+# 		return {}
 
-	symbols = ELEMENTS.symbols + ['D', 'T']
+# 	symbols = ELEMENTS.symbols + ['D', 'T']
 
-	if re.findall('|'.join(invalid_re), stoich):
-		raise ValueError(f"Unrecognised formula: {stoich}")
+# 	if re.findall('|'.join(invalid_re), stoich):
+# 		raise ValueError(f"Unrecognised formula: {stoich}")
 
-	return {symbols.index(k) + 1: n for k, n in _get_formula_parser().parseString(stoich)}
+# 	return {symbols.index(k) + 1: n for k, n in _get_formula_parser().parseString(stoich)}
 
 
 def string_to_composition(
 		formula: str,
 		prefixes: Optional[Iterable[str]] = None,
 		suffixes: Sequence[str] = ("(s)", "(l)", "(g)", "(aq)"),
 		) -> Dict[int, int]:
@@ -307,30 +306,32 @@
 		if idx == 0:
 			m = 1
 		else:
 			m, stoich = _get_leading_integer(stoich)
 
 		# comp = _parse_stoich(stoich)
 		if stoich == 'e':  # special case, the electron is not an element
-			comp = {}
+			pass
 		else:
 			try:
 				if re.findall('|'.join(invalid_re), stoich):
 					raise ValueError(f"Unrecognised formula: {formula}")
 
-				comp = _get_formula_parser().parseString(stoich)
+				comp = _get_formula_parser().parse_string(stoich)
 			except pyparsing.ParseException:
 				raise ValueError(f"Unrecognised formula: {formula}")
 
 		# for k, v in comp.items():
-		for k, v in comp:
-			if k not in tot_comp:
-				tot_comp[k] = m * v
-			else:
-				tot_comp[k] += m * v
+			k: int
+			v: int
+			for k, v in comp:
+				if k not in tot_comp:
+					tot_comp[k] = m * v
+				else:
+					tot_comp[k] += m * v
 
 	if chg_tok is not None:
 		tot_comp[0] = _get_charge(chg_tok)
 
 	return tot_comp
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/iso_dist.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/iso_dist.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/compound.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/compound.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 #  |  DOI: `10.1021/acs.jproteome.8b00717 <http://dx.doi.org/10.1021/acs.jproteome.8b00717>`_
 #
 
 # stdlib
 from typing import Dict, Optional
 
 # 3rd party
-import quantities  # type: ignore
+import quantities  # type: ignore[import]
 from domdf_python_tools.bases import Dictable
 from domdf_python_tools.doctools import prettify_docstrings
 
 # this package
 from chemistry_tools.formulae.formula import Formula
 from chemistry_tools.formulae.html import string_to_html
 from chemistry_tools.formulae.latex import string_to_latex
@@ -160,25 +160,25 @@
 			self.html_name = html_name
 		else:
 			self.html_name = string_to_html(self.formula.hill_formula)
 
 		self.data: Optional[Dict] = data or {}
 
 	@property
-	def __dict__(self):
+	def __dict__(self):  # noqa: MAN002
 		return dict(
 				name=self.name,
 				latex_name=self.latex_name,
 				unicode_name=self.unicode_name,
 				html_name=self.html_name,
 				formula=self.formula,
 				data=self.data,
 				)
 
-	def __eq__(self, other) -> bool:
+	def __eq__(self, other) -> bool:  # noqa: MAN001
 		if isinstance(other, str):
 			return self.name == other
 		else:
 			return super().__eq__(other)
 
 	@property
 	def charge(self) -> int:
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/__init__.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/latex.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/latex.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/composition.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/composition.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/_parser_core.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/_parser_core.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/formula.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/formula.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 									f"'charge' keyword argument. {charge}, {self.charge}"
 									)
 
 					charge = composition.charge
 
 		self._set_charge(charge)
 
-	def _set_charge(self, charge: int):
+	def _set_charge(self, charge: int) -> None:
 		# Get charge
 		if charge and self.charge:
 			if charge != self.charge:
 				# No point raising error if the charges are the same
 				raise ValueError(
 						"Charge is specified in both the formula and with the "
 						f"'charge' keyword argument. {charge}, {self.charge}"
@@ -631,72 +631,72 @@
 	def copy(self: F) -> F:
 		"""
 		Returns a copy of the :class:`~.Formula`.
 		"""
 
 		return self.__class__(self, charge=self.charge)
 
-	def __missing__(self, key):
+	def __missing__(self, key) -> int:  # noqa: MAN001
 		# override default behavior: we don't want to add 0's to the dictionary
 		return 0
 
-	def __setitem__(self, key, value):
+	def __setitem__(self, key: str, value: float) -> None:
 		if isinstance(value, float):
 			value = int(round(value))
 		elif not isinstance(value, int):
 			raise TypeError(f"Only integers allowed as values in Formula, got {type(value).__name__}.")
 		if value:  # reject 0's
 			super(defaultdict, self).__setitem__(key, value)
 		elif key in self:
 			del self[key]
 
-	def __add__(self, other):
+	def __add__(self, other):  # noqa: MAN001,MAN002
 		result = self.copy()
 		for elem, count in other.items():
 			result[elem] += count
 		return result
 
-	def __iadd__(self, other):
+	def __iadd__(self, other) -> "Formula":  # noqa: MAN001
 		for elem, count in other.items():
 			self[elem] += count
 		return self
 
-	def __radd__(self, other):
+	def __radd__(self, other):  # noqa: MAN001,MAN002
 		return self + other
 
-	def __sub__(self, other):
+	def __sub__(self, other):  # noqa: MAN001,MAN002
 		result = self.copy()
 		for elem, count in other.items():
 			result[elem] -= count
 		return result
 
-	def __isub__(self, other):
+	def __isub__(self, other) -> "Formula":  # noqa: MAN001
 		for elem, count in other.items():
 			self[elem] -= count
 		return self
 
-	def __rsub__(self, other):
+	def __rsub__(self, other):  # noqa: MAN001,MAN002
 		return (self - other) * (-1)
 
-	def __mul__(self, other):
+	def __mul__(self, other) -> "Formula":  # noqa: MAN001
 		if not isinstance(other, int):
 			raise TypeError(f'Cannot multiply Formula by non-integer "{other}"')
 		return type(self)({k: v * other for k, v in self.items()})
 
-	def __imul__(self, other):
+	def __imul__(self, other) -> "Formula":  # noqa: MAN001
 		if not isinstance(other, int):
 			raise TypeError(f'Cannot multiply Formula by non-integer "{other}"')
 		for elem in self:
 			self[elem] *= other
 		return self
 
-	def __rmul__(self, other):
+	def __rmul__(self, other):  # noqa: MAN001,MAN002
 		return self * other
 
-	def __eq__(self, other) -> bool:
+	def __eq__(self, other) -> bool:  # noqa: MAN001
 		if isinstance(other, (dict, Formula)):
 			self_items = {i for i in self.items() if i[1]}
 			other_items = {i for i in other.items() if i[1]}
 
 			if isinstance(other, Formula):
 				return self_items == other_items and self.charge == other.charge
 			else:
@@ -870,15 +870,15 @@
 
 		.. latex:clearpage::
 		"""
 
 		return len(self)
 
 	@property
-	def elements(self) -> List[str]:  # type: ignore
+	def elements(self) -> List[str]:  # type: ignore[override]
 		"""
 		A list of the element symbols in the formula.
 		"""
 
 		return list(self.keys())
 
 	@property
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/formulae/unicode.py` & `chemistry_tools-1.0.0b1/chemistry_tools/formulae/unicode.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/lookup.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/lookup.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/full_record.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/full_record.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/utils.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/utils.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/description.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/description.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 	return parsed_data[0]["CID"]
 
 
 def rest_get_description(
 		identifier: Union[str, int, Sequence[Union[str, int]]],
 		namespace: Union[PubChemNamespace, str] = PubChemNamespace.name,
 		**kwargs,
-		):
+		) -> Dict[str, Any]:
 	"""
 	Obtains the description for the given compound from the PubChem REST API.
 
 	:param identifier: Identifiers (e.g. name, CID) for the compound to look up.
 		When using the CID namespace data for multiple compounds can be retrieved at once by
 		supplying either a comma-separated string or a list.
 	:param namespace: The type of identifier to look up. Valid values are in :class:`~.PubChemNamespace`.
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/errors.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 #  |  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 #  |  THE SOFTWARE.
 #
 
 # stdlib
 import json
 
+# 3rd party
+import requests
+
 __all__ = [
 		"ResponseParseError",
 		"PubChemHTTPError",
 		"BadRequestError",
 		"NotFoundError",
 		"MethodNotAllowedError",
 		"TimeoutError",
@@ -111,15 +114,15 @@
 
 
 class PubChemHTTPError(Exception):
 	"""
 	Generic error class to handle all HTTP error codes.
 	"""
 
-	def __init__(self, e):
+	def __init__(self, e: requests.Response):
 		self.code = e.status_code
 		self.msg = e.reason
 		try:
 			self.msg += f': {json.loads(e.content.decode())["Fault"]["Details"][0]}'
 		except (ValueError, IndexError, KeyError):
 			pass
 		if self.code == 400:
@@ -140,59 +143,59 @@
 
 
 class BadRequestError(PubChemHTTPError):
 	"""
 	Request is improperly formed (syntax error in the URL, POST body, etc.).
 	"""
 
-	def __init__(self, msg="Request is improperly formed"):
+	def __init__(self, msg: str = "Request is improperly formed"):
 		self.msg = msg
 
 
 class NotFoundError(PubChemHTTPError):
 	"""
 	The input record was not found (e.g. invalid CID).
 	"""
 
-	def __init__(self, msg="The input record was not found"):
+	def __init__(self, msg: str = "The input record was not found"):
 		self.msg = msg
 
 
 class MethodNotAllowedError(PubChemHTTPError):
 	"""
 	Request not allowed (such as invalid MIME type in the HTTP Accept header).
 	"""
 
-	def __init__(self, msg="Request not allowed"):
+	def __init__(self, msg: str = "Request not allowed"):
 		self.msg = msg
 
 
 class HTTPTimeoutError(PubChemHTTPError):
 	"""
 	The request timed out, from server overload or too broad a request.
 
 	.. versionchanged:: 0.4.0  Renamed from TimeoutErrpr
 	"""
 
-	def __init__(self, msg="The request timed out"):
+	def __init__(self, msg: str = "The request timed out"):
 		self.msg = msg
 
 
 TimeoutError = HTTPTimeoutError  # noqa: A001  # pylint: disable=redefined-builtin
 
 
 class UnimplementedError(PubChemHTTPError):
 	"""
 	The requested operation has not (yet) been implemented by the server.
 	"""
 
-	def __init__(self, msg="The requested operation has not been implemented"):
+	def __init__(self, msg: str = "The requested operation has not been implemented"):
 		self.msg = msg
 
 
 class ServerError(PubChemHTTPError):
 	"""
 	Some problem on the server side (such as a database server down, etc.).
 	"""
 
-	def __init__(self, msg="Some problem on the server side"):
+	def __init__(self, msg: str = "Some problem on the server side"):
 		self.msg = msg
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/bond.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/bond.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 		self.aid2: int = aid2
 		self.order: BondType = BondType(order)
 		self.style = style
 
 	def __repr__(self) -> str:
 		return f"Bond({self.aid1}, {self.aid2}, {self.order!r})"
 
-	def __eq__(self, other) -> bool:
+	def __eq__(self, other) -> bool:  # noqa: MAN001
 		return (
 			isinstance(other, type(self))
 			and self.aid1 == other.aid1
 			and self.aid2 == other.aid2
 			and self.order == other.order
 			and self.style == other.style
 			)  # yapf: disable
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 	# INCHI = Inchi = inchi = "inchi"# TODO: requires argument
 	# Formula = FORMULA = formula = "formula"
 	# SDF = Sdf = sdf = "sdf"
 
 	# TODO: listkey for formula lookup https://pubchemdocs.ncbi.nlm.nih.gov/pug-rest$_Toc494865583
 
-	def __new__(cls, value, doc):  # noqa: D102
+	def __new__(cls, value: str, doc: str):  # noqa: D102
 		obj = str.__new__(cls, value)  # noqa
 		obj._value_ = value
 		obj.__doc__ = doc
 		return obj
 
 	@classmethod
 	def is_valid_value(cls, value: Any) -> bool:
@@ -72,15 +72,15 @@
 	"""
 
 	JSON = Json = json = "JSON"
 	XML = Xml = xml = "XML"
 	CSV = csv = Csv = "CSV"
 	PNG = png = Png = "PNG"
 
-	def __new__(cls, value):  # noqa: D102
+	def __new__(cls, value: str):  # noqa: D102
 		obj = str.__new__(cls, value)  # noqa
 		obj._value_ = value
 		obj.__doc__ = f"{value} Format"
 		return obj
 
 	@classmethod
 	def is_valid_value(cls, value: Any) -> bool:
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/enums.pyi` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class PubChemNamespace(StrEnum):
 	CID = Cid = cid = "cid"
 	Name = NAME = name = "name"
 	SMILES = Smiles = smiles = "smiles"
 	INCHIKEY = Inchikey = inchikey = "inchikey"
 
-	def __new__(cls, value, doc): ...
+	def __new__(cls, value: str, doc: str): ...
 
 	@classmethod
 	def is_valid_value(cls, value: Any) -> bool: ...
 
 # @document_enum
 
 class PubChemFormats(StrEnum):
@@ -44,15 +44,15 @@
 	Enum of supported formats for the PubChem REST API.
 	"""
 	JSON = Json = json = "JSON"
 	XML = Xml = xml = "XML"
 	CSV = csv = Csv = "CSV"
 	PNG = png = Png = "PNG"
 
-	def __new__(cls, value): ...
+	def __new__(cls, value: str): ...
 
 	@classmethod
 	def is_valid_value(cls, value: Any) -> bool: ...
 
 class CoordinateType(IntEnum):
 	TWO_D = ...
 	THREE_D = ...
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/compound.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/compound.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # stdlib
 from typing import Any, Dict, FrozenSet, List, Optional, Sequence, Type, TypeVar, Union
 
 # 3rd party
 from domdf_python_tools.bases import Dictable
 from domdf_python_tools.doctools import prettify_docstrings
-from pandas import DataFrame, Series  # type: ignore
+from pandas import DataFrame, Series  # type: ignore[import]
 
 # this package
 from chemistry_tools._memoized_property import memoized_property
 from chemistry_tools.formulae import Formula
 from chemistry_tools.pubchem.atom import Atom, parse_atoms
 from chemistry_tools.pubchem.bond import Bond, parse_bonds
 from chemistry_tools.pubchem.enums import CoordinateType
@@ -83,15 +83,15 @@
 	Each Compound is uniquely identified by a CID.
 
 	:param title: The title of the compound record (usually the name of the compound)
 	:param CID:
 	:param description:
 	"""
 
-	def __init__(self, title: str, CID: int, description, **_):
+	def __init__(self, title: str, CID: int, description: str, **_):
 		super().__init__()
 
 		self.title: str = str(title)
 		self.CID: int = int(CID)
 		self.description: str = str(description)
 		self._properties: Dict = {prop: None for prop in valid_properties}
 		self.record_type: str = "2d"
@@ -99,15 +99,15 @@
 
 		# Pre-cache all properties
 		# self.get_properties("all")
 
 		self._has_full_record: bool = False
 
 	@property
-	def __dict__(self):
+	def __dict__(self):  # noqa: MAN002
 		return dict(
 				title=self.title,
 				CID=self.CID,
 				description=self.description,
 				properties=self._properties,
 				record_type=self.record_type,
 				counts=self._record["counts"],
@@ -214,15 +214,15 @@
 		if "bonds" not in self._record:
 			return None
 
 		bonds_dict = self._record["bonds"]
 		coords_dict = self._record.get("coords", None)
 		return parse_bonds(bonds_dict, coords_dict)
 
-	def precache(self):
+	def precache(self) -> None:
 		"""
 		Precache all properties for this compound.
 		"""
 
 		self.get_properties("all")
 		_ = self._atoms
 		_ = self._bonds
@@ -345,15 +345,15 @@
 
 			else:
 				self._synonyms = data["synonyms"]
 
 		return self._synonyms
 
 	@classmethod
-	def from_cid(cls: Type['C'], cid, record_type: str = "2d") -> "Compound":
+	def from_cid(cls: Type['C'], cid: Union[str, int], record_type: str = "2d") -> "Compound":
 		"""
 		Returns the Compound objects for the compound with the given CID.
 		"""
 
 		# this package
 		from chemistry_tools.pubchem.lookup import get_compounds
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/atom.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/atom.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 		self.y: Optional[float] = y
 		self.z: Optional[float] = z
 		self.charge: int = charge
 
 	def __repr__(self) -> str:
 		return f"Atom({self.aid}, {self.element})"
 
-	def __eq__(self, other) -> bool:
+	def __eq__(self, other) -> bool:  # noqa: MAN001
 		return (
 			isinstance(other, type(self))
 			and self.aid == other.aid
 			and self.element == other.element
 			and self.x == other.x
 			and self.y == other.y
 			and self.z == other.z
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/images.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 
 # stdlib
 from io import BytesIO
 from typing import Sequence, Union
 
 # 3rd party
-from PIL import Image  # type: ignore  # nodep
+from PIL import Image  # type: ignore[import]  # nodep
 
 # this package
 from .enums import PubChemNamespace
 from .pug_rest import do_rest_get
 
 __all__ = ["get_structure_image"]
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/__init__.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/pug_rest.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/pug_rest.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/synonyms.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/synonyms.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,35 +36,35 @@
 class Synonyms(List[str]):
 	"""
 	Contains a list of synonyms for a compound.
 
 	:param initlist: The content to initialise the list with.
 	"""
 
-	def __init__(self, initlist):
+	def __init__(self, initlist):  # noqa: MAN001
 		super().__init__()
 
 		for val in initlist:
 			self.append(str(val))
 
-	def __contains__(self, synonym) -> bool:
+	def __contains__(self, synonym) -> bool:  # noqa: MAN001
 		"""
 		Return ``synonym in self``.
 
 		The comparison treats hyphens and underscores as whitespace.
 
 		:param synonym:
 		"""
 
 		for v in self:
 			if self._prep_contains(v) == self._prep_contains(synonym):
 				return True
 		return False
 
-	def append(self, synonym: str):
+	def append(self, synonym: str) -> None:
 		"""
 		Append ``synonym`` to the end of the list.
 
 		:param synonym:
 		"""
 
 		if synonym not in self:
```

### Comparing `chemistry_tools-0.6.0/chemistry_tools/pubchem/properties.py` & `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 #  |  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  |  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 #  |  THE SOFTWARE.
 #
 
 # stdlib
 import warnings
-from typing import Any, Callable, Dict, Iterable, List, NamedTuple, Sequence, Union
+from typing import Any, Callable, Dict, Iterable, List, NamedTuple, Optional, Sequence, Union
 
 # 3rd party
-from pandas import DataFrame  # type: ignore
+from pandas import DataFrame  # type: ignore[import]
 
 # this package
 from chemistry_tools.formulae import Formula
 
 # this package
 from .enums import PubChemFormats, PubChemNamespace
 from .pug_rest import do_rest_get
@@ -307,15 +307,15 @@
 
 #: Allows properties to optionally be specified as underscore_separated, consistent with Compound attributes
 PROPERTY_MAP: Dict[str, str] = {prop.attr_name: prop.name for prop in _properties}
 
 
 def rest_get_properties_json(
 		identifier: Union[str, int, Sequence[Union[str, int]]],
-		namespace=PubChemNamespace.name,
+		namespace: Union[str, PubChemNamespace] = PubChemNamespace.name,
 		properties: Union[Sequence[str], str] = '',
 		**kwargs
 		) -> Dict:
 	"""
 	Returns the properties for the compound with the given identifier as a dictionary.
 
 	:param identifier: Identifiers (e.g. name, CID) for the compound to look up.
@@ -343,15 +343,15 @@
 
 
 def rest_get_properties(
 		identifier: Union[str, int, Sequence[Union[str, int]]],
 		namespace=PubChemNamespace.name,
 		properties: Union[Sequence[str], str] = '',
 		format_: Union[PubChemFormats, str] = PubChemFormats.CSV,
-		):
+		) -> str:
 	r"""
 	Returns the properties for the compound with the given identifier in the desired format.
 
 	:param identifier: Identifiers (e.g. name, CID) for the compound to look up.
 		When using the CID namespace data for multiple compounds can be retrieved at once by
 		supplying either a comma-separated string or a list.
 	:param namespace: The type of identifier to look up. Valid values are in :class:`~.PubChemNamespace`
@@ -516,15 +516,15 @@
 					compounds[cid][var] = entry[var]
 
 	return list(compounds.values())
 
 
 class __BasePubChemProperty(NamedTuple):
 	label: str
-	name: str
+	name: Optional[str]
 	value: Any
 	dtype: Callable
 	source: Dict
 
 
 class PubChemProperty(__BasePubChemProperty):
 	"""
@@ -535,15 +535,15 @@
 	:param value: The property's value.
 	:param dtype: The data type property's value.
 	:param source: Dictionary of property sources.
 	"""
 
 	__slots__: List[str] = []
 
-	def __new__(cls, label, name=None, value=None, dtype=None, source=None):  # noqa: D102
+	def __new__(cls, label: str, name: Optional[str] = None, value=None, dtype=None, source=None):  # noqa: D102
 		if source is None:
 			source = {}
 
 		if dtype:
 			value = dtype(value)
 		label = str(label)
 		if name:
```


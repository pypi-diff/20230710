# Comparing `tmp/skypy-0.5.2rc1.tar.gz` & `tmp/skypy-0.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypy-0.5.2rc1.tar", last modified: Mon Jul 10 17:30:44 2023, max compression
+gzip compressed data, was "skypy-0.5rc1.tar", last modified: Tue Nov  2 14:41:21 2021, max compression
```

## Comparing `skypy-0.5.2rc1.tar` & `skypy-0.5rc1.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.733134 skypy-0.5.2rc1/
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.600432 skypy-0.5.2rc1/.github/
--rw-r--r--   0 rpr        (502) staff       (20)      131 2023-03-26 13:50:26.000000 skypy-0.5.2rc1/.github/CODEOWNERS
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.601915 skypy-0.5.2rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 rpr        (502) staff       (20)      555 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 rpr        (502) staff       (20)      176 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/.github/ISSUE_TEMPLATE/new-model-proposal.md
--rw-r--r--   0 rpr        (502) staff       (20)      344 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.604012 skypy-0.5.2rc1/.github/workflows/
--rw-r--r--   0 rpr        (502) staff       (20)      487 2023-03-31 14:47:06.000000 skypy-0.5.2rc1/.github/workflows/codestyle.yaml
--rw-r--r--   0 rpr        (502) staff       (20)     1033 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/.github/workflows/compatibility.yaml
--rw-r--r--   0 rpr        (502) staff       (20)     1434 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/.github/workflows/tests.yaml
--rw-r--r--   0 rpr        (502) staff       (20)      739 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/.gitignore
--rw-r--r--   0 rpr        (502) staff       (20)      749 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/.mailmap
--rw-r--r--   0 rpr        (502) staff       (20)      189 2023-01-29 10:09:51.000000 skypy-0.5.2rc1/.readthedocs.yml
--rw-r--r--   0 rpr        (502) staff       (20)     4347 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/.zenodo.json
--rw-r--r--   0 rpr        (502) staff       (20)     1078 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/CITATION.rst
--rw-r--r--   0 rpr        (502) staff       (20)     9536 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 rpr        (502) staff       (20)     8325 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/CONTRIBUTING.rst
--rw-r--r--   0 rpr        (502) staff       (20)     1477 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/LICENSE.rst
--rw-r--r--   0 rpr        (502) staff       (20)      295 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/MANIFEST.in
--rw-r--r--   0 rpr        (502) staff       (20)     4667 2023-07-10 17:30:44.733542 skypy-0.5.2rc1/PKG-INFO
--rw-r--r--   0 rpr        (502) staff       (20)     4293 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/README.rst
--rw-r--r--   0 rpr        (502) staff       (20)       53 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/codecov.yml
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.611444 skypy-0.5.2rc1/docs/
--rw-r--r--   0 rpr        (502) staff       (20)     4703 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/Makefile
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.616382 skypy-0.5.2rc1/docs/_static/
--rw-r--r--   0 rpr        (502) staff       (20)      294 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/_static/skypy.css
--rw-r--r--   0 rpr        (502) staff       (20)     4286 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/_static/skypy_image.ico
--rw-r--r--   0 rpr        (502) staff       (20)    19630 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/_static/skypy_image.png
--rw-r--r--   0 rpr        (502) staff       (20)    27005 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/_static/skypy_image.svg
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.620667 skypy-0.5.2rc1/docs/arch/
--rw-r--r--   0 rpr        (502) staff       (20)     5773 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/arch/adr-01.md
--rw-r--r--   0 rpr        (502) staff       (20)      677 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/arch/adr-02.md
--rw-r--r--   0 rpr        (502) staff       (20)     3545 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/docs/arch/adr-03.md
--rw-r--r--   0 rpr        (502) staff       (20)     9043 2023-03-26 13:50:26.000000 skypy-0.5.2rc1/docs/conf.py
--rw-r--r--   0 rpr        (502) staff       (20)    12727 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/docs/configuration_files.rst
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.621380 skypy-0.5.2rc1/docs/developer/
--rw-r--r--   0 rpr        (502) staff       (20)       36 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/developer/contributing.rst
--rw-r--r--   0 rpr        (502) staff       (20)      886 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/docs/feature_list.rst
--rw-r--r--   0 rpr        (502) staff       (20)     2309 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/docs/galaxies.rst
--rw-r--r--   0 rpr        (502) staff       (20)     1410 2023-03-26 13:50:26.000000 skypy-0.5.2rc1/docs/index.rst
--rw-r--r--   0 rpr        (502) staff       (20)     2797 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/docs/install.rst
--rw-r--r--   0 rpr        (502) staff       (20)      474 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/docs/luminosity.yml
--rw-r--r--   0 rpr        (502) staff       (20)     4549 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/make.bat
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.622164 skypy-0.5.2rc1/docs/pipeline/
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.623686 skypy-0.5.2rc1/docs/pipeline/examples/
--rw-r--r--   0 rpr        (502) staff       (20)      301 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/pipeline/examples/config.yml
--rw-r--r--   0 rpr        (502) staff       (20)      151 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/pipeline/examples/pipeline.yml
--rw-r--r--   0 rpr        (502) staff       (20)     4063 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/docs/pipeline/index.rst
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.625398 skypy-0.5.2rc1/docs/project/
--rw-r--r--   0 rpr        (502) staff       (20)       32 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/docs/project/citation.rst
--rw-r--r--   0 rpr        (502) staff       (20)       39 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/docs/project/code_of_conduct.rst
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.626251 skypy-0.5.2rc1/docs/utils/
--rw-r--r--   0 rpr        (502) staff       (20)     4500 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/docs/utils/index.rst
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.628323 skypy-0.5.2rc1/examples/
--rw-r--r--   0 rpr        (502) staff       (20)      335 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/examples/README.rst
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.640384 skypy-0.5.2rc1/examples/galaxies/
--rw-r--r--   0 rpr        (502) staff       (20)      122 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/examples/galaxies/README.rst
--rw-r--r--   0 rpr        (502) staff       (20)     1111 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/examples/galaxies/Shen+03_early.txt
--rw-r--r--   0 rpr        (502) staff       (20)     1616 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/examples/galaxies/Shen+03_late.txt
--rw-r--r--   0 rpr        (502) staff       (20)     2884 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/examples/galaxies/lopez_sanjuan+17_B1.ecsv
--rw-r--r--   0 rpr        (502) staff       (20)     3880 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/examples/galaxies/plot_photometry.py
--rw-r--r--   0 rpr        (502) staff       (20)     4641 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/examples/galaxies/plot_schechter.py
--rw-r--r--   0 rpr        (502) staff       (20)     4310 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/examples/galaxies/plot_size.py
--rw-r--r--   0 rpr        (502) staff       (20)     3018 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/examples/galaxies/sdss_dered_10deg2.ecsv
--rw-r--r--   0 rpr        (502) staff       (20)     2330 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/examples/galaxies/sdss_photometry.yml
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.641913 skypy-0.5.2rc1/licenses/
--rw-r--r--   0 rpr        (502) staff       (20)     1658 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 rpr        (502) staff       (20)     1476 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/licenses/kcorrect.rst
--rw-r--r--   0 rpr        (502) staff       (20)      134 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/pyproject.toml
--rw-r--r--   0 rpr        (502) staff       (20)     1560 2023-07-10 17:30:44.736137 skypy-0.5.2rc1/setup.cfg
--rwxr-xr-x   0 rpr        (502) staff       (20)     1954 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/setup.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.644044 skypy-0.5.2rc1/skypy/
--rw-r--r--   0 rpr        (502) staff       (20)      675 2023-03-26 13:50:26.000000 skypy-0.5.2rc1/skypy/__init__.py
--rw-r--r--   0 rpr        (502) staff       (20)     1799 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/_astropy_init.py
--rw-r--r--   0 rpr        (502) staff       (20)     1957 2023-07-10 17:24:23.000000 skypy-0.5.2rc1/skypy/conftest.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.647416 skypy-0.5.2rc1/skypy/data/
--rw-r--r--   0 rpr        (502) staff       (20)      245 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/data/README.rst
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.647806 skypy-0.5.2rc1/skypy/data/kcorrect/
--rw-r--r--   0 rpr        (502) staff       (20)  2183040 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/data/kcorrect/k_nmf_derived.default.fits
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.676394 skypy-0.5.2rc1/skypy/extern/
--rw-r--r--   0 rpr        (502) staff       (20)      220 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/extern/__init__.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.685122 skypy-0.5.2rc1/skypy/galaxies/
--rw-r--r--   0 rpr        (502) staff       (20)      437 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/galaxies/__init__.py
--rw-r--r--   0 rpr        (502) staff       (20)     5585 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/galaxies/_schechter.py
--rw-r--r--   0 rpr        (502) staff       (20)     2100 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/galaxies/luminosity.py
--rw-r--r--   0 rpr        (502) staff       (20)    10410 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/galaxies/morphology.py
--rw-r--r--   0 rpr        (502) staff       (20)     9565 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/galaxies/redshift.py
--rw-r--r--   0 rpr        (502) staff       (20)     7947 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/galaxies/spectrum.py
--rw-r--r--   0 rpr        (502) staff       (20)     2167 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/galaxies/stellar_mass.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.688719 skypy-0.5.2rc1/skypy/galaxies/tests/
--rw-r--r--   0 rpr        (502) staff       (20)        0 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/galaxies/tests/__init__.py
--rw-r--r--   0 rpr        (502) staff       (20)      312 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/galaxies/tests/test_import.py
--rw-r--r--   0 rpr        (502) staff       (20)     1764 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/galaxies/tests/test_luminosity.py
--rw-r--r--   0 rpr        (502) staff       (20)     8238 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/galaxies/tests/test_morphology.py
--rw-r--r--   0 rpr        (502) staff       (20)     5692 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/galaxies/tests/test_redshift.py
--rw-r--r--   0 rpr        (502) staff       (20)     2058 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/galaxies/tests/test_schechter.py
--rw-r--r--   0 rpr        (502) staff       (20)     7104 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/galaxies/tests/test_spectrum.py
--rw-r--r--   0 rpr        (502) staff       (20)     2308 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/galaxies/tests/test_stellar_mass.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.690337 skypy-0.5.2rc1/skypy/pipeline/
--rw-r--r--   0 rpr        (502) staff       (20)      234 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/__init__.py
--rw-r--r--   0 rpr        (502) staff       (20)     3352 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/_config.py
--rw-r--r--   0 rpr        (502) staff       (20)     2790 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/_items.py
--rw-r--r--   0 rpr        (502) staff       (20)    10997 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/_pipeline.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.691258 skypy-0.5.2rc1/skypy/pipeline/scripts/
--rw-r--r--   0 rpr        (502) staff       (20)      167 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/scripts/__init__.py
--rw-r--r--   0 rpr        (502) staff       (20)     1838 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/pipeline/scripts/skypy.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.694151 skypy-0.5.2rc1/skypy/pipeline/tests/
--rw-r--r--   0 rpr        (502) staff       (20)        0 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/__init__.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.698505 skypy-0.5.2rc1/skypy/pipeline/tests/data/
--rw-r--r--   0 rpr        (502) staff       (20)       27 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/bad_function.yml
--rw-r--r--   0 rpr        (502) staff       (20)       25 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/bad_module.yml
--rw-r--r--   0 rpr        (502) staff       (20)       52 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/bad_object.yml
--rw-r--r--   0 rpr        (502) staff       (20)        0 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/empty_config.yml
--rw-r--r--   0 rpr        (502) staff       (20)       13 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/numeric_key.yml
--rw-r--r--   0 rpr        (502) staff       (20)       78 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/numeric_kwarg.yml
--rw-r--r--   0 rpr        (502) staff       (20)       72 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/numeric_nested_key.yml
--rw-r--r--   0 rpr        (502) staff       (20)       40 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/quantities.yml
--rw-r--r--   0 rpr        (502) staff       (20)      657 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/test_config.yml
--rw-r--r--   0 rpr        (502) staff       (20)       10 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/data/test_empty_ref.yml
--rw-r--r--   0 rpr        (502) staff       (20)     2275 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/tests/test_config.py
--rw-r--r--   0 rpr        (502) staff       (20)       59 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/test_import.py
--rw-r--r--   0 rpr        (502) staff       (20)     2249 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/pipeline/tests/test_items.py
--rw-r--r--   0 rpr        (502) staff       (20)    11036 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/pipeline/tests/test_pipeline.py
--rw-r--r--   0 rpr        (502) staff       (20)     4042 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/pipeline/tests/test_skypy.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.699586 skypy-0.5.2rc1/skypy/tests/
--rw-r--r--   0 rpr        (502) staff       (20)      108 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/tests/__init__.py
--rw-r--r--   0 rpr        (502) staff       (20)       50 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/tests/test_import.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.701775 skypy-0.5.2rc1/skypy/utils/
--rw-r--r--   0 rpr        (502) staff       (20)      308 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/utils/__init__.py
--rw-r--r--   0 rpr        (502) staff       (20)     2366 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/utils/_decorators.py
--rw-r--r--   0 rpr        (502) staff       (20)    10823 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/utils/photometry.py
--rw-r--r--   0 rpr        (502) staff       (20)     3754 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/utils/random.py
--rw-r--r--   0 rpr        (502) staff       (20)     2638 2023-01-28 13:58:15.000000 skypy-0.5.2rc1/skypy/utils/special.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.705454 skypy-0.5.2rc1/skypy/utils/tests/
--rw-r--r--   0 rpr        (502) staff       (20)        0 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/utils/tests/__init__.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.706233 skypy-0.5.2rc1/skypy/utils/tests/data/
--rw-r--r--   0 rpr        (502) staff       (20)    11841 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/utils/tests/data/gammaincc.txt
--rw-r--r--   0 rpr        (502) staff       (20)     1367 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/utils/tests/test_decorators.py
--rw-r--r--   0 rpr        (502) staff       (20)      145 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/utils/tests/test_import.py
--rw-r--r--   0 rpr        (502) staff       (20)     6739 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/skypy/utils/tests/test_photometry.py
--rw-r--r--   0 rpr        (502) staff       (20)     2756 2022-05-19 08:12:48.000000 skypy-0.5.2rc1/skypy/utils/tests/test_random.py
--rw-r--r--   0 rpr        (502) staff       (20)     3158 2023-06-28 15:34:39.000000 skypy-0.5.2rc1/skypy/utils/tests/test_special.py
--rw-r--r--   0 rpr        (502) staff       (20)      340 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy/version.py
-drwxr-xr-x   0 rpr        (502) staff       (20)        0 2023-07-10 17:30:44.646838 skypy-0.5.2rc1/skypy.egg-info/
--rw-r--r--   0 rpr        (502) staff       (20)     4667 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy.egg-info/PKG-INFO
--rw-r--r--   0 rpr        (502) staff       (20)     3467 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy.egg-info/SOURCES.txt
--rw-r--r--   0 rpr        (502) staff       (20)        1 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy.egg-info/dependency_links.txt
--rw-r--r--   0 rpr        (502) staff       (20)       61 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy.egg-info/entry_points.txt
--rw-r--r--   0 rpr        (502) staff       (20)        1 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy.egg-info/not-zip-safe
--rw-r--r--   0 rpr        (502) staff       (20)      174 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy.egg-info/requires.txt
--rw-r--r--   0 rpr        (502) staff       (20)        6 2023-07-10 17:30:44.000000 skypy-0.5.2rc1/skypy.egg-info/top_level.txt
--rw-r--r--   0 rpr        (502) staff       (20)     3784 2023-07-10 17:26:01.000000 skypy-0.5.2rc1/tox.ini
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.973173 skypy-0.5rc1/
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.795431 skypy-0.5rc1/.github/
+-rw-r--r--   0 rpr        (502) staff       (20)      131 2021-09-06 08:23:36.000000 skypy-0.5rc1/.github/CODEOWNERS
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.798474 skypy-0.5rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 rpr        (502) staff       (20)      555 2021-09-06 08:23:36.000000 skypy-0.5rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 rpr        (502) staff       (20)      176 2021-09-06 08:23:36.000000 skypy-0.5rc1/.github/ISSUE_TEMPLATE/new-model-proposal.md
+-rw-r--r--   0 rpr        (502) staff       (20)      344 2021-09-18 16:47:59.000000 skypy-0.5rc1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.804426 skypy-0.5rc1/.github/workflows/
+-rw-r--r--   0 rpr        (502) staff       (20)      487 2021-09-18 16:47:59.000000 skypy-0.5rc1/.github/workflows/codestyle.yaml
+-rw-r--r--   0 rpr        (502) staff       (20)     1033 2021-10-26 08:02:14.000000 skypy-0.5rc1/.github/workflows/compatibility.yaml
+-rw-r--r--   0 rpr        (502) staff       (20)     1434 2021-09-18 16:47:59.000000 skypy-0.5rc1/.github/workflows/tests.yaml
+-rw-r--r--   0 rpr        (502) staff       (20)      739 2021-09-06 08:23:36.000000 skypy-0.5rc1/.gitignore
+-rw-r--r--   0 rpr        (502) staff       (20)      749 2021-09-18 16:47:59.000000 skypy-0.5rc1/.mailmap
+-rw-r--r--   0 rpr        (502) staff       (20)      189 2021-10-26 12:08:16.000000 skypy-0.5rc1/.readthedocs.yml
+-rw-r--r--   0 rpr        (502) staff       (20)     4347 2021-09-18 16:47:59.000000 skypy-0.5rc1/.zenodo.json
+-rw-r--r--   0 rpr        (502) staff       (20)     1078 2021-11-02 14:35:05.000000 skypy-0.5rc1/CITATION.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     9536 2021-09-18 16:47:59.000000 skypy-0.5rc1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     8325 2021-09-18 16:47:59.000000 skypy-0.5rc1/CONTRIBUTING.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     1477 2021-09-06 08:23:36.000000 skypy-0.5rc1/LICENSE.rst
+-rw-r--r--   0 rpr        (502) staff       (20)      295 2021-09-06 08:23:36.000000 skypy-0.5rc1/MANIFEST.in
+-rw-r--r--   0 rpr        (502) staff       (20)     4665 2021-11-02 14:41:21.973487 skypy-0.5rc1/PKG-INFO
+-rw-r--r--   0 rpr        (502) staff       (20)     4293 2021-09-18 16:47:59.000000 skypy-0.5rc1/README.rst
+-rw-r--r--   0 rpr        (502) staff       (20)       53 2021-09-06 08:23:36.000000 skypy-0.5rc1/codecov.yml
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.811807 skypy-0.5rc1/docs/
+-rw-r--r--   0 rpr        (502) staff       (20)     4703 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/Makefile
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.816995 skypy-0.5rc1/docs/_static/
+-rw-r--r--   0 rpr        (502) staff       (20)      294 2021-09-17 12:48:33.000000 skypy-0.5rc1/docs/_static/skypy.css
+-rw-r--r--   0 rpr        (502) staff       (20)     4286 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/_static/skypy_image.ico
+-rw-r--r--   0 rpr        (502) staff       (20)    19630 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/_static/skypy_image.png
+-rw-r--r--   0 rpr        (502) staff       (20)    27005 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/_static/skypy_image.svg
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.825962 skypy-0.5rc1/docs/arch/
+-rw-r--r--   0 rpr        (502) staff       (20)     5773 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/arch/adr-01.md
+-rw-r--r--   0 rpr        (502) staff       (20)      677 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/arch/adr-02.md
+-rw-r--r--   0 rpr        (502) staff       (20)     3545 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/arch/adr-03.md
+-rw-r--r--   0 rpr        (502) staff       (20)     9043 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/conf.py
+-rw-r--r--   0 rpr        (502) staff       (20)    12727 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/configuration_files.rst
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.828548 skypy-0.5rc1/docs/developer/
+-rw-r--r--   0 rpr        (502) staff       (20)       36 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/developer/contributing.rst
+-rw-r--r--   0 rpr        (502) staff       (20)      886 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/feature_list.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     2309 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/galaxies.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     1410 2021-11-02 14:35:05.000000 skypy-0.5rc1/docs/index.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     2797 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/install.rst
+-rw-r--r--   0 rpr        (502) staff       (20)      474 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/luminosity.yml
+-rw-r--r--   0 rpr        (502) staff       (20)     4549 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/make.bat
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.829154 skypy-0.5rc1/docs/pipeline/
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.830825 skypy-0.5rc1/docs/pipeline/examples/
+-rw-r--r--   0 rpr        (502) staff       (20)      301 2021-09-08 12:55:22.000000 skypy-0.5rc1/docs/pipeline/examples/config.yml
+-rw-r--r--   0 rpr        (502) staff       (20)      151 2021-09-06 08:23:36.000000 skypy-0.5rc1/docs/pipeline/examples/pipeline.yml
+-rw-r--r--   0 rpr        (502) staff       (20)     4063 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/pipeline/index.rst
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.831951 skypy-0.5rc1/docs/project/
+-rw-r--r--   0 rpr        (502) staff       (20)       32 2021-11-02 14:35:05.000000 skypy-0.5rc1/docs/project/citation.rst
+-rw-r--r--   0 rpr        (502) staff       (20)       39 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/project/code_of_conduct.rst
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.832687 skypy-0.5rc1/docs/utils/
+-rw-r--r--   0 rpr        (502) staff       (20)     4500 2021-09-18 16:47:59.000000 skypy-0.5rc1/docs/utils/index.rst
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.833255 skypy-0.5rc1/examples/
+-rw-r--r--   0 rpr        (502) staff       (20)      335 2021-09-06 08:23:36.000000 skypy-0.5rc1/examples/README.rst
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.864663 skypy-0.5rc1/examples/galaxies/
+-rw-r--r--   0 rpr        (502) staff       (20)      122 2021-09-06 08:23:36.000000 skypy-0.5rc1/examples/galaxies/README.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     1111 2021-09-06 08:23:36.000000 skypy-0.5rc1/examples/galaxies/Shen+03_early.txt
+-rw-r--r--   0 rpr        (502) staff       (20)     1616 2021-09-06 08:23:36.000000 skypy-0.5rc1/examples/galaxies/Shen+03_late.txt
+-rw-r--r--   0 rpr        (502) staff       (20)     2884 2021-09-06 08:23:36.000000 skypy-0.5rc1/examples/galaxies/lopez_sanjuan+17_B1.ecsv
+-rw-r--r--   0 rpr        (502) staff       (20)     3880 2021-09-18 16:47:59.000000 skypy-0.5rc1/examples/galaxies/plot_photometry.py
+-rw-r--r--   0 rpr        (502) staff       (20)     4641 2021-10-26 11:21:02.000000 skypy-0.5rc1/examples/galaxies/plot_schechter.py
+-rw-r--r--   0 rpr        (502) staff       (20)     4310 2021-09-18 16:47:59.000000 skypy-0.5rc1/examples/galaxies/plot_size.py
+-rw-r--r--   0 rpr        (502) staff       (20)     3018 2021-09-18 15:48:46.000000 skypy-0.5rc1/examples/galaxies/sdss_dered_10deg2.ecsv
+-rw-r--r--   0 rpr        (502) staff       (20)     2330 2021-11-02 14:33:17.000000 skypy-0.5rc1/examples/galaxies/sdss_photometry.yml
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.867101 skypy-0.5rc1/licenses/
+-rw-r--r--   0 rpr        (502) staff       (20)     1658 2021-09-06 08:23:36.000000 skypy-0.5rc1/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 rpr        (502) staff       (20)     1476 2021-09-06 08:23:36.000000 skypy-0.5rc1/licenses/kcorrect.rst
+-rw-r--r--   0 rpr        (502) staff       (20)      134 2021-09-07 13:13:28.000000 skypy-0.5rc1/pyproject.toml
+-rw-r--r--   0 rpr        (502) staff       (20)     1560 2021-11-02 14:41:21.975605 skypy-0.5rc1/setup.cfg
+-rwxr-xr-x   0 rpr        (502) staff       (20)     1954 2021-09-06 08:23:36.000000 skypy-0.5rc1/setup.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.870912 skypy-0.5rc1/skypy/
+-rw-r--r--   0 rpr        (502) staff       (20)      675 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/__init__.py
+-rw-r--r--   0 rpr        (502) staff       (20)     1799 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/_astropy_init.py
+-rw-r--r--   0 rpr        (502) staff       (20)     1957 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/conftest.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.893511 skypy-0.5rc1/skypy/data/
+-rw-r--r--   0 rpr        (502) staff       (20)      245 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/data/README.rst
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.896395 skypy-0.5rc1/skypy/data/kcorrect/
+-rw-r--r--   0 rpr        (502) staff       (20)  2183040 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/data/kcorrect/k_nmf_derived.default.fits
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.906643 skypy-0.5rc1/skypy/extern/
+-rw-r--r--   0 rpr        (502) staff       (20)      220 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/extern/__init__.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.911609 skypy-0.5rc1/skypy/galaxies/
+-rw-r--r--   0 rpr        (502) staff       (20)      437 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/galaxies/__init__.py
+-rw-r--r--   0 rpr        (502) staff       (20)     5585 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/galaxies/_schechter.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2100 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/luminosity.py
+-rw-r--r--   0 rpr        (502) staff       (20)    10410 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/morphology.py
+-rw-r--r--   0 rpr        (502) staff       (20)     9565 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/redshift.py
+-rw-r--r--   0 rpr        (502) staff       (20)     7947 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/spectrum.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2167 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/stellar_mass.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.917551 skypy-0.5rc1/skypy/galaxies/tests/
+-rw-r--r--   0 rpr        (502) staff       (20)        0 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/galaxies/tests/__init__.py
+-rw-r--r--   0 rpr        (502) staff       (20)      312 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/tests/test_import.py
+-rw-r--r--   0 rpr        (502) staff       (20)     1764 2021-09-08 12:55:22.000000 skypy-0.5rc1/skypy/galaxies/tests/test_luminosity.py
+-rw-r--r--   0 rpr        (502) staff       (20)     8238 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/galaxies/tests/test_morphology.py
+-rw-r--r--   0 rpr        (502) staff       (20)     5692 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/tests/test_redshift.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2058 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/tests/test_schechter.py
+-rw-r--r--   0 rpr        (502) staff       (20)     7104 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/galaxies/tests/test_spectrum.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2308 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/galaxies/tests/test_stellar_mass.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.921592 skypy-0.5rc1/skypy/pipeline/
+-rw-r--r--   0 rpr        (502) staff       (20)      234 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/__init__.py
+-rw-r--r--   0 rpr        (502) staff       (20)     3352 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/_config.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2790 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/_items.py
+-rw-r--r--   0 rpr        (502) staff       (20)    10997 2021-10-26 08:02:14.000000 skypy-0.5rc1/skypy/pipeline/_pipeline.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.922685 skypy-0.5rc1/skypy/pipeline/scripts/
+-rw-r--r--   0 rpr        (502) staff       (20)      167 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/scripts/__init__.py
+-rw-r--r--   0 rpr        (502) staff       (20)     1838 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/scripts/skypy.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.929585 skypy-0.5rc1/skypy/pipeline/tests/
+-rw-r--r--   0 rpr        (502) staff       (20)        0 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/__init__.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.939621 skypy-0.5rc1/skypy/pipeline/tests/data/
+-rw-r--r--   0 rpr        (502) staff       (20)       27 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/bad_function.yml
+-rw-r--r--   0 rpr        (502) staff       (20)       25 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/bad_module.yml
+-rw-r--r--   0 rpr        (502) staff       (20)       52 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/tests/data/bad_object.yml
+-rw-r--r--   0 rpr        (502) staff       (20)        0 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/empty_config.yml
+-rw-r--r--   0 rpr        (502) staff       (20)       13 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/numeric_key.yml
+-rw-r--r--   0 rpr        (502) staff       (20)       78 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/numeric_kwarg.yml
+-rw-r--r--   0 rpr        (502) staff       (20)       72 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/numeric_nested_key.yml
+-rw-r--r--   0 rpr        (502) staff       (20)       40 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/quantities.yml
+-rw-r--r--   0 rpr        (502) staff       (20)      657 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/tests/data/test_config.yml
+-rw-r--r--   0 rpr        (502) staff       (20)       10 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/data/test_empty_ref.yml
+-rw-r--r--   0 rpr        (502) staff       (20)     2275 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/tests/test_config.py
+-rw-r--r--   0 rpr        (502) staff       (20)       59 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/pipeline/tests/test_import.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2249 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/pipeline/tests/test_items.py
+-rw-r--r--   0 rpr        (502) staff       (20)    11036 2021-10-26 08:02:14.000000 skypy-0.5rc1/skypy/pipeline/tests/test_pipeline.py
+-rw-r--r--   0 rpr        (502) staff       (20)     4042 2021-11-02 14:35:05.000000 skypy-0.5rc1/skypy/pipeline/tests/test_skypy.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.943899 skypy-0.5rc1/skypy/tests/
+-rw-r--r--   0 rpr        (502) staff       (20)      108 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/tests/__init__.py
+-rw-r--r--   0 rpr        (502) staff       (20)       50 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/tests/test_import.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.947134 skypy-0.5rc1/skypy/utils/
+-rw-r--r--   0 rpr        (502) staff       (20)      308 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/utils/__init__.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2366 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/utils/_decorators.py
+-rw-r--r--   0 rpr        (502) staff       (20)    10823 2021-09-18 15:45:30.000000 skypy-0.5rc1/skypy/utils/photometry.py
+-rw-r--r--   0 rpr        (502) staff       (20)     3754 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/utils/random.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2638 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/utils/special.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.968732 skypy-0.5rc1/skypy/utils/tests/
+-rw-r--r--   0 rpr        (502) staff       (20)        0 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/utils/tests/__init__.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.969491 skypy-0.5rc1/skypy/utils/tests/data/
+-rw-r--r--   0 rpr        (502) staff       (20)    11841 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/utils/tests/data/gammaincc.txt
+-rw-r--r--   0 rpr        (502) staff       (20)     1367 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/utils/tests/test_decorators.py
+-rw-r--r--   0 rpr        (502) staff       (20)      145 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/utils/tests/test_import.py
+-rw-r--r--   0 rpr        (502) staff       (20)     6739 2021-09-18 16:47:59.000000 skypy-0.5rc1/skypy/utils/tests/test_photometry.py
+-rw-r--r--   0 rpr        (502) staff       (20)     2756 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/utils/tests/test_random.py
+-rw-r--r--   0 rpr        (502) staff       (20)     3144 2021-09-06 08:23:36.000000 skypy-0.5rc1/skypy/utils/tests/test_special.py
+-rw-r--r--   0 rpr        (502) staff       (20)      338 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy/version.py
+drwxr-xr-x   0 rpr        (502) staff       (20)        0 2021-11-02 14:41:21.892133 skypy-0.5rc1/skypy.egg-info/
+-rw-r--r--   0 rpr        (502) staff       (20)     4665 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy.egg-info/PKG-INFO
+-rw-r--r--   0 rpr        (502) staff       (20)     3467 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy.egg-info/SOURCES.txt
+-rw-r--r--   0 rpr        (502) staff       (20)        1 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy.egg-info/dependency_links.txt
+-rw-r--r--   0 rpr        (502) staff       (20)       61 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy.egg-info/entry_points.txt
+-rw-r--r--   0 rpr        (502) staff       (20)        1 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy.egg-info/not-zip-safe
+-rw-r--r--   0 rpr        (502) staff       (20)      174 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy.egg-info/requires.txt
+-rw-r--r--   0 rpr        (502) staff       (20)        6 2021-11-02 14:41:21.000000 skypy-0.5rc1/skypy.egg-info/top_level.txt
+-rw-r--r--   0 rpr        (502) staff       (20)     3517 2021-10-26 08:02:14.000000 skypy-0.5rc1/tox.ini
```

### Comparing `skypy-0.5.2rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `skypy-0.5rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/.github/workflows/compatibility.yaml` & `skypy-0.5rc1/.github/workflows/compatibility.yaml`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/.github/workflows/tests.yaml` & `skypy-0.5rc1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/.gitignore` & `skypy-0.5rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/.mailmap` & `skypy-0.5rc1/.mailmap`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/.zenodo.json` & `skypy-0.5rc1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/CITATION.rst` & `skypy-0.5rc1/CITATION.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/CODE_OF_CONDUCT.rst` & `skypy-0.5rc1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/CONTRIBUTING.rst` & `skypy-0.5rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/LICENSE.rst` & `skypy-0.5rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/PKG-INFO` & `skypy-0.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypy
-Version: 0.5.2rc1
+Version: 0.5rc1
 Summary: A package for modelling the Universe.
 Home-page: http://skypy.info
 Author: SkyPy Team
 Author-email: adam.amara@port.ac.uk
 License: BSD 3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `skypy-0.5.2rc1/README.rst` & `skypy-0.5rc1/README.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/Makefile` & `skypy-0.5rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/_static/skypy_image.ico` & `skypy-0.5rc1/docs/_static/skypy_image.ico`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/_static/skypy_image.png` & `skypy-0.5rc1/docs/_static/skypy_image.png`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/_static/skypy_image.svg` & `skypy-0.5rc1/docs/_static/skypy_image.svg`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/arch/adr-01.md` & `skypy-0.5rc1/docs/arch/adr-01.md`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/arch/adr-02.md` & `skypy-0.5rc1/docs/arch/adr-02.md`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/arch/adr-03.md` & `skypy-0.5rc1/docs/arch/adr-03.md`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/conf.py` & `skypy-0.5rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/configuration_files.rst` & `skypy-0.5rc1/docs/configuration_files.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/feature_list.rst` & `skypy-0.5rc1/docs/feature_list.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/galaxies.rst` & `skypy-0.5rc1/docs/galaxies.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/index.rst` & `skypy-0.5rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/install.rst` & `skypy-0.5rc1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/make.bat` & `skypy-0.5rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/pipeline/index.rst` & `skypy-0.5rc1/docs/pipeline/index.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/docs/utils/index.rst` & `skypy-0.5rc1/docs/utils/index.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/Shen+03_early.txt` & `skypy-0.5rc1/examples/galaxies/Shen+03_early.txt`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/Shen+03_late.txt` & `skypy-0.5rc1/examples/galaxies/Shen+03_late.txt`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/lopez_sanjuan+17_B1.ecsv` & `skypy-0.5rc1/examples/galaxies/lopez_sanjuan+17_B1.ecsv`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/plot_photometry.py` & `skypy-0.5rc1/examples/galaxies/plot_photometry.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/plot_schechter.py` & `skypy-0.5rc1/examples/galaxies/plot_schechter.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/plot_size.py` & `skypy-0.5rc1/examples/galaxies/plot_size.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/sdss_dered_10deg2.ecsv` & `skypy-0.5rc1/examples/galaxies/sdss_dered_10deg2.ecsv`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/examples/galaxies/sdss_photometry.yml` & `skypy-0.5rc1/examples/galaxies/sdss_photometry.yml`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/licenses/TEMPLATE_LICENCE.rst` & `skypy-0.5rc1/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/licenses/kcorrect.rst` & `skypy-0.5rc1/licenses/kcorrect.rst`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/setup.cfg` & `skypy-0.5rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/setup.py` & `skypy-0.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/__init__.py` & `skypy-0.5rc1/skypy/__init__.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/_astropy_init.py` & `skypy-0.5rc1/skypy/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/conftest.py` & `skypy-0.5rc1/skypy/conftest.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/data/kcorrect/k_nmf_derived.default.fits` & `skypy-0.5rc1/skypy/data/kcorrect/k_nmf_derived.default.fits`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/_schechter.py` & `skypy-0.5rc1/skypy/galaxies/_schechter.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/luminosity.py` & `skypy-0.5rc1/skypy/galaxies/luminosity.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/morphology.py` & `skypy-0.5rc1/skypy/galaxies/morphology.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/redshift.py` & `skypy-0.5rc1/skypy/galaxies/redshift.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/spectrum.py` & `skypy-0.5rc1/skypy/galaxies/spectrum.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/stellar_mass.py` & `skypy-0.5rc1/skypy/galaxies/stellar_mass.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/tests/test_luminosity.py` & `skypy-0.5rc1/skypy/galaxies/tests/test_luminosity.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/tests/test_morphology.py` & `skypy-0.5rc1/skypy/galaxies/tests/test_morphology.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/tests/test_redshift.py` & `skypy-0.5rc1/skypy/galaxies/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/tests/test_schechter.py` & `skypy-0.5rc1/skypy/galaxies/tests/test_schechter.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/tests/test_spectrum.py` & `skypy-0.5rc1/skypy/galaxies/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/galaxies/tests/test_stellar_mass.py` & `skypy-0.5rc1/skypy/galaxies/tests/test_stellar_mass.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/_config.py` & `skypy-0.5rc1/skypy/pipeline/_config.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/_items.py` & `skypy-0.5rc1/skypy/pipeline/_items.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/_pipeline.py` & `skypy-0.5rc1/skypy/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/scripts/skypy.py` & `skypy-0.5rc1/skypy/pipeline/scripts/skypy.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/tests/data/test_config.yml` & `skypy-0.5rc1/skypy/pipeline/tests/data/test_config.yml`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/tests/test_config.py` & `skypy-0.5rc1/skypy/pipeline/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/tests/test_items.py` & `skypy-0.5rc1/skypy/pipeline/tests/test_items.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/tests/test_pipeline.py` & `skypy-0.5rc1/skypy/pipeline/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/pipeline/tests/test_skypy.py` & `skypy-0.5rc1/skypy/pipeline/tests/test_skypy.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/_decorators.py` & `skypy-0.5rc1/skypy/utils/_decorators.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/photometry.py` & `skypy-0.5rc1/skypy/utils/photometry.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/random.py` & `skypy-0.5rc1/skypy/utils/random.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/special.py` & `skypy-0.5rc1/skypy/utils/special.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/tests/data/gammaincc.txt` & `skypy-0.5rc1/skypy/utils/tests/data/gammaincc.txt`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/tests/test_decorators.py` & `skypy-0.5rc1/skypy/utils/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/tests/test_photometry.py` & `skypy-0.5rc1/skypy/utils/tests/test_photometry.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/tests/test_random.py` & `skypy-0.5rc1/skypy/utils/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/skypy/utils/tests/test_special.py` & `skypy-0.5rc1/skypy/utils/tests/test_special.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import numpy.testing as npt
 from astropy.utils.data import get_pkg_data_filename
-import pytest
+from astropy.tests.helper import raises
 
 from skypy.utils.special import gammaincc
 
 
 def test_gammaincc_scalar():
     # test with scalar input and expect scalar output
     npt.assert_allclose(gammaincc(1.2, 1.5), 0.28893139222051745)
@@ -76,17 +76,17 @@
         for numbers in zip(a[fail], x[fail], g[fail], v[fail]):
             lines.append('gammaincc(%g, %g) = %g != %g)' % numbers)
 
     # now do the assertion
     npt.assert_allclose(g, v, rtol=1e-10, atol=0, err_msg='\n'.join(lines))
 
 
+@raises(ValueError)
 def test_gammaincc_neg_x_scalar():
     # negative x raises an exception
-    with pytest.raises(ValueError):
-        gammaincc(0.5, -1.0)
+    gammaincc(0.5, -1.0)
 
 
+@raises(ValueError)
 def test_gammaincc_neg_x_array():
     # negative x in array raises an exception
-    with pytest.raises(ValueError):
-        gammaincc(0.5, [3.0, 2.0, 1.0, 0.0, -1.0])
+    gammaincc(0.5, [3.0, 2.0, 1.0, 0.0, -1.0])
```

### Comparing `skypy-0.5.2rc1/skypy.egg-info/PKG-INFO` & `skypy-0.5rc1/skypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypy
-Version: 0.5.2rc1
+Version: 0.5rc1
 Summary: A package for modelling the Universe.
 Home-page: http://skypy.info
 Author: SkyPy Team
 Author-email: adam.amara@port.ac.uk
 License: BSD 3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `skypy-0.5.2rc1/skypy.egg-info/SOURCES.txt` & `skypy-0.5rc1/skypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypy-0.5.2rc1/tox.ini` & `skypy-0.5rc1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,21 @@
     build_docs
     linkcheck
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
 isolated_build = true
+indexserver =
+    NIGHTLY = https://pypi.anaconda.org/scipy-wheels-nightly/simple
 
 [testenv]
 
 # Pass through the following environment variables which may be needed for the CI
-passenv = HOME,WINDIR,LC_ALL,LC_CTYPE,CC,CI,TRAVIS
+passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI TRAVIS
 
 # Run the tests in a temporary directory to make sure that we don't import
 # this package from the source tree
 changedir = .tmp/{envname}
 
 # tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
@@ -71,16 +73,16 @@
     scipy17: scipy==1.7.*
 
     astropy40: astropy==4.0.*
     astropy41: astropy==4.1.*
     astropy42: astropy==4.2.*
     astropy43: astropy==4.3.*
 
-    dev: numpy
-    dev: scipy
+    dev: :NIGHTLY:numpy
+    dev: :NIGHTLY:scipy
     dev: git+https://github.com/astropy/astropy.git#egg=astropy
 
     latest: astropy==4.3.*
     latest: numpy==1.21.*
     latest: scipy==1.7.*
 
     oldest: astropy==4.0.*
@@ -97,21 +99,14 @@
     dev: True
 
 commands =
     pip freeze
     !cov: pytest --pyargs skypy {toxinidir}/docs {posargs}
     cov: pytest --pyargs skypy {toxinidir}/docs --cov skypy --cov-config={toxinidir}/setup.cfg {posargs}
 
-# For dev environment, use scipy-nightly-wheels as the default index server (for numpy and scipy)
-# and PyPI as the extra index server (for all other dependencies, except astropy which is installed
-# directly from GitHub).
-setenv =
-    dev: PIP_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
-    dev: PIP_EXTRA_INDEX_URL = https://pypi.org/simple
-
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
     sphinx-build -W -b html . _build/html
```


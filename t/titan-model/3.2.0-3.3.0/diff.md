# Comparing `tmp/titan-model-3.2.0.tar.gz` & `tmp/titan_model-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-model-3.2.0.tar", max compression
+gzip compressed data, was "titan_model-3.3.0.tar", max compression
```

## Comparing `titan-model-3.2.0.tar` & `titan_model-3.3.0.tar`

### file list

```diff
@@ -1,93 +1,104 @@
--rw-r--r--   0        0        0    35149 2022-09-12 14:17:29.124214 titan-model-3.2.0/LICENSE
--rw-r--r--   0        0        0     3274 2022-09-12 14:17:29.124214 titan-model-3.2.0/README.md
--rw-r--r--   0        0        0     1284 2022-09-12 14:17:29.128216 titan-model-3.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/__init__.py
--rw-r--r--   0        0        0    14466 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/agent.py
--rw-r--r--   0        0        0     1963 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/distributions.py
--rw-r--r--   0        0        0      128 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/exposures/__init__.py
--rw-r--r--   0        0        0     4924 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/exposures/base_exposure.py
--rw-r--r--   0        0        0    12381 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/exposures/hiv.py
--rw-r--r--   0        0        0     6781 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/exposures/knowledge.py
--rw-r--r--   0        0        0    11055 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/exposures/monkeypox.py
--rw-r--r--   0        0        0      300 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/__init__.py
--rw-r--r--   0        0        0     5792 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/base_feature.py
--rw-r--r--   0        0        0     1720 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/external_exposure.py
--rw-r--r--   0        0        0     9094 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/haart.py
--rw-r--r--   0        0        0     7095 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/high_risk.py
--rw-r--r--   0        0        0     5735 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/incar.py
--rw-r--r--   0        0        0     2262 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/partner_tracing.py
--rw-r--r--   0        0        0    12127 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/prep.py
--rw-r--r--   0        0        0     7116 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/random_trial.py
--rw-r--r--   0        0        0     3181 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/syringe_services.py
--rw-r--r--   0        0        0     4306 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/features/vaccine.py
--rw-r--r--   0        0        0      117 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/interactions/__init__.py
--rw-r--r--   0        0        0      854 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/interactions/base_interaction.py
--rw-r--r--   0        0        0     2089 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/interactions/injection.py
--rw-r--r--   0        0        0     1033 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/interactions/pca.py
--rw-r--r--   0        0        0     1603 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/interactions/sex.py
--rw-r--r--   0        0        0     7935 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/location.py
--rw-r--r--   0        0        0    17889 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/model.py
--rw-r--r--   0        0        0    11481 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/output.py
--rw-r--r--   0        0        0      761 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/params/agent_zero.yml
--rw-r--r--   0        0        0     1659 2022-09-12 14:17:29.128216 titan-model-3.2.0/titan/params/assort_mix.yml
--rw-r--r--   0        0        0     1835 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/calibration.yml
--rw-r--r--   0        0        0     4463 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/classes.yml
--rw-r--r--   0        0        0    14814 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/demographics.yml
--rw-r--r--   0        0        0      328 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/enter_exit.yml
--rw-r--r--   0        0        0      376 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/exposures.yml
--rw-r--r--   0        0        0      629 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/external_exposure.yml
--rw-r--r--   0        0        0     1891 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/features.yml
--rw-r--r--   0        0        0      778 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/haart.yml
--rw-r--r--   0        0        0      732 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/high_risk.yml
--rw-r--r--   0        0        0     1156 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/hiv.yml
--rw-r--r--   0        0        0      817 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/incar.yml
--rw-r--r--   0        0        0     1447 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/knowledge.yml
--rw-r--r--   0        0        0     3720 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/location.yml
--rw-r--r--   0        0        0     2041 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/model.yml
--rw-r--r--   0        0        0      776 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/monkeypox.yml
--rw-r--r--   0        0        0     1780 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/outputs.yml
--rw-r--r--   0        0        0     1011 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/partner_tracing.yml
--rw-r--r--   0        0        0     7651 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/partnership.yml
--rw-r--r--   0        0        0     1733 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/prep.yml
--rw-r--r--   0        0        0      694 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/random_trial.yml
--rw-r--r--   0        0        0      961 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/syringe_services.yml
--rw-r--r--   0        0        0     1103 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/timeline_scaling.yml
--rw-r--r--   0        0        0      647 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/params/vaccine.yml
--rw-r--r--   0        0        0     4746 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/parse_params.py
--rw-r--r--   0        0        0     9895 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/partnering.py
--rw-r--r--   0        0        0    18930 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/population.py
--rw-r--r--   0        0        0     7869 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/population_io.py
--rw-r--r--   0        0        0     1374 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/probabilities.py
--rwxr-xr-x   0        0        0    13305 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/run_titan.py
--rw-r--r--   0        0        0      647 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/atlanta/assort_mix.yml
--rw-r--r--   0        0        0      126 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/atlanta/calibration.yml
--rw-r--r--   0        0        0     3041 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/atlanta/demographics.yml
--rw-r--r--   0        0        0     1278 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/atlanta/model.yml
--rw-r--r--   0        0        0      108 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/atlanta/outputs.yml
--rw-r--r--   0        0        0      864 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/atlanta/partnership.yml
--rw-r--r--   0        0        0     3056 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/chicago/chicago_baseCase.yml
--rw-r--r--   0        0        0     1551 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/mississippi/demographics.yml
--rw-r--r--   0        0        0     1524 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/mississippi/model.yml
--rw-r--r--   0        0        0     2969 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/missouri/demographics.yml
--rw-r--r--   0        0        0     1923 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/missouri/model.yml
--rw-r--r--   0        0        0      110 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/agent_zero.yml
--rw-r--r--   0        0        0      431 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/assort_mix.yml
--rw-r--r--   0        0        0      337 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/classes.yml
--rw-r--r--   0        0        0     3567 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/demographics.yml
--rw-r--r--   0        0        0       41 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/exposures.yml
--rw-r--r--   0        0        0      212 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/model.yml
--rw-r--r--   0        0        0      138 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/monkeypox.yml
--rw-r--r--   0        0        0     2334 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/partnership.yml
--rw-r--r--   0        0        0       90 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-monkeypox/vaccine.yml
--rw-r--r--   0        0        0     5899 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-msm/demographics.yml
--rw-r--r--   0        0        0      249 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-msm/hiv.yml
--rw-r--r--   0        0        0     2372 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-msm/location.yml
--rw-r--r--   0        0        0     1320 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-msm/model.yml
--rw-r--r--   0        0        0     2415 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/nyc-msm/partnership.yml
--rw-r--r--   0        0        0     2963 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/rhode-island/demographics.yml
--rw-r--r--   0        0        0     1960 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/rhode-island/model.yml
--rw-r--r--   0        0        0     2850 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/scott/demographics.yml
--rw-r--r--   0        0        0     4253 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/settings/scott/model.yml
--rw-r--r--   0        0        0    12852 2022-09-12 14:17:29.132218 titan-model-3.2.0/titan/utils.py
--rw-r--r--   0        0        0     4834 1970-01-01 00:00:00.000000 titan-model-3.2.0/setup.py
--rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 titan-model-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 15:41:15.932137 titan_model-3.3.0/LICENSE
+-rw-r--r--   0        0        0     3274 2023-07-10 15:41:15.932137 titan_model-3.3.0/README.md
+-rw-r--r--   0        0        0     1284 2023-07-10 15:41:15.932137 titan_model-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-10 15:41:15.932137 titan_model-3.3.0/titan/__init__.py
+-rw-r--r--   0        0        0    14466 2023-07-10 15:41:15.932137 titan_model-3.3.0/titan/agent.py
+-rw-r--r--   0        0        0     1963 2023-07-10 15:41:15.932137 titan_model-3.3.0/titan/distributions.py
+-rw-r--r--   0        0        0      128 2023-07-10 15:41:15.932137 titan_model-3.3.0/titan/exposures/__init__.py
+-rw-r--r--   0        0        0     4923 2023-07-10 15:41:15.932137 titan_model-3.3.0/titan/exposures/base_exposure.py
+-rw-r--r--   0        0        0    12380 2023-07-10 15:41:15.932137 titan_model-3.3.0/titan/exposures/hiv.py
+-rw-r--r--   0        0        0     6780 2023-07-10 15:41:15.932137 titan_model-3.3.0/titan/exposures/knowledge.py
+-rw-r--r--   0        0        0    11054 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/exposures/monkeypox.py
+-rw-r--r--   0        0        0      300 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/__init__.py
+-rw-r--r--   0        0        0     5792 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/base_feature.py
+-rw-r--r--   0        0        0     1719 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/external_exposure.py
+-rw-r--r--   0        0        0     9094 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/haart.py
+-rw-r--r--   0        0        0     7103 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/high_risk.py
+-rw-r--r--   0        0        0     5734 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/incar.py
+-rw-r--r--   0        0        0     2261 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/partner_tracing.py
+-rw-r--r--   0        0        0    12126 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/prep.py
+-rw-r--r--   0        0        0     7115 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/random_trial.py
+-rw-r--r--   0        0        0     3180 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/syringe_services.py
+-rw-r--r--   0        0        0     4305 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/features/vaccine.py
+-rw-r--r--   0        0        0      117 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/interactions/__init__.py
+-rw-r--r--   0        0        0      853 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/interactions/base_interaction.py
+-rw-r--r--   0        0        0     2088 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/interactions/injection.py
+-rw-r--r--   0        0        0     1032 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/interactions/pca.py
+-rw-r--r--   0        0        0     1602 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/interactions/sex.py
+-rw-r--r--   0        0        0     7934 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/location.py
+-rw-r--r--   0        0        0    18184 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/model.py
+-rw-r--r--   0        0        0    11479 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/output.py
+-rw-r--r--   0        0        0      761 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/agent_zero.yml
+-rw-r--r--   0        0        0     1659 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/assort_mix.yml
+-rw-r--r--   0        0        0     1835 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/calibration.yml
+-rw-r--r--   0        0        0     4463 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/classes.yml
+-rw-r--r--   0        0        0    14814 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/demographics.yml
+-rw-r--r--   0        0        0      328 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/enter_exit.yml
+-rw-r--r--   0        0        0      376 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/exposures.yml
+-rw-r--r--   0        0        0      629 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/external_exposure.yml
+-rw-r--r--   0        0        0     1891 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/features.yml
+-rw-r--r--   0        0        0      778 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/haart.yml
+-rw-r--r--   0        0        0      732 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/high_risk.yml
+-rw-r--r--   0        0        0     1156 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/hiv.yml
+-rw-r--r--   0        0        0      817 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/incar.yml
+-rw-r--r--   0        0        0     1447 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/knowledge.yml
+-rw-r--r--   0        0        0     3720 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/location.yml
+-rw-r--r--   0        0        0     2041 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/model.yml
+-rw-r--r--   0        0        0      776 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/monkeypox.yml
+-rw-r--r--   0        0        0     1780 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/outputs.yml
+-rw-r--r--   0        0        0     1011 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/partner_tracing.yml
+-rw-r--r--   0        0        0     7761 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/partnership.yml
+-rw-r--r--   0        0        0     1733 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/prep.yml
+-rw-r--r--   0        0        0      694 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/random_trial.yml
+-rw-r--r--   0        0        0      961 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/syringe_services.yml
+-rw-r--r--   0        0        0     1103 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/timeline_scaling.yml
+-rw-r--r--   0        0        0      647 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/params/vaccine.yml
+-rw-r--r--   0        0        0     4746 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/parse_params.py
+-rw-r--r--   0        0        0     9895 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/partnering.py
+-rw-r--r--   0        0        0    18929 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/population.py
+-rw-r--r--   0        0        0     7869 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/population_io.py
+-rw-r--r--   0        0        0     1374 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/probabilities.py
+-rwxr-xr-x   0        0        0    13305 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/run_titan.py
+-rw-r--r--   0        0        0      647 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/atlanta/assort_mix.yml
+-rw-r--r--   0        0        0      126 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/atlanta/calibration.yml
+-rw-r--r--   0        0        0     3041 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/atlanta/demographics.yml
+-rw-r--r--   0        0        0     1278 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/atlanta/model.yml
+-rw-r--r--   0        0        0      108 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/atlanta/outputs.yml
+-rw-r--r--   0        0        0      864 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/atlanta/partnership.yml
+-rw-r--r--   0        0        0     3056 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/chicago/chicago_baseCase.yml
+-rw-r--r--   0        0        0     1551 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/mississippi/demographics.yml
+-rw-r--r--   0        0        0     1524 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/mississippi/model.yml
+-rw-r--r--   0        0        0     2969 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/missouri/demographics.yml
+-rw-r--r--   0        0        0     1923 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/missouri/model.yml
+-rw-r--r--   0        0        0      110 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/agent_zero.yml
+-rw-r--r--   0        0        0      431 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/assort_mix.yml
+-rw-r--r--   0        0        0      337 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/classes.yml
+-rw-r--r--   0        0        0     3567 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/demographics.yml
+-rw-r--r--   0        0        0       41 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/exposures.yml
+-rw-r--r--   0        0        0      212 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/model.yml
+-rw-r--r--   0        0        0      138 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/monkeypox.yml
+-rw-r--r--   0        0        0     2334 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/partnership.yml
+-rw-r--r--   0        0        0       90 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-monkeypox/vaccine.yml
+-rw-r--r--   0        0        0     5899 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-msm/demographics.yml
+-rw-r--r--   0        0        0      249 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-msm/hiv.yml
+-rw-r--r--   0        0        0     2372 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-msm/location.yml
+-rw-r--r--   0        0        0     1320 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-msm/model.yml
+-rw-r--r--   0        0        0     2415 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/nyc-msm/partnership.yml
+-rw-r--r--   0        0        0      408 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/assort_mix.yml
+-rw-r--r--   0        0        0       85 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/calibration.yml
+-rw-r--r--   0        0        0    10097 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/classes.yml
+-rw-r--r--   0        0        0    14020 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/demographics.yml
+-rw-r--r--   0        0        0       25 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/haart.yml
+-rw-r--r--   0        0        0      155 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/high_risk.yml
+-rw-r--r--   0        0        0       71 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/hiv.yml
+-rw-r--r--   0        0        0      116 2023-07-10 15:41:15.936137 titan_model-3.3.0/titan/settings/philly-gis/incar.yml
+-rw-r--r--   0        0        0   411827 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/philly-gis/location.yml
+-rw-r--r--   0        0        0      384 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/philly-gis/model.yml
+-rw-r--r--   0        0        0      692 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/philly-gis/partnership.yml
+-rw-r--r--   0        0        0     2559 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/philly-gis/timeline_scaling.yml
+-rw-r--r--   0        0        0     2963 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/rhode-island/demographics.yml
+-rw-r--r--   0        0        0     1960 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/rhode-island/model.yml
+-rw-r--r--   0        0        0     2850 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/scott/demographics.yml
+-rw-r--r--   0        0        0     4253 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/settings/scott/model.yml
+-rw-r--r--   0        0        0    12850 2023-07-10 15:41:15.940137 titan_model-3.3.0/titan/utils.py
+-rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 titan_model-3.3.0/PKG-INFO
```

### Comparing `titan-model-3.2.0/LICENSE` & `titan_model-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/README.md` & `titan_model-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/pyproject.toml` & `titan_model-3.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "titan-model"
-version = "3.2.0"
+version = "3.3.0"
 description = "TITAN Agent Based Model"
 license = "GPL-3.0-only"
 authors = ["Sam Bessey <sam_bessey@brown.edu>", "Mary McGrath <mary_mcgrath@brown.edu>"]
 readme = "README.md"
 homepage = "https://titanmodel.org"
 repository = "https://github.com/pph-collective/TITAN"
 documentation = "https://pph-collective.github.io/titan"
@@ -13,17 +13,17 @@
 
 [tool.poetry.dependencies]
 python = "^3.6"
 paraml= "^0.1"
 networkx = "^2.4"
 nanoid = "^2.0"
 numpy = "^1.18"
-black = {version = "^20.8b1", optional = true}
+black = {version = "^23.1.0", optional = true}
 flake8 = {version = "^3.8", optional = true}
-mypy = {version = "^0.812", optional = true}
+mypy = {version = "^1.0.0", optional = true}
 mkdocs = {version = "^1.1", optional = true}
 mkdocs-material = {version = "^7.0", optional = true}
 mkdocstrings = {version = "^0.15.0", optional = true}
 oyaml = "^1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
```

### Comparing `titan-model-3.2.0/titan/agent.py` & `titan_model-3.3.0/titan/agent.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/distributions.py` & `titan_model-3.3.0/titan/distributions.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/exposures/base_exposure.py` & `titan_model-3.3.0/titan/exposures/base_exposure.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from .. import agent
 from .. import population
 from .. import model
 
 
 class BaseExposure:
-
     name: str = ""
     """Name of exposure in the params file.  Also used to name the attribute in Agent"""
 
     stats: List[str] = []
     """List of names of stats that come from this exposure (e.g. hiv.dx)"""
 
     def __init__(self, agent: "agent.Agent"):
```

### Comparing `titan-model-3.2.0/titan/exposures/hiv.py` & `titan_model-3.3.0/titan/exposures/hiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from .. import agent
 from .. import population
 from .. import model
 from .. import utils
 
 
 class HIV(base_exposure.BaseExposure):
-
     name: str = "hiv"
     stats: List[str] = ["hiv", "hiv_dx", "hiv_aids", "hiv_new", "hiv_dx_new"]
     """
         HIV collects the following stats:
 
         * hiv - number of agents with active hiv
         * hiv_dx - number of agents with diagnosed hiv
```

### Comparing `titan-model-3.2.0/titan/exposures/knowledge.py` & `titan_model-3.3.0/titan/exposures/knowledge.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .. import agent as ag
 from .. import population
 from .. import model
 from .. import utils
 
 
 class Knowledge(base_exposure.BaseExposure):
-
     name: str = "knowledge"
     stats: List[str] = ["knowledge_aware"]
     """
     Knowledge collects the following stats:
 
     * knowledge_aware - number of agents with active knowledge
     """
```

### Comparing `titan-model-3.2.0/titan/exposures/monkeypox.py` & `titan_model-3.3.0/titan/exposures/monkeypox.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from .. import agent
 from .. import population
 from .. import model
 from .. import utils
 
 
 class MonkeyPox(base_exposure.BaseExposure):
-
     name: str = "monkeypox"
     stats: List[str] = [
         "monkeypox",
         "monkeypox_dx",
         "monkeypox_new",
         "monkeypox_dx_new",
     ]
```

### Comparing `titan-model-3.2.0/titan/features/base_feature.py` & `titan_model-3.3.0/titan/features/base_feature.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/features/external_exposure.py` & `titan_model-3.3.0/titan/features/external_exposure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from . import base_feature
 from .. import agent
 from .. import population
 from .. import model
 
 
 class ExternalExposure(base_feature.BaseFeature):
-
     name = "external_exposure"
 
     def __init__(self, agent: "agent.Agent"):
         super().__init__(agent)
 
         self.active = False
```

### Comparing `titan-model-3.2.0/titan/features/haart.py` & `titan_model-3.3.0/titan/features/haart.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/features/high_risk.py` & `titan_model-3.3.0/titan/features/high_risk.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .. import agent
 from .. import population
 from .. import model
 from ..distributions import poisson
 
 
 class HighRisk(base_feature.BaseFeature):
-
     name = "high_risk"
     stats = [
         "high_risk_new",
         "high_risk_new_hiv",
         "high_risk_new_aids",
         "high_risk_new_dx",
         "high_risk_new_haart",
@@ -72,15 +71,14 @@
         if not self.active:
             # released last step, evaluate agent for high risk
             if self.agent.incar.release_time == model.time - 1:  # type: ignore[attr-defined]
                 self.become_high_risk(model.pop, model.time)
 
             # incarcerated last step, evaluate agent's partners for high risk
             elif self.agent.incar.time == model.time - 1:  # type: ignore[attr-defined]
-
                 # put partners in high risk
                 for partner in self.agent.get_partners(
                     self.agent.location.params.high_risk.partnership_types
                 ):
                     if (
                         not partner.high_risk.active  # type: ignore[attr-defined]
                         and model.run_random.random()
@@ -126,15 +124,15 @@
                 stats["hiv_new_high_risk"] += 1
             if self.ever:
                 stats["hiv_new_high_risk_ever"] += 1
 
     # ============== HELPER METHODS ================
 
     def become_high_risk(
-        self, pop: "population.Population", time: int, duration: int = None
+        self, pop: "population.Population", time: int, duration: Optional[int] = None
     ):
         """
         Mark an agent as high risk and assign a duration to their high risk period
 
         args:
             pop: the model poopulation
             time: the time step the agent is becoming high risk
```

### Comparing `titan-model-3.2.0/titan/features/incar.py` & `titan_model-3.3.0/titan/features/incar.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from .. import agent
 from .. import population
 from .. import model
 from .. import utils
 
 
 class Incar(base_feature.BaseFeature):
-
     name = "incar"
     stats = ["incar", "incar_hiv", "new_release", "new_release_hiv"]
     """
         Incar collects the following stats:
 
         * incar - number of agents with active incar
         * incar_hiv - number of agents with active incar and HIV
```

### Comparing `titan-model-3.2.0/titan/features/partner_tracing.py` & `titan_model-3.3.0/titan/features/partner_tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from . import base_feature
 from .. import agent
 from .. import model
 
 
 class PartnerTracing(base_feature.BaseFeature):
-
     name = "partner_tracing"
 
     def __init__(self, agent: "agent.Agent"):
         super().__init__(agent)
 
         self.active = False
         self.time = None
```

### Comparing `titan-model-3.2.0/titan/features/prep.py` & `titan_model-3.3.0/titan/features/prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .. import population
 from .. import model
 from ..parse_params import ObjMap
 from .. import exposures
 
 
 class Prep(base_feature.BaseFeature):
-
     name = "prep"
     stats = ["prep", "prep_new", "prep_injectable", "prep_oral"]
     """
         PrEP collects the following stats:
 
         * prep - number of agents with active PrEP
         * prep_new - number of agents who became active PrEP this time step
```

### Comparing `titan-model-3.2.0/titan/features/random_trial.py` & `titan_model-3.3.0/titan/features/random_trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from .. import utils
 from .. import model
 
 import networkx as nx  # type: ignore
 
 
 class RandomTrial(base_feature.BaseFeature):
-
     name = "random_trial"
     stats = [
         "random_trial",
         "random_trial_treated",
         "random_trial_suitable",
         "random_trial_treated_hiv",
     ]
```

### Comparing `titan-model-3.2.0/titan/features/syringe_services.py` & `titan_model-3.3.0/titan/features/syringe_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from . import base_feature
 from .. import model as hiv_model
 from .. import utils
 
 
 class SyringeServices(base_feature.BaseFeature):
-
     name = "syringe_services"
 
     enrolled_risk = 0.0
 
     def __init__(self, agent):
         super().__init__(agent)
```

### Comparing `titan-model-3.2.0/titan/features/vaccine.py` & `titan_model-3.3.0/titan/features/vaccine.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from . import base_feature
 from .. import agent
 from .. import population
 from .. import model
 
 
 class Vaccine(base_feature.BaseFeature):
-
     name = "vaccine"
     stats = ["vaccine"]
     """
         Vaccine collects the following stats:
 
         * vaccine - number of agents with active vaccine
     """
```

### Comparing `titan-model-3.2.0/titan/interactions/base_interaction.py` & `titan_model-3.3.0/titan/interactions/base_interaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from .. import model
 from .. import agent
 
 
 class BaseInteraction:
-
     name: str = ""
     """Name of interaction in the params file."""
 
     @classmethod
     def interact(cls, model: "model.TITAN", rel: "agent.Relationship"):
         """
         Given a model and a relation, have the agents in the relationship interact for a time step.
```

### Comparing `titan-model-3.2.0/titan/interactions/injection.py` & `titan_model-3.3.0/titan/interactions/injection.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .. import features
 from .. import model
 from .. import agent
 from ..distributions import poisson
 
 
 class Injection(base_interaction.BaseInteraction):
-
     name = "injection"
 
     @classmethod
     def get_num_acts(cls, model: "model.TITAN", rel: "agent.Relationship") -> int:
         """
         Simulate random transmission of HIV between two PWID agents through injection.
```

### Comparing `titan-model-3.2.0/titan/interactions/pca.py` & `titan_model-3.3.0/titan/interactions/pca.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from . import base_interaction
 from .. import model
 from .. import agent
 from .. import utils
 
 
 class PCA(base_interaction.BaseInteraction):
-
     name = "pca"
 
     @classmethod
     def get_num_acts(cls, model: "model.TITAN", rel: "agent.Relationship") -> int:
         params = model.params.partnership.pca.frequency[rel.bond_type]
 
         if params.type == "bins":
```

### Comparing `titan-model-3.2.0/titan/interactions/sex.py` & `titan_model-3.3.0/titan/interactions/sex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from . import base_interaction
 from ..distributions import poisson
 from .. import model
 from .. import agent
 
 
 class Sex(base_interaction.BaseInteraction):
-
     name = "sex"
 
     @classmethod
     def get_num_acts(cls, model: "model.TITAN", rel: "agent.Relationship") -> int:
         """
         Simulate random transmission of HIV between two agents through Sex. One of the agents must be HIV+.
```

### Comparing `titan-model-3.2.0/titan/location.py` & `titan_model-3.3.0/titan/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
 # LocationEdges are very much a WIP and not actually used anywhere yet
 # outstanding questions:
 # * should edges be directed? bi-drectional? uni-drectional, but both directions housed in the same edge?
 # * what attributes do edges need?
 # * how will mobility be implemented?
 # * assorting?
 class LocationEdge:
-
     next_edge_id = 0
 
     @classmethod
     def update_id_counter(cls, last_id: int):
         cls.next_edge_id = last_id + 1
 
     def __init__(
```

### Comparing `titan-model-3.2.0/titan/model.py` & `titan_model-3.3.0/titan/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,17 @@
         logging.info(
             f"\n                                                  .: TIME {self.time}"
         )
         logging.info(
             "  STARTING HIV count:{}  Total Incarcerated:{}  HR+:{}  "
             "PrEP:{}".format(
                 len(exposures.HIV.agents),
-                sum([1 for a in self.pop.all_agents if a.incar.active]),  # type: ignore[attr-defined]
-                sum([1 for a in self.pop.all_agents if a.high_risk.active]),  # type: ignore[attr-defined]
-                sum([1 for a in self.pop.all_agents if a.prep.active]),  # type: ignore[attr-defined]
+                sum([1 for a in self.pop.all_agents if a.incar.active]),  # type: ignore[misc, attr-defined]
+                sum([1 for a in self.pop.all_agents if a.high_risk.active]),  # type: ignore[misc, attr-defined]
+                sum([1 for a in self.pop.all_agents if a.prep.active]),  # type: ignore[misc, attr-defined]
             )
         )
 
         self.timeline_scaling()
 
         self.update_all_agents()
 
@@ -231,15 +231,21 @@
             * age
             * all exposures
             * all features (agent level)
         """
         # If static network, ignore relationship progression
         if not self.params.features.static_network:
             for rel in copy(self.pop.relationships):
-                if rel.progress():
+                if (
+                    self.params.partnership.dissolve.enabled
+                    and self.time == self.params.partnership.dissolve.time
+                ):
+                    rel.progress(force=True)
+                    self.pop.remove_relationship(rel)
+                elif rel.progress():
                     self.pop.remove_relationship(rel)
 
         if self.params.features.exit_enter:
             self.exit()
             self.enter()
 
         if self.params.location.migration.enabled:
```

### Comparing `titan-model-3.2.0/titan/output.py` & `titan_model-3.3.0/titan/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     if f.tell() == 0:
         f.write(
             "run_id\trunseed\tpopseed\tt\tcomponent\tagents"
             "\tinfected\ttrt\ttrtinfected"
             "\tdensity\tEffectiveSize\tdeg_cent\n"
         )
 
-    for (id, comp) in enumerate(components):
+    for id, comp in enumerate(components):
         num_nodes = comp.number_of_nodes()
 
         average_size = effective_size(comp) / num_nodes
         comp_density = nx.density(comp)
 
         deg_cent = mean(list(nx.degree_centrality(comp).values()))
         nhiv = ntrthiv = ntrt = 0
```

### Comparing `titan-model-3.2.0/titan/params/agent_zero.yml` & `titan_model-3.3.0/titan/params/agent_zero.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/assort_mix.yml` & `titan_model-3.3.0/titan/params/assort_mix.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/calibration.yml` & `titan_model-3.3.0/titan/params/calibration.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/classes.yml` & `titan_model-3.3.0/titan/params/classes.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/demographics.yml` & `titan_model-3.3.0/titan/params/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/external_exposure.yml` & `titan_model-3.3.0/titan/params/external_exposure.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/features.yml` & `titan_model-3.3.0/titan/params/features.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/haart.yml` & `titan_model-3.3.0/titan/params/haart.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/high_risk.yml` & `titan_model-3.3.0/titan/params/high_risk.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/hiv.yml` & `titan_model-3.3.0/titan/params/hiv.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/incar.yml` & `titan_model-3.3.0/titan/params/incar.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/knowledge.yml` & `titan_model-3.3.0/titan/params/knowledge.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/location.yml` & `titan_model-3.3.0/titan/params/location.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/model.yml` & `titan_model-3.3.0/titan/params/model.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/monkeypox.yml` & `titan_model-3.3.0/titan/params/monkeypox.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/outputs.yml` & `titan_model-3.3.0/titan/params/outputs.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/partner_tracing.yml` & `titan_model-3.3.0/titan/params/partner_tracing.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/partnership.yml` & `titan_model-3.3.0/titan/params/partnership.yml`

 * *Files 2% similar despite different names*

```diff
@@ -254,7 +254,14 @@
     same_component:
       prob:
         default: 0
         type: float
         description: Probability that for a given partnering attempt, the agent tries to partner with only other agents in their component. Otherwise, the agent tries to partner with agents from any component.  Network must be enabled.
         min: 0
         max: 1
+  dissolve:
+    time:
+      type: int
+      default: -9999
+    enabled:
+      type: bool
+      default: false
```

### Comparing `titan-model-3.2.0/titan/params/prep.yml` & `titan_model-3.3.0/titan/params/prep.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/random_trial.yml` & `titan_model-3.3.0/titan/params/random_trial.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/syringe_services.yml` & `titan_model-3.3.0/titan/params/syringe_services.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/timeline_scaling.yml` & `titan_model-3.3.0/titan/params/timeline_scaling.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/params/vaccine.yml` & `titan_model-3.3.0/titan/params/vaccine.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/parse_params.py` & `titan_model-3.3.0/titan/parse_params.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/partnering.py` & `titan_model-3.3.0/titan/partnering.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/population.py` & `titan_model-3.3.0/titan/population.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,14 @@
                 ]
             )
             attempts = {a: 0 for a in eligible_agents}
 
             while eligible_agents:
                 agent = eligible_agents.popleft()
                 if len(agent.partners[bond]) < agent.target_partners[bond]:
-
                     # no match
                     if self.update_agent_partners(agent, bond, network_components):
                         attempts[agent] += 1
 
                     # add agent back to eligible pool
                     if (
                         len(agent.partners[bond]) < agent.target_partners[bond]
```

### Comparing `titan-model-3.2.0/titan/population_io.py` & `titan_model-3.3.0/titan/population_io.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/probabilities.py` & `titan_model-3.3.0/titan/probabilities.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/run_titan.py` & `titan_model-3.3.0/titan/run_titan.py`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/atlanta/assort_mix.yml` & `titan_model-3.3.0/titan/settings/atlanta/assort_mix.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/atlanta/demographics.yml` & `titan_model-3.3.0/titan/settings/atlanta/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/atlanta/model.yml` & `titan_model-3.3.0/titan/settings/atlanta/model.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/atlanta/partnership.yml` & `titan_model-3.3.0/titan/settings/atlanta/partnership.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/chicago/chicago_baseCase.yml` & `titan_model-3.3.0/titan/settings/chicago/chicago_baseCase.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/mississippi/demographics.yml` & `titan_model-3.3.0/titan/settings/mississippi/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/mississippi/model.yml` & `titan_model-3.3.0/titan/settings/mississippi/model.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/missouri/demographics.yml` & `titan_model-3.3.0/titan/settings/missouri/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/missouri/model.yml` & `titan_model-3.3.0/titan/settings/missouri/model.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/nyc-monkeypox/demographics.yml` & `titan_model-3.3.0/titan/settings/nyc-monkeypox/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/nyc-monkeypox/partnership.yml` & `titan_model-3.3.0/titan/settings/nyc-monkeypox/partnership.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/nyc-msm/demographics.yml` & `titan_model-3.3.0/titan/settings/nyc-msm/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/nyc-msm/location.yml` & `titan_model-3.3.0/titan/settings/nyc-msm/location.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/nyc-msm/model.yml` & `titan_model-3.3.0/titan/settings/nyc-msm/model.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/nyc-msm/partnership.yml` & `titan_model-3.3.0/titan/settings/nyc-msm/partnership.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/rhode-island/demographics.yml` & `titan_model-3.3.0/titan/settings/rhode-island/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/rhode-island/model.yml` & `titan_model-3.3.0/titan/settings/rhode-island/model.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/scott/demographics.yml` & `titan_model-3.3.0/titan/settings/scott/demographics.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/settings/scott/model.yml` & `titan_model-3.3.0/titan/settings/scott/model.yml`

 * *Files identical despite different names*

### Comparing `titan-model-3.2.0/titan/utils.py` & `titan_model-3.3.0/titan/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
                 add_edge(edges, loc, grid[i + 1][j + 1])
                 if i >= 1:
                     add_edge(edges, loc, grid[i - 1][j + 1])
                 if j >= 1:
                     add_edge(edges, loc, grid[i + 1][j - 1])
 
     res = {}
-    for (i, edge) in enumerate(edges):
+    for i, edge in enumerate(edges):
         res[f"edge_{i+1}"] = {"location_1": edge[0], "location_2": edge[1]}
 
     return res
 
 
 def grid_file_to_edge_yml(
     file_path: str, outfile_path: str, diagonal_neighbors: bool = False
```

### Comparing `titan-model-3.2.0/PKG-INFO` & `titan_model-3.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: titan-model
-Version: 3.2.0
+Version: 3.3.0
 Summary: TITAN Agent Based Model
 Home-page: https://titanmodel.org
 License: GPL-3.0-only
 Author: Sam Bessey
 Author-email: sam_bessey@brown.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Provides-Extra: linting
-Requires-Dist: black (>=20.8b1,<21.0); extra == "linting"
-Requires-Dist: flake8 (>=3.8,<4.0); extra == "linting"
-Requires-Dist: mkdocs (>=1.1,<2.0); extra == "docs"
-Requires-Dist: mkdocs-material (>=7.0,<8.0); extra == "docs"
-Requires-Dist: mkdocstrings (>=0.15.0,<0.16.0); extra == "docs"
-Requires-Dist: mypy (>=0.812,<0.813); extra == "linting"
+Requires-Dist: black (>=23.1.0,<24.0.0) ; extra == "linting"
+Requires-Dist: flake8 (>=3.8,<4.0) ; extra == "linting"
+Requires-Dist: mkdocs (>=1.1,<2.0) ; extra == "docs"
+Requires-Dist: mkdocs-material (>=7.0,<8.0) ; extra == "docs"
+Requires-Dist: mkdocstrings (>=0.15.0,<0.16.0) ; extra == "docs"
+Requires-Dist: mypy (>=1.0.0,<2.0.0) ; extra == "linting"
 Requires-Dist: nanoid (>=2.0,<3.0)
 Requires-Dist: networkx (>=2.4,<3.0)
 Requires-Dist: numpy (>=1.18,<2.0)
 Requires-Dist: oyaml (>=1.0,<2.0)
 Requires-Dist: paraml (>=0.1,<0.2)
 Project-URL: Documentation, https://pph-collective.github.io/titan
 Project-URL: Repository, https://github.com/pph-collective/TITAN
```


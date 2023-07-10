# Comparing `tmp/pureml_evaluate-0.0.1.tar.gz` & `tmp/pureml_evaluate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml_evaluate-0.0.1.tar", max compression
+gzip compressed data, was "pureml_evaluate-0.0.2.tar", max compression
```

## Comparing `pureml_evaluate-0.0.1.tar` & `pureml_evaluate-0.0.2.tar`

### file list

```diff
@@ -1,259 +1,281 @@
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.1/README.md
--rw-r--r--   0        0        0       19 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.1/pureml_evaluate/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 19:28:58.934213 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/__init__.py
--rw-r--r--   0        0        0     3550 2023-06-15 07:55:19.931261 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/evaluator.py
--rw-r--r--   0        0        0     2013 2023-06-14 19:32:30.588585 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/grade.py
--rw-r--r--   0        0        0        0 2023-06-14 19:31:28.734789 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/model/fairness/__init__.py
--rw-r--r--   0        0        0     5772 2023-06-15 07:47:25.113756 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/model/fairness/fairness.py
--rw-r--r--   0        0        0        0 2023-06-14 19:31:28.734789 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/model/performance/__init__.py
--rw-r--r--   0        0        0     2009 2023-06-15 07:47:05.769380 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/model/performance/classification.py
--rw-r--r--   0        0        0     1020 2023-06-15 07:46:40.308871 pureml_evaluate-0.0.1/pureml_evaluate/evaluators/model/performance/regression.py
--rw-r--r--   0        0        0       89 2023-06-14 19:32:30.820592 pureml_evaluate-0.0.1/pureml_evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      361 2023-06-14 19:32:30.860593 pureml_evaluate-0.0.1/pureml_evaluate/metrics/metric_base.py
--rw-r--r--   0        0        0        0 2023-06-04 16:57:58.850890 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/accuracy/README.md
--rw-r--r--   0        0        0      664 2023-06-14 19:32:30.932595 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/accuracy/accuracy.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/accuracy/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/additive_chi2_kernel/README.md
--rw-r--r--   0        0        0      596 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/additive_chi2_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_mutual_info_score/README.md
--rw-r--r--   0        0        0      673 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_mutual_info_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_rand_score/README.md
--rw-r--r--   0        0        0      573 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_rand_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:30.932595 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/auc/README.md
--rw-r--r--   0        0        0      582 2023-06-14 19:32:31.176602 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/auc/auc.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/auc/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/average_precision_score/README.md
--rw-r--r--   0        0        0     1148 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/average_precision_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/balanced_accuracy_score/README.md
--rw-r--r--   0        0        0      643 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/balanced_accuracy_score/balanced_accuracy_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/balanced_accuracy_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/brier_score_loss/README.md
--rw-r--r--   0        0        0     1041 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/brier_score_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/calinski_harabasz_score/README.md
--rw-r--r--   0        0        0      546 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/calinski_harabasz_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/chi2_kernel/README.md
--rw-r--r--   0        0        0      580 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/chi2_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/class_likelihood_ratios/README.md
--rw-r--r--   0        0        0      637 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.200603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/class_likelihood_ratios/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.204603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cohen_kappa_score/README.md
--rw-r--r--   0        0        0      644 2023-06-14 19:32:31.204603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.204603 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cohen_kappa_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/completeness_score/README.md
--rw-r--r--   0        0        0      567 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/completeness_score/completeness_score.py
--rw-r--r--   0        0        0       15 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/completeness_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/confusion_matrix/README.md
--rw-r--r--   0        0        0      698 2023-06-14 20:44:21.981665 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/confusion_matrix/confusion_matrix.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/confusion_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/contingency_matrix/README.md
--rw-r--r--   0        0        0      634 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py
--rw-r--r--   0        0        0       19 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/contingency_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_distances/README.md
--rw-r--r--   0        0        0      558 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_similarity/README.md
--rw-r--r--   0        0        0      630 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_similarity/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/coverage_error/README.md
--rw-r--r--   0        0        0      578 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/coverage_error/coverage_error.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/coverage_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.352607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_absolute_error_score/README.md
--rw-r--r--   0        0        0      675 2023-06-14 19:32:31.352607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.352607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_absolute_error_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.352607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_pinball_score/README.md
--rw-r--r--   0        0        0      670 2023-06-14 19:32:31.352607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.352607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_pinball_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.352607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_tweedie_score/README.md
--rw-r--r--   0        0        0      670 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_tweedie_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/davies_bouldin_score/README.md
--rw-r--r--   0        0        0      551 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/davies_bouldin_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/dcg_score/README.md
--rw-r--r--   0        0        0     1053 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/dcg_score/dcg_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/dcg_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/det_curve/README.md
--rw-r--r--   0        0        0     1010 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/det_curve/det_curve.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/det_curve/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/euclidean_distances/README.md
--rw-r--r--   0        0        0      631 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/euclidean_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/explained_variance_score/README.md
--rw-r--r--   0        0        0      679 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.356607 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/explained_variance_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/f1_score/README.md
--rw-r--r--   0        0        0      734 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/f1_score/f1_score.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/f1_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fbeta_score/README.md
--rw-r--r--   0        0        0      717 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fbeta_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fowlkes_mallows_score/README.md
--rw-r--r--   0        0        0      582 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py
--rw-r--r--   0        0        0       13 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fowlkes_mallows_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hamming_loss/README.md
--rw-r--r--   0        0        0      631 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hamming_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/haversine_distances/README.md
--rw-r--r--   0        0        0      507 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/haversine_distances/haversine_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/haversine_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hinge_loss/README.md
--rw-r--r--   0        0        0     1098 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hinge_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/README.md
--rw-r--r--   0        0        0      798 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.244791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_score/README.md
--rw-r--r--   0        0        0      547 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py
--rw-r--r--   0        0        0       13 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/jaccard_score/README.md
--rw-r--r--   0        0        0      715 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/jaccard_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_average_precision_score/README.md
--rw-r--r--   0        0        0      669 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py
--rw-r--r--   0        0        0       15 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_average_precision_score/requirementx.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_loss/README.md
--rw-r--r--   0        0        0      598 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/laplacian_kernel/README.md
--rw-r--r--   0        0        0      528 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/laplacian_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/linear_kernel/README.md
--rw-r--r--   0        0        0      519 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/linear_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/log_loss/README.md
--rw-r--r--   0        0        0     1134 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/log_loss/log_loss.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/log_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/manhattan_distances/README.md
--rw-r--r--   0        0        0      506 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/manhattan_distances/manhattan_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/manhattan_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/matthews_corrcoef/README.md
--rw-r--r--   0        0        0      652 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/matthews_corrcoef/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/max_error/README.md
--rw-r--r--   0        0        0      540 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/max_error/max_error.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/max_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_error/README.md
--rw-r--r--   0        0        0      699 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_percentage_error/README.md
--rw-r--r--   0        0        0      750 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_percentage_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_gamma_deviance/README.md
--rw-r--r--   0        0        0      662 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_gamma_deviance/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_pinball_loss/README.md
--rw-r--r--   0        0        0      680 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_pinball_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_poisson_deviance/README.md
--rw-r--r--   0        0        0      680 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_poisson_deviance/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_error/README.md
--rw-r--r--   0        0        0      754 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_log_error/README.md
--rw-r--r--   0        0        0      749 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_log_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_tweedie_deviance/README.md
--rw-r--r--   0        0        0      697 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_tweedie_deviance/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/median_absolute_error/README.md
--rw-r--r--   0        0        0      744 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/median_absolute_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/multilabel_confusion_matrix/README.md
--rw-r--r--   0        0        0      724 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/multilabel_confusion_matrix/multilabel_confusion_matrix.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/multilabel_confusion_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mutual_info_score/README.md
--rw-r--r--   0        0        0      676 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mutual_info_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/nan_euclidean_distances/README.md
--rw-r--r--   0        0        0      647 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py
--rw-r--r--   0        0        0       19 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/nan_euclidean_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/ndcg_score/README.md
--rw-r--r--   0        0        0     1068 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.420609 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/ndcg_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/normalized_mutual_info_score/README.md
--rw-r--r--   0        0        0      648 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/normalized_mutual_info_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pair_confusion_matrix/README.md
--rw-r--r--   0        0        0      549 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pair_confusion_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_cosine_distances/README.md
--rw-r--r--   0        0        0      518 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_cosine_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_distances/README.md
--rw-r--r--   0        0        0      525 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_distances/paired_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_euclidean_distances/README.md
--rw-r--r--   0        0        0      525 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_euclidean_distances/requirements.txt
--rw-r--r--   0        0        0      529 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances/README.md
--rw-r--r--   0        0        0      602 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin/README.md
--rw-r--r--   0        0        0      608 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/README.md
--rw-r--r--   0        0        0      714 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_chunked/README.md
--rw-r--r--   0        0        0      668 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_chunked/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_kernels/README.md
--rw-r--r--   0        0        0      591 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_kernels/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/polynomial_kernel/README.md
--rw-r--r--   0        0        0      571 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/polynomial_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision/README.md
--rw-r--r--   0        0        0      849 2023-06-14 19:32:31.596614 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision/precision.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.596614 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision_recall_curve/README.md
--rw-r--r--   0        0        0     1292 2023-06-14 19:32:31.596614 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.596614 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision_recall_curve/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.596614 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/r2_score/README.md
--rw-r--r--   0        0        0      675 2023-06-14 19:32:31.596614 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/r2_score/r2_score.py
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.596614 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/r2_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/rand_score/README.md
--rw-r--r--   0        0        0      511 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/rand_score/rand_score.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/rand_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/rbf_kernel/README.md
--rw-r--r--   0        0        0      493 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/rbf_kernel/rbf_kernel.py
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/rbf_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/recall/README.md
--rw-r--r--   0        0        0      834 2023-06-14 19:32:31.684617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/recall/recall.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/recall/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_auc/README.md
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_auc/requirements.txt
--rw-r--r--   0        0        0     1272 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_auc/roc_auc.py
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_curve/README.md
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_curve/requirements.txt
--rw-r--r--   0        0        0     1207 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_curve/roc_curve.py
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/sigmoid_kernel/README.md
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/sigmoid_kernel/requirements.txt
--rw-r--r--   0        0        0      522 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_samples/README.md
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_samples/requirements.txt
--rw-r--r--   0        0        0      521 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_score/README.md
--rw-r--r--   0        0        0       14 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_score/requirements.txt
--rw-r--r--   0        0        0      619 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/top_k_accuracy_score/README.md
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/top_k_accuracy_score/requirements.txt
--rw-r--r--   0        0        0     1141 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/top_k_accuracy_score/top_k_accuracy_score.py
--rw-r--r--   0        0        0        0 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/v_measure_score/README.md
--rw-r--r--   0        0        0       13 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/v_measure_score/requirements.txt
--rw-r--r--   0        0        0      550 2023-06-21 16:35:59.248791 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py
--rw-r--r--   0        0        0        0 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/zero_one_loss/README.md
--rw-r--r--   0        0        0       14 2023-06-14 19:32:31.696617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/zero_one_loss/requirements.txt
--rw-r--r--   0        0        0      682 2023-06-14 19:32:31.700617 pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/zero_one_loss/zero_one_loss.py
--rw-r--r--   0        0        0      812 2023-06-14 19:32:31.828621 pureml_evaluate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 pureml_evaluate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/README.md
+-rw-r--r--   0        0        0       19 2023-07-10 21:08:37.688024 pureml_evaluate-0.0.2/pureml_evaluate/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/__init__.py
+-rw-r--r--   0        0        0      510 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/data_metric_base.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/__init__.py
+-rw-r--r--   0        0        0       60 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/check.py
+-rw-r--r--   0        0        0      717 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/class_imbalance.py
+-rw-r--r--   0        0        0     1338 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/column_info.py
+-rw-r--r--   0        0        0      998 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/conflicting_labels.py
+-rw-r--r--   0        0        0      855 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/data_duplicates.py
+-rw-r--r--   0        0        0      440 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/feature_feature_correlation.py
+-rw-r--r--   0        0        0     2184 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/feature_label_correlation.py
+-rw-r--r--   0        0        0     1599 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/identifier_label_correlation.py
+-rw-r--r--   0        0        0      711 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/is_single_value.py
+-rw-r--r--   0        0        0     1024 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/mixed_data_types.py
+-rw-r--r--   0        0        0     1228 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/mixed_nulls.py
+-rw-r--r--   0        0        0     1849 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/outlier_sample_detection.py
+-rw-r--r--   0        0        0      677 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/percent_of_nulls.py
+-rw-r--r--   0        0        0     1203 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/special_character.py
+-rw-r--r--   0        0        0     1899 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/string_length_outOfBounds.py
+-rw-r--r--   0        0        0     1877 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/string_mismatch.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.409891 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/__init__.py
+-rw-r--r--   0        0        0     3122 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/config.json
+-rw-r--r--   0        0        0     4756 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/evaluator.py
+-rw-r--r--   0        0        0     2013 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/grade.py
+-rw-r--r--   0        0        0    18803 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/graphs_generator.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/fairness/__init__.py
+-rw-r--r--   0        0        0     6119 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/fairness/fairness.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/__init__.py
+-rw-r--r--   0        0        0     3184 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/classification.py
+-rw-r--r--   0        0        0     2412 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/regression.py
+-rw-r--r--   0        0        0     7488 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/risk_evaluator.py
+-rw-r--r--   0        0        0       89 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      361 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/metric_base.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:57:58.850890 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/README.md
+-rw-r--r--   0        0        0      778 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/accuracy.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/README.md
+-rw-r--r--   0        0        0      596 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/README.md
+-rw-r--r--   0        0        0      673 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/README.md
+-rw-r--r--   0        0        0      573 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/README.md
+-rw-r--r--   0        0        0      582 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/auc.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/README.md
+-rw-r--r--   0        0        0     1160 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/balanced_accuracy_score/README.md
+-rw-r--r--   0        0        0      655 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/balanced_accuracy_score/balanced_accuracy_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/balanced_accuracy_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/README.md
+-rw-r--r--   0        0        0     1052 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/README.md
+-rw-r--r--   0        0        0      546 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/README.md
+-rw-r--r--   0        0        0      580 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/README.md
+-rw-r--r--   0        0        0      637 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/README.md
+-rw-r--r--   0        0        0      644 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/README.md
+-rw-r--r--   0        0        0      567 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/completeness_score.py
+-rw-r--r--   0        0        0       15 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/confusion_matrix/README.md
+-rw-r--r--   0        0        0      814 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/confusion_matrix/confusion_matrix.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/confusion_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/README.md
+-rw-r--r--   0        0        0      634 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py
+-rw-r--r--   0        0        0       19 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/README.md
+-rw-r--r--   0        0        0      558 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/README.md
+-rw-r--r--   0        0        0      630 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/README.md
+-rw-r--r--   0        0        0      578 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/coverage_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/README.md
+-rw-r--r--   0        0        0      686 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/README.md
+-rw-r--r--   0        0        0      683 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/README.md
+-rw-r--r--   0        0        0      681 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/README.md
+-rw-r--r--   0        0        0      551 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/README.md
+-rw-r--r--   0        0        0     1053 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/dcg_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/README.md
+-rw-r--r--   0        0        0     1010 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/det_curve.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/README.md
+-rw-r--r--   0        0        0      631 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/README.md
+-rw-r--r--   0        0        0      690 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/f1_score/README.md
+-rw-r--r--   0        0        0      985 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/f1_score/f1_score.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/f1_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/README.md
+-rw-r--r--   0        0        0      717 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/README.md
+-rw-r--r--   0        0        0      582 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py
+-rw-r--r--   0        0        0       13 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/README.md
+-rw-r--r--   0        0        0      631 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/haversine_distances/README.md
+-rw-r--r--   0        0        0      507 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/haversine_distances/haversine_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/haversine_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/README.md
+-rw-r--r--   0        0        0     1098 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/README.md
+-rw-r--r--   0        0        0      798 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/README.md
+-rw-r--r--   0        0        0      547 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py
+-rw-r--r--   0        0        0       13 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/README.md
+-rw-r--r--   0        0        0      715 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/README.md
+-rw-r--r--   0        0        0      669 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py
+-rw-r--r--   0        0        0       15 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/requirementx.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/README.md
+-rw-r--r--   0        0        0      598 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/README.md
+-rw-r--r--   0        0        0      528 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/README.md
+-rw-r--r--   0        0        0      519 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/README.md
+-rw-r--r--   0        0        0     1395 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/log_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/manhattan_distances/README.md
+-rw-r--r--   0        0        0      506 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/manhattan_distances/manhattan_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/manhattan_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/README.md
+-rw-r--r--   0        0        0      652 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/README.md
+-rw-r--r--   0        0        0      552 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/max_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/README.md
+-rw-r--r--   0        0        0      712 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/README.md
+-rw-r--r--   0        0        0      761 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/README.md
+-rw-r--r--   0        0        0      674 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/README.md
+-rw-r--r--   0        0        0      680 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/README.md
+-rw-r--r--   0        0        0      691 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/README.md
+-rw-r--r--   0        0        0      765 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/README.md
+-rw-r--r--   0        0        0      760 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/README.md
+-rw-r--r--   0        0        0      697 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/README.md
+-rw-r--r--   0        0        0      755 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/README.md
+-rw-r--r--   0        0        0      724 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/multilabel_confusion_matrix.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/README.md
+-rw-r--r--   0        0        0      676 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/README.md
+-rw-r--r--   0        0        0      647 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py
+-rw-r--r--   0        0        0       19 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/README.md
+-rw-r--r--   0        0        0     1068 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/README.md
+-rw-r--r--   0        0        0      648 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/README.md
+-rw-r--r--   0        0        0      549 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/README.md
+-rw-r--r--   0        0        0      518 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/README.md
+-rw-r--r--   0        0        0      525 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/paired_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/README.md
+-rw-r--r--   0        0        0      525 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/requirements.txt
+-rw-r--r--   0        0        0      529 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/README.md
+-rw-r--r--   0        0        0      602 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/README.md
+-rw-r--r--   0        0        0      608 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/README.md
+-rw-r--r--   0        0        0      714 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/README.md
+-rw-r--r--   0        0        0      668 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/README.md
+-rw-r--r--   0        0        0      591 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/README.md
+-rw-r--r--   0        0        0      571 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/README.md
+-rw-r--r--   0        0        0     1095 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/precision.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/README.md
+-rw-r--r--   0        0        0     1292 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/README.md
+-rw-r--r--   0        0        0      687 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/r2_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rand_score/README.md
+-rw-r--r--   0        0        0      511 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rand_score/rand_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rand_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rbf_kernel/README.md
+-rw-r--r--   0        0        0      493 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rbf_kernel/rbf_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rbf_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/recall/README.md
+-rw-r--r--   0        0        0     1062 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/recall/recall.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/recall/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/README.md
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/requirements.txt
+-rw-r--r--   0        0        0     2568 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/roc_auc.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/requirements.txt
+-rw-r--r--   0        0        0     1207 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/roc_curve.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/requirements.txt
+-rw-r--r--   0        0        0      522 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/requirements.txt
+-rw-r--r--   0        0        0      521 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/requirements.txt
+-rw-r--r--   0        0        0      619 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/requirements.txt
+-rw-r--r--   0        0        0     1357 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/top_k_accuracy_score.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/README.md
+-rw-r--r--   0        0        0       13 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/requirements.txt
+-rw-r--r--   0        0        0      550 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/requirements.txt
+-rw-r--r--   0        0        0      682 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/zero_one_loss.py
+-rw-r--r--   0        0        0      922 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 pureml_evaluate-0.0.2/PKG-INFO
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/evaluators/grade.py` & `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/grade.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/evaluators/model/fairness/fairness.py` & `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/fairness/fairness.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,25 +124,30 @@
             "equalized_odds_ratio": equalized_odds_ratio,
         }
 
         metrics = {}
 
         for metric_name, metric_func in fairness_metrics.items():
             try:
-                metrics[metric_name] = metric_func(
-                    y_true=self.references, y_pred=self.predictions)
+                metrics[metric_name] = {'value':metric_func(
+                    y_true=self.references, y_pred=self.predictions)}
             except Exception as e:
                 print("Unable to compute", metric_name)
                 print(e)
 
         for metric_name, metric_func in demography_metrics.items():
-            try:
-                metrics[metric_name] = metric_func(
+            try:                       #Converted them to list to add Status and Risk Analysis afterwards.
+                # metrics[metric_name] = [metric_func(
+                #     y_true=self.references, y_pred=self.predictions,
+                #     sensitive_features=self.sensitive_features)]
+
+                # Converting them to dict.
+                metrics[metric_name] = {'value':metric_func(
                     y_true=self.references, y_pred=self.predictions,
-                    sensitive_features=self.sensitive_features)
+                    sensitive_features=self.sensitive_features)}
             except Exception as e:
                 print("Unable to compute", metric_name)
                 print(e)
 
         return metrics
 
         # metricframe_unmitigated = MetricFrame(
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/evaluators/model/performance/classification.py` & `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/classification.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,86 @@
 from pureml_evaluate.metrics.model.accuracy.accuracy import Accuracy
 from pureml_evaluate.metrics.model.precision.precision import Precision
 from pureml_evaluate.metrics.model.recall.recall import Recall
 from pureml_evaluate.metrics.model.f1_score.f1_score import F1
 from pureml_evaluate.metrics.model.confusion_matrix.confusion_matrix import ConfusionMatrix
-
+from pureml_evaluate.metrics.model.balanced_accuracy_score.balanced_accuracy_score import BalancedAccuracyScore
+from pureml_evaluate.metrics.model.top_k_accuracy_score.top_k_accuracy_score import TopKAccuracyScore
+from pureml_evaluate.metrics.model.log_loss.log_loss import LogLoss
+from pureml_evaluate.metrics.model.roc_auc.roc_auc import ROC_AUC
+from pureml_evaluate.metrics.model.average_precision_score.average_precision_score import AveragePrecisionScore
+from pureml_evaluate.metrics.model.brier_score_loss.brier_score_loss import BrierScoreLoss
 
 class Classification:
     def __init__(self):
         self.task_type = "classification"
         self.evaluation_type = "performance"
 
-        self.kwargs = None
+        self.kwargs = {}
 
         self.references = None
         self.predictions = None
         self.prediction_scores = None
 
         self.label_type = "binary"
 
         self.metrics = [
             Accuracy(),
             Precision(),
             Recall(),
             F1(),
-            ConfusionMatrix(),
-        ]  # , ROC_AUC()]
+            #ConfusionMatrix(),
+            BalancedAccuracyScore(),
+            TopKAccuracyScore(),
+            LogLoss(),
+            AveragePrecisionScore(),
+          ROC_AUC()
+          ]
         self.scores = {}
 
     def compute(self):
         self.setup()
+        if self.label_type == 'binary':   #To Get results for BrierScoreLoss. As it supports only for binary classification
+            self.metrics.append(BrierScoreLoss())
+        
 
         for m in self.metrics:
             # Adding  prediction scores to kwargs. It will be utilized my metrics needing it(roc_auc).
 
             try:
 
                 self.kwargs["prediction_scores"] = self.prediction_scores
                 score = m.compute(
-                    references=self.references, predictions=self.predictions, **self.kwargs
+                    references=self.references, predictions=self.predictions, kwargs=self.kwargs
                 )
+                # **self.kwargs is changed to kwargs=self.kwargs. As **self.kwargs when passed to compute function is having type None.
 
                 self.scores.update(score)
             except Exception as e:
                 print("Unable to compute", m)
+                print(f"Exception: {e}")
 
         return self.scores
 
     def setup(self):
         self.is_multiclass()
         self.setup_kwargs()
 
     def get_predictions(self):
         pass
 
     def is_multiclass(self):
         # print(self.predictions)
         # print(self.references)
         if self.predictions is not None:
+            self.references = tuple(self.references)
+            self.predictions = tuple(self.predictions)
             labels_all = set(self.references).union(self.predictions)
             if len(labels_all) > 2:
                 self.label_type = "multilabel"
+            
 
     def setup_kwargs(self):
         if "average" not in self.kwargs:
             if self.label_type == "multilabel":
                 self.kwargs["average"] = "micro"
+
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/accuracy/accuracy.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from sklearn.metrics import accuracy_score
-from pureml_evaluate.metrics.metric_base import MetricBase
 from typing import Any
+from sklearn.metrics import class_likelihood_ratios
+from pureml_evaluate.metrics.metric_base import MetricBase
 
-class Accuracy(MetricBase):
-    name = 'accuracy'
+class ClassLikelihoodRatios(MetricBase):
+    name = 'class_likelihood_ratios'
     input_type = 'int'
-    output_type: Any= None
-    kwargs = {}
+    output_type: Any = None
+    kwargs = { }
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions, normalize=True, sample_weight=None, **kwargs):
+    def compute(self, references, predictions, sample_weight=None, **kwargs):
 
-        score = accuracy_score(y_true=references, y_pred=predictions, normalize=normalize,
-                                sample_weight=sample_weight)
+        score = class_likelihood_ratios(y_true=references, y_pred=predictions,  sample_weight=sample_weight)
         
         score = {
-            self.name : float(score)
+            self.name : score
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/auc/auc.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/auc.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,12 +26,12 @@
             score = float(score)
         elif prediction_scores is None:
             score = average_precision_score(y_true=references, y_score=predictions, average=average,
                                 sample_weight=sample_weight)
             score = float(score)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' : float(score)}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/balanced_accuracy_score/balanced_accuracy_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from typing import Any
-from sklearn.metrics import balanced_accuracy_score
+from sklearn.metrics import jaccard_score
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-class BalancedAccuracyScore(MetricBase):
-    name = 'balanced_accuracy_score'
+class JaccardScore(MetricBase):
+    name = 'jaccard_score'
     input_type = 'int'
     output_type: Any = None
     kwargs = { }
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions, sample_weight=None, **kwargs):
+    def compute(self, references, predictions, pos_label=1, average='binary',
+                 sample_weight=None, **kwargs):
 
-        score = balanced_accuracy_score(y_true=references, y_pred=predictions, sample_weight=sample_weight)
+        score = jaccard_score(y_true=references, y_pred=predictions, pos_label=pos_label,
+                                average=average, sample_weight=sample_weight)
         
         score = {
-            self.name : float(score)
+            self.name : score
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,12 +22,12 @@
             score = brier_score_loss(y_true=references, y_prob=prediction_scores, sample_weight=sample_weight,pos_label=pos_label)
             score = float(score)
         elif prediction_scores is None:
             score = brier_score_loss(y_true=references, y_prob=predictions, sample_weight=sample_weight,pos_label=pos_label)
             score = float(score)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' :float(score)}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Any
-from sklearn.metrics import class_likelihood_ratios
+from sklearn.metrics import hamming_loss
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-class ClassLikelihoodRatios(MetricBase):
-    name = 'class_likelihood_ratios'
+class HammingLoss(MetricBase):
+    name = 'hamming_loss'
     input_type = 'int'
     output_type: Any = None
     kwargs = { }
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions, sample_weight=None, **kwargs):
+    def compute(self, references, predictions,sample_weight=None, **kwargs):
 
-        score = class_likelihood_ratios(y_true=references, y_pred=predictions,  sample_weight=sample_weight)
+        score = hamming_loss(y_true=references, y_pred=predictions,
+                                sample_weight=sample_weight)
         
         score = {
-            self.name : score
+            self.name : float(score)
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/completeness_score/completeness_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/completeness_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/confusion_matrix/confusion_matrix.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/multilabel_confusion_matrix.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from sklearn.metrics import confusion_matrix
-import numpy as np
+from typing import Any,Dict
+from sklearn.metrics import multilabel_confusion_matrix
 from pureml_evaluate.metrics.metric_base import MetricBase
-from typing import Any
 
-
-class ConfusionMatrix(MetricBase):
-    name = "confusion_matrix"
-    input_type = "int"
+class MultilabelConfusionMatrix(MetricBase):
+    name = 'multilabel_confusion_matrix'
+    input_type = 'int'
     output_type: Any = None
-    kwargs = {}
+    kwargs: Dict = None
+        
 
     def parse_data(self, data):
-
+        
         return data
 
-    def compute(
-        self, references, predictions, normalize="true", sample_weight=None, **kwargs
-    ):
-
-        matrix = confusion_matrix(
-            y_true=references,
-            y_pred=predictions,
-            normalize=normalize,
-            sample_weight=sample_weight,
-        )
 
-        matrix = {self.name: matrix.tolist()}
 
-        return matrix
+    def compute(self, references, predictions, labels=None, sample_weight=None, **kwargs):
+
+        score = multilabel_confusion_matrix(y_true=references, y_pred=predictions, labels=labels,
+                                sample_weight=sample_weight)
+        
+        score = {
+            self.name : score
+            }
+ 
+
+        return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/coverage_error/coverage_error.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/coverage_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-
-from sklearn.metrics import d2_absolute_error_score
+from typing import Any,Dict
+from sklearn.metrics import mean_gamma_deviance
 from pureml_evaluate.metrics.metric_base import MetricBase
-from typing import Any
 
-class D2AbsoluteErrorScore(MetricBase):
-    name = 'd2_absolute_error_score'
+class MeanGammaDeviance(MetricBase):
+    name = 'mean_gamma_deviance'
     input_type = 'int'
     output_type: Any = None
-    kwargs = { }
-        
+    kwargs: Dict = None
+
 
     def parse_data(self, data):
         
         return data
 
 
-
     def compute(self, references, predictions, sample_weight=None, **kwargs):
 
-        score = d2_absolute_error_score(y_true=references, y_pred=predictions,
+        score = mean_gamma_deviance(y_true=references, y_pred=predictions,
                                 sample_weight=sample_weight)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' :float(score) }
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/zero_one_loss.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-
-from sklearn.metrics import d2_pinball_score
+from typing import Any,Dict
+from sklearn.metrics import zero_one_loss
 from pureml_evaluate.metrics.metric_base import MetricBase
-from typing import Any 
 
-class D2PinballScore(MetricBase):
-    name = 'd2_pinball_score'
+class ZeroOneLoss(MetricBase):
+    name = 'zero_one_loss'
     input_type = 'int'
     output_type:Any = None
-    kwargs = {}
+    kwargs:Dict = None
         
 
     def parse_data(self, data):
         
         return data
 
 
-    def compute(self, references, predictions, alpha=0.5, sample_weight=None, **kwargs):
 
-        score = d2_pinball_score(y_true=references, y_pred=predictions, alpha=alpha,
+    def compute(self, references, predictions, normalize=True, sample_weight=None, **kwargs):
+
+        score = zero_one_loss(y_true=references, y_pred=predictions, normalize=normalize,
                                 sample_weight=sample_weight)
         
         score = {
             self.name : float(score)
             }
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
     def compute(self, references, predictions, power=0, sample_weight=None, **kwargs):
 
         score = d2_tweedie_score(y_true=references, y_pred=predictions, power=power,
                                 sample_weight=sample_weight)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' :float(score)}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/dcg_score/dcg_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/dcg_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/det_curve/det_curve.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/det_curve.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 
     def compute(self, references, predictions, sample_weight=None, **kwargs):
 
         score = explained_variance_score(y_true=references, y_pred=predictions,
                                 sample_weight=sample_weight)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' :float(score)}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/f1_score/f1_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from typing import Any
-from sklearn.metrics import f1_score
+from sklearn.metrics import fbeta_score
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-
-class F1(MetricBase):
-
-    name = 'f1'
+class FbetaScore(MetricBase):
+    name = 'fbeta_score'
     input_type = 'int'
     output_type: Any = None
     kwargs = { }
         
 
     def parse_data(self, data):
         
         return data
 
 
+    def compute(self, references, predictions, average='binary', sample_weight=None,beta = 0.5, pos_label=1, **kwargs):
 
-    def compute(self, predictions, references, labels=None, pos_label=1, average="binary", sample_weight=None, **kwargs):
-        
-        score = f1_score(y_true=references, y_pred=predictions, labels=labels, 
-                         pos_label=pos_label, average=average, sample_weight=sample_weight)
+        score = fbeta_score(y_true=references, y_pred=predictions, average=average,
+                                sample_weight=sample_weight, pos_label=pos_label,beta=beta)
         
         score = {
-            self.name : float(score) if score.size == 1 else score
+            self.name : float(score)
             }
+ 
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/r2_score.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from typing import Any
-from sklearn.metrics import fbeta_score
+from typing import Any,Dict
+from sklearn.metrics import r2_score
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-class FbetaScore(MetricBase):
-    name = 'fbeta_score'
+class R2Score(MetricBase):
+    name = 'r2_score'
     input_type = 'int'
     output_type: Any = None
-    kwargs = { }
+    kwargs: Dict = None
         
 
     def parse_data(self, data):
         
         return data
 
 
-    def compute(self, references, predictions, average='binary', sample_weight=None,beta = 0.5, pos_label=1, **kwargs):
 
-        score = fbeta_score(y_true=references, y_pred=predictions, average=average,
-                                sample_weight=sample_weight, pos_label=pos_label,beta=beta)
+    def compute(self, references, predictions, sample_weight=None, multioutput='uniform_average',**kwargs):
+
+        score = r2_score(y_true=references, y_pred=predictions,
+                                sample_weight=sample_weight,multioutput=multioutput)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' : score}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Any
-from sklearn.metrics import hamming_loss
+from typing import Any,Dict
+from sklearn.metrics import mean_absolute_percentage_error
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-class HammingLoss(MetricBase):
-    name = 'hamming_loss'
+class MeanAbsolutePercentageError(MetricBase):
+    name = 'mean_absolute_percentage_error'
     input_type = 'int'
     output_type: Any = None
-    kwargs = { }
+    kwargs: Dict = None
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions,sample_weight=None, **kwargs):
+    def compute(self, references, predictions, sample_weight=None,multioutput = None, **kwargs):
 
-        score = hamming_loss(y_true=references, y_pred=predictions,
-                                sample_weight=sample_weight)
+        score = mean_absolute_percentage_error(y_true=references, y_pred=predictions,
+                                sample_weight=sample_weight,multioutput=multioutput)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' :score}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/accuracy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-from typing import Any
-from sklearn.metrics import jaccard_score
+from sklearn.metrics import accuracy_score
 from pureml_evaluate.metrics.metric_base import MetricBase
+from typing import Any
+import matplotlib.pyplot as plt
 
-class JaccardScore(MetricBase):
-    name = 'jaccard_score'
+class Accuracy(MetricBase):
+    name = 'accuracy'
     input_type = 'int'
-    output_type: Any = None
-    kwargs = { }
+    output_type: Any= None
+    kwargs = {}
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions, pos_label=1, average='binary',
-                 sample_weight=None, **kwargs):
+    def compute(self, references, predictions, normalize=True, sample_weight=None, **kwargs):
 
-        score = jaccard_score(y_true=references, y_pred=predictions, pos_label=pos_label,
-                                average=average, sample_weight=sample_weight)
+        score = accuracy_score(y_true=references, y_pred=predictions, normalize=normalize,
+                                sample_weight=sample_weight)
         
+        # score = {
+        #     self.name : float(score)
+        #     }
+
         score = {
-            self.name : score
-            }
- 
+            self.name : {'value' : float(score)}
+        }
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/log_loss/log_loss.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/log_loss.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,24 +15,27 @@
         return data
 
 
 
     def compute(self, references, predictions=None, prediction_scores=None, sample_weight=None,
                 normalize=True, labels=None, **kwargs):
         
+        #prediction_scores = kwargs.get('prediction_scores',None) #To get prediction_scores from kwargs
+        if 'kwargs' in kwargs and 'prediction_scores' in kwargs['kwargs']:
+            prediction_scores = kwargs['kwargs']['prediction_scores']
         if prediction_scores is None and predictions is None:
             score = None
         elif predictions is None:
             score = log_loss(y_true=references, y_pred=prediction_scores, sample_weight=sample_weight,
                                  normalize=normalize, labels=labels)
             score = float(score)
         elif prediction_scores is None:
             score = log_loss(y_true=references, y_pred=predictions,  sample_weight=sample_weight,
                                 normalize=normalize, labels=labels)
             score = float(score)
         
         score = {
-            self.name : score
+            self.name : {'value' : score}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/max_error/max_error.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/max_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
 
     def compute(self, references, predictions,  **kwargs):
 
         score = max_error(y_true=references, y_pred=predictions)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' : float(score)}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 
 
     def compute(self, predictions, references, sample_weight=None, multioutput="uniform_average", **kwargs):
         
         score = mean_absolute_error(y_true=references, y_pred=predictions, sample_weight=sample_weight, multioutput=multioutput)
         
         score = {
-            self.name : score
+            self.name : {'value' : score }
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any,Dict
-from sklearn.metrics import mean_absolute_percentage_error
+from sklearn.metrics import median_absolute_error
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-class MeanAbsolutePercentageError(MetricBase):
-    name = 'mean_absolute_percentage_error'
+class MedianAbsoluteError(MetricBase):
+    name = 'median_absolute_error'
     input_type = 'int'
     output_type: Any = None
     kwargs: Dict = None
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions, sample_weight=None,multioutput = None, **kwargs):
+    def compute(self, references, predictions, normalize=True, sample_weight=None,multioutput = 'uniform_average', **kwargs):
 
-        score = mean_absolute_percentage_error(y_true=references, y_pred=predictions,
+        score = median_absolute_error(y_true=references, y_pred=predictions,
                                 sample_weight=sample_weight,multioutput=multioutput)
         
         score = {
-            self.name : score
+            self.name : {'value': score}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from typing import Any,Dict
-from sklearn.metrics import mean_gamma_deviance
+from sklearn.metrics import ndcg_score
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-class MeanGammaDeviance(MetricBase):
-    name = 'mean_gamma_deviance'
+class NdcgScore(MetricBase):
+    name = 'ndcg_score'
     input_type = 'int'
-    output_type: Any = None
-    kwargs: Dict = None
-
+    output_type:Any = None
+    kwargs:Dict = None
+        
 
     def parse_data(self, data):
         
         return data
 
 
-    def compute(self, references, predictions, sample_weight=None, **kwargs):
 
-        score = mean_gamma_deviance(y_true=references, y_pred=predictions,
+    def compute(self, references, predictions=None, prediction_scores=None, k=None, sample_weight=None, **kwargs):
+        
+        if prediction_scores is None and predictions is None:
+            score = None
+        elif predictions is None:
+            score = ndcg_score(y_true=references, y_score=prediction_scores, k=k,
                                 sample_weight=sample_weight)
+            score = float(score)
+        elif prediction_scores is None:
+            score = ndcg_score(y_true=references, y_score=predictions, k=k,
+                                sample_weight=sample_weight)
+            score = float(score)
+        
         
         score = {
             self.name : float(score)
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 
     def compute(self, references, predictions, sample_weight=None, **kwargs):
 
         score = mean_poisson_deviance(y_true=references, y_pred=predictions, 
                                 sample_weight=sample_weight)
         
         score = {
-            self.name : float(score)
+            self.name : {'value' :float(score)}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
     def compute(self, predictions, references, sample_weight=None, multioutput="uniform_average", squared=True, **kwargs):
 
         score = mean_squared_error(y_true=references, y_pred=predictions, sample_weight=sample_weight,
                                     multioutput=multioutput, squared=squared)
         
         score = {
-            self.name : score
+            self.name : {'value': score}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 
     def compute(self, references, predictions, squared=True, sample_weight=None,multioutput = None, **kwargs):
 
         score = mean_squared_log_error(y_true=references, y_pred=predictions, squared=squared,
                                 sample_weight=sample_weight,multioutput=multioutput)
         
         score = {
-            self.name : score
+            self.name : {'value': score}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from typing import Any,Dict
-from sklearn.metrics import median_absolute_error
+
+from sklearn.metrics import d2_absolute_error_score
 from pureml_evaluate.metrics.metric_base import MetricBase
+from typing import Any
 
-class MedianAbsoluteError(MetricBase):
-    name = 'median_absolute_error'
+class D2AbsoluteErrorScore(MetricBase):
+    name = 'd2_absolute_error_score'
     input_type = 'int'
     output_type: Any = None
-    kwargs: Dict = None
+    kwargs = { }
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions, normalize=True, sample_weight=None,multioutput = 'uniform_average', **kwargs):
+    def compute(self, references, predictions, sample_weight=None, **kwargs):
 
-        score = median_absolute_error(y_true=references, y_pred=predictions,
-                                sample_weight=sample_weight,multioutput=multioutput)
+        score = d2_absolute_error_score(y_true=references, y_pred=predictions,
+                                sample_weight=sample_weight)
         
         score = {
-            self.name : score
+            self.name : {'value' :float(score)}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/top_k_accuracy_score.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from typing import Any,Dict
-from sklearn.metrics import ndcg_score
+from sklearn.metrics import top_k_accuracy_score
 from pureml_evaluate.metrics.metric_base import MetricBase
 
-class NdcgScore(MetricBase):
-    name = 'ndcg_score'
+class TopKAccuracyScore(MetricBase):
+    name = 'top_k_accuracy_score'
     input_type = 'int'
-    output_type:Any = None
-    kwargs:Dict = None
+    output_type: Any = None
+    kwargs: Dict = None
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions=None, prediction_scores=None, k=None, sample_weight=None, **kwargs):
-        
+    def compute(self, references, predictions=None, prediction_scores=None, normalize=True, sample_weight=None, **kwargs):
+
+        #prediction_scores = kwargs.get('prediction_scores',None)
+        if 'kwargs' in kwargs and 'prediction_scores' in kwargs['kwargs']:
+            prediction_scores = kwargs['kwargs']['prediction_scores']
         if prediction_scores is None and predictions is None:
             score = None
         elif predictions is None:
-            score = ndcg_score(y_true=references, y_score=prediction_scores, k=k,
+            score = top_k_accuracy_score(y_true=references, y_score=prediction_scores, normalize=normalize,
                                 sample_weight=sample_weight)
             score = float(score)
         elif prediction_scores is None:
-            score = ndcg_score(y_true=references, y_score=predictions, k=k,
+            score = top_k_accuracy_score(y_true=references, y_score=predictions, normalize=normalize,
                                 sample_weight=sample_weight)
             score = float(score)
         
-        
         score = {
-            self.name : float(score)
+            self.name : {'value' : score}
             }
  
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_distances/paired_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/paired_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision/precision.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/precision.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,22 @@
         return data
 
 
 
     def compute(self, predictions, references, labels=None, pos_label=1, average="binary", sample_weight=None,
                  zero_division="warn", **kwargs):
         
+        if 'kwargs' in kwargs and 'average' in kwargs['kwargs']:
+            average = kwargs['kwargs']['average']
+        
         score = precision_score(y_true=references, y_pred=predictions, labels=labels, pos_label=pos_label,
                                  average=average, sample_weight=sample_weight, zero_division=zero_division)
         
-        score = {
-            self.name : float(score) if score.size == 1 else score
-            }
+        # score = {
+        #     self.name : float(score) if score.size == 1 else score
+        #     }
 
+        score = {
+            self.name : {'value' : float(score) if score.size == 1 else score}
+        }
+        
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/recall/recall.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import Any,Dict
-from sklearn.metrics import recall_score
-from pureml_evaluate.metrics.metric_base import MetricBase
-
 
-class Recall(MetricBase):
+from sklearn.metrics import d2_pinball_score
+from pureml_evaluate.metrics.metric_base import MetricBase
+from typing import Any 
 
-    name = 'recall'
+class D2PinballScore(MetricBase):
+    name = 'd2_pinball_score'
     input_type = 'int'
-    output_type: Any = None
-    kwargs: Dict = None
+    output_type:Any = None
+    kwargs = {}
         
 
     def parse_data(self, data):
         
         return data
 
 
+    def compute(self, references, predictions, alpha=0.5, sample_weight=None, **kwargs):
 
-    def compute(self, predictions, references, labels=None, pos_label=1, average="binary", 
-                sample_weight=None, zero_division="warn", **kwargs):
-        
-        score = recall_score(y_true=references, y_pred=predictions, labels=labels, pos_label=pos_label, 
-                             average=average, sample_weight=sample_weight, zero_division=zero_division)
+        score = d2_pinball_score(y_true=references, y_pred=predictions, alpha=alpha,
+                                sample_weight=sample_weight)
         
         score = {
-            self.name : float(score) if score.size == 1 else score
+            self.name : {'value' : float(score) }
             }
+ 
 
         return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_auc/roc_auc.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/roc_auc.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,36 +3,60 @@
 from typing import Any,Dict
 
 class ROC_AUC(MetricBase):
 
     name = 'roc_auc'
     input_type = 'float'
     output_type: Any = None
-    kwargs: Dict = None
+    kwargs: Dict = { }
         
 
     def parse_data(self, data):
         
         return data
 
 
 
-    def compute(self, references, predictions=None, prediction_scores=None, average="macro", sample_weight=None,
-                max_fpr=None, multi_class="raise", labels=None, **kwargs):
+    # def compute(self, references, predictions=None, prediction_scores=None, average="macro", sample_weight=None,
+    #             max_fpr=None, multi_class="raise", labels=None, **kwargs):
         
-        if prediction_scores is None and predictions is None:
-            score = None
-        elif predictions is None:
-            score = roc_auc_score(y_true=references, y_score=prediction_scores, average=average, sample_weight=sample_weight,
-                                multi_class=multi_class, max_fpr=max_fpr, labels=labels)
-            score = float(score)
-        elif prediction_scores is None:
-            score = roc_auc_score(y_true=references, y_score=predictions, average=average, sample_weight=sample_weight,
-                                multi_class=multi_class, max_fpr=max_fpr, labels=labels)
-            score = float(score)
+    #     if prediction_scores is None and predictions is None:
+    #         score = None
+    #     elif predictions is None:
+    #         score = roc_auc_score(y_true=references, y_score=prediction_scores, average=average, sample_weight=sample_weight,
+    #                             multi_class=multi_class, max_fpr=max_fpr, labels=labels)
+    #         score = float(score)
+    #     elif prediction_scores is None:
+    #         score = roc_auc_score(y_true=references, y_score=predictions, average=average, sample_weight=sample_weight,
+    #                             multi_class=multi_class, max_fpr=max_fpr, labels=labels)
+    #         score = float(score)
         
-        score = {
-            self.name : score
-            }
- 
+    #     score = {
+    #         self.name : score
+    #         }
+    def compute(self, references, predictions=None, prediction_scores=None, average="macro", sample_weight=None,
+            max_fpr=None, multi_class="raise", labels=None, **kwargs):
+
+            if 'kwargs' in kwargs and 'average' in kwargs['kwargs']:
+                 average = kwargs['kwargs']['average']
+                 #prediction_scores = kwargs['kwargs']['prediction_scores']
+                 multi_class = 'ovo'
+            
+            if prediction_scores is None and predictions is None:
+                score = None
+            elif predictions is None:
+                score = roc_auc_score(y_true=references, y_score=prediction_scores, average=average,
+                                    sample_weight=sample_weight, multi_class=multi_class, max_fpr=max_fpr, labels=labels)
+                score = float(score)
+                
+            elif prediction_scores is None:
+                score = roc_auc_score(y_true=references, y_score=predictions, average=average,
+                                    sample_weight=sample_weight, multi_class=multi_class, max_fpr=max_fpr, labels=labels)
+                score = float(score)
+            
+            score = {self.name: {'value' : score}
+                                 }
+
+            return score
+
 
-        return score
+        #return score
```

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/roc_curve/roc_curve.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/roc_curve.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py` & `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.1/pyproject.toml` & `pureml_evaluate-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [tool.poetry]
 name = "pureml-evaluate"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 
 packages = [{include = "pureml_evaluate"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 scikit-learn = "^1.2.2"
 fairlearn = "^0.8.0"
 joblib = "^1.2.0"
+daisy = "^1.0"
+scipy = "^1.11.1"
+pandas = "^1.4.3"
+reportlab = "^4.0.4"
+seaborn = "^0.12.2"
+PyPDF2 = "^3.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pureml_evaluate-0.0.1/PKG-INFO` & `pureml_evaluate-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: pureml-evaluate
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyPDF2 (>=3.0.1,<4.0.0)
+Requires-Dist: daisy (>=1.0,<2.0)
 Requires-Dist: fairlearn (>=0.8.0,<0.9.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: reportlab (>=4.0.4,<5.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: scipy (>=1.11.1,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Description-Content-Type: text/markdown
```


# Comparing `tmp/lale-0.7.7.tar.gz` & `tmp/lale-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lale-0.7.7.tar", last modified: Fri Mar 31 14:57:04 2023, max compression
+gzip compressed data, was "dist/lale-0.7.8.tar", last modified: Tue Apr 18 22:19:27 2023, max compression
```

## Comparing `lale-0.7.7.tar` & `lale-0.7.8.tar`

### file list

```diff
@@ -1,390 +1,390 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-03-31 14:57:04.000000 lale-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-03-31 14:56:52.000000 lale-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-31 14:56:52.000000 lale-0.7.7/lale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/data_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/movie_review.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/datasets/multitable/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/multitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/multitable/fetch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/multitable/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/datasets/openml/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/openml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26859 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/openml/openml_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/sklearn_to_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/datasets/uci/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/uci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/uci/uci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-31 14:56:52.000000 lale-0.7.7/lale/datasets/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-03-31 14:56:52.000000 lale-0.7.7/lale/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-03-31 14:56:52.000000 lale-0.7.7/lale/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-03-31 14:56:52.000000 lale-0.7.7/lale/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)    46947 2023-03-31 14:56:52.000000 lale-0.7.7/lale/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-03-31 14:56:52.000000 lale-0.7.7/lale/json_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/_common_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/aif360/
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/_suppress_aif360_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/adversarial_debiasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/calibrated_eq_odds_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    50557 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/disparate_impact_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/eq_odds_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/gerry_fair_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/lfr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/meta_fair_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/optim_preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/orbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/prejudice_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/protected_attributes_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/redacting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/reject_option_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/reweighing.py
--rw-r--r--   0 runner    (1001) docker     (123)    85188 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/aif360/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/autoai_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/_common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/boolean2float.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/cat_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/cat_imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/column_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/compress_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/date_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/float32_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/float_str2_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/fs1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/fs2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/num_imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/numpy_column_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/numpy_permute_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/numpy_replace_missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/numpy_replace_unknown_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/opt_standard_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/t_no_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/ta1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/ta2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/tam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/tb1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/tb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/text_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/tgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autoai_libs/word2vec_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/additive_chi2_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/ard_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/bayesian_ridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/bernoulli_nb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/bernoulli_rbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/binarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/birch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/calibrated_classifier_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/complement_nb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/dictionary_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/elastic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/elastic_net_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/factor_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/gaussian_process_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/gaussian_process_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/gaussian_random_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/huber_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/k_bins_discretizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/kernel_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/kernel_ridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/label_binarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/label_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/label_spreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/lars_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/lasso_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/lasso_lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/lasso_lars_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/lasso_lars_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/latent_dirichlet_allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/linear_discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/locally_linear_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/logistic_regression_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/max_abs_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/mini_batch_dictionary_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/mini_batch_k_means.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/mini_batch_sparse_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/mlp_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/multi_label_binarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/multi_task_elastic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/multi_task_elastic_net_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/multi_task_lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/multi_task_lasso_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/nearest_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/nu_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/nu_svr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/orthogonal_matching_pursuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/orthogonal_matching_pursuit_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/passive_aggressive_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/pls_canonical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/plssvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/power_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/radius_neighbors_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/radius_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/random_trees_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/ransac_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/rbf_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/ridge_classifier_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/ridge_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/skewed_chi2_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/sparse_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/sparse_random_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/theil_sen_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/transformed_target_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/autogen/truncated_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/category_encoders/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/category_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/category_encoders/hashing_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/category_encoders/target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/imblearn/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/_common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/adasyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/all_knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/base_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/borderline_smote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/condensed_nearest_neighbour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/edited_nearest_neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/instance_hardness_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/random_over_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/repeated_edited_nearest_neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/smote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/smoteenn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/smoten.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/smotenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/imblearn/svm_smote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/lale/
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/auto_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/both.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/concat_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/grid_search_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/halving_grid_search_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    24787 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/identity_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/no_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/observing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/optimize_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/optimize_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/sample_based_voting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/smac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/time_series_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lale/topk_voting_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/lightgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lightgbm/lgbm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/lightgbm/lgbm_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/rasl/
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/_eval_pandas_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/_eval_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/batched_bagging_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/batching.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/concat_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/group_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/hashing_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/join.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/min_max_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/monoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/orderby.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/ordinal_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/relational.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/select_k_best.py
--rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/simple_imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/sort_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/spark_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/split_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/standard_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    57880 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/rasl/task_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/_common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/ada_boost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/ada_boost_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/bagging_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/bagging_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/decision_tree_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/dummy_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/dummy_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/extra_trees_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/extra_trees_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/feature_agglomeration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/fit_spec_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/gaussian_nb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21170 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/gradient_boosting_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18271 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/isolation_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/isomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/k_means.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/k_neighbors_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/k_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/linear_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/linear_svr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/min_max_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/missing_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/mlp_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/multi_output_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/multinomial_nb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/nystroem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/ordinal_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/passive_aggressive_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/polynomial_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/quadratic_discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/quantile_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/random_forest_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/rfe.py
--rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/ridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/ridge_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/robust_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/select_k_best.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/sgd_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/sgd_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/simple_imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/stacking_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/stacking_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/stacking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/standard_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/svr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/tfidf_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/variance_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/voting_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/sklearn/voting_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/snapml/
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/batched_tree_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/batched_tree_ensemble_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_boosting_machine_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_boosting_machine_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_decision_tree_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_random_forest_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/snapml/snap_svm_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/lib/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/xgboost/_common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    33375 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/xgboost/xgb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-03-31 14:56:52.000000 lale-0.7.7/lale/lib/xgboost/xgb_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-03-31 14:56:52.000000 lale-0.7.7/lale/operator_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)   213691 2023-03-31 14:56:52.000000 lale-0.7.7/lale/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    29239 2023-03-31 14:56:52.000000 lale-0.7.7/lale/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:56:52.000000 lale-0.7.7/lale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-03-31 14:56:52.000000 lale-0.7.7/lale/schema2enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-03-31 14:56:52.000000 lale-0.7.7/lale/schema_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)    43964 2023-03-31 14:56:52.000000 lale-0.7.7/lale/schema_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-03-31 14:56:52.000000 lale-0.7.7/lale/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-03-31 14:56:52.000000 lale-0.7.7/lale/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/search/
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/PGO.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/lale_grid_search_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    19805 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/lale_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/lale_smac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/op2hp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23807 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/schema2search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-03-31 14:56:52.000000 lale-0.7.7/lale/search/search_space_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-31 14:56:52.000000 lale-0.7.7/lale/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-31 14:56:52.000000 lale-0.7.7/lale/sklearn_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-03-31 14:56:52.000000 lale-0.7.7/lale/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/Visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/VisitorMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/VisitorPathError.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/batch_data_dictionary_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/hdf5_to_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/numpy_to_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/numpy_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/pandas_to_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-31 14:56:52.000000 lale-0.7.7/lale/util/pandas_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-03-31 14:56:52.000000 lale-0.7.7/lale/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/lale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-03-31 14:57:03.000000 lale-0.7.7/lale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-03-31 14:57:04.000000 lale-0.7.7/lale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:57:03.000000 lale-0.7.7/lale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-31 14:57:03.000000 lale-0.7.7/lale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 14:57:03.000000 lale-0.7.7/lale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 14:57:04.000000 lale-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-31 14:56:52.000000 lale-0.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:57:04.000000 lale-0.7.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-31 14:56:52.000000 lale-0.7.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-03-31 14:56:52.000000 lale-0.7.7/test/mock_custom_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-31 14:56:52.000000 lale-0.7.7/test/mock_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    57014 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_aif360.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_aif360_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_autoai_libs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_autoai_output_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_autogen_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_core_classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    49238 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_core_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    48983 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_core_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_core_regressors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_core_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27885 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_custom_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_halving_gridsearchcv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_interoperability.py
--rw-r--r--   0 runner    (1001) docker     (123)    63329 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_json_pretty_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_lale_lib_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_nlp_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    43526 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_pgo.py
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)   110818 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_relational.py
--rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_relational_from_sklearn_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)   103433 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_relational_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_sklearn_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_snapml.py
--rw-r--r--   0 runner    (1001) docker     (123)    58526 2023-03-31 14:56:52.000000 lale-0.7.7/test/test_type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-18 22:19:27.000000 lale-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-18 22:19:16.000000 lale-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-18 22:19:16.000000 lale-0.7.8/lale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/data_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/movie_review.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/datasets/multitable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/multitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/multitable/fetch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/multitable/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/datasets/openml/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/openml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26859 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/openml/openml_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/sklearn_to_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/datasets/uci/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/uci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/uci/uci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-18 22:19:16.000000 lale-0.7.8/lale/datasets/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-04-18 22:19:16.000000 lale-0.7.8/lale/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-04-18 22:19:16.000000 lale-0.7.8/lale/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-18 22:19:16.000000 lale-0.7.8/lale/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46947 2023-04-18 22:19:16.000000 lale-0.7.8/lale/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-04-18 22:19:16.000000 lale-0.7.8/lale/json_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/_common_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/aif360/
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/_suppress_aif360_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/adversarial_debiasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/calibrated_eq_odds_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50557 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/disparate_impact_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/eq_odds_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/gerry_fair_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/lfr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/meta_fair_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/optim_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/prejudice_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/protected_attributes_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/redacting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/reject_option_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/reweighing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85188 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/aif360/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/autoai_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/_common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/boolean2float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/cat_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/cat_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/column_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/compress_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/date_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/float32_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/float_str2_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/fs1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/fs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/num_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/numpy_column_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/numpy_permute_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/numpy_replace_missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/numpy_replace_unknown_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/opt_standard_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/t_no_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/ta1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/ta2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/tam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/tb1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/tb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/text_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/tgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autoai_libs/word2vec_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/additive_chi2_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/ard_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/bayesian_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/bernoulli_nb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/bernoulli_rbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/birch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/calibrated_classifier_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/complement_nb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/dictionary_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/elastic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/elastic_net_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/factor_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/gaussian_process_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/gaussian_process_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/gaussian_random_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/huber_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/incremental_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/k_bins_discretizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/kernel_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/kernel_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/label_binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/label_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/label_spreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/lars_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/lasso_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/lasso_lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/lasso_lars_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/lasso_lars_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/latent_dirichlet_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/linear_discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/locally_linear_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/logistic_regression_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/max_abs_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/mini_batch_dictionary_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/mini_batch_k_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/mini_batch_sparse_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/mlp_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/multi_label_binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/multi_task_elastic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/multi_task_elastic_net_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/multi_task_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/multi_task_lasso_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/nearest_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/nu_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/nu_svr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/orthogonal_matching_pursuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/orthogonal_matching_pursuit_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/passive_aggressive_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/pls_canonical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/plssvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/power_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/radius_neighbors_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/radius_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/random_trees_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/ransac_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/rbf_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/ridge_classifier_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/ridge_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/skewed_chi2_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/sparse_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/sparse_random_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/theil_sen_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/transformed_target_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/autogen/truncated_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/category_encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/category_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/category_encoders/hashing_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/category_encoders/target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/imblearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/_common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/adasyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/all_knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/base_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/borderline_smote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/condensed_nearest_neighbour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/edited_nearest_neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/instance_hardness_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/random_over_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/repeated_edited_nearest_neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/smote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/smoteenn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/smoten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/smotenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/imblearn/svm_smote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/lale/
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/auto_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/both.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/concat_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/grid_search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/halving_grid_search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24787 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/identity_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/no_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/observing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/optimize_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/optimize_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/sample_based_voting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/smac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/time_series_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lale/topk_voting_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lightgbm/lgbm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/lightgbm/lgbm_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/rasl/
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/_eval_pandas_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/_eval_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/batched_bagging_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/batching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/concat_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/group_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/hashing_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/min_max_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/monoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/orderby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/ordinal_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/relational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/select_k_best.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/simple_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/sort_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/spark_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/split_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/standard_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57980 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/rasl/task_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/_common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/ada_boost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/ada_boost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/bagging_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/bagging_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/decision_tree_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/dummy_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/dummy_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/extra_trees_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/extra_trees_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/feature_agglomeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/fit_spec_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/gaussian_nb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21170 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/gradient_boosting_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18271 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/isolation_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/isomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/k_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/k_neighbors_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/k_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/linear_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/linear_svr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/min_max_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/missing_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/mlp_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/multi_output_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/multinomial_nb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/nystroem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/ordinal_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/passive_aggressive_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/polynomial_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/quadratic_discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/quantile_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/random_forest_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/rfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/ridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/ridge_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/robust_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/select_k_best.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/sgd_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/sgd_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/simple_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/stacking_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/stacking_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/stacking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/standard_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/svr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/tfidf_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/variance_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/voting_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/sklearn/voting_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/snapml/
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/batched_tree_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/batched_tree_ensemble_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_boosting_machine_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_boosting_machine_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_decision_tree_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_random_forest_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/snapml/snap_svm_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/lib/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/xgboost/_common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33375 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/xgboost/xgb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-04-18 22:19:16.000000 lale-0.7.8/lale/lib/xgboost/xgb_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-04-18 22:19:16.000000 lale-0.7.8/lale/operator_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213691 2023-04-18 22:19:16.000000 lale-0.7.8/lale/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29239 2023-04-18 22:19:16.000000 lale-0.7.8/lale/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:16.000000 lale-0.7.8/lale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-18 22:19:16.000000 lale-0.7.8/lale/schema2enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-04-18 22:19:16.000000 lale-0.7.8/lale/schema_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43964 2023-04-18 22:19:16.000000 lale-0.7.8/lale/schema_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-18 22:19:16.000000 lale-0.7.8/lale/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-18 22:19:16.000000 lale-0.7.8/lale/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/search/
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/PGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/lale_grid_search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19805 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/lale_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/lale_smac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/op2hp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23807 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/schema2search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-18 22:19:16.000000 lale-0.7.8/lale/search/search_space_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-18 22:19:16.000000 lale-0.7.8/lale/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 22:19:16.000000 lale-0.7.8/lale/sklearn_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-18 22:19:16.000000 lale-0.7.8/lale/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/VisitorMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/VisitorPathError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/batch_data_dictionary_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/hdf5_to_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/numpy_to_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/numpy_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/pandas_to_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-18 22:19:16.000000 lale-0.7.8/lale/util/pandas_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-04-18 22:19:16.000000 lale-0.7.8/lale/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/lale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-18 22:19:27.000000 lale-0.7.8/lale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-04-18 22:19:27.000000 lale-0.7.8/lale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:19:27.000000 lale-0.7.8/lale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-18 22:19:27.000000 lale-0.7.8/lale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 22:19:27.000000 lale-0.7.8/lale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:19:27.000000 lale-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-18 22:19:16.000000 lale-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:19:27.000000 lale-0.7.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-18 22:19:17.000000 lale-0.7.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-04-18 22:19:17.000000 lale-0.7.8/test/mock_custom_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-18 22:19:17.000000 lale-0.7.8/test/mock_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57014 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_aif360.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_aif360_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_autoai_libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_autoai_output_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_autogen_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_core_classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49238 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_core_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48983 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_core_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_core_regressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_core_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27885 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_custom_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_halving_gridsearchcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_interoperability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64209 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_json_pretty_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_lale_lib_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_nlp_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43526 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_pgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110818 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_relational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_relational_from_sklearn_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103433 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_relational_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_sklearn_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_snapml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58526 2023-04-18 22:19:17.000000 lale-0.7.8/test/test_type_checking.py
```

### Comparing `lale-0.7.7/PKG-INFO` & `lale-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lale
-Version: 0.7.7
+Version: 0.7.8
 Summary: Library for Semi-Automated Data Science
 Home-page: https://github.com/IBM/lale
 Author: Guillaume Baudart, Martin Hirzel, Kiran Kate, Parikshit Ram, Avraham Shinnar
 License: Apache License 2.0
 Description: # Lale
         
         [![Tests](https://github.com/IBM/lale/workflows/Tests/badge.svg?branch=master)](https://github.com/IBM/lale/actions?query=workflow%3ATests+branch%3Amaster)
```

### Comparing `lale-0.7.7/README.md` & `lale-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/__init__.py` & `lale-0.7.8/lale/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
-__version__ = "0.7.7"
+__version__ = "0.7.8"
 
 try:
     # This variable is injected in the __builtins__ by the build
     # process. It is used to not try to import rest of the lale packages when
     # it is being installed.
     __LALE_SETUP__  # type: ignore  # pylint:disable=used-before-assignment
 except NameError:
```

### Comparing `lale-0.7.7/lale/datasets/__init__.py` & `lale-0.7.8/lale/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/data_schemas.py` & `lale-0.7.8/lale/datasets/data_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/movie_review.py` & `lale-0.7.8/lale/datasets/movie_review.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         print(f"created directory {download_data_dir}")
         # this request is to a hardcoded https url, so does not risk leaking local data
         urllib.request.urlretrieve(download_base_url, data_file_path)  # nosec
 
     X = []
     y = []
     with tarfile.open(data_file_path) as data_file:
-        data_file.extractall(path=download_data_dir)
+        data_file.extractall(path=download_data_dir)  # nosec B202
 
     with open(
         os.path.join(download_data_dir, "rt-polaritydata", "rt-polarity.neg"), "rb"
     ) as neg_data_file:
         for line in neg_data_file.readlines():
             X.append(str(line))
             y.append(-1)
```

### Comparing `lale-0.7.7/lale/datasets/multitable/__init__.py` & `lale-0.7.8/lale/datasets/multitable/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/multitable/fetch_datasets.py` & `lale-0.7.8/lale/datasets/multitable/fetch_datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/multitable/util.py` & `lale-0.7.8/lale/datasets/multitable/util.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/openml/__init__.py` & `lale-0.7.8/lale/datasets/openml/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/openml/openml_datasets.py` & `lale-0.7.8/lale/datasets/openml/openml_datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/sklearn_to_pandas.py` & `lale-0.7.8/lale/datasets/sklearn_to_pandas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/uci/uci_datasets.py` & `lale-0.7.8/lale/datasets/uci/uci_datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/datasets/util.py` & `lale-0.7.8/lale/datasets/util.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/docstrings.py` & `lale-0.7.8/lale/docstrings.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/expressions.py` & `lale-0.7.8/lale/expressions.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/grammar.py` & `lale-0.7.8/lale/grammar.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/helpers.py` & `lale-0.7.8/lale/helpers.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/json_operator.py` & `lale-0.7.8/lale/json_operator.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/__init__.py` & `lale-0.7.8/lale/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/_common_schemas.py` & `lale-0.7.8/lale/lib/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/__init__.py` & `lale-0.7.8/lale/lib/aif360/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/_suppress_aif360_warnings.py` & `lale-0.7.8/lale/lib/aif360/_suppress_aif360_warnings.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/adversarial_debiasing.py` & `lale-0.7.8/lale/lib/aif360/adversarial_debiasing.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/calibrated_eq_odds_postprocessing.py` & `lale-0.7.8/lale/lib/aif360/calibrated_eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/datasets.py` & `lale-0.7.8/lale/lib/aif360/datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/disparate_impact_remover.py` & `lale-0.7.8/lale/lib/aif360/disparate_impact_remover.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/eq_odds_postprocessing.py` & `lale-0.7.8/lale/lib/aif360/eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/gerry_fair_classifier.py` & `lale-0.7.8/lale/lib/aif360/gerry_fair_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/lfr.py` & `lale-0.7.8/lale/lib/aif360/lfr.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/meta_fair_classifier.py` & `lale-0.7.8/lale/lib/aif360/meta_fair_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/optim_preproc.py` & `lale-0.7.8/lale/lib/aif360/optim_preproc.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/orbit.py` & `lale-0.7.8/lale/lib/aif360/orbit.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/prejudice_remover.py` & `lale-0.7.8/lale/lib/aif360/prejudice_remover.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/protected_attributes_encoder.py` & `lale-0.7.8/lale/lib/aif360/protected_attributes_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/redacting.py` & `lale-0.7.8/lale/lib/aif360/redacting.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/reject_option_classification.py` & `lale-0.7.8/lale/lib/aif360/reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/reweighing.py` & `lale-0.7.8/lale/lib/aif360/reweighing.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/aif360/util.py` & `lale-0.7.8/lale/lib/aif360/util.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/__init__.py` & `lale-0.7.8/lale/lib/autoai_libs/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/_common_schemas.py` & `lale-0.7.8/lale/lib/autoai_libs/_common_schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,15 @@
             },
         },
         {
             "description": "If None, the column types are discovered.",
             "enum": [None],
         },
     ],
+    "transient": "alwaysPrint",  # since positional argument
     "default": None,
 }
 
 _hparam_sklearn_version_family: JSON_TYPE = {
     "description": "The sklearn version for backward compatibility with versions 019 and 020dev. Currently unused.",
     "enum": ["20", "21", "22", "23", "24", None, "1"],
     "default": None,
@@ -92,74 +93,82 @@
         "default": None,
     }
 
 
 _hparam_fs_cols_ids_must_keep: JSON_TYPE = {
     "description": "Serial numbers of the columns that must be kept irrespective of their feature importance.",
     "laleType": "Any",  # Found a value `range(0, 20)`
+    "transient": "alwaysPrint",  # since positional argument
     "default": [],
 }
 
 _hparams_fs_additional_col_count_to_keep: JSON_TYPE = {
     "description": "How many columns need to be retained.",
     "type": "integer",
+    "transient": "alwaysPrint",  # since positional argument
     "minimum": 0,
 }
 
 _hparams_fs_ptype: JSON_TYPE = {
     "description": "Problem type.",
     "enum": ["classification", "regression"],
+    "transient": "alwaysPrint",  # since positional argument
     "default": "classification",
 }
 
 
 def _hparams_column_index_list(description: str) -> JSON_TYPE:
     return {
         "description": description,
         "anyOf": [
             {"type": "array", "items": {"type": "integer", "minimum": 0}},
             {"enum": [None]},
         ],
+        "transient": "alwaysPrint",  # since positional argument
         "default": None,
     }
 
 
 _hparams_transformer_name: JSON_TYPE = {
     "description": "A string name that uniquely identifies this transformer from others.",
     "anyOf": [{"type": "string"}, {"enum": [None]}],
+    "transient": "alwaysPrint",  # since positional argument
     "default": None,
 }
 
 
 def _hparams_fun_pointer(description: str) -> JSON_TYPE:
     return {
         "description": description,
         "laleType": "Any",
+        "transient": "alwaysPrint",  # since positional argument
         "default": None,
     }
 
 
 _hparams_datatype_spec: JSON_TYPE = {"type": "array", "items": {"type": "string"}}
 
 
 def _hparams_datatypes(description: str) -> JSON_TYPE:
     return {
         "description": description,
         "anyOf": [
             _hparams_datatype_spec,
             {"enum": [None]},
         ],
+        "transient": "alwaysPrint",  # since positional argument
         "default": None,
     }
 
 
 def _hparams_feat_constraints(description: str) -> JSON_TYPE:
     return {
         "description": description,
         "laleType": "Any",
+        "transient": "alwaysPrint",  # since positional argument
         "default": None,
     }
 
 
 _hparams_tgraph: JSON_TYPE = {
     "description": "Should be the invoking TGraph() object.",
     "anyOf": [
@@ -192,9 +201,10 @@
     "anyOf": [{"type": "object"}, {"enum": [None]}],
     "default": None,
 }
 
 _hparams_tans_class: JSON_TYPE = {
     "description": "A class that implements fit() and transform() in accordance with the transformation function definition.",
     "laleType": "Any",
+    "transient": "alwaysPrint",  # since positional argument
     "default": None,
 }
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/boolean2float.py` & `lale-0.7.8/lale/lib/autoai_libs/boolean2float.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/cat_encoder.py` & `lale-0.7.8/lale/lib/autoai_libs/cat_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 IBM Corporation
+# Copyright 2020-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -90,14 +90,15 @@
                 "encode_unknown_with",
             ],
             "relevantToOptimizer": ["encoding"],
             "properties": {
                 "encoding": {
                     "description": "The type of encoding to use.",
                     "enum": ["onehot", "ordinal"],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": "ordinal",
                 },
                 "categories": {
                     "description": "Categories (unique values) per feature.",
                     "anyOf": [
                         {
                             "description": "Determine categories automatically from training data.",
@@ -117,28 +118,31 @@
                                         "items": {"type": "number"},
                                         "description": "Should be sorted.",
                                     },
                                 ]
                             },
                         },
                     ],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": "auto",
                 },
                 "dtype": {
                     "description": "Desired dtype of output, must be number. See https://docs.scipy.org/doc/numpy-1.14.0/reference/arrays.scalars.html#arrays-scalars-built-in",
                     "laleType": "Any",
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": "float64",
                 },
                 "handle_unknown": {
                     "description": """Whether to raise an error or ignore if an unknown categorical feature is present during transform.
 When this parameter is set to `ignore` and an unknown category is encountered during transform,
 the resulting one-hot encoded columns for this feature will be all zeros for encoding 'onehot' and
 the resulting encoding with be set to the value indicated by `encode_unknown_with` for encoding 'ordinal'.
 In the inverse transform, an unknown category will be denoted as None.""",
                     "enum": ["error", "ignore"],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": "ignore",
                 },
                 "sklearn_version_family": _hparam_sklearn_version_family,
                 "activate_flag": _hparam_activate_flag_unmodified,
                 "encode_unknown_with": {
                     "description": """When an unknown categorical feature value is found during transform, and 'handle_unknown' is
 set to 'ignore', and encoding is 'ordinal', that value is encoded with this value. Default of 'auto' sets it to an integer equal to n+1, where
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/cat_imputer.py` & `lale-0.7.8/lale/lib/autoai_libs/cat_imputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2022 IBM Corporation
+# Copyright 2020-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -68,24 +68,26 @@
                             "description": "Replace using most frequent value each column. Used with strings or numeric data.",
                         },
                         {
                             "enum": ["constant"],
                             "description": "Replace with fill_value. Can be used with strings or numeric data.",
                         },
                     ],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": "mean",
                 },
                 "missing_values": {
                     "description": "The placeholder for the missing values. All occurrences of missing_values will be imputed.",
                     "anyOf": [
                         {"type": "number"},
                         {"type": "string"},
                         {"enum": [np.nan]},
                         {"enum": [None]},
                     ],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": np.nan,
                 },
                 "sklearn_version_family": _hparam_sklearn_version_family,
                 "activate_flag": _hparam_activate_flag_unmodified,
             },
         }
     ]
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/column_selector.py` & `lale-0.7.8/lale/lib/autoai_libs/column_selector.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/compress_strings.py` & `lale-0.7.8/lale/lib/autoai_libs/compress_strings.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/date_transformer.py` & `lale-0.7.8/lale/lib/autoai_libs/date_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/float32_transform.py` & `lale-0.7.8/lale/lib/autoai_libs/float32_transform.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/float_str2_float.py` & `lale-0.7.8/lale/lib/autoai_libs/float_str2_float.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 IBM Corporation
+# Copyright 2020-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/fs1.py` & `lale-0.7.8/lale/lib/autoai_libs/fs1.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/fs2.py` & `lale-0.7.8/lale/lib/autoai_libs/fs2.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
             "properties": {
                 "cols_ids_must_keep": _hparam_fs_cols_ids_must_keep,
                 "additional_col_count_to_keep": _hparams_fs_additional_col_count_to_keep,
                 "ptype": _hparams_fs_ptype,
                 "eval_algo": {
                     "description": "A supervised model where fit() sets `feature_importances_`.",
                     "laleType": "Any",
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": None,
                 },
             },
         }
     ]
 }
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/num_imputer.py` & `lale-0.7.8/lale/lib/autoai_libs/num_imputer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2022 IBM Corporation
+# Copyright 2020-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -46,25 +46,27 @@
             "additionalProperties": False,
             "required": ["strategy", "missing_values", "activate_flag"],
             "relevantToOptimizer": ["strategy"],
             "properties": {
                 "strategy": {
                     "description": "The imputation strategy.",
                     "enum": ["mean", "median", "most_frequent"],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": "mean",
                 },
                 "missing_values": {
                     "description": "The placeholder for the missing values. All occurrences of missing_values will be imputed.",
                     "anyOf": [
                         {"laleType": "Any"},
                         {
                             "description": "For missing values encoded as np.nan.",
                             "enum": [np.nan],
                         },
                     ],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": np.nan,
                 },
                 "activate_flag": _hparam_activate_flag_unmodified,
             },
         }
     ]
 }
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/numpy_column_selector.py` & `lale-0.7.8/lale/lib/autoai_libs/numpy_column_selector.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/numpy_permute_array.py` & `lale-0.7.8/lale/lib/autoai_libs/numpy_permute_array.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/numpy_replace_missing_values.py` & `lale-0.7.8/lale/lib/autoai_libs/numpy_replace_missing_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 IBM Corporation
+# Copyright 2020-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -43,14 +43,15 @@
             "properties": {
                 "missing_values": {
                     "description": 'List of values considered as "missing" for the array.',
                     "anyOf": [
                         {"type": "array", "items": {"laleType": "Any"}},
                         {"enum": [None]},
                     ],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": None,
                 },
                 "filling_values": {
                     "description": "Value to replace the missing values.",
                     "laleType": "Any",
                     "default": None,
                 },
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/numpy_replace_unknown_values.py` & `lale-0.7.8/lale/lib/autoai_libs/numpy_replace_unknown_values.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/opt_standard_scaler.py` & `lale-0.7.8/lale/lib/autoai_libs/opt_standard_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/t_no_op.py` & `lale-0.7.8/lale/lib/autoai_libs/t_no_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 IBM Corporation
+# Copyright 2020-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -49,14 +49,15 @@
             "relevantToOptimizer": [],
             "properties": {
                 "fun": _hparams_fun_pointer(description="Function pointer (ignored)."),
                 "name": _hparams_transformer_name,
                 "datatypes": {
                     "description": "List of datatypes that are valid input (ignored).",
                     "laleType": "Any",
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": None,
                 },
                 "feat_constraints": _hparams_feat_constraints(
                     description="Constraints that must be satisfied by a column to be considered a valid input to this transform (ignored)."
                 ),
                 "tgraph": {
                     "description": "Should be the invoking TGraph() object.",
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/ta1.py` & `lale-0.7.8/lale/lib/autoai_libs/ta1.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/ta2.py` & `lale-0.7.8/lale/lib/autoai_libs/ta2.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/tam.py` & `lale-0.7.8/lale/lib/autoai_libs/tam.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/tb1.py` & `lale-0.7.8/lale/lib/autoai_libs/tb1.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/tb2.py` & `lale-0.7.8/lale/lib/autoai_libs/tb2.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/text_transformer.py` & `lale-0.7.8/lale/lib/autoai_libs/text_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/tgen.py` & `lale-0.7.8/lale/lib/autoai_libs/tgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,28 +70,30 @@
             "properties": {
                 "fun": _hparams_fun_pointer(description="The function pointer."),
                 "name": _hparams_transformer_name,
                 "arg_count": {
                     "description": "Number of arguments to the function, e.g., 1 for unary, 2 for binary, and so on.",
                     "type": "integer",
                     "minimum": 1,
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": 1,
                 },
                 "datatypes_list": {
                     "description": "A list of arg_count lists that correspond to the acceptable input data types for each argument.",
                     "anyOf": [
                         {
                             "type": "array",
                             "items": {
                                 "description": "List of datatypes that are valid input to the corresponding argument (numeric, float, int, etc.).",
                                 **_hparams_datatype_spec,
                             },
                         },
                         {"enum": [None]},
                     ],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": None,
                 },
                 "feat_constraints_list": {
                     "description": "A list of arg_count lists that correspond to some constraints that should be imposed on selection of the input features.",
                     "anyOf": [
                         {
                             "type": "array",
@@ -99,14 +101,15 @@
                                 "description": "List of feature constraints for the corresponding argument.",
                                 "type": "array",
                                 "items": {"laleType": "Any"},
                             },
                         },
                         {"enum": [None]},
                     ],
+                    "transient": "alwaysPrint",  # since positional argument
                     "default": None,
                 },
                 "tgraph": _hparams_tgraph,
                 "apply_all": _hparams_apply_all,
                 "col_names": _hparams_col_names,
                 "col_dtypes": _hparam_col_dtypes,
                 "col_as_json_objects": _hparams_col_as_json_objects,
```

### Comparing `lale-0.7.7/lale/lib/autoai_libs/util.py` & `lale-0.7.8/lale/lib/autoai_libs/util.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autoai_libs/word2vec_transformer.py` & `lale-0.7.8/lale/lib/autoai_libs/word2vec_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/__init__.py` & `lale-0.7.8/lale/lib/autogen/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/additive_chi2_sampler.py` & `lale-0.7.8/lale/lib/autogen/additive_chi2_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/ard_regression.py` & `lale-0.7.8/lale/lib/autogen/ard_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/bayesian_ridge.py` & `lale-0.7.8/lale/lib/autogen/bayesian_ridge.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/bernoulli_nb.py` & `lale-0.7.8/lale/lib/autogen/bernoulli_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/bernoulli_rbm.py` & `lale-0.7.8/lale/lib/autogen/bernoulli_rbm.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/binarizer.py` & `lale-0.7.8/lale/lib/autogen/binarizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/birch.py` & `lale-0.7.8/lale/lib/autogen/birch.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/calibrated_classifier_cv.py` & `lale-0.7.8/lale/lib/autogen/calibrated_classifier_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/cca.py` & `lale-0.7.8/lale/lib/autogen/cca.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/complement_nb.py` & `lale-0.7.8/lale/lib/autogen/complement_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/dictionary_learning.py` & `lale-0.7.8/lale/lib/autogen/dictionary_learning.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/elastic_net.py` & `lale-0.7.8/lale/lib/autogen/elastic_net.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/elastic_net_cv.py` & `lale-0.7.8/lale/lib/autogen/elastic_net_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/factor_analysis.py` & `lale-0.7.8/lale/lib/autogen/factor_analysis.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/fast_ica.py` & `lale-0.7.8/lale/lib/autogen/fast_ica.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/gaussian_process_classifier.py` & `lale-0.7.8/lale/lib/autogen/gaussian_process_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/gaussian_process_regressor.py` & `lale-0.7.8/lale/lib/autogen/gaussian_process_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/gaussian_random_projection.py` & `lale-0.7.8/lale/lib/autogen/gaussian_random_projection.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/huber_regressor.py` & `lale-0.7.8/lale/lib/autogen/huber_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/incremental_pca.py` & `lale-0.7.8/lale/lib/autogen/incremental_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/k_bins_discretizer.py` & `lale-0.7.8/lale/lib/autogen/k_bins_discretizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/kernel_pca.py` & `lale-0.7.8/lale/lib/autogen/kernel_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/kernel_ridge.py` & `lale-0.7.8/lale/lib/autogen/kernel_ridge.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/label_binarizer.py` & `lale-0.7.8/lale/lib/autogen/label_binarizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/label_encoder.py` & `lale-0.7.8/lale/lib/autogen/label_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/label_propagation.py` & `lale-0.7.8/lale/lib/autogen/label_propagation.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/label_spreading.py` & `lale-0.7.8/lale/lib/autogen/label_spreading.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/lars.py` & `lale-0.7.8/lale/lib/autogen/lars.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/lars_cv.py` & `lale-0.7.8/lale/lib/autogen/lars_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/lasso.py` & `lale-0.7.8/lale/lib/autogen/lasso.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/lasso_cv.py` & `lale-0.7.8/lale/lib/autogen/lasso_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/lasso_lars.py` & `lale-0.7.8/lale/lib/autogen/lasso_lars.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/lasso_lars_cv.py` & `lale-0.7.8/lale/lib/autogen/lasso_lars_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/lasso_lars_ic.py` & `lale-0.7.8/lale/lib/autogen/lasso_lars_ic.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/latent_dirichlet_allocation.py` & `lale-0.7.8/lale/lib/autogen/latent_dirichlet_allocation.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/linear_discriminant_analysis.py` & `lale-0.7.8/lale/lib/autogen/linear_discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/locally_linear_embedding.py` & `lale-0.7.8/lale/lib/autogen/locally_linear_embedding.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/logistic_regression_cv.py` & `lale-0.7.8/lale/lib/autogen/logistic_regression_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/max_abs_scaler.py` & `lale-0.7.8/lale/lib/autogen/max_abs_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/mini_batch_dictionary_learning.py` & `lale-0.7.8/lale/lib/autogen/mini_batch_dictionary_learning.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/mini_batch_k_means.py` & `lale-0.7.8/lale/lib/autogen/mini_batch_k_means.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/mini_batch_sparse_pca.py` & `lale-0.7.8/lale/lib/autogen/mini_batch_sparse_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/mlp_regressor.py` & `lale-0.7.8/lale/lib/autogen/mlp_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/multi_label_binarizer.py` & `lale-0.7.8/lale/lib/autogen/multi_label_binarizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/multi_task_elastic_net.py` & `lale-0.7.8/lale/lib/autogen/multi_task_elastic_net.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/multi_task_elastic_net_cv.py` & `lale-0.7.8/lale/lib/autogen/multi_task_elastic_net_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/multi_task_lasso.py` & `lale-0.7.8/lale/lib/autogen/multi_task_lasso.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/multi_task_lasso_cv.py` & `lale-0.7.8/lale/lib/autogen/multi_task_lasso_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/nearest_centroid.py` & `lale-0.7.8/lale/lib/autogen/nearest_centroid.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/nu_svc.py` & `lale-0.7.8/lale/lib/autogen/nu_svc.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/nu_svr.py` & `lale-0.7.8/lale/lib/autogen/nu_svr.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/orthogonal_matching_pursuit.py` & `lale-0.7.8/lale/lib/autogen/orthogonal_matching_pursuit.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/orthogonal_matching_pursuit_cv.py` & `lale-0.7.8/lale/lib/autogen/orthogonal_matching_pursuit_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/passive_aggressive_regressor.py` & `lale-0.7.8/lale/lib/autogen/passive_aggressive_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/perceptron.py` & `lale-0.7.8/lale/lib/autogen/perceptron.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/pls_canonical.py` & `lale-0.7.8/lale/lib/autogen/pls_canonical.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/pls_regression.py` & `lale-0.7.8/lale/lib/autogen/pls_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/plssvd.py` & `lale-0.7.8/lale/lib/autogen/plssvd.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/power_transformer.py` & `lale-0.7.8/lale/lib/autogen/power_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/radius_neighbors_classifier.py` & `lale-0.7.8/lale/lib/autogen/radius_neighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/radius_neighbors_regressor.py` & `lale-0.7.8/lale/lib/autogen/radius_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/random_trees_embedding.py` & `lale-0.7.8/lale/lib/autogen/random_trees_embedding.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/ransac_regressor.py` & `lale-0.7.8/lale/lib/autogen/ransac_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/rbf_sampler.py` & `lale-0.7.8/lale/lib/autogen/rbf_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/ridge_classifier_cv.py` & `lale-0.7.8/lale/lib/autogen/ridge_classifier_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/ridge_cv.py` & `lale-0.7.8/lale/lib/autogen/ridge_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/skewed_chi2_sampler.py` & `lale-0.7.8/lale/lib/autogen/skewed_chi2_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/sparse_pca.py` & `lale-0.7.8/lale/lib/autogen/sparse_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/sparse_random_projection.py` & `lale-0.7.8/lale/lib/autogen/sparse_random_projection.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/theil_sen_regressor.py` & `lale-0.7.8/lale/lib/autogen/theil_sen_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/transformed_target_regressor.py` & `lale-0.7.8/lale/lib/autogen/transformed_target_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/autogen/truncated_svd.py` & `lale-0.7.8/lale/lib/autogen/truncated_svd.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/category_encoders/__init__.py` & `lale-0.7.8/lale/lib/category_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/category_encoders/hashing_encoder.py` & `lale-0.7.8/lale/lib/category_encoders/hashing_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/category_encoders/target_encoder.py` & `lale-0.7.8/lale/lib/category_encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/dataframe.py` & `lale-0.7.8/lale/lib/dataframe.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/__init__.py` & `lale-0.7.8/lale/lib/imblearn/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/_common_schemas.py` & `lale-0.7.8/lale/lib/imblearn/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/adasyn.py` & `lale-0.7.8/lale/lib/imblearn/adasyn.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/all_knn.py` & `lale-0.7.8/lale/lib/imblearn/all_knn.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/base_resampler.py` & `lale-0.7.8/lale/lib/imblearn/base_resampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/borderline_smote.py` & `lale-0.7.8/lale/lib/imblearn/borderline_smote.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/condensed_nearest_neighbour.py` & `lale-0.7.8/lale/lib/imblearn/condensed_nearest_neighbour.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/edited_nearest_neighbours.py` & `lale-0.7.8/lale/lib/imblearn/edited_nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/instance_hardness_threshold.py` & `lale-0.7.8/lale/lib/imblearn/instance_hardness_threshold.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/random_over_sampler.py` & `lale-0.7.8/lale/lib/imblearn/random_over_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/repeated_edited_nearest_neighbours.py` & `lale-0.7.8/lale/lib/imblearn/repeated_edited_nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/smote.py` & `lale-0.7.8/lale/lib/imblearn/smote.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/smoteenn.py` & `lale-0.7.8/lale/lib/imblearn/smoteenn.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/smoten.py` & `lale-0.7.8/lale/lib/imblearn/smoten.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/smotenc.py` & `lale-0.7.8/lale/lib/imblearn/smotenc.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/imblearn/svm_smote.py` & `lale-0.7.8/lale/lib/imblearn/svm_smote.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/__init__.py` & `lale-0.7.8/lale/lib/lale/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/auto_pipeline.py` & `lale-0.7.8/lale/lib/lale/auto_pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/both.py` & `lale-0.7.8/lale/lib/lale/both.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/concat_features.py` & `lale-0.7.8/lale/lib/lale/concat_features.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/grid_search_cv.py` & `lale-0.7.8/lale/lib/lale/grid_search_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/halving_grid_search_cv.py` & `lale-0.7.8/lale/lib/lale/halving_grid_search_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/hyperopt.py` & `lale-0.7.8/lale/lib/lale/hyperopt.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/identity_wrapper.py` & `lale-0.7.8/lale/lib/lale/identity_wrapper.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/no_op.py` & `lale-0.7.8/lale/lib/lale/no_op.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/observing.py` & `lale-0.7.8/lale/lib/lale/observing.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/optimize_last.py` & `lale-0.7.8/lale/lib/lale/optimize_last.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/optimize_suffix.py` & `lale-0.7.8/lale/lib/lale/optimize_suffix.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/sample_based_voting.py` & `lale-0.7.8/lale/lib/lale/sample_based_voting.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/smac.py` & `lale-0.7.8/lale/lib/lale/smac.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/tee.py` & `lale-0.7.8/lale/lib/lale/tee.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/time_series_transformer.py` & `lale-0.7.8/lale/lib/lale/time_series_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lale/topk_voting_classifier.py` & `lale-0.7.8/lale/lib/lale/topk_voting_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lightgbm/__init__.py` & `lale-0.7.8/lale/lib/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lightgbm/lgbm_classifier.py` & `lale-0.7.8/lale/lib/lightgbm/lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/lightgbm/lgbm_regressor.py` & `lale-0.7.8/lale/lib/lightgbm/lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/__init__.py` & `lale-0.7.8/lale/lib/rasl/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/_eval_pandas_df.py` & `lale-0.7.8/lale/lib/rasl/_eval_pandas_df.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/_eval_spark_df.py` & `lale-0.7.8/lale/lib/rasl/_eval_spark_df.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/_util.py` & `lale-0.7.8/lale/lib/rasl/_util.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/aggregate.py` & `lale-0.7.8/lale/lib/rasl/aggregate.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/alias.py` & `lale-0.7.8/lale/lib/rasl/alias.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/batched_bagging_classifier.py` & `lale-0.7.8/lale/lib/rasl/batched_bagging_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/batching.py` & `lale-0.7.8/lale/lib/rasl/batching.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/concat_features.py` & `lale-0.7.8/lale/lib/rasl/concat_features.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/convert.py` & `lale-0.7.8/lale/lib/rasl/convert.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/datasets.py` & `lale-0.7.8/lale/lib/rasl/datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/filter.py` & `lale-0.7.8/lale/lib/rasl/filter.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/functions.py` & `lale-0.7.8/lale/lib/rasl/functions.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/group_by.py` & `lale-0.7.8/lale/lib/rasl/group_by.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/hashing_encoder.py` & `lale-0.7.8/lale/lib/rasl/hashing_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/join.py` & `lale-0.7.8/lale/lib/rasl/join.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/map.py` & `lale-0.7.8/lale/lib/rasl/map.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/metrics.py` & `lale-0.7.8/lale/lib/rasl/metrics.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/min_max_scaler.py` & `lale-0.7.8/lale/lib/rasl/min_max_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/monoid.py` & `lale-0.7.8/lale/lib/rasl/monoid.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/one_hot_encoder.py` & `lale-0.7.8/lale/lib/rasl/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/orderby.py` & `lale-0.7.8/lale/lib/rasl/orderby.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/ordinal_encoder.py` & `lale-0.7.8/lale/lib/rasl/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/project.py` & `lale-0.7.8/lale/lib/rasl/project.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/relational.py` & `lale-0.7.8/lale/lib/rasl/relational.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/scan.py` & `lale-0.7.8/lale/lib/rasl/scan.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/scores.py` & `lale-0.7.8/lale/lib/rasl/scores.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/select_k_best.py` & `lale-0.7.8/lale/lib/rasl/select_k_best.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/simple_imputer.py` & `lale-0.7.8/lale/lib/rasl/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/sort_index.py` & `lale-0.7.8/lale/lib/rasl/sort_index.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/spark_explainer.py` & `lale-0.7.8/lale/lib/rasl/spark_explainer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/split_xy.py` & `lale-0.7.8/lale/lib/rasl/split_xy.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/standard_scaler.py` & `lale-0.7.8/lale/lib/rasl/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/target_encoder.py` & `lale-0.7.8/lale/lib/rasl/target_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/rasl/task_graphs.py` & `lale-0.7.8/lale/lib/rasl/task_graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,20 +137,21 @@
                 f"""Spilling of {type(self.y)} is not supported.
             Supported types are: pandas DataFrame, pandas Series, and numpy ndarray."""
             )
         self.X, self.y = name_X, name_y
 
     def load_spilled(self) -> None:
         assert isinstance(self.X, pathlib.Path) and isinstance(self.y, pathlib.Path)
+        # we know these are pickles written by us, so we can trust them
         try:
-            data_X = pd.read_pickle(self.X)
+            data_X = pd.read_pickle(self.X)  # nosec B301
         except FileNotFoundError:
             data_X = np.load(f"{self.X}" + ".npy", allow_pickle=True)
         try:
-            data_y = pd.read_pickle(self.y)
+            data_y = pd.read_pickle(self.y)  # nosec B301
         except FileNotFoundError:
             data_y = np.load(f"{self.y}" + ".npy", allow_pickle=True)
         self.X, self.y = data_X, data_y
 
     def delete_if_spilled(self) -> None:
         if isinstance(self.X, pathlib.Path) and isinstance(self.y, pathlib.Path):
             self.X.unlink()
```

### Comparing `lale-0.7.7/lale/lib/sklearn/__init__.py` & `lale-0.7.8/lale/lib/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/_common_schemas.py` & `lale-0.7.8/lale/lib/sklearn/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/ada_boost_classifier.py` & `lale-0.7.8/lale/lib/sklearn/ada_boost_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/ada_boost_regressor.py` & `lale-0.7.8/lale/lib/sklearn/ada_boost_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/bagging_classifier.py` & `lale-0.7.8/lale/lib/sklearn/bagging_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/bagging_regressor.py` & `lale-0.7.8/lale/lib/sklearn/bagging_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/column_transformer.py` & `lale-0.7.8/lale/lib/sklearn/column_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/decision_tree_classifier.py` & `lale-0.7.8/lale/lib/sklearn/decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/decision_tree_regressor.py` & `lale-0.7.8/lale/lib/sklearn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/dummy_classifier.py` & `lale-0.7.8/lale/lib/sklearn/dummy_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/dummy_regressor.py` & `lale-0.7.8/lale/lib/sklearn/dummy_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/extra_trees_classifier.py` & `lale-0.7.8/lale/lib/sklearn/extra_trees_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/extra_trees_regressor.py` & `lale-0.7.8/lale/lib/sklearn/extra_trees_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/feature_agglomeration.py` & `lale-0.7.8/lale/lib/sklearn/feature_agglomeration.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/fit_spec_proxy.py` & `lale-0.7.8/lale/lib/sklearn/fit_spec_proxy.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/function_transformer.py` & `lale-0.7.8/lale/lib/sklearn/function_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/gaussian_nb.py` & `lale-0.7.8/lale/lib/sklearn/gaussian_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/gradient_boosting_classifier.py` & `lale-0.7.8/lale/lib/sklearn/gradient_boosting_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/gradient_boosting_regressor.py` & `lale-0.7.8/lale/lib/sklearn/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/isolation_forest.py` & `lale-0.7.8/lale/lib/sklearn/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/isomap.py` & `lale-0.7.8/lale/lib/sklearn/isomap.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/k_means.py` & `lale-0.7.8/lale/lib/sklearn/k_means.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/k_neighbors_classifier.py` & `lale-0.7.8/lale/lib/sklearn/k_neighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/k_neighbors_regressor.py` & `lale-0.7.8/lale/lib/sklearn/k_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/linear_regression.py` & `lale-0.7.8/lale/lib/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/linear_svc.py` & `lale-0.7.8/lale/lib/sklearn/linear_svc.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/linear_svr.py` & `lale-0.7.8/lale/lib/sklearn/linear_svr.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/logistic_regression.py` & `lale-0.7.8/lale/lib/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/min_max_scaler.py` & `lale-0.7.8/lale/lib/sklearn/min_max_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/missing_indicator.py` & `lale-0.7.8/lale/lib/sklearn/missing_indicator.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/mlp_classifier.py` & `lale-0.7.8/lale/lib/sklearn/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/multi_output_regressor.py` & `lale-0.7.8/lale/lib/sklearn/multi_output_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/multinomial_nb.py` & `lale-0.7.8/lale/lib/sklearn/multinomial_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/nmf.py` & `lale-0.7.8/lale/lib/sklearn/nmf.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/normalizer.py` & `lale-0.7.8/lale/lib/sklearn/normalizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/nystroem.py` & `lale-0.7.8/lale/lib/sklearn/nystroem.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/one_hot_encoder.py` & `lale-0.7.8/lale/lib/sklearn/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/ordinal_encoder.py` & `lale-0.7.8/lale/lib/sklearn/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/passive_aggressive_classifier.py` & `lale-0.7.8/lale/lib/sklearn/passive_aggressive_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/pca.py` & `lale-0.7.8/lale/lib/sklearn/pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/perceptron.py` & `lale-0.7.8/lale/lib/sklearn/perceptron.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/pipeline.py` & `lale-0.7.8/lale/lib/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/polynomial_features.py` & `lale-0.7.8/lale/lib/sklearn/polynomial_features.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/quadratic_discriminant_analysis.py` & `lale-0.7.8/lale/lib/sklearn/quadratic_discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/quantile_transformer.py` & `lale-0.7.8/lale/lib/sklearn/quantile_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/random_forest_classifier.py` & `lale-0.7.8/lale/lib/sklearn/random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/random_forest_regressor.py` & `lale-0.7.8/lale/lib/sklearn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/rfe.py` & `lale-0.7.8/lale/lib/sklearn/rfe.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/ridge.py` & `lale-0.7.8/lale/lib/sklearn/ridge.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/ridge_classifier.py` & `lale-0.7.8/lale/lib/sklearn/ridge_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/robust_scaler.py` & `lale-0.7.8/lale/lib/sklearn/robust_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/select_k_best.py` & `lale-0.7.8/lale/lib/sklearn/select_k_best.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/sgd_classifier.py` & `lale-0.7.8/lale/lib/sklearn/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/sgd_regressor.py` & `lale-0.7.8/lale/lib/sklearn/sgd_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/simple_imputer.py` & `lale-0.7.8/lale/lib/sklearn/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/stacking_classifier.py` & `lale-0.7.8/lale/lib/sklearn/stacking_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/stacking_regressor.py` & `lale-0.7.8/lale/lib/sklearn/stacking_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/stacking_utils.py` & `lale-0.7.8/lale/lib/sklearn/stacking_utils.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/standard_scaler.py` & `lale-0.7.8/lale/lib/sklearn/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/svc.py` & `lale-0.7.8/lale/lib/sklearn/svc.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/svr.py` & `lale-0.7.8/lale/lib/sklearn/svr.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/tfidf_vectorizer.py` & `lale-0.7.8/lale/lib/sklearn/tfidf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/variance_threshold.py` & `lale-0.7.8/lale/lib/sklearn/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/voting_classifier.py` & `lale-0.7.8/lale/lib/sklearn/voting_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/sklearn/voting_regressor.py` & `lale-0.7.8/lale/lib/sklearn/voting_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/__init__.py` & `lale-0.7.8/lale/lib/snapml/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/batched_tree_ensemble_classifier.py` & `lale-0.7.8/lale/lib/snapml/batched_tree_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/batched_tree_ensemble_regressor.py` & `lale-0.7.8/lale/lib/snapml/batched_tree_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_boosting_machine_classifier.py` & `lale-0.7.8/lale/lib/snapml/snap_boosting_machine_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_boosting_machine_regressor.py` & `lale-0.7.8/lale/lib/snapml/snap_boosting_machine_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_decision_tree_classifier.py` & `lale-0.7.8/lale/lib/snapml/snap_decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_decision_tree_regressor.py` & `lale-0.7.8/lale/lib/snapml/snap_decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_linear_regression.py` & `lale-0.7.8/lale/lib/snapml/snap_linear_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_logistic_regression.py` & `lale-0.7.8/lale/lib/snapml/snap_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_random_forest_classifier.py` & `lale-0.7.8/lale/lib/snapml/snap_random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_random_forest_regressor.py` & `lale-0.7.8/lale/lib/snapml/snap_random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/snapml/snap_svm_classifier.py` & `lale-0.7.8/lale/lib/snapml/snap_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/xgboost/__init__.py` & `lale-0.7.8/lale/lib/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/xgboost/_common_schemas.py` & `lale-0.7.8/lale/lib/xgboost/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/xgboost/xgb_classifier.py` & `lale-0.7.8/lale/lib/xgboost/xgb_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/lib/xgboost/xgb_regressor.py` & `lale-0.7.8/lale/lib/xgboost/xgb_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/operator_wrapper.py` & `lale-0.7.8/lale/operator_wrapper.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/operators.py` & `lale-0.7.8/lale/operators.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/pretty_print.py` & `lale-0.7.8/lale/pretty_print.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/schema2enums.py` & `lale-0.7.8/lale/schema2enums.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/schema_ranges.py` & `lale-0.7.8/lale/schema_ranges.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/schema_simplifier.py` & `lale-0.7.8/lale/schema_simplifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/schema_utils.py` & `lale-0.7.8/lale/schema_utils.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/schemas.py` & `lale-0.7.8/lale/schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/PGO.py` & `lale-0.7.8/lale/search/PGO.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/__init__.py` & `lale-0.7.8/lale/search/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/lale_grid_search_cv.py` & `lale-0.7.8/lale/search/lale_grid_search_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/lale_hyperopt.py` & `lale-0.7.8/lale/search/lale_hyperopt.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/lale_smac.py` & `lale-0.7.8/lale/search/lale_smac.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/op2hp.py` & `lale-0.7.8/lale/search/op2hp.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/schema2search_space.py` & `lale-0.7.8/lale/search/schema2search_space.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/search_space.py` & `lale-0.7.8/lale/search/search_space.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/search/search_space_grid.py` & `lale-0.7.8/lale/search/search_space_grid.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/settings.py` & `lale-0.7.8/lale/settings.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/sklearn_compat.py` & `lale-0.7.8/lale/sklearn_compat.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/type_checking.py` & `lale-0.7.8/lale/type_checking.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/Visitor.py` & `lale-0.7.8/lale/util/Visitor.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/VisitorMeta.py` & `lale-0.7.8/lale/util/VisitorMeta.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/VisitorPathError.py` & `lale-0.7.8/lale/util/VisitorPathError.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/__init__.py` & `lale-0.7.8/lale/util/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/batch_data_dictionary_dataset.py` & `lale-0.7.8/lale/util/batch_data_dictionary_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/hdf5_to_torch_dataset.py` & `lale-0.7.8/lale/util/hdf5_to_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/numpy_to_torch_dataset.py` & `lale-0.7.8/lale/util/numpy_to_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/numpy_torch_dataset.py` & `lale-0.7.8/lale/util/numpy_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/pandas_to_torch_dataset.py` & `lale-0.7.8/lale/util/pandas_to_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/util/pandas_torch_dataset.py` & `lale-0.7.8/lale/util/pandas_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale/visualize.py` & `lale-0.7.8/lale/visualize.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale.egg-info/PKG-INFO` & `lale-0.7.8/lale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lale
-Version: 0.7.7
+Version: 0.7.8
 Summary: Library for Semi-Automated Data Science
 Home-page: https://github.com/IBM/lale
 Author: Guillaume Baudart, Martin Hirzel, Kiran Kate, Parikshit Ram, Avraham Shinnar
 License: Apache License 2.0
 Description: # Lale
         
         [![Tests](https://github.com/IBM/lale/workflows/Tests/badge.svg?branch=master)](https://github.com/IBM/lale/actions?query=workflow%3ATests+branch%3Amaster)
```

### Comparing `lale-0.7.7/lale.egg-info/SOURCES.txt` & `lale-0.7.8/lale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/lale.egg-info/requires.txt` & `lale-0.7.8/lale.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 click==8.0.4
 graphviz
 hyperopt<=0.2.5,>=0.2
 jsonschema
 jsonsubschema>=0.0.6
 scikit-learn<=1.2.0,>=1.0.0
 scipy<1.11.0
-pandas
+pandas<2.0.0
 packaging
 decorator
 astunparse
 typing-extensions
 
 [dev]
 pre-commit
@@ -47,15 +47,15 @@
 sphinx>=5.0.0
 sphinx_rtd_theme>=0.5.2
 docutils<0.17
 m2r2
 sphinxcontrib.apidoc
 sphinxcontrib-svg2pdfconverter
 pytest
-pyspark
+pyspark<=3.3.2
 func_timeout
 category-encoders
 pynisher==0.6.4
 
 [tutorial]
 ipython<8.8.0
 jupyter
```

### Comparing `lale-0.7.7/setup.py` & `lale-0.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 IBM Corporation
+# Copyright 2019-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,15 +45,15 @@
         "click==8.0.4",
         "graphviz",
         "hyperopt>=0.2,<=0.2.5",
         "jsonschema",
         "jsonsubschema>=0.0.6",
         "scikit-learn>=1.0.0,<=1.2.0",
         "scipy<1.11.0",
-        "pandas",
+        "pandas<2.0.0",
         "packaging",
         "decorator",
         "astunparse",
         "typing-extensions",
     ]
 
 import lale  # noqa: E402  # pylint:disable=wrong-import-position
@@ -90,15 +90,15 @@
         "sphinx>=5.0.0",
         "sphinx_rtd_theme>=0.5.2",
         "docutils<0.17",
         "m2r2",
         "sphinxcontrib.apidoc",
         "sphinxcontrib-svg2pdfconverter",
         "pytest",
-        "pyspark",
+        "pyspark<=3.3.2",
         "func_timeout",
         "category-encoders",
         "pynisher==0.6.4",
     ],
     "fairness": [
         "liac-arff>=2.4.0",
         "aif360<0.6.0",
```

### Comparing `lale-0.7.7/test/__init__.py` & `lale-0.7.8/test/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/mock_custom_operators.py` & `lale-0.7.8/test/mock_custom_operators.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/mock_module.py` & `lale-0.7.8/test/mock_module.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_aif360.py` & `lale-0.7.8/test/test_aif360.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_aif360_ensembles.py` & `lale-0.7.8/test/test_aif360_ensembles.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_autoai_libs.py` & `lale-0.7.8/test/test_autoai_libs.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_autoai_output_consumption.py` & `lale-0.7.8/test/test_autoai_output_consumption.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_autogen_lib.py` & `lale-0.7.8/test/test_autogen_lib.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_category_encoders.py` & `lale-0.7.8/test/test_category_encoders.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_core_classifiers.py` & `lale-0.7.8/test/test_core_classifiers.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_core_misc.py` & `lale-0.7.8/test/test_core_misc.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_core_pipeline.py` & `lale-0.7.8/test/test_core_pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_core_regressors.py` & `lale-0.7.8/test/test_core_regressors.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_core_transformers.py` & `lale-0.7.8/test/test_core_transformers.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_custom_schemas.py` & `lale-0.7.8/test/test_custom_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_grammar.py` & `lale-0.7.8/test/test_grammar.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_halving_gridsearchcv.py` & `lale-0.7.8/test/test_halving_gridsearchcv.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_interoperability.py` & `lale-0.7.8/test/test_interoperability.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_json_pretty_viz.py` & `lale-0.7.8/test/test_json_pretty_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2022 IBM Corporation
+# Copyright 2019-2023 IBM Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -445,14 +445,41 @@
     dtype=np.float64,
     handle_unknown="error",
     sklearn_version_family="23",
 )
 pipeline = cat_encoder >> LR()"""
         self._roundtrip(expected, lale.pretty_print.to_string(pipeline))
 
+    def test_autoai_libs_cat_encoder_defaults(self):
+        import numpy as np
+
+        from lale.lib.autoai_libs import CatEncoder
+        from lale.lib.sklearn import LogisticRegression as LR
+
+        cat_encoder = CatEncoder(
+            dtype=np.float64, handle_unknown="error", sklearn_version_family="1"
+        )
+        pipeline = cat_encoder >> LR()
+        expected = """from autoai_libs.transformers.exportable import CatEncoder
+import numpy as np
+from sklearn.linear_model import LogisticRegression as LR
+from sklearn.pipeline import make_pipeline
+
+cat_encoder = CatEncoder(
+    dtype=np.float64,
+    handle_unknown="error",
+    sklearn_version_family="1",
+    encoding="ordinal",
+    categories="auto",
+)
+pipeline = make_pipeline(cat_encoder, LR())"""
+        self._roundtrip(
+            expected, lale.pretty_print.to_string(pipeline, astype="sklearn")
+        )
+
     def test_autoai_libs_fs1(self):
         from autoai_libs.cognito.transforms.transform_utils import FS1
 
         from lale.lib.sklearn import LogisticRegression as LR
 
         fs1 = FS1(
             cols_ids_must_keep=range(0, 7),
```

### Comparing `lale-0.7.7/test/test_lale_lib_versions.py` & `lale-0.7.8/test/test_lale_lib_versions.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_nlp_operators.py` & `lale-0.7.8/test/test_nlp_operators.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_notebooks.py` & `lale-0.7.8/test/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_optimizers.py` & `lale-0.7.8/test/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_pgo.py` & `lale-0.7.8/test/test_pgo.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_pipeline.py` & `lale-0.7.8/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_relational.py` & `lale-0.7.8/test/test_relational.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_relational_from_sklearn_manual.py` & `lale-0.7.8/test/test_relational_from_sklearn_manual.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_relational_sklearn.py` & `lale-0.7.8/test/test_relational_sklearn.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_replace.py` & `lale-0.7.8/test/test_replace.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_sklearn_compat.py` & `lale-0.7.8/test/test_sklearn_compat.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_snapml.py` & `lale-0.7.8/test/test_snapml.py`

 * *Files identical despite different names*

### Comparing `lale-0.7.7/test/test_type_checking.py` & `lale-0.7.8/test/test_type_checking.py`

 * *Files identical despite different names*


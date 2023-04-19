# Comparing `tmp/krisi-0.0.8.tar.gz` & `tmp/krisi-0.1.0.tar.gz`

## Comparing `krisi-0.0.8.tar` & `krisi-0.1.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 krisi-0.0.8/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.0.8/.isort.cfg
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 krisi-0.0.8/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.0.8/.vscode/launch.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 krisi-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0   104237 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/a_full_rundown_notebook.ipynb
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/basic_df.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/basic_loading.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/basic_pdf_report.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/basic_report_rolling.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/basic_saving.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/basic_scorecard.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/compare_classification.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/compare_regression.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/default_metric_selection.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/extended_scorecard.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/loading_generating_report.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/minimal_classification.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/minimal_html_report.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/minimal_pdf_report.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/minimal_regression.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 krisi-0.0.8/examples/training_arima_report.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    13612 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/console.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/report.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/type.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/library/pdf_layouts/default/template.css
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/library/pdf_layouts/default/template.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/data.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/io.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/modeling_types.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/models.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/printing.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 krisi-0.0.8/src/krisi/utils/runner.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 krisi-0.0.8/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.0.8/LICENSE
--rw-r--r--   0        0        0    26702 2020-02-02 00:00:00.000000 krisi-0.0.8/README.md
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 krisi-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    31203 2020-02-02 00:00:00.000000 krisi-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.0/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.0/.isort.cfg
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 krisi-0.1.0/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.0/.vscode/launch.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0   106892 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/a_full_rundown_notebook.ipynb
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_df.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_loading.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_pdf_report.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_report_rolling.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_saving.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_scorecard.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/compare_classification.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/compare_regression.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/default_metric_selection.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/extended_scorecard.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/loading_generating_report.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_classification.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_html_report.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_pdf_report.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_regression.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/printing_methods.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/training_arima_report.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/dataset.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    15797 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/type.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/default/template.css
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/default/template.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/modeling_types.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/models.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/runner.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 krisi-0.1.0/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.0/LICENSE
+-rw-r--r--   0        0        0    27699 2020-02-02 00:00:00.000000 krisi-0.1.0/README.md
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 krisi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    32200 2020-02-02 00:00:00.000000 krisi-0.1.0/PKG-INFO
```

### Comparing `krisi-0.0.8/examples/a_full_rundown_notebook.ipynb` & `krisi-0.1.0/examples/a_full_rundown_notebook.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997919761338879%*

 * *Differences: {"'cells'": '{7: {\'source\': ["\'\'\' Printing a minimal result by passing in `minimal` '*

 * *            '\'\'\'\\n", "scorecard.print(\'minimal\')"]}, 8: {\'source\': ["\'\'\' Printing a '*

 * *            'more detailed result by passing in `extended` (this is the default) \'\'\'\\n", '*

 * *            '"scorecard.print(\'extended\')"]}, 9: {\'source\': {insert: [(15, \'* '*

 * *            '`ScoreCard.save()` throws back itself, so that you can immediately chain a '*

 * *            "`print()`')], delete: [15]}}, 10: {'sourc […]*

```diff
@@ -106,16 +106,16 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "''' Printing a minimal result by passing in `extended = False` '''\n",
-                "scorecard.print_summary(extended=False)"
+                "''' Printing a minimal result by passing in `minimal` '''\n",
+                "scorecard.print('minimal')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [
@@ -294,16 +294,16 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "''' Printing a more detailed result by passing in `extended = True` (this is the default) '''\n",
-                "scorecard.print_summary()"
+                "''' Printing a more detailed result by passing in `extended` (this is the default) '''\n",
+                "scorecard.print('extended')"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -318,15 +318,15 @@
                 "   * `SaveModes.svg` (Creates an `svg` image of the console output)\n",
                 "   * `SaveModes.html` (Creates an `html` version of the console output)\n",
                 "\n",
                 "Let's just save the scorecard object that we can load in later, by passing in either `[SaveMode.obj]` or simply `[\"obj\"]`.\n",
                 "\n",
                 "Two things to note:\n",
                 "* The scorecard gets saved by default to `output/<project_name>/<current_time>_<model_name>_<dataset_name>`. However, we only need to worry about the `project_name` when loading, our helper function scans the directory of the specified project.\n",
-                "* `ScoreCard.save()` throws back itself, so that you can immediately chain a `print_summary()`"
+                "* `ScoreCard.save()` throws back itself, so that you can immediately chain a `print()`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {},
             "outputs": [
@@ -364,15 +364,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "scorecard.metadata.project_name = \"Our example project\"\n",
-                "scorecard.save(save_modes=[\"obj\"]).print_summary(extended=False)\n"
+                "scorecard.save(save_modes=[\"obj\"]).print('minimal')\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -506,15 +506,15 @@
                 "project_name = \"Comparing Multiple Scorecards\"\n",
                 "\n",
                 "for i in range(5):\n",
                 "    score(np.random.normal(0, 0.1, 1000), \n",
                 "          np.random.normal(0, 0.1, 1000), \n",
                 "          project_name=project_name).save()\n",
                 "\n",
-                "compare(load_scorecards(project_name),sort_metric_key='rmse', metrics_to_display=['mae', 'mse'])"
+                "compare(load_scorecards(project_name),sort_by='rmse', metric_keys=['mae', 'mse'])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `krisi-0.0.8/examples/basic_report_rolling.py` & `krisi-0.1.0/examples/basic_report_rolling.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,14 @@
         insample_predictions=insample_prediction,
         y_outsample=test[target_col],
         outsample_predictions=outsample_prediction,
     )
 
     """ Console log Reports """
     print(report_outsample)
-    report_insample.print_summary()
+    report_insample.print()
 
     return report_insample, report_outsample
 
 
 if __name__ == "__main__":
     basic_report_rolling()
```

### Comparing `krisi-0.0.8/examples/default_metric_selection.py` & `krisi-0.1.0/examples/default_metric_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     minimal_regression_metrics,
 )
 
 score(
     y=np.random.normal(0, 0.1, 1000),
     predictions=np.random.normal(0, 0.1, 1000),
     default_metrics=all_regression_metrics,  # This is the default
-).print_summary()
+).print()
 
 score(
     y=np.random.normal(0, 0.1, 1000),
     predictions=np.random.normal(0, 0.1, 1000),
     default_metrics=minimal_regression_metrics,
-).print_summary(input_analysis=False)
+).print(input_analysis=False)
 
 score(
     y=np.random.normal(0, 0.1, 1000),
     predictions=np.random.normal(0, 0.1, 1000),
     default_metrics=low_computation_regression_mterics,
-).print_summary(input_analysis=False)
+).print(input_analysis=False)
```

### Comparing `krisi-0.0.8/examples/extended_scorecard.py` & `krisi-0.1.0/examples/extended_scorecard.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     parameters={"hyper_1": 5.0},
 )
 
 # Updating a metric
 sc.yet_another_metric = dict(info="Giving description to a metric")
 
 """ Print scorecard summary """
-sc.print_summary(with_info=True, extended=True)
+sc.print("extended", with_info=True)
```

### Comparing `krisi-0.0.8/examples/loading_generating_report.py` & `krisi-0.1.0/examples/loading_generating_report.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/examples/minimal_html_report.py` & `krisi-0.1.0/examples/minimal_html_report.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/examples/training_arima_report.py` & `krisi-0.1.0/examples/training_arima_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         y_insample=train[target_col],
         insample_predictions=insample_prediction,
         y_outsample=test[target_col],
         outsample_predictions=outsample_prediction,
     )
 
     """ Console log Reports """
-    report_outsample.print_summary()
-    report_insample.print_summary(extended=True)
+    report_outsample.print()
+    report_insample.print("extended")
 
     return report_insample, report_outsample
 
 
 if __name__ == "__main__":
     training_arima_report()
```

### Comparing `krisi-0.0.8/src/krisi/evaluate/assertions.py` & `krisi-0.1.0/src/krisi/evaluate/assertions.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/evaluate/metric.py` & `krisi-0.1.0/src/krisi/evaluate/metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,22 +77,37 @@
                     for i in range(len(y) - 1)
                 ]
         except Exception as e:
             result_rolling = e
 
         self.__safe_set(result_rolling, key="result_rolling")
 
+    def is_evaluated(self, rolling: bool = False):
+        if rolling:
+            return self.result_rolling is not None
+        else:
+            return self.result is not None
+
     def get_diagram_over_time(self) -> Optional[List[InteractiveFigure]]:
         return create_diagram_rolling(self)
 
     def get_diagrams(
         self,
     ) -> Optional[List[InteractiveFigure]]:
         return create_diagram(self)
 
+    def print(
+        self,
+        mode: Union[str, List[str]] = "dummy",
+        with_info: bool = False,
+        input_analysis: bool = True,
+        title: Optional[str] = None,
+    ) -> None:
+        pass
+
     def __safe_set(
         self, result: Union[Exception, MetricResult, List[MetricResult]], key: str
     ):
         if self.__dict__[key] is not None:
             raise ValueError("This metric already contains a result.")
         else:
             self.__dict__[key] = result
```

### Comparing `krisi-0.0.8/src/krisi/evaluate/score.py` & `krisi-0.1.0/src/krisi/evaluate/score.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/evaluate/scorecard.py` & `krisi-0.1.0/src/krisi/evaluate/scorecard.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,35 @@
 )
 from krisi.evaluate.library.default_metrics_regression import all_regression_metrics
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.type import (
     MetricCategories,
     PathConst,
     Predictions,
+    PrintMode,
     SampleTypes,
     SaveModes,
     ScoreCardMetadata,
     Targets,
 )
 from krisi.evaluate.utils import handle_unnamed
-from krisi.report.console import get_minimal_summary, get_summary
+from krisi.report.console import (
+    get_large_metric_summary,
+    get_minimal_summary,
+    get_summary,
+)
 from krisi.report.report import create_report_from_scorecard
 from krisi.report.type import DisplayModes, InteractiveFigure
 from krisi.utils.io import save_console, save_minimal_summary, save_object
 from krisi.utils.iterable_helpers import (
     flatten,
     map_newdict_on_olddict,
     remove_nans,
     strip_builtin_functions,
+    wrap_in_list,
 )
 
 
 @dataclass
 class ScoreCard:
     """ScoreCard Object.
 
@@ -47,15 +53,15 @@
     Examples
     --------
     >>> from krisi import ScoreCard
     ... y_pred, y_true = [0, 2, 1, 3], [0, 1, 2, 3]
     ... sc = ScoreCard()
     ... sc.evaluate(y_pred, y_true, defaults=True) # Calculate predefined metrics
     ... sc["own_metric"] = (y_pred - y_true).mean() # Add a metric result directly
-    ... sc.print_summary(extended=True)
+    ... sc.print('extended')
     """
 
     y: Targets
     predictions: Predictions
     sample_type: SampleTypes
     default_metrics_keys: List[str]
     custom_metrics_keys: List[str]
@@ -118,28 +124,34 @@
 
         for metric in custom_metrics:
             self.__dict__[metric.key] = deepcopy(metric)
 
     def __setitem__(self, key: str, item: Any) -> None:
         self.__setattr__(key, item)
 
-    def __getitem__(self, key: str) -> Any:
-        return getattr(self, key, "Unknown metric")
+    def __getitem__(self, key: Union[str, List[str]]) -> Union["ScoreCard", Metric]:
+        if isinstance(key, List):
+            scorecard_copy = deepcopy(self)
+            all_keys = list(scorecard_copy.__dict__.keys())
+            for k in all_keys:
+                if k not in key:
+                    if isinstance(scorecard_copy.__dict__[k], Metric):
+                        del scorecard_copy.__dict__[k]
+
+            return scorecard_copy
+        elif isinstance(key, str):
+            return getattr(self, key, Metric("Unknown Metric"))
 
     def __delitem__(self, key: str) -> None:
-        setattr(self, key, None)
+        del self[key]
 
     def __str__(self) -> str:
         print(Pretty(self.__dict__))
         return ""
 
-    def __repr__(self) -> str:
-        print(Pretty(self.__dict__))
-        return ""
-
     def __setattr__(self, key: str, item: Any) -> None:
         """Defines Dictionary like behaviour and ensures that a Metric can be
         added as a
             - Metric object,
             - Dictionary,
             - Direct result (float, int or a List of float or int). Gets wrapped in a ``Metric`` object
 
@@ -222,41 +234,54 @@
         regression, classification, multi-label classification.
 
 
         Returns
         -------
         List of Metrics
         """
-        return [self.__dict__[key] for key in self.default_metrics_keys]
+        return [
+            self.__dict__[key]
+            for key in self.default_metrics_keys
+            if key in self.__dict__
+        ]
 
     def get_custom_metrics(self) -> List[Metric]:
         """Returns a List of Custom ``Metric``s defined by the user on initalization
         of the ``ScoreCard``
 
         Returns
         -------
         List of Metrics
         """
         predifined_custom_metrics = [
-            self.__dict__[key] for key in self.custom_metrics_keys
+            self.__dict__[key]
+            for key in self.custom_metrics_keys
+            if key in self.__dict__
         ]
         modified_custom_metrics = [
             value
             for key, value in self.__dict__.items()
             if key not in self.custom_metrics_keys + self.default_metrics_keys
             and hasattr(value, "key")
         ]
 
         return predifined_custom_metrics + modified_custom_metrics
 
-    def get_all_metrics(self, defaults: bool = True) -> List[Metric]:
+    def get_all_metrics(
+        self, defaults: bool = True, only_evaluated: bool = False
+    ) -> List[Metric]:
         if defaults:
-            return self.get_default_metrics() + self.get_custom_metrics()
+            metrics = self.get_default_metrics() + self.get_custom_metrics()
         else:
-            return self.get_custom_metrics()
+            metrics = self.get_custom_metrics()
+
+        if only_evaluated:
+            return [metric for metric in metrics if metric.is_evaluated()]
+        else:
+            return metrics
 
     def evaluate(self, defaults: bool = True) -> "ScoreCard":
         """Evaluates ``Metric``s present on the ``ScoreCard``
 
         Parameters
         ----------
         y: Targets = Union[np.ndarray, pd.Series, List[Union[int, float]]]
@@ -307,32 +332,60 @@
         self: ScoreCard
         """
         for metric in self.get_all_metrics(defaults=defaults):
             if metric.restrict_to_sample is not self.sample_type:
                 metric.evaluate_over_time(self.y, self.predictions, window=window)
         return self
 
-    def print_summary(
+    def print(
         self,
+        mode: Union[str, PrintMode, List[PrintMode], List[str]] = PrintMode.extended,
         with_info: bool = False,
-        extended: bool = True,
         input_analysis: bool = True,
+        title: Optional[str] = None,
+        frame_or_series: bool = True,
     ) -> None:
-        if extended:
-            summary = get_summary(
-                self,
-                repr=True,
-                categories=[el.value for el in MetricCategories],
-                with_info=with_info,
-                input_analysis=input_analysis,
-            )
-        else:
-            summary = get_minimal_summary(self)
+        """
+        Prints the ScoreCard to the console.
+
+        Parameters
+        ----------
+        mode: Union[str, PrintMode, List[PrintMode], List[str]] = PrintMode.extended
+            - PrintMode.extended or 'extended' prints the full ScoreCard, with targets, predictions, residuals, etc.
+            - PrintMode.minimal or 'minimal' prints the name and the matching result of each metric in the ScoreCard, without fancy formatting
+            - PrintMode.minimal_table or 'minimal_table' creates a table format of just the metric name and the accompanying result
+
+        with_info: bool
+            Wether descriptions of each metrics should be printed or not
 
-        print(summary)
+        input_analysis: bool = True
+            Wether it should print analysis about the raw `targets` and `predictions`
+
+        title: Optional[str] = None
+            Title of the table when mode = 'minimal_table'
+        """
+
+        modes = [PrintMode.from_str(mode_) for mode_ in wrap_in_list(mode)]
+        if title is None:
+            title = self.metadata.project_name
+        for mode in modes:
+            if mode is PrintMode.extended:
+                print(
+                    get_summary(
+                        self,
+                        repr=True,
+                        categories=[el.value for el in MetricCategories],
+                        with_info=with_info,
+                        input_analysis=input_analysis,
+                    )
+                )
+            elif mode is PrintMode.minimal:
+                print(get_minimal_summary(self, dataframe=frame_or_series))
+            elif mode is PrintMode.minimal_table:
+                print(get_large_metric_summary(self, title))
 
     def save(
         self,
         path: Path = PathConst.default_eval_output_path,
         with_info: bool = False,
         save_modes: List[Union[SaveModes, str]] = [
             SaveModes.minimal,
```

### Comparing `krisi-0.0.8/src/krisi/evaluate/type.py` & `krisi-0.1.0/src/krisi/evaluate/type.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,7 +59,23 @@
 class ScoreCardMetadata:
     project_name: str = ""
     project_description: str = ""
     model_name: str = ""
     model_description: str = ""
     dataset_name: str = ""
     dataset_description: str = ""
+
+
+class PrintMode(Enum):
+    extended = "extended"
+    minimal = "minimal"
+    minimal_table = "minimal_table"
+
+    @staticmethod
+    def from_str(value: Union[str, "PrintMode"]) -> "PrintMode":
+        if isinstance(value, PrintMode):
+            return value
+        for strategy in PrintMode:
+            if strategy.value == value:
+                return strategy
+        else:
+            raise ValueError(f"Unknown PrintMode: {value}")
```

### Comparing `krisi-0.0.8/src/krisi/evaluate/utils.py` & `krisi-0.1.0/src/krisi/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-0.1.0/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-0.1.0/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/evaluate/library/diagrams.py` & `krisi-0.1.0/src/krisi/evaluate/library/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/console.py` & `krisi-0.1.0/src/krisi/report/console.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import TYPE_CHECKING, Iterable, List, Union
 
+import pandas as pd
 from rich import box
 from rich.console import Group
 from rich.layout import Layout
 from rich.panel import Panel
+from rich.table import Table
 
 from krisi.utils.iterable_helpers import group_by_categories
 from krisi.utils.printing import (
     create_metric_table,
     create_y_pred_table,
     metrics_empty_in_category,
 )
@@ -29,38 +31,62 @@
         obj.result is None
         and obj.result_rolling is not None
         and isinstance(obj.result_rolling, Iterable)
     ):
         result_ = (
             "[" + ", ".join([f"{result:<0.5}" for result in obj.result_rolling]) + "]"
         )
+    elif obj.result is None:
+        result_ = ""
+    elif isinstance(obj.result, Iterable) and not isinstance(obj.result, str):
+        result_ = obj.result
     else:
         result_ = f"{obj.result:<15.5}"
 
     return f"{obj.name:>40s} ({obj.key}): {result_}{hyperparams:>15s}"
 
 
-def get_minimal_summary(obj: "ScoreCard") -> str:
+def get_minimal_summary(obj: "ScoreCard", dataframe: bool) -> Union[pd.DataFrame, str]:
+    if dataframe:
+        all_metrics = [
+            metric
+            for metric in obj.get_all_metrics()
+            if isinstance(metric.result, (float, int))
+        ]
+        return pd.Series(
+            [metric.result for metric in all_metrics],
+            name=obj.metadata.model_name,
+            index=[f"{metric.name:>40s}" for metric in all_metrics],
+        ).to_frame()
+
     return "\n".join(
         [
             f"{metric.name:>40s} - {metric.result:<15.5}"
             for metric in obj.get_all_metrics()
             if isinstance(metric.result, (float, int))
         ]
     )
 
 
+def get_large_metric_summary(obj: "ScoreCard", title: str) -> Table:
+    return create_metric_table(
+        title=title,
+        metrics=obj.get_all_metrics(),
+        with_info=False,
+        with_parameters=False,
+    )
+
+
 def get_summary(
     obj: "ScoreCard",
     categories: List[str],
     repr: bool = True,
     with_info: bool = False,
     input_analysis: bool = True,
 ) -> Union[Panel, Layout]:
-
     category_groups = group_by_categories(list(vars(obj).values()), categories)
     input_analysis_table = (
         [create_y_pred_table(obj.classification, obj.y, obj.predictions)]
         if input_analysis
         else []
     )
```

### Comparing `krisi-0.0.8/src/krisi/report/interactive.py` & `krisi-0.1.0/src/krisi/report/interactive.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/pdf.py` & `krisi-0.1.0/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/report.py` & `krisi-0.1.0/src/krisi/report/report.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/type.py` & `krisi-0.1.0/src/krisi/report/type.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/library/console/diagrams.py` & `krisi-0.1.0/src/krisi/report/library/console/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/library/pdf_layouts/default/template.html` & `krisi-0.1.0/src/krisi/report/library/pdf_layouts/default/template.html`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/utils/console_plot.py` & `krisi-0.1.0/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/utils/data.py` & `krisi-0.1.0/src/krisi/utils/data.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/utils/io.py` & `krisi-0.1.0/src/krisi/utils/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Union
 
+import pandas as pd
 from rich.console import Console
 
 from krisi.evaluate.type import MetricCategories, PathConst, SaveModes
 from krisi.report.console import get_minimal_summary, get_summary
 
 if TYPE_CHECKING:
     from krisi.evaluate.scorecard import ScoreCard
@@ -45,16 +46,21 @@
         console.save_svg(
             os.path.join(path, Path("console.svg")),
             title="save_table_svg.py",
             clear=False,
         )
 
 
-def save_minimal_summary(obj: "ScoreCard", path: Path) -> None:
-    text_summary = get_minimal_summary(obj)
+def save_minimal_summary(
+    obj: "ScoreCard", path: Path, frame_or_series: bool = True
+) -> None:
+    text_summary = get_minimal_summary(obj, dataframe=frame_or_series)
+
+    if isinstance(text_summary, (pd.Series, pd.DataFrame)):
+        text_summary = text_summary.to_string()
 
     final_path = Path(os.path.join(path, Path("minimal.txt")))
 
     with open(final_path, "w", encoding="utf-8") as f:
         f.write(text_summary)
```

### Comparing `krisi-0.0.8/src/krisi/utils/iterable_helpers.py` & `krisi-0.1.0/src/krisi/utils/iterable_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
 from krisi.evaluate.type import Predictions, Targets
 
 if TYPE_CHECKING:
@@ -94,7 +94,14 @@
         return [el for el in iter if el is not None]
     else:
         return {key: el for key, el in iter.items() if el is not None}
 
 
 def calculate_nans(ds: Union[Targets, Predictions]) -> int:
     return ds.isna().sum() if isinstance(ds, pd.Series) else sum(np.isnan(ds))
+
+
+T = TypeVar("T")
+
+
+def wrap_in_list(input: Union[T, List[T]]) -> List[T]:
+    return input if isinstance(input, List) else [input]
```

### Comparing `krisi-0.0.8/src/krisi/utils/models.py` & `krisi-0.1.0/src/krisi/utils/models.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/src/krisi/utils/printing.py` & `krisi-0.1.0/src/krisi/utils/printing.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,28 +49,35 @@
         else:
             # Create a Console Plot
             return plotextMixin(result, line_plot, title=metric.name)
     else:
         return Pretty(result, max_depth=2, max_length=3)
 
 
-def __create_metric(metric: "Metric", with_info: bool) -> List[str]:
-    metric_summarized = [
-        f"{metric.name} ({metric.key})",
-        __display_result(metric),
-        Pretty(metric.parameters),
-        Pretty(metric.info),
-    ]
-    metric_summarized = metric_summarized if with_info else metric_summarized[:-1]
+def __create_metric(
+    metric: "Metric", with_info: bool, with_parameters: bool
+) -> List[str]:
+    metric_summarized = (
+        [
+            f"{metric.name} ({metric.key})",
+            __display_result(metric),
+        ]
+        + ([Pretty(metric.parameters)] if with_parameters else [])
+        + ([Pretty(metric.info)] if with_info else [])
+    )
 
     return metric_summarized
 
 
 def create_metric_table(
-    title: str, metrics: List["Metric"], with_info: bool, show_header: bool = False
+    title: str,
+    metrics: List["Metric"],
+    with_info: bool,
+    show_header: bool = False,
+    with_parameters: bool = True,
 ) -> Table:
     table = Table(
         title=title,
         # show_edge=False,
         show_footer=False,
         show_lines=True,
         show_header=show_header,
@@ -78,22 +85,23 @@
         box=box.ROUNDED,
     )
 
     table.add_column(
         "Metric Name", justify="right", style="cyan", width=1, no_wrap=False
     )
     table.add_column("Result", style="magenta", width=5)
-    table.add_column("Parameters", style="green", width=1)
+    if with_parameters:
+        table.add_column("Parameters", style="green", width=1)
     if with_info:
         table.add_column("Info", width=3)
 
     for metric in metrics:
         if metric.result is None and metric.result_rolling is None:
             continue
-        metric_summarized = __create_metric(metric, with_info)
+        metric_summarized = __create_metric(metric, with_info, with_parameters)
         table.add_row(*metric_summarized)
 
     return table
 
 
 def metrics_empty_in_category(metrics: List["Metric"]) -> bool:
     return (
```

### Comparing `krisi-0.0.8/src/krisi/utils/runner.py` & `krisi-0.1.0/src/krisi/utils/runner.py`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/.gitignore` & `krisi-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/LICENSE` & `krisi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-0.0.8/README.md` & `krisi-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-
-
-<p align="center">
-  <a href="https://dream-faster.github.io/krisi/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/krisi/docs.yaml?logo=readthedocs"></a>
-  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-  <a href="https://github.com/dream-faster/fold/actions/workflows/tests.yaml"><img alt="Tests" src="https://github.com/dream-faster/fold/actions/workflows/tests.yaml/badge.svg"/></a>
-  <a href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
+<p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
+  <a style="margin:2px" href="https://dream-faster.github.io/krisi/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/krisi/docs.yaml?logo=readthedocs"></a>
+  <a style="margin:2px" href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+  <a style="margin:2px" href="https://github.com/dream-faster/krisi/actions/workflows/tests.yaml"><img alt="Tests" src="https://github.com/dream-faster/krisi/actions/workflows/tests.yaml/badge.svg"/></a>
+  <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
 </p>
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/krisi/">
@@ -82,15 +80,15 @@
 
 You can quickly evaluate your predictions by running:
 
 ```python
 import numpy as np
 from krisi.evaluate import score
 
-score(y=np.random.rand(1000), predictions=np.random.rand(1000)).print_summary()
+score(y=np.random.rand(1000), predictions=np.random.rand(1000)).print()
 ```
 
 Krisi's main object is the ``ScoreCard`` that contains predefined ``Metric``s and which you can add further ``Metric``s to.
 
 
 ```python
 from krisi.evaluate import ScoreCard
@@ -104,15 +102,15 @@
 # Calculate predefined metrics
 sc.evaluate(defaults=True)
 
 # Add a new metric
 sc["own_metric"] = (target - predictions).mean()
 
 # Print the result
-sc.print_summary()
+sc.print()
 ```
 Outputs:
 ```
 ┏━━━━━━━━━━━━━━━━━━━━━━━━ Result of <your_model_name> on <your_dataset_name> tested on insample ━━━━━━━━━━━━━━━━━━━━━━━━━┓
 ┃                                                                                                                        ┃
 ┃                                                  Residual Diagnostics                                                  ┃
 ┃ ╭───────────────────────────┬─────────────────────────────────────────────────────────────┬──────────────────────────╮ ┃
@@ -180,15 +178,15 @@
     parameters={"hyper_1": 5.0},
 )
 
 # Updating the metadata of an existing metric
 sc.metric_barebones = dict(info="Giving description to a metric")
 
 # Print a pretty summary to the console
-sc.print_summary(with_info=True)
+sc.print(with_info=True)
 ```
 Outputs:
 ```
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ Result of <your_model_name> on <your_dataset_name> tested on insample ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
 ┃                                                                                                                                 ┃
 ┃                                                      Residual Diagnostics                                                       ┃
 ┃ ╭─────────────────────┬────────────────────────────────────────────────┬────────────────────┬─────────────────────────────────╮ ┃
@@ -273,18 +271,22 @@
 - Mean Absolute Error
 - Mean Absolute Percentage Error
 - Mean Squared Error
 - Root Mean Squared Error
 - Root Mean Squared Log Error
 
 
+## Our Open-core Time Series Toolkit
 
+[![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
+[![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
+[![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
+[![Fold/Wrapper](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
 
+If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/mark-szulyovszky/consultation)!
 
 ## Contribution
 
+Join our [Discord](https://discord.gg/EKJQgfuBpE) for live discussion!
 
-The project uses ``isort`` and ``black`` for formatting.
-
-Submit an issue or reach out to us on info at dreamfaster.ai for any inquiries.
+Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
 
-[Join our Discord community!](https://discord.gg/EKJQgfuBpE)
```

#### html2text {}

```diff
@@ -28,22 +28,22 @@
 quickly look at results pretty printed to the console.**
 ## Installation The project was entirely built in ``python``. Prerequisites *
 ``python >= 3.7`` and ``pip`` Then run: * ``pip install krisi`` If you'd like
 to also use interactive plotting (html) and pdf generation then run: * ``pip
 install krisi "krisi[plotting]"``
 ## Quickstart You can quickly evaluate your predictions by running: ```python
 import numpy as np from krisi.evaluate import score score(y=np.random.rand
-(1000), predictions=np.random.rand(1000)).print_summary() ``` Krisi's main
-object is the ``ScoreCard`` that contains predefined ``Metric``s and which you
-can add further ``Metric``s to. ```python from krisi.evaluate import ScoreCard
-import numpy as np # Random targets and predictions for Demo target,
-predictions = np.random.rand(1000), np.random.rand(1000) sc = ScoreCard(target,
-predictions) # Calculate predefined metrics sc.evaluate(defaults=True) # Add a
-new metric sc["own_metric"] = (target - predictions).mean() # Print the result
-sc.print_summary() ``` Outputs: ```
+(1000), predictions=np.random.rand(1000)).print() ``` Krisi's main object is
+the ``ScoreCard`` that contains predefined ``Metric``s and which you can add
+further ``Metric``s to. ```python from krisi.evaluate import ScoreCard import
+numpy as np # Random targets and predictions for Demo target, predictions =
+np.random.rand(1000), np.random.rand(1000) sc = ScoreCard(target, predictions)
+# Calculate predefined metrics sc.evaluate(defaults=True) # Add a new metric sc
+["own_metric"] = (target - predictions).mean() # Print the result sc.print()
+``` Outputs: ```
 âââââââââââââââââââââââââ
 Result of  on  tested on insample
 ââââââââââââââââââââââââââ
 â â â Residual Diagnostics â â
 â­ââââââââââââââââââââââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¬âââââââââââââââââââââââââââ®
 â â â Metric Name â Result â Parameters â â â
 âââââââââââââââââââââââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¼âââââââââââââââââââââââââââ¤
@@ -85,15 +85,15 @@
 (target - predictions).mean() # Adding a simple new metric (a float) # As a
 Dictionary: sc["metric_barebones"] = calculated_metric_example # As an Object
 assignment: sc.another_metric_barebones = calculated_metric_example * 2.0 sc
 ["metric_with_metadata"] = Metric( name="A new, own Metric",
 category=MetricCategories.residual, result=calculated_metric_example * 3.0,
 parameters={"hyper_1": 5.0}, ) # Updating the metadata of an existing metric
 sc.metric_barebones = dict(info="Giving description to a metric") # Print a
-pretty summary to the console sc.print_summary(with_info=True) ``` Outputs: ```
+pretty summary to the console sc.print(with_info=True) ``` Outputs: ```
 ââââââââââââââââââââââââââââââ
 Result of  on  tested on insample
 ââââââââââââââââââââââââââââââ
 â â â Residual Diagnostics â â
 â­ââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââââ¬âââââââââââââââââââââ¬ââââââââââââââââââââââââââââââââââ®
 â â â Metric Name â Result â Parameters â Info â â â
 âââââââââââââââââââââââ¼âââââââââââââââââââââââââââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââââââââââââââ¤
@@ -152,11 +152,23 @@
 ```
 ## Default Metrics See ``evaluate/library/default_metrics.py`` for source.
 Contributors are continously adding new default metrics, press watch to keep
 track of the project and see in issues planned default metrics. Residual
 Diagnostics - Mean of the Residuals - Standard Deviation of the Residuals -
 Ljung Box Statistics - (wip) Autocorrelation of Residuals Regression Errors -
 Mean Absolute Error - Mean Absolute Percentage Error - Mean Squared Error -
-Root Mean Squared Error - Root Mean Squared Log Error ## Contribution The
-project uses ``isort`` and ``black`` for formatting. Submit an issue or reach
-out to us on info at dreamfaster.ai for any inquiries. [Join our Discord
-community!](https://discord.gg/EKJQgfuBpE)
+Root Mean Squared Error - Root Mean Squared Log Error ## Our Open-core Time
+Series Toolkit [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/
+main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://
+github.com/dream-faster/krisi) [![Fold](https://raw.githubusercontent.com/
+dream-faster/fold/main/docs/images/overview_diagrams/
+dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold) [![Fold/
+Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
+overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/
+dream-faster/fold-models) [![Fold/Wrapper](https://raw.githubusercontent.com/
+dream-faster/fold/main/docs/images/overview_diagrams/
+dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-
+wrappers) If you want to try them out, we'd love to hear about your use case
+and help, [please book a free 30-min call with us](https://calendly.com/mark-
+szulyovszky/consultation)! ## Contribution Join our [Discord](https://
+discord.gg/EKJQgfuBpE) for live discussion! Submit an issue or reach out to us
+on info at dream-faster.ai for any inquiries.
```

### Comparing `krisi-0.0.8/pyproject.toml` & `krisi-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -129,15 +129,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-0.0.8/PKG-INFO` & `krisi-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 0.0.8
+Version: 0.1.0
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
         
@@ -82,21 +82,19 @@
 Requires-Dist: isort~=5.10.1; extra == 'quality'
 Requires-Dist: pre-commit~=2.20.0; extra == 'quality'
 Provides-Extra: tests
 Requires-Dist: pytest-cov>=4.0; extra == 'tests'
 Requires-Dist: pytest~=7.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
 
-
-
-<p align="center">
-  <a href="https://dream-faster.github.io/krisi/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/krisi/docs.yaml?logo=readthedocs"></a>
-  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-  <a href="https://github.com/dream-faster/fold/actions/workflows/tests.yaml"><img alt="Tests" src="https://github.com/dream-faster/fold/actions/workflows/tests.yaml/badge.svg"/></a>
-  <a href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
+<p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
+  <a style="margin:2px" href="https://dream-faster.github.io/krisi/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/krisi/docs.yaml?logo=readthedocs"></a>
+  <a style="margin:2px" href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+  <a style="margin:2px" href="https://github.com/dream-faster/krisi/actions/workflows/tests.yaml"><img alt="Tests" src="https://github.com/dream-faster/krisi/actions/workflows/tests.yaml/badge.svg"/></a>
+  <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
 </p>
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/krisi/">
@@ -170,15 +168,15 @@
 
 You can quickly evaluate your predictions by running:
 
 ```python
 import numpy as np
 from krisi.evaluate import score
 
-score(y=np.random.rand(1000), predictions=np.random.rand(1000)).print_summary()
+score(y=np.random.rand(1000), predictions=np.random.rand(1000)).print()
 ```
 
 Krisi's main object is the ``ScoreCard`` that contains predefined ``Metric``s and which you can add further ``Metric``s to.
 
 
 ```python
 from krisi.evaluate import ScoreCard
@@ -192,15 +190,15 @@
 # Calculate predefined metrics
 sc.evaluate(defaults=True)
 
 # Add a new metric
 sc["own_metric"] = (target - predictions).mean()
 
 # Print the result
-sc.print_summary()
+sc.print()
 ```
 Outputs:
 ```
 ┏━━━━━━━━━━━━━━━━━━━━━━━━ Result of <your_model_name> on <your_dataset_name> tested on insample ━━━━━━━━━━━━━━━━━━━━━━━━━┓
 ┃                                                                                                                        ┃
 ┃                                                  Residual Diagnostics                                                  ┃
 ┃ ╭───────────────────────────┬─────────────────────────────────────────────────────────────┬──────────────────────────╮ ┃
@@ -268,15 +266,15 @@
     parameters={"hyper_1": 5.0},
 )
 
 # Updating the metadata of an existing metric
 sc.metric_barebones = dict(info="Giving description to a metric")
 
 # Print a pretty summary to the console
-sc.print_summary(with_info=True)
+sc.print(with_info=True)
 ```
 Outputs:
 ```
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ Result of <your_model_name> on <your_dataset_name> tested on insample ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
 ┃                                                                                                                                 ┃
 ┃                                                      Residual Diagnostics                                                       ┃
 ┃ ╭─────────────────────┬────────────────────────────────────────────────┬────────────────────┬─────────────────────────────────╮ ┃
@@ -361,18 +359,22 @@
 - Mean Absolute Error
 - Mean Absolute Percentage Error
 - Mean Squared Error
 - Root Mean Squared Error
 - Root Mean Squared Log Error
 
 
+## Our Open-core Time Series Toolkit
 
+[![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
+[![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
+[![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
+[![Fold/Wrapper](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
 
+If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/mark-szulyovszky/consultation)!
 
 ## Contribution
 
+Join our [Discord](https://discord.gg/EKJQgfuBpE) for live discussion!
 
-The project uses ``isort`` and ``black`` for formatting.
-
-Submit an issue or reach out to us on info at dreamfaster.ai for any inquiries.
+Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
 
-[Join our Discord community!](https://discord.gg/EKJQgfuBpE)
```


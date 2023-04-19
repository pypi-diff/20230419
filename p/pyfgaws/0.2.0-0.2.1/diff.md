# Comparing `tmp/pyfgaws-0.2.0.tar.gz` & `tmp/pyfgaws-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfgaws-0.2.0.tar", last modified: Fri Mar 10 00:50:12 2023, max compression
+gzip compressed data, was "pyfgaws-0.2.1.tar", last modified: Wed Apr 19 14:01:02 2023, max compression
```

## Comparing `pyfgaws-0.2.0.tar` & `pyfgaws-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.0/LICENSE
--rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.0/LICENSE
--rw-r--r--   0        0        0     2480 2022-06-14 04:40:34.280516 pyfgaws-0.2.0/README.md
--rw-r--r--   0        0        0       58 2022-06-02 20:36:50.013456 pyfgaws-0.2.0/pyfgaws/__init__.py
--rw-r--r--   0        0        0     1926 2023-03-10 00:49:14.418971 pyfgaws-0.2.0/pyfgaws/__main__.py
--rw-r--r--   0        0        0       81 2022-06-02 20:37:10.604331 pyfgaws-0.2.0/pyfgaws/batch/__init__.py
--rw-r--r--   0        0        0    21455 2023-03-10 00:49:14.419264 pyfgaws-0.2.0/pyfgaws/batch/api.py
--rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014080 pyfgaws-0.2.0/pyfgaws/batch/tests/__init__.py
--rw-r--r--   0        0        0     5802 2023-03-10 00:49:14.419509 pyfgaws-0.2.0/pyfgaws/batch/tests/test_api.py
--rw-r--r--   0        0        0    11210 2023-03-10 00:49:14.419728 pyfgaws-0.2.0/pyfgaws/batch/tools.py
--rw-r--r--   0        0        0     1137 2022-06-02 20:36:50.014555 pyfgaws-0.2.0/pyfgaws/core/__init__.py
--rw-r--r--   0        0        0     1295 2022-06-02 20:36:50.014672 pyfgaws-0.2.0/pyfgaws/core/logging.py
--rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014769 pyfgaws-0.2.0/pyfgaws/core/tests/__init__.py
--rw-r--r--   0        0        0      988 2022-06-02 20:36:50.014891 pyfgaws-0.2.0/pyfgaws/core/tests/test_core.py
--rw-r--r--   0        0        0      106 2022-06-02 20:36:50.015044 pyfgaws-0.2.0/pyfgaws/logs/__init__.py
--rw-r--r--   0        0        0     2309 2023-03-10 00:49:14.419917 pyfgaws-0.2.0/pyfgaws/logs/api.py
--rw-r--r--   0        0        0        0 2022-06-02 20:36:50.015263 pyfgaws-0.2.0/pyfgaws/logs/tests/__init__.py
--rw-r--r--   0        0        0     3165 2023-03-10 00:49:14.420126 pyfgaws-0.2.0/pyfgaws/logs/tests/test_api.py
--rw-r--r--   0        0        0     1303 2023-03-10 00:49:14.420356 pyfgaws-0.2.0/pyfgaws/logs/tools.py
--rw-r--r--   0        0        0     1711 2023-03-10 00:49:14.420575 pyfgaws-0.2.0/pyfgaws/tests/__init__.py
--rw-r--r--   0        0        0     2132 2023-03-10 00:49:14.420771 pyfgaws-0.2.0/pyfgaws/tests/test_main.py
--rw-r--r--   0        0        0     1329 2023-03-10 00:49:45.097990 pyfgaws-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3620 2023-03-10 00:50:12.726976 pyfgaws-0.2.0/setup.py
--rw-r--r--   0        0        0     3706 2023-03-10 00:50:12.727286 pyfgaws-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1081 2022-06-02 20:36:50.012095 pyfgaws-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2480 2022-06-14 04:40:34.280516 pyfgaws-0.2.1/README.md
+-rw-r--r--   0        0        0       58 2022-06-02 20:36:50.013456 pyfgaws-0.2.1/pyfgaws/__init__.py
+-rw-r--r--   0        0        0     1926 2023-03-10 00:49:14.418971 pyfgaws-0.2.1/pyfgaws/__main__.py
+-rw-r--r--   0        0        0       81 2022-06-02 20:37:10.604331 pyfgaws-0.2.1/pyfgaws/batch/__init__.py
+-rw-r--r--   0        0        0    21455 2023-03-10 00:49:14.419264 pyfgaws-0.2.1/pyfgaws/batch/api.py
+-rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014080 pyfgaws-0.2.1/pyfgaws/batch/tests/__init__.py
+-rw-r--r--   0        0        0     5802 2023-03-10 00:49:14.419509 pyfgaws-0.2.1/pyfgaws/batch/tests/test_api.py
+-rw-r--r--   0        0        0    12325 2023-04-19 14:00:10.882084 pyfgaws-0.2.1/pyfgaws/batch/tools.py
+-rw-r--r--   0        0        0     1137 2022-06-02 20:36:50.014555 pyfgaws-0.2.1/pyfgaws/core/__init__.py
+-rw-r--r--   0        0        0     1295 2022-06-02 20:36:50.014672 pyfgaws-0.2.1/pyfgaws/core/logging.py
+-rw-r--r--   0        0        0        0 2022-06-02 20:36:50.014769 pyfgaws-0.2.1/pyfgaws/core/tests/__init__.py
+-rw-r--r--   0        0        0      988 2022-06-02 20:36:50.014891 pyfgaws-0.2.1/pyfgaws/core/tests/test_core.py
+-rw-r--r--   0        0        0      106 2022-06-02 20:36:50.015044 pyfgaws-0.2.1/pyfgaws/logs/__init__.py
+-rw-r--r--   0        0        0     2309 2023-03-10 00:49:14.419917 pyfgaws-0.2.1/pyfgaws/logs/api.py
+-rw-r--r--   0        0        0        0 2022-06-02 20:36:50.015263 pyfgaws-0.2.1/pyfgaws/logs/tests/__init__.py
+-rw-r--r--   0        0        0     3165 2023-03-10 00:49:14.420126 pyfgaws-0.2.1/pyfgaws/logs/tests/test_api.py
+-rw-r--r--   0        0        0     1303 2023-03-10 00:49:14.420356 pyfgaws-0.2.1/pyfgaws/logs/tools.py
+-rw-r--r--   0        0        0     1711 2023-03-10 00:49:14.420575 pyfgaws-0.2.1/pyfgaws/tests/__init__.py
+-rw-r--r--   0        0        0     2132 2023-03-10 00:49:14.420771 pyfgaws-0.2.1/pyfgaws/tests/test_main.py
+-rw-r--r--   0        0        0     1329 2023-04-19 14:00:43.396323 pyfgaws-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3620 2023-04-19 14:01:02.576784 pyfgaws-0.2.1/setup.py
+-rw-r--r--   0        0        0     3706 2023-04-19 14:01:02.577065 pyfgaws-0.2.1/PKG-INFO
```

### Comparing `pyfgaws-0.2.0/LICENSE` & `pyfgaws-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/README.md` & `pyfgaws-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/__main__.py` & `pyfgaws-0.2.1/pyfgaws/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/batch/api.py` & `pyfgaws-0.2.1/pyfgaws/batch/api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/batch/tests/test_api.py` & `pyfgaws-0.2.1/pyfgaws/batch/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/batch/tools.py` & `pyfgaws-0.2.1/pyfgaws/batch/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -229,48 +229,63 @@
 def monitor(
     *,
     job_ids: Optional[List[str]] = None,
     queue: Optional[str] = None,
     region_name: Optional[str] = None,
     delay: Optional[int] = None,
     per_job: bool = False,
+    monitor_queue: bool = False,
 ) -> None:
     """Monitor the Batch jobs with given job identifiers or job queue.
 
+    If job identifiers are given, then this tool will exit once all jobs have reached a terminal
+    state.  If a job queue is given, then this tool will keep polling for new jobs as long as there
+    are known jobs that are not in a terminal state.  In other words, exit once all known jobs have
+    completed, and if a queue is given, keep checking to see if any new jobs show up.
+
     Args:
         job_ids: the AWS batch job identifier(s)
         queue: the name of the AWS batch queue
         region_name: the AWS region
         delay: the number of seconds to wait after polling for status(es).
         per_job: true to monitor per-job status information, otherwise jobs will be summarized by
                   status
+        monitor-queue: never exit and keep monitoring for new jobs.  Can only be used with the
+                       `--queue` option
     """
     logger = logging.getLogger(__name__)
     assert (
         job_ids is not None or queue is not None
     ), "Either --job-ids or --queue must be specified"
     assert job_ids is None or queue is None, "Both --job-ids or --queue cannot be specified"
+    assert queue is None or not monitor_queue, "--queue must be used with --monitor-queue"
 
     client: batch.Client = boto3.client(
         service_name="batch", region_name=region_name  # type: ignore
     )
 
-    # get the job ids from the queue if necessary
-    if job_ids is None:
-        logger.info(f"Retrieving job ids for queue: {queue}")
-        job_ids = list_jobs(client=client, queue=queue)
-
-    # get the list of batch jobs from job ids
-    jobs: List[BatchJob] = [BatchJob.from_id(client=client, job_id=job_id) for job_id in job_ids]
-
-    logger.info(f"Monitoring {len(job_ids):,d} jobs.")
+    # get the list of batch jobs from job ids.  If using a queue, the job ids will be retrieved
+    # later
+    jobs: List[BatchJob] = []
+    if job_ids is not None:
+        jobs = [BatchJob.from_id(client=client, job_id=job_id) for job_id in job_ids]
+        logger.info(f"Monitoring {len(job_ids):,d} jobs.")
+    else:
+        logger.info(f"Monitoring jobs for queue: {queue}")
 
     while True:
         print("\033[H")  # clear the screen!
-        logger.info("Polling job status")
+
+        # if monitoring a queue, get the full list of jobs
+        if queue is not None:
+            logger.info(f"Retrieving job ids for queue: {queue}")
+            # add newly seen jobs
+            for job_id in list_jobs(client=client, queue=queue):
+                if all(job_id != job.job_id for job in jobs):
+                    jobs.append(BatchJob.from_id(client=client, job_id=job_id))
 
         # print out detailed stats, and update status counts
         status_counts: Dict[Optional[Status], int] = {status: 0 for status in Status}
         status_counts[None] = 0
         table_detail: List[List[str]] = [["JOB_NAME", "JOB_ID", "STATUS"]]
         job: BatchJob
         num_done: int = 0
@@ -282,24 +297,27 @@
                 table_detail.append([job.name, job.job_id, status_name])
             if status is not None and (status == Status.Succeeded or status == Status.Failed):
                 num_done += 1
         print("\033[2J\033[H")  # clear the screen!
         if per_job:
             print(column_it(table_detail, delimiter="  "))
 
+        # we are done polling if we're not monitoring a queue and all the known jobs are complete
+        all_done = not monitor_queue and num_done == len(jobs)
+
         # print out summary stats
-        if num_done == len(job_ids) or not per_job:
+        if all_done or not per_job:
             table_summary: List[List[str]] = [["STATUS", "COUNT"]]
             for status, count in status_counts.items():
                 status_name = "Unknown" if status is None else status.name
                 table_summary.append([status_name, f"{count:,d}"])
             print("\033[2J\033[H")  # clear the screen!
             print(column_it(table_summary, delimiter="  "))
 
-        if num_done == len(job_ids):
+        if all_done:
             break
 
         if delay is None:
             time.sleep(DEFAULT_LOGS_POLLING_INTERVAL)
         else:
             time.sleep(delay)
```

### Comparing `pyfgaws-0.2.0/pyfgaws/core/__init__.py` & `pyfgaws-0.2.1/pyfgaws/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/core/logging.py` & `pyfgaws-0.2.1/pyfgaws/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/core/tests/test_core.py` & `pyfgaws-0.2.1/pyfgaws/core/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/logs/api.py` & `pyfgaws-0.2.1/pyfgaws/logs/api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/logs/tests/test_api.py` & `pyfgaws-0.2.1/pyfgaws/logs/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/logs/tools.py` & `pyfgaws-0.2.1/pyfgaws/logs/tools.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/tests/__init__.py` & `pyfgaws-0.2.1/pyfgaws/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyfgaws/tests/test_main.py` & `pyfgaws-0.2.1/pyfgaws/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyfgaws-0.2.0/pyproject.toml` & `pyfgaws-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfgaws"
-version = "0.2.0"
+version = "0.2.1"
 description = "Tools and python libraries for working with AWS."
 authors = ["Nils Homer", "Tim Fennell"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fulcrumgenomics/pyfgaws"
 repository = "https://github.com/fulcrumgenomics/pyfgaws"
 keywords = ["aws", "bioinformatics"]
```

### Comparing `pyfgaws-0.2.0/setup.py` & `pyfgaws-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'namegenerator>=1.0.6,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['fgaws-tools = pyfgaws.__main__:main']}
 
 setup_kwargs = {
     'name': 'pyfgaws',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Tools and python libraries for working with AWS.',
     'long_description': '\n[![Language][language-badge]][language-link]\n[![Code Style][code-style-badge]][code-style-link]\n[![Type Checked][type-checking-badge]][type-checking-link]\n[![PEP8][pep-8-badge]][pep-8-link]\n[![Code Coverage][code-coverage-badge]][code-coverage-link]\n[![License][license-badge]][license-link]\n\n---\n\n[![Python package][python-package-badge]][python-package-link]\n[![PyPI version][pypi-badge]][pypi-link]\n[![PyPI download total][pypi-downloads-badge]][pypi-downloads-link]\n\n---\n\n[language-badge]:       http://img.shields.io/badge/language-python-brightgreen.svg\n[language-link]:        http://www.python.org/\n[code-style-badge]:     https://img.shields.io/badge/code%20style-black-000000.svg\n[code-style-link]:      https://black.readthedocs.io/en/stable/ \n[type-checking-badge]:  http://www.mypy-lang.org/static/mypy_badge.svg\n[type-checking-link]:   http://mypy-lang.org/\n[pep-8-badge]:          https://img.shields.io/badge/code%20style-pep8-brightgreen.svg\n[pep-8-link]:           https://www.python.org/dev/peps/pep-0008/\n[code-coverage-badge]:  https://codecov.io/gh/fulcrumgenomics/pyfgaws/branch/main/graph/badge.svg\n[code-coverage-link]:   https://codecov.io/gh/fulcrumgenomics/pyfgaws\n[license-badge]:        http://img.shields.io/badge/license-MIT-blue.svg\n[license-link]:         https://github.com/fulcrumgenomics/pyfgaws/blob/main/LICENSE\n[python-package-badge]: https://github.com/fulcrumgenomics/pyfgaws/workflows/Python%20package/badge.svg\n[python-package-link]:  https://github.com/fulcrumgenomics/pyfgaws/actions?query=workflow%3A%22Python+package%22\n[pypi-badge]:           https://badge.fury.io/py/pyfgaws.svg\n[pypi-link]:            https://pypi.python.org/pypi/pyfgaws\n[pypi-downloads-badge]: https://img.shields.io/pypi/dm/pyfgaws\n[pypi-downloads-link]:  https://pypi.python.org/pypi/pyfgaws\n\n# pyfgaws\n\n`pip install pyfgaws`\n\n**Requires python 3.8**\n\n# Getting Setup\n\nConda is used to install a specific version of python and [poetry][poetry-link]\nwhich is then used to manage the python development environment.  If not already installed, install \n[miniconda from the latest platform-appropriate installer](miniconda-link). Then run:\n\n```\nconda create -n pyfgaws -c conda-forge -c bioconda --file conda-requirements.txt\n```\n\nThen activate the new environment and install the toolkit:\n\n```\nconda activate pyfgaws\npoetry install\n```\n\n[miniconda-link]: https://docs.conda.io/en/latest/miniconda.html\n[poetry-link]:    https://github.com/python-poetry/poetry\n',
     'author': 'Nils Homer',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fulcrumgenomics/pyfgaws',
```

### Comparing `pyfgaws-0.2.0/PKG-INFO` & `pyfgaws-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfgaws
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools and python libraries for working with AWS.
 Home-page: https://github.com/fulcrumgenomics/pyfgaws
 License: MIT
 Keywords: aws,bioinformatics
 Author: Nils Homer
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```


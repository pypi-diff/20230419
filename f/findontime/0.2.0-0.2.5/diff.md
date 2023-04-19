# Comparing `tmp/findontime-0.2.0.tar.gz` & `tmp/findontime-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findontime-0.2.0.tar", max compression
+gzip compressed data, was "findontime-0.2.5.tar", max compression
```

## Comparing `findontime-0.2.0.tar` & `findontime-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    31904 2023-04-09 11:15:18.037313 findontime-0.2.0/LICENSE
--rw-r--r--   0        0        0    11060 2023-04-14 12:51:03.222693 findontime-0.2.0/README.md
--rw-r--r--   0        0        0      875 2023-04-14 12:55:02.990727 findontime-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-11 13:13:09.220772 findontime-0.2.0/src/findontime/__init__.py
--rw-r--r--   0        0        0      315 2023-04-13 15:22:43.482616 findontime-0.2.0/src/findontime/__main__.py
--rw-r--r--   0        0        0     1997 2023-04-13 10:13:25.550855 findontime-0.2.0/src/findontime/configs.py
--rw-r--r--   0        0        0     9288 2023-04-13 13:28:27.639194 findontime-0.2.0/src/findontime/connectors.py
--rw-r--r--   0        0        0     3646 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/drones.py
--rw-r--r--   0        0        0    14936 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/insaflu_uploads.py
--rw-r--r--   0        0        0     9302 2023-04-13 14:13:56.590072 findontime-0.2.0/src/findontime/manager.py
--rw-r--r--   0        0        0     4822 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/plot_utils.py
--rw-r--r--   0        0        0     9902 2023-04-09 11:12:06.161507 findontime-0.2.0/src/findontime/plotting_from_all_reports.py
--rw-r--r--   0        0        0     3447 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/records.py
--rw-r--r--   0        0        0     3444 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/tables_post.py
--rw-r--r--   0        0        0    21536 2023-04-13 13:27:24.031739 findontime-0.2.0/src/findontime/upload_utils.py
--rw-r--r--   0        0        0    12293 2023-04-14 12:55:33.681719 findontime-0.2.0/setup.py
--rw-r--r--   0        0        0    11964 2023-04-14 12:55:33.682532 findontime-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    31904 2023-04-09 11:15:18.037313 findontime-0.2.5/LICENSE
+-rw-r--r--   0        0        0    11060 2023-04-14 12:51:03.222693 findontime-0.2.5/README.md
+-rw-r--r--   0        0        0      875 2023-04-19 11:19:11.744737 findontime-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-11 13:13:09.220772 findontime-0.2.5/src/findontime/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-13 15:22:43.482616 findontime-0.2.5/src/findontime/__main__.py
+-rw-r--r--   0        0        0     2471 2023-04-18 15:46:13.271182 findontime-0.2.5/src/findontime/configs.py
+-rw-r--r--   0        0        0     9288 2023-04-13 13:28:27.639194 findontime-0.2.5/src/findontime/connectors.py
+-rw-r--r--   0        0        0     3646 2023-04-11 13:01:20.270281 findontime-0.2.5/src/findontime/drones.py
+-rw-r--r--   0        0        0    16655 2023-04-19 11:17:45.199895 findontime-0.2.5/src/findontime/insaflu_uploads.py
+-rw-r--r--   0        0        0     9365 2023-04-18 15:46:17.183215 findontime-0.2.5/src/findontime/manager.py
+-rw-r--r--   0        0        0     4822 2023-04-11 13:01:20.270281 findontime-0.2.5/src/findontime/plot_utils.py
+-rw-r--r--   0        0        0     9902 2023-04-09 11:12:06.161507 findontime-0.2.5/src/findontime/plotting_from_all_reports.py
+-rw-r--r--   0        0        0     3447 2023-04-19 11:13:32.517266 findontime-0.2.5/src/findontime/records.py
+-rw-r--r--   0        0        0     3444 2023-04-11 13:01:20.270281 findontime-0.2.5/src/findontime/tables_post.py
+-rw-r--r--   0        0        0    21536 2023-04-13 13:27:24.031739 findontime-0.2.5/src/findontime/upload_utils.py
+-rw-r--r--   0        0        0    12293 2023-04-19 11:19:23.627763 findontime-0.2.5/setup.py
+-rw-r--r--   0        0        0    11964 2023-04-19 11:19:23.628511 findontime-0.2.5/PKG-INFO
```

### Comparing `findontime-0.2.0/LICENSE` & `findontime-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/README.md` & `findontime-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/pyproject.toml` & `findontime-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findontime"
-version = "0.2.0"
+version = "0.2.5"
 description = "A tool to upload Fastq files to the INSaFLU database and perform metagenomics pathogen detection"
 authors = ["SantosJGND <dourado.jns@gmail.com>", "insapathogenomics <insapathogenomics@insa.min-saude.pt>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `findontime-0.2.0/src/findontime/configs.py` & `findontime-0.2.5/src/findontime/configs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import sys
 from dataclasses import dataclass
 from typing import Optional, Type
 
 from fastq_handler.configs import InputState, OutputDirs, RunParams
+
 from findontime.tables_post import InsafluTables
 from findontime.upload_utils import InsafluUpload, UploadStrategy
 
 default_log_handler = logging.StreamHandler(sys.stdout)
 default_log_handler.setLevel(logging.INFO)
 formatter = logging.Formatter(
     '%(asctime)s - %(message)s')
@@ -39,14 +40,33 @@
     tsv_temp_name: str = "televir_metadata.tsv"
     metadata_dirname: str = "metadata_dir"
     logs_dirname: str = "logs"
     db_path: str = "insaflu.db"
 
 
 @dataclass
+class RunConfigMeta(InputState, RunParams, InfluOutput):
+    """
+    class to hold run config"""
+
+    def __post_init__(self):
+        """
+        post init
+        """
+        if self.actions is None:
+            self.actions = []
+
+        self.logs_dir = os.path.join(self.output_dir, self.logs_dirname)
+        self.output_dir = os.path.abspath(self.output_dir)
+
+        self.metadata_dir = os.path.join(
+            self.output_dir, self.metadata_dirname)
+
+
+@dataclass
 class InfluConfig(InfluParams, InfluUpload, InfluOutput):
     """
     TelevirConfig class
     """
 
     def __post_init__(self):
```

### Comparing `findontime-0.2.0/src/findontime/connectors.py` & `findontime-0.2.5/src/findontime/connectors.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/src/findontime/drones.py` & `findontime-0.2.5/src/findontime/drones.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/src/findontime/insaflu_uploads.py` & `findontime-0.2.5/src/findontime/insaflu_uploads.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import datetime
 import logging
 import os
 import sys
 from typing import List
 
 import pandas as pd
-
 from fastq_handler.fastq_handler import DirectoryProcessingSimple, PreMain
 from fastq_handler.records import Processed
+
 from findontime.configs import InfluConfig, default_log_handler
 from findontime.plot_utils import plot_project_results
 from findontime.records import InsafluFile, MetadataEntry
 from findontime.upload_utils import InsafluSampleCodes, InsafluUpload
 
 
 class InfluProcessed(Processed):
@@ -161,17 +161,19 @@
         )
 
     def insaflu_process(self):
         """
         prepare processed files for upload
         """
 
-        files_to_upload = self.processed.processed.fastq.tolist()
+        files_to_upload = self.processed.processed_fastq_list()
+
+        processed_df = self.processed.processed_entries
 
-        for ix, row in self.processed.processed.iterrows():
+        for ix, row in processed_df.iterrows():
 
             fastq_file = row.fastq
             merged_file = row.merged
             merged_name = self.get_filename_from_path(merged_file)
 
             if self.run_metadata.upload_strategy.is_to_upload(files_to_upload, ix):
                 status = self.uploader.get_sample_status(
@@ -209,55 +211,39 @@
         self.run_metadata = run_metadata
         self.uploader = run_metadata.uploader
         self.processed = InfluProcessed(
             self.run_metadata.logs_dir,
         )
 
 
-class InsafluFileProcess(PreMain, InsafluSetup):
+class PreMainWithMetadata(PreMain):
     """
-    InsafluUpload class
     """
+    metadata_dirname = "metadata_dir"
 
     processed: InfluProcessed
-    run_metadata: InfluConfig
-    projects_results: list = []
-    metadata_dirname = "metadata_dir"
 
     def __init__(self, run_metadata: InfluConfig):
-        PreMain.__init__(self, run_metadata)
-        InsafluSetup.__init__(self, run_metadata)
-
+        super().__init__(run_metadata)
         self.logger = logging.getLogger(__name__)
         self.logger.addHandler(default_log_handler)
 
         self.prep_metadata_dir()
-
-        self.test = False
+        self.run_metadata = run_metadata
+        self.processed = InfluProcessed(
+            self.run_metadata.logs_dir,
+        )
 
     def prep_metadata_dir(self):
         """
         create output directories
         """
 
         os.makedirs(self.run_metadata.metadata_dir, exist_ok=True)
 
-    def update_projects(self, project_file: str):
-        """
-        update project added
-        """
-        if project_file not in self.projects_results:
-            if os.path.exists(project_file):
-                self.projects_results.append(project_file)
-
-    def get_directory_processing(self, fastq_dir: str):
-
-        return InfluDirectoryProcessing(fastq_dir, self.run_metadata, self.processed,
-                                        self.start_time, test=self.test)
-
     def write_metadata(self, metadata: List[MetadataEntry], metadata_filename: str):
         """
         update metadata
         """
 
         metadata_df = [
             x.export_as_dataframe() for x in metadata
@@ -274,78 +260,150 @@
     def metadata_from_files(self, files_list: List[InsafluFile]) -> List[MetadataEntry]:
         """
         generate metadata from files
         """
         metadata_list = [
             self.processed.generate_metadata_entry(
                 x.file_path,
-                self.fastq_dir,
+                os.path.dirname(x.file_path),
                 x.remote_path,
                 tag=self.run_metadata.name_tag
             ) for x in files_list
         ]
         return metadata_list
 
-    def get_samples_to_submit(self) -> List[InsafluFile]:
-        """
-        get samples to submit
-        """
-        samples_to_submit = self.uploader.logger.generate_fastq_list_status(
-            InsafluSampleCodes.STATUS_UPLOADED)
-
-        return samples_to_submit
-
     def generate_metatadata_filename(self):
         """
         generate metadata filename
         """
         time_now = datetime.datetime.now()
         formatted_time = time_now.strftime("%Y%m%d_%H%M%S")
 
         metadata_filename = f"{self.run_metadata.name_tag}_{formatted_time}_metadata.tsv"
         return metadata_filename
 
-    def submit(self):
+    def get_samples_to_submit(self):
+        """
+        get samples to submit
+        """
+        files_to_upload = self.processed.processed.fastq.tolist()
+        merged_files = self.processed.processed.merged.tolist()
+        dirs = self.processed.processed.dir.tolist()
+
+        insaflu_file_list = []
+        for i, fastq1 in enumerate(files_to_upload):
+
+            _, barcode = self.processed.get_run_barcode(fastq1, self.fastq_dir)
+            sample_id = self.processed.get_sample_id_from_merged(
+                merged_files[i]
+            )
+
+            insaflu_file_list.append(
+                InsafluFile(
+                    sample_id=sample_id,
+                    barcode=barcode,
+                    file_path=os.path.join(dirs[i], fastq1),
+                    remote_path=merged_files[i],
+                    status=0)
+            )
+
+        return insaflu_file_list
+
+    def metadata_prepare(self):
         """
         submit sample to remote server"""
 
         samples_to_submit = self.get_samples_to_submit()
         sample_metadata = self.metadata_from_files(samples_to_submit)
 
         if len(sample_metadata) == 0:
-            return
+            return ""
 
         self.logger.info(f"Submitting {len(sample_metadata)} sample(s)")
 
-        self.submit_samples(sample_metadata)
+        insaflu_metadata_file = self.generate_metatadata_filename()
+        metadata_filepath = os.path.join(
+            self.run_metadata.metadata_dir,
+            insaflu_metadata_file
+        )
+
+        self.write_metadata(
+            sample_metadata,
+            metadata_filepath
+        )
+
+        return metadata_filepath
+
+    def run(self):
+        """
+        run main
+        """
+        super().run()
+        metadata_filepath = self.metadata_prepare()
+
+        return metadata_filepath
+
+
+class InsafluFileProcess(PreMainWithMetadata, InsafluSetup):
+    """
+    InsafluUpload class
+    """
+
+    processed: InfluProcessed
+    run_metadata: InfluConfig
+    projects_results: list = []
+    metadata_dirname = "metadata_dir"
+
+    def __init__(self, run_metadata: InfluConfig):
+        PreMainWithMetadata.__init__(self, run_metadata)
+        InsafluSetup.__init__(self, run_metadata)
+
+        self.test = False
+
+    def update_projects(self, project_file: str):
+        """
+        update project added
+        """
+        if project_file not in self.projects_results:
+            if os.path.exists(project_file):
+                self.projects_results.append(project_file)
+
+    def get_directory_processing(self, fastq_dir: str):
+
+        return InfluDirectoryProcessing(fastq_dir, self.run_metadata, self.processed,
+                                        self.start_time, test=self.test)
+
+    def get_samples_to_submit(self) -> List[InsafluFile]:
+        """
+        get samples to submit
+        """
+        samples_to_submit = self.uploader.logger.generate_fastq_list_status(
+            InsafluSampleCodes.STATUS_UPLOADED)
+
+        return samples_to_submit
 
     def clean_remote(self):
         """
         clean remote server
         """
         samples_to_clean = self.uploader.logger.generate_file_list_status(
             InsafluSampleCodes.STATUS_SUBMITTED)
 
         for file in samples_to_clean:
             self.uploader.clean_upload(file.remote_path)
 
-    def submit_samples(self, sample_metadata: List[MetadataEntry]):
+    def submit_samples(self, metadata_filepath: str):
         """
         submit samples
         """
-        insaflu_metadata_file = self.generate_metatadata_filename()
-        metadata_filepath = os.path.join(
-            self.run_metadata.metadata_dir,
-            insaflu_metadata_file
-        )
 
-        self.write_metadata(
-            sample_metadata,
-            metadata_filepath
-        )
+        if not os.path.exists(metadata_filepath):
+            return
+
+        insaflu_metadata_file = os.path.basename(metadata_filepath)
 
         self.uploader.upload_file(
             metadata_filepath,
             self.uploader.get_remote_path(insaflu_metadata_file),
             "metad",
             "metad",
             self.uploader.TAG_METADATA,
@@ -385,16 +443,17 @@
 
             file_name, _ = self.processed.get_run_info(fastq.file_path)
 
             _ = self.uploader.update_sample_status_remote(
                 file_name, fastq.file_path, test=self.test)
 
     def run(self):
-        super().run()
-        self.submit()
+        PreMainWithMetadata.run(self)
+        metadata_filepath = self.metadata_prepare()
+        self.submit_samples(metadata_filepath)
         self.clean_remote()
         self.monitor_samples_status()
         self.export_global_metadata()
         self.save_to_db()
 
 
 class TelevirFileProcess(InsafluSetup):
@@ -515,20 +574,20 @@
 
             self.deploy_televir_batch()
 
             self.download_project_results()
 
             self.logger.info("Plotting results")
             _ = plot_project_results(
-                self.projects_results, self.processed.processed, self.output_dir)
+                self.projects_results, self.processed.processed_entries, self.output_dir)
 
     def run_return_plot(self):
 
         if self.run_metadata.deploy_televir:
 
             self.deploy_televir_batch()
 
             self.download_project_results()
             return plot_project_results(
-                self.projects_results, self.processed.processed, self.run_metadata.output_dir, write_html=False)
+                self.projects_results,  self.processed.processed_entries, self.run_metadata.output_dir, write_html=False)
 
         return None
```

### Comparing `findontime-0.2.0/src/findontime/manager.py` & `findontime-0.2.5/src/findontime/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 
-from typing import Protocol
 import argparse
 import os
 import signal
 import sys
 import time
 from dataclasses import dataclass
-from typing import Tuple
+from typing import Protocol, Tuple
 
-from fastq_handler.fastq_handler import PreMain
-from fastq_handler.actions import ProcessActionMergeWithLast, ProcessActionDownsize
-from fastq_handler.configs import RunConfig
-from findontime.configs import InfluConfig
+from fastq_handler.actions import (ProcessActionDownsize,
+                                   ProcessActionMergeWithLast)
+
+from findontime.configs import InfluConfig, RunConfigMeta
 from findontime.connectors import ConnectorDocker, ConnectorParamiko
 from findontime.drones import (InsafluFileProcessThread, LockWithOwner,
                                TelevirFileProcessThread, signal_handler)
 from findontime.insaflu_uploads import (InfluConfig, InsafluFileProcess,
+                                        PreMainWithMetadata,
                                         TelevirFileProcess)
-from findontime.upload_utils import InsafluUploadRemote, UploadAll, UploadLast, UploadNone
+from findontime.upload_utils import (InsafluUploadRemote, UploadAll,
+                                     UploadLast, UploadNone)
 
 
 def get_arguments():
 
     parser = argparse.ArgumentParser(description="Process fastq files.")
     parser.add_argument(
         "-i", "--in_dir", help="Input directory", required=True)
@@ -134,30 +135,30 @@
         if args.downsize:
             actions.append(ProcessActionDownsize(args.max_size))
 
         if not actions:
             print("No actions specified, will merge files by default")
             actions.append(ProcessActionMergeWithLast())
 
-        run_metadata = RunConfig(
+        run_metadata = RunConfigMeta(
             fastq_dir=args.in_dir,
             output_dir=args.out_dir,
             name_tag=args.tag,
             actions=actions,
             keep_name=args.keep_names,
             sleep_time=args.sleep,
             max_size=(args.max_size),
         )
         actions = []
 
         return run_metadata
 
-    def setup_compressor(self, run_metadata: RunConfig):
+    def setup_compressor(self, run_metadata: RunConfigMeta):
 
-        compressor = PreMain(run_metadata)
+        compressor = PreMainWithMetadata(run_metadata)
 
         return compressor
 
     def run(self):
 
         compressor = self.setup_compressor(self.setup_config(self.args))
```

### Comparing `findontime-0.2.0/src/findontime/plot_utils.py` & `findontime-0.2.5/src/findontime/plot_utils.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/src/findontime/plotting_from_all_reports.py` & `findontime-0.2.5/src/findontime/plotting_from_all_reports.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/src/findontime/records.py` & `findontime-0.2.5/src/findontime/records.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/src/findontime/tables_post.py` & `findontime-0.2.5/src/findontime/tables_post.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/src/findontime/upload_utils.py` & `findontime-0.2.5/src/findontime/upload_utils.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.0/setup.py` & `findontime-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'xopen==1.7.0']
 
 entry_points = \
 {'console_scripts': ['findontime = findontime.__main__:main']}
 
 setup_kwargs = {
     'name': 'findontime',
-    'version': '0.2.0',
+    'version': '0.2.5',
     'description': 'A tool to upload Fastq files to the INSaFLU database and perform metagenomics pathogen detection',
     'long_description': '# findONTime\n\n[![PyPI version](https://badge.fury.io/py/findontime.svg)](https://badge.fury.io/py/findontime)\n[![PyPI version](https://img.shields.io/pypi/pyversions/findontime.svg)](https://pypi.python.org/pypi/findontime/)\n[![PyPI version](https://img.shields.io/pypi/format/findontime.svg)](https://pypi.python.org/pypi/findontime/)\n\nThe **findONTime** tool **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. It can also automatically **upload the files the INSaFLU-TELEVIR platform** and launch the **metagenomics virus detection** analysis using the TELEVIR module.\n\n## Motivation\n\nReducing the time needed for pathogen detection and the sequencing costs per sample is crucial in the context of diagnostics using metagenomics sequencing. In fact, when performing hypothesis-free viral diagnosis by sequencing complex biological samples, the proportion of the virus in a sample is unknown. As such, the amount of sequencing data, and consequently run length, needed to accurately detect the virus cannot be predicted a priori.\n\n**findONTime runs concurrently with MinION sequencing and monitors the FASTQ files that are being generated in real-time for each sample, merges the files (at user defined time intervals), uploads them to the INSaFLU-TELEVIR platform and launches the metagenomics virus detection analysis using the [TELEVIR module](https://insaflu.readthedocs.io/en/latest/metagenomics_virus_detection.html)**.\n\nThis allows users to **detect a virus in a sample as early as possible during the sequencing run**, reducing the time gap between obtaining the sample and the diagnosis, and also **reducing sequencing costs** (as ONT runs can be stopped at any time and the flow cells can be cleaned and reused). **findONTime** can be used as a “start-to-end” solution or for particular tasks (e.g., merging ONT output files, metadata preparation and upload to INSaFLU-TELEVIR).\n\n## Details\n\n- It **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. For this, it relies on [fastq-handler](https://pypi.org/project/fastq-handler/), a package to process ONT fastq files by concatenating reads as they are generated during a sequencing run.\n\n- It can also automatically **upload the files the INSaFLU-TELEVIR platform** (docker installation or local server) and launch the **metagenomics virus detection** analysis using the TELEVIR module.\n\n- The user has the option to upload all files collected throughout the ONT run (sampling occurs at user-defined period) or only upload the lastest file (i.e, the file compiling all reads generated until the lastest sampling point).\n\n- For upload, metadata files are also generated for each sequence file, according to the INSaFLU-TELEVIR input template file. Metadata files are stored in the metadata sub-directory following the output directory specified by the user.\n\n### Upload reads to INSaFLU-TELEVIR\n\n_findONTime_ can interact with the INSaFLU-TELEVIR platfotm in two ways:\n\n- **Docker**. The user needs to have the INSaFLU-TELEVIR docker installed and running. The tool will then upload the files to the docker image. The user needs to provide the name of the docker image and the path for uploads.\n\n- **SSH**. The user needs to have access to an INSaFLU-TELEVIR database server. The tool will then upload the files to the database using SSH. The user needs to provide the path for uploads and the credentials for the database server.\n\n**Note**: Automatic upload to the [INSaFLU-TELEVIR website](https://insaflu.insa.pt/) accounts is not available yet. If you only have an online account (and not a local INSaFLU installation), findONTime will be run concurrently with MinION sequencing to monitor and concatenate the FASTQ files that are being generated in real-time for each sample and prepare metadata templates ready to be upload to INSaFLU-TELEVIR.\n\n### Launch a virus detection analysis (TELEVIR)\n\nIf requested the tool creates one INSaFLU-TELEVIR project for each inpp directory containing fastq files. The project name is the name of the directory. Files generated within the same directory are uploaded to the same project.\n\nIf you have a local INSaFLU-TELEVIR installation (docker or server), and set the "--televir argument", findONTtimeThe tool can creates one INSaFLU-TELEVIR (virus detection) project including the samples under ONT sequencing. The project name is defined by the user (--tag argument) and the sample names are the ones of the input directory (usually barcode01, barcode02, etc) with an extra user-defined tag as suffix.\n\n### Input Files\n\n- **fastq.gz** - Output directory for the ONT run, containing sequence files. The files can be in subfolders. The files can be gzipped or not.\n\n- **config.ini** - A configuration file containing the parameters for the tool. The file is generated by the tool when it is run for the first time. The user can edit the file to change the parameters.\n\nConfig must contain:\n\n- section [INSAFLU] containing insaflu username and app directory path.\n\n- (optional) section [SSH] containing ssh credentials: username, ip_address and rsa key;\n\n- (optional) section [DOCKER] containing docker image name.\n\nsee example [config.ini](config.ini)\n\n## API\n\n```bash\n\nusage: findontime [-h] -i IN_DIR -o OUT_DIR [-s SLEEP] [-n TAG] [--config CONFIG] [--max_size MAX_SIZE] [--merge] [--downsize] [--upload {last,all,none}] [--connect {docker,ssh}] [--keep_names] [--monitor] [--televir]\n\nProcess fastq files.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -i IN_DIR, --in_dir IN_DIR\n                        Input directory\n  -o OUT_DIR, --out_dir OUT_DIR\n                        Output directory\n  -s SLEEP, --sleep SLEEP\n                        Sleep time between checks in monitor mode (default 600 seconds)\n  -n TAG, --tag TAG     name tag, if given, will be added to the output file names\n  --config CONFIG       config file\n  --max_size MAX_SIZE   max size of the output file, in kilobytes (default 400000 kbytes)\n  --merge               merge files\n  --downsize            downsize fastq files to max_size\n  --upload {last,all,none}\n                        file upload strategy (default: last)\n  --connect {docker,ssh}\n                        file upload strategy (default: docker)\n  --keep_names          keep original file names\n  --monitor             monitor directory until killed\n  --televir             deploy televir pathogen identification on each sample\n\n```\n\n### REQUIREMENTS\n\n- **python 3.6** or higher\n- dataclasses==0.6\n- natsort==8.3.1\n- pandas==1.5.3\n- paramiko==3.1.0\n- pip==21.2.3\n- setuptools==57.4.0\n- xopen==1.7.0\n\n### INSTALLATION\n\n```bash\npython -m venv .venv\nsource .venv/bin/activate\npython -m pip install findontime\n```\n\n### USAGE\n\n_(from simple to more advanced usage situations)_\n\n- Example 1. **Merge fastq files from an ONT run.**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix --max_size 100000000 --merge --upload none\n\n```\n\n_NOTE: In this simpler usage case, the fastq.gz files will only be only merged, i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform. In case you want to concatenate all ONT same-sample files (file_0.fastq.gz, file_1.fastq.gz, etc), make sure you set up a "max_size" (e.g., 100000000 kbytes) enough to ensure that the merged file compiles all partial files._\n\n- Example 2. **Merge fastq files generated during a ONT run at every 10 min (600 seconds).**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 100000000 --monitor --merge --upload none\n\n```\n\n_NOTE: In this simpler usage case, the fastq.gz files will only be only merged, i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform. In case you want to concatenate all ONT same-sample files (file_0.fastq.gz, file_1.fastq.gz, etc), make sure you set up a "max_size" (e.g., 100000000 kbytes) enough to ensure that the merged file compiles all partial files._\n\n- Example 3. **Merge fastq files generated during a ONT run at every 10 min (600 seconds), downsize the merged file to 400 MB (ready to be uploaded to INSaFLU-TELEVIR).**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --merge --upload none --downsize\n\n```\n\n_NOTE: In this case, the fastq.gz files will only be concatenated (i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform), but the merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes). This usage is useful to prepare files ready to be uploaded to the online [INSaFLU-TELEVIR platform](https://insaflu.insa.pt/), which is currently limited to an upload max size per file of 400 MB._\n\n- Example 4. **Merge fastq files generated during a ONT run at every 10 min (600 seconds) and upload them to INSaFLU-TELEVIR**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --connect docker --merge --upload last --connect docker\n\n```\n\n_NOTE: In this case, the fastq.gz files will be concatenated and automatically uploaded to the INSaFLU-TELEVIR platform. The merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes), which must be fitted to the maximum upload file size defined in your local INSaFLU_TELEVIR installation_\n\n- Example 5. **Merge fastq files generated during a ONT run at every 10 min (600 seconds), upload them to INSaFLU-TELEVIR and run a virus detection project**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --connect docker --merge --upload last –-televir\n\n```\n\n_NOTE: In this case, the fastq.gz files will be concatenated, automatically uploaded to the INSaFLU-TELEVIR platform and run under a virus detection (TELEVIR) project. The merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes), which must be fitted to the maximum upload file size defined in your local INSaFLU_TELEVIR installation_\n\n### TESTING\n\nRunning pytest in the root directory will run all tests that do not interact with INSaFLU-TELEVIR. In order to test the upload and metagenomics functionalities, the user needs to provide a valid config file to a local docker installation, and to pass the `--docker` flag to pytest:\n\n```bash\n\npytest --docker --config-file config.ini\n\n```\n\n### MAIN OUTPUT\n\n> **Note:** The output directory structure is maintained.\n\n- **fastq.gz** files containing all reads from the previous files.\n- **log.txt** file containing the concatenation process.\n- **metadata** individual metadata files for each fastq file uploaded.\n- **results.tsv** file containing the main results of the TELEVIR pathogen detection. One file per project.\n\n## Maintainers\n\n- [**@santosjgnd**](https://github.com/SantosJGND)\n- [**@insaflu**](https://github.com/insapathogenomics)\n',
     'author': 'SantosJGND',
     'author_email': 'dourado.jns@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `findontime-0.2.0/PKG-INFO` & `findontime-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findontime
-Version: 0.2.0
+Version: 0.2.5
 Summary: A tool to upload Fastq files to the INSaFLU database and perform metagenomics pathogen detection
 License: MIT
 Author: SantosJGND
 Author-email: dourado.jns@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


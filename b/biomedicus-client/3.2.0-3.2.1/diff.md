# Comparing `tmp/biomedicus_client-3.2.0.tar.gz` & `tmp/biomedicus_client-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedicus_client-3.2.0.tar", last modified: Mon Apr 17 22:41:04 2023, max compression
+gzip compressed data, was "biomedicus_client-3.2.1.tar", last modified: Wed Apr 19 18:23:41 2023, max compression
```

## Comparing `biomedicus_client-3.2.0.tar` & `biomedicus_client-3.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/
--rw-r--r--   0 ben       (1000) ben       (1000)    11358 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/LICENSE.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       46 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/MANIFEST.in
--rw-r--r--   0 ben       (1000) ben       (1000)    16086 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)     1495 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/README.md
--rw-r--r--   0 ben       (1000) ben       (1000)     2140 2023-04-17 22:38:27.000000 biomedicus_client-3.2.0/pyproject.toml
--rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/setup.cfg
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client/
--rw-r--r--   0 ben       (1000) ben       (1000)      809 2023-04-17 15:52:14.000000 biomedicus_client-3.2.0/src/biomedicus_client/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)      691 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/__main__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1328 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/
--rw-r--r--   0 ben       (1000) ben       (1000)      870 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1502 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/command.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2077 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/config_writing.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1078 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/parser.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/
--rw-r--r--   0 ben       (1000) ben       (1000)      717 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3335 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/_run.py
--rw-r--r--   0 ben       (1000) ben       (1000)      636 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/biomedicus_default_pipeline.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     5789 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/default_pipeline.py
--rw-r--r--   0 ben       (1000) ben       (1000)     4506 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/rtf_to_text.py
--rw-r--r--   0 ben       (1000) ben       (1000)      313 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/rtf_to_text_pipeline.yml
--rw-r--r--   0 ben       (1000) ben       (1000)      619 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/scaleout_pipeline_config.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     4026 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/sources.py
--rw-r--r--   0 ben       (1000) ben       (1000)      160 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client/version.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)    16086 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)     1029 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       56 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/entry_points.txt
--rw-r--r--   0 ben       (1000) ben       (1000)      133 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       18 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/
+-rw-r--r--   0 ben       (1000) ben       (1000)    11358 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/LICENSE.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       46 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/MANIFEST.in
+-rw-r--r--   0 ben       (1000) ben       (1000)    16086 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1495 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/README.md
+-rw-r--r--   0 ben       (1000) ben       (1000)     2140 2023-04-17 22:38:27.000000 biomedicus_client-3.2.1/pyproject.toml
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/setup.cfg
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/src/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/src/biomedicus_client/
+-rw-r--r--   0 ben       (1000) ben       (1000)      809 2023-04-17 15:52:14.000000 biomedicus_client-3.2.1/src/biomedicus_client/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      691 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/src/biomedicus_client/__main__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3317 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/_run.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1353 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/cli.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/
+-rw-r--r--   0 ben       (1000) ben       (1000)      870 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1502 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/command.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2077 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/config_writing.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1078 2023-03-13 16:38:29.000000 biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/parser.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5561 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/default_pipeline.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/src/biomedicus_client/pipeline_confs/
+-rw-r--r--   0 ben       (1000) ben       (1000)      998 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/pipeline_confs/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      636 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/pipeline_confs/biomedicus_default_pipeline.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)      313 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/pipeline_confs/rtf_to_text_pipeline.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)      619 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/pipeline_confs/scaleout_pipeline.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     4392 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/rtf_to_text.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4173 2023-04-19 18:22:30.000000 biomedicus_client-3.2.1/src/biomedicus_client/sources.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      160 2023-04-19 18:23:40.000000 biomedicus_client-3.2.1/src/biomedicus_client/version.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-19 18:23:40.985551 biomedicus_client-3.2.1/src/biomedicus_client.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)    16086 2023-04-19 18:23:40.000000 biomedicus_client-3.2.1/src/biomedicus_client.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1010 2023-04-19 18:23:40.000000 biomedicus_client-3.2.1/src/biomedicus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-19 18:23:40.000000 biomedicus_client-3.2.1/src/biomedicus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       56 2023-04-19 18:23:40.000000 biomedicus_client-3.2.1/src/biomedicus_client.egg-info/entry_points.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)      133 2023-04-19 18:23:40.000000 biomedicus_client-3.2.1/src/biomedicus_client.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       18 2023-04-19 18:23:40.000000 biomedicus_client-3.2.1/src/biomedicus_client.egg-info/top_level.txt
```

### Comparing `biomedicus_client-3.2.0/LICENSE.txt` & `biomedicus_client-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/PKG-INFO` & `biomedicus_client-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedicus_client
-Version: 3.2.0
+Version: 3.2.1
 Summary: A biomedical and clinical natural language processing engine.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomedicus_client-3.2.0/README.md` & `biomedicus_client-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/pyproject.toml` & `biomedicus_client-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/__init__.py` & `biomedicus_client-3.2.1/src/biomedicus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/__main__.py` & `biomedicus_client-3.2.1/src/biomedicus_client/__main__.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/cli.py` & `biomedicus_client-3.2.1/src/biomedicus_client/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,27 +11,32 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """biomedicus_client command line interface"""
 
 import logging
 
+from biomedicus_client import pipeline_confs
+from biomedicus_client._run import RunCommand
 from biomedicus_client.cli_tools import create_parser, WriteConfigsCommand
-from biomedicus_client.pipeline import RunCommand, default_pipeline, rtf_to_text
+from biomedicus_client.rtf_to_text import RunRtfToTextCommand
+
+__all__ = ('main',)
+
 
 CLIENT_CONFIGS = {
-    'pipeline': default_pipeline.default_pipeline_config,
-    'scaleout_pipeline': default_pipeline.scaleout_pipeline_config,
-    'rtf_only_pipeline': rtf_to_text.default_rtf_to_text_pipeline_config
+    'pipeline': pipeline_confs.DEFAULT,
+    'scaleout_pipeline': pipeline_confs.SCALEOUT,
+    'rtf_only_pipeline': pipeline_confs.RTF_TO_TEXT
 }
 
 
 def main(args=None):
     parser = create_parser(
         WriteConfigsCommand(CLIENT_CONFIGS),
         RunCommand(),
-        rtf_to_text.RunRtfToTextCommand()
+        RunRtfToTextCommand()
     )
     conf = parser.parse_args(args)
     logging.basicConfig(level=conf.log_level)
     f = conf.f
     f(conf)
```

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/__init__.py` & `biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/command.py` & `biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/command.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/config_writing.py` & `biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/config_writing.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/parser.py` & `biomedicus_client-3.2.1/src/biomedicus_client/cli_tools/parser.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/_run.py` & `biomedicus_client-3.2.1/src/biomedicus_client/_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Support for running the default pipeline by default and optionally arbitrary pipelines."""
 
 from argparse import ArgumentParser
 from typing import List
 
+from biomedicus_client.sources import WatcherSource, rtf_source, RtfHandler, TxtHandler
 from mtap import events_client
 from mtap.pipeline import FilesInDirectoryProcessingSource
 
+from biomedicus_client import default_pipeline
 from biomedicus_client.cli_tools import Command
-from biomedicus_client.pipeline import default_pipeline
-from biomedicus_client.pipeline.sources import WatcherSource, RtfHandler, rtf_source, TxtHandler
 
 
 class RunCommand(Command):
     @property
     def command(self) -> str:
         return "run"
```

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/biomedicus_default_pipeline.yml` & `biomedicus_client-3.2.1/src/biomedicus_client/pipeline_confs/biomedicus_default_pipeline.yml`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/default_pipeline.py` & `biomedicus_client-3.2.1/src/biomedicus_client/default_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,70 +13,71 @@
 #  limitations under the License.
 """Support for creating and running the biomedicus default pipeline."""
 
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import Optional, Union
 
-from importlib_resources import files
+from importlib_resources import as_file
 from mtap import Pipeline, LocalProcessor, RemoteProcessor
 from mtap.serialization import SerializerRegistry, SerializationProcessor
 
-__all__ = ['default_pipeline_config', 'scaleout_pipeline_config', 'create', 'from_args', 'argument_parser']
+__all__ = ['create', 'from_args', 'argument_parser']
 
-default_pipeline_config = files('biomedicus_client.pipeline').joinpath('biomedicus_default_pipeline.yml')
-scaleout_pipeline_config = files('biomedicus_client.pipeline').joinpath('scaleout_pipeline_config.yml')
+from biomedicus_client import pipeline_confs
 
 
-def create(config: Optional[Union[str, Path]] = None,
+def create(config: Optional[Union[str, bytes, Path]] = None,
            *, events_addresses: Optional[str] = None,
            rtf: bool = False,
            rtf_address: str = "localhost:50200",
            serializer: Optional[str] = None,
            output_directory: Union[str, Path] = None,
            include_label_text: bool = False,
            address: Optional[str] = None,
            **_) -> Pipeline:
     """The biomedicus default pipeline for processing clinical documents.
 
     Args
-        config (Optional[Union[str, Path]]): A path to an MTAP pipeline configuration YAML file to
-            use instead of the default.
+        config: A path to an MTAP pipeline configuration YAML file to use instead of the default.
 
     Keyword Args
-        events_addresses (Optional[str]): The address (or addresses, comma separated) for the
-            events service.
-        rtf (bool): Whether to include the rtf processor at the start of the pipeline. The rtf
-            processor will convert RTF data stored in the "rtf" Binary on the event to the
-            "plaintext" Document.
-        rtf_address (str): The address of the remote rtf processor.
-        serializer (Optional[str]): An optional serializer (examples: 'json', 'yml', 'pickle').
-        output_directory (Optional[Path]): Where the serializer should output the serialized files.
-        address (Optional[str]): An optional address to use for all processors.
+        events_addresses: The address (or addresses, comma separated) for the events service.
+        rtf: Whether to include the rtf processor at the start of the pipeline. The rtf processor will convert RTF data
+            stored in the "rtf" Binary on the event to the "plaintext" Document.
+        rtf_address: The address of the remote rtf processor.
+        serializer: An optional serializer (examples: 'json', 'yml', 'pickle').
+        output_directory: Where the serializer should output the serialized files.
+        address: An optional address to use for all processors.
 
     Returns
         Pipeline
 
     """
     if config is None:
-        config = default_pipeline_config
-    pipeline = Pipeline.from_yaml_file(config)
+        with as_file(pipeline_confs.DEFAULT) as config:
+            pipeline = Pipeline.from_yaml_file(config)
+    else:
+        pipeline = Pipeline.from_yaml_file(config)
 
     if events_addresses is not None:
         pipeline.events_address = events_addresses
 
     serializer = None if serializer == 'None' else serializer
     if serializer is not None:
         serialization_proc = SerializationProcessor(SerializerRegistry.get(serializer),
                                                     output_directory,
                                                     include_label_text=include_label_text)
         ser_comp = LocalProcessor(serialization_proc, component_id='serializer')
         pipeline.append(ser_comp)
 
     if rtf:
+        if rtf_address is None:
+            rtf_address = 'localhost:50200'
+
         rtf_processor = RemoteProcessor(processor_name='biomedicus-rtf',
                                         address=rtf_address,
                                         params={'output_document_name': 'plaintext'})
         pipeline.insert(0, rtf_processor)
 
     if address is not None:
         pipeline.events_address = address
@@ -122,15 +123,14 @@
     parser.add_argument(
         '--rtf',
         action='store_true',
         help="Flag to use a source for the rtf reader instead of plain text."
     )
     parser.add_argument(
         '--rtf-address',
-        default="localhost:50200",
         help="The address (or addresses, comma separated) for the rtf to text converter processor."
     )
     parser.add_argument(
         '--address', '-a',
         help="An address override, used for the dockerized BioMedICUS."
     )
     return parser
```

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/rtf_to_text.py` & `biomedicus_client-3.2.1/src/biomedicus_client/rtf_to_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,25 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Support for creating and running the rtf-to-text pipeline."""
 
 from argparse import ArgumentParser, Namespace
 from os import PathLike
-
-from importlib_resources import files
 from pathlib import Path
 from typing import Union, Optional, List
 
+from biomedicus_client.sources import rtf_source
+from importlib_resources import as_file
 from mtap import Pipeline, LocalProcessor, EventProcessor, processor, events_client
 
+from biomedicus_client import pipeline_confs
 from biomedicus_client.cli_tools import Command
-from biomedicus_client.pipeline.sources import rtf_source
-
-__all__ = ['default_rtf_to_text_pipeline_config', 'create', 'from_args', 'argument_parser', 'RunRtfToTextCommand']
 
-default_rtf_to_text_pipeline_config = files('biomedicus_client.pipeline').joinpath('rtf_to_text_pipeline.yml')
+__all__ = ['create', 'from_args', 'argument_parser', 'RunRtfToTextCommand']
 
 
 @processor('write-plaintext')
 class WritePlaintext(EventProcessor):
     def __init__(self, output_directory: Path):
         self.output_directory = output_directory
 
@@ -53,16 +51,18 @@
         output_directory:
         **_:
 
     Returns:
 
     """
     if config is None:
-        config = default_rtf_to_text_pipeline_config
-    pipeline = Pipeline.from_yaml_file(config)
+        with as_file(pipeline_confs.RTF_TO_TEXT) as config:
+            pipeline = Pipeline.from_yaml_file(config)
+    else:
+        pipeline = Pipeline.from_yaml_file(config)
 
     if events_addresses is not None:
         pipeline.events_address = events_addresses
 
     if output_directory is not None:
         pipeline += [LocalProcessor(
             WritePlaintext(Path(output_directory)),
@@ -74,26 +74,23 @@
 def argument_parser():
     """The argument parser for the biomedicus rtf-to-text pipeline.
 
     Returns: ArgumentParser object.
 
     """
     parser = ArgumentParser(add_help=False)
-    parser.add_argument('--config', default=None,
-                        help='Path to the pipeline configuration file.')
+    parser.add_argument('--config', default=None, help='Path to the pipeline configuration file.')
     parser.add_argument('--output_directory', '-o', default='output', help="The output directory to write txt out.")
-    parser.add_argument('--events-addresses', default=None,
-                        help="The address for the events service.")
+    parser.add_argument('--events-addresses', default=None, help="The address for the events service.")
     return parser
 
 
 def from_args(args: Namespace) -> Pipeline:
     if not isinstance(args, Namespace):
-        raise ValueError('"args" parameter should be the parsed arguments from '
-                         '"rtf_to_text.argument_parser()"')
+        raise ValueError('"args" parameter should be the parsed arguments from "rtf_to_text.argument_parser()"')
     return create(**vars(args))
 
 
 class RunRtfToTextCommand(Command):
     @property
     def command(self) -> str:
         return "run-rtf-to-text"
```

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/scaleout_pipeline_config.yml` & `biomedicus_client-3.2.1/src/biomedicus_client/pipeline_confs/scaleout_pipeline.yml`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/sources.py` & `biomedicus_client-3.2.1/src/biomedicus_client/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,30 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Input sources for running pipelines."""
 
 import fnmatch
 import time
 from pathlib import Path
+from typing import Generator, Iterator
 
 from mtap import Event
 from mtap.pipeline import ProcessingSource
 from mtap.types import EventsClient
 from watchdog.events import FileSystemEventHandler, FileSystemEvent
 
+__all__ = [
+    'rtf_source',
+    'RtfHandler',
+    'TxtHandler',
+    'WatcherSource'
+]
 
-def rtf_source(input_directory: Path, extension_glob: str, events_client: EventsClient):
+
+def rtf_source(input_directory: Path, extension_glob: str, events_client: EventsClient) -> Iterator[Event]:
     input_directory = Path(input_directory)
     for path in input_directory.rglob(extension_glob):
         with path.open('rb', errors=None) as f:
             rtf = f.read()
         relative = str(path.relative_to(input_directory))
         with Event(event_id=relative, client=events_client, only_create_new=True) as event:
             event.binaries['rtf'] = rtf
```

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client.egg-info/PKG-INFO` & `biomedicus_client-3.2.1/src/biomedicus_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedicus-client
-Version: 3.2.0
+Version: 3.2.1
 Summary: A biomedical and clinical natural language processing engine.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomedicus_client-3.2.0/src/biomedicus_client.egg-info/SOURCES.txt` & `biomedicus_client-3.2.1/src/biomedicus_client.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 src/biomedicus_client/__init__.py
 src/biomedicus_client/__main__.py
+src/biomedicus_client/_run.py
 src/biomedicus_client/cli.py
+src/biomedicus_client/default_pipeline.py
+src/biomedicus_client/rtf_to_text.py
+src/biomedicus_client/sources.py
 src/biomedicus_client/version.py
 src/biomedicus_client.egg-info/PKG-INFO
 src/biomedicus_client.egg-info/SOURCES.txt
 src/biomedicus_client.egg-info/dependency_links.txt
 src/biomedicus_client.egg-info/entry_points.txt
 src/biomedicus_client.egg-info/requires.txt
 src/biomedicus_client.egg-info/top_level.txt
 src/biomedicus_client/cli_tools/__init__.py
 src/biomedicus_client/cli_tools/command.py
 src/biomedicus_client/cli_tools/config_writing.py
 src/biomedicus_client/cli_tools/parser.py
-src/biomedicus_client/pipeline/__init__.py
-src/biomedicus_client/pipeline/_run.py
-src/biomedicus_client/pipeline/biomedicus_default_pipeline.yml
-src/biomedicus_client/pipeline/default_pipeline.py
-src/biomedicus_client/pipeline/rtf_to_text.py
-src/biomedicus_client/pipeline/rtf_to_text_pipeline.yml
-src/biomedicus_client/pipeline/scaleout_pipeline_config.yml
-src/biomedicus_client/pipeline/sources.py
+src/biomedicus_client/pipeline_confs/__init__.py
+src/biomedicus_client/pipeline_confs/biomedicus_default_pipeline.yml
+src/biomedicus_client/pipeline_confs/rtf_to_text_pipeline.yml
+src/biomedicus_client/pipeline_confs/scaleout_pipeline.yml
```


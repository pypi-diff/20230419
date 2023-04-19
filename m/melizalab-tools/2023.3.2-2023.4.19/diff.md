# Comparing `tmp/melizalab-tools-2023.3.2.tar.gz` & `tmp/melizalab-tools-2023.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melizalab-tools-2023.3.2.tar", last modified: Wed Mar  8 19:24:42 2023, max compression
+gzip compressed data, was "melizalab-tools-2023.4.19.tar", last modified: Wed Apr 19 14:42:31 2023, max compression
```

## Comparing `melizalab-tools-2023.3.2.tar` & `melizalab-tools-2023.4.19.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-03-08 19:24:42.338965 melizalab-tools-2023.3.2/
--rw-r--r--   0 dmeliza    (503) staff       (20)     1414 2023-03-08 19:24:42.339107 melizalab-tools-2023.3.2/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      888 2023-02-22 16:22:22.000000 melizalab-tools-2023.3.2/README.md
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-03-08 19:24:42.330789 melizalab-tools-2023.3.2/dlab/
--rw-r--r--   0 dmeliza    (503) staff       (20)       24 2022-10-13 22:35:34.000000 melizalab-tools-2023.3.2/dlab/__init__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      277 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/core.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1805 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/extracellular.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     5990 2023-02-22 16:22:33.000000 melizalab-tools-2023.3.2/dlab/extract_waveforms.py
--rw-r--r--   0 dmeliza    (503) staff       (20)    17385 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/kilo.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     5743 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/nbank.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2032 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/plotting.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     5048 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/pprox.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1789 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/signal.py
--rw-r--r--   0 dmeliza    (503) staff       (20)    13292 2023-02-22 16:22:33.000000 melizalab-tools-2023.3.2/dlab/song_detect.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1786 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/dlab/spikes.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2050 2023-02-22 16:22:33.000000 melizalab-tools-2023.3.2/dlab/util.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-03-08 19:24:42.336408 melizalab-tools-2023.3.2/melizalab_tools.egg-info/
--rw-r--r--   0 dmeliza    (503) staff       (20)     1414 2023-03-08 19:24:42.000000 melizalab-tools-2023.3.2/melizalab_tools.egg-info/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      578 2023-03-08 19:24:42.000000 melizalab-tools-2023.3.2/melizalab_tools.egg-info/SOURCES.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-03-08 19:24:42.000000 melizalab-tools-2023.3.2/melizalab_tools.egg-info/dependency_links.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)      103 2023-03-08 19:24:42.000000 melizalab-tools-2023.3.2/melizalab_tools.egg-info/entry_points.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2022-10-12 18:42:40.000000 melizalab-tools-2023.3.2/melizalab_tools.egg-info/not-zip-safe
--rw-r--r--   0 dmeliza    (503) staff       (20)      198 2023-03-08 19:24:42.000000 melizalab-tools-2023.3.2/melizalab_tools.egg-info/requires.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        5 2023-03-08 19:24:42.000000 melizalab-tools-2023.3.2/melizalab_tools.egg-info/top_level.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)      121 2023-02-16 22:14:18.000000 melizalab-tools-2023.3.2/pyproject.toml
--rw-r--r--   0 dmeliza    (503) staff       (20)     1205 2023-03-08 19:24:42.340335 melizalab-tools-2023.3.2/setup.cfg
--rw-r--r--   0 dmeliza    (503) staff       (20)      106 2020-11-05 14:34:56.000000 melizalab-tools-2023.3.2/setup.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-03-08 19:24:42.338557 melizalab-tools-2023.3.2/tests/
--rw-r--r--   0 dmeliza    (503) staff       (20)     8717 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/tests/test_pprox.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      521 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/tests/test_signal.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1579 2023-03-08 19:24:21.000000 melizalab-tools-2023.3.2/tests/test_spikes.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.432894 melizalab-tools-2023.4.19/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1379 2023-04-19 14:42:31.433019 melizalab-tools-2023.4.19/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      852 2023-03-17 16:55:38.000000 melizalab-tools-2023.4.19/README.md
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.417307 melizalab-tools-2023.4.19/dlab/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       24 2022-10-13 22:35:34.000000 melizalab-tools-2023.4.19/dlab/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      898 2023-03-16 17:12:17.000000 melizalab-tools-2023.4.19/dlab/cache.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      122 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/dlab/core.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1838 2023-03-16 17:04:03.000000 melizalab-tools-2023.4.19/dlab/extracellular.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6024 2023-03-16 17:04:03.000000 melizalab-tools-2023.4.19/dlab/extract_waveforms.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)    17548 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/dlab/kilo.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6483 2023-03-17 16:55:38.000000 melizalab-tools-2023.4.19/dlab/nbank.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2034 2023-03-10 23:03:29.000000 melizalab-tools-2023.4.19/dlab/plotting.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     5048 2023-03-08 19:24:21.000000 melizalab-tools-2023.4.19/dlab/pprox.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1790 2023-03-10 23:03:29.000000 melizalab-tools-2023.4.19/dlab/signal.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     4275 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/dlab/spikes.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2055 2023-03-16 17:04:03.000000 melizalab-tools-2023.4.19/dlab/util.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.422634 melizalab-tools-2023.4.19/melizalab_tools.egg-info/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1379 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      572 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)       65 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/entry_points.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2022-10-12 18:42:40.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/not-zip-safe
+-rw-r--r--   0 dmeliza    (503) staff       (20)      131 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/requires.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        5 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/top_level.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)      121 2023-02-16 22:14:18.000000 melizalab-tools-2023.4.19/pyproject.toml
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1087 2023-04-19 14:42:31.434216 melizalab-tools-2023.4.19/setup.cfg
+-rw-r--r--   0 dmeliza    (503) staff       (20)      106 2020-11-05 14:34:56.000000 melizalab-tools-2023.4.19/setup.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.432384 melizalab-tools-2023.4.19/tests/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     8717 2023-03-08 19:24:21.000000 melizalab-tools-2023.4.19/tests/test_pprox.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      506 2023-03-10 19:08:55.000000 melizalab-tools-2023.4.19/tests/test_signal.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1601 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/tests/test_spikes.py
```

### Comparing `melizalab-tools-2023.3.2/PKG-INFO` & `melizalab-tools-2023.4.19/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melizalab-tools
-Version: 2023.3.2
+Version: 2023.4.19
 Summary: Meliza lab scripts and modules for auditory neurophysiology
 Home-page: https://github.com/melizalab/melizalab-tools
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
@@ -23,15 +23,13 @@
 
 ### modules
 
 - `dlab.pprox`: functions for working with [pprox](https://meliza.org/spec:2/pprox/) objects, a data format for storing multi-trial point process data (e.g. spike times evoked by stimulus presentation).
 
 ### console scripts
 
-- `song-detect`: This is a wrapper for the [quicksong](https://github.com/melizalab/quicksong/) package, an algorithm for automatically segmenting acoustic recordings into songs. 
-
-- `group-kilo-spikes`
+- `group-kilo-spikes`: sort spike times output from [kilosort](https://github.com/MouseLand/Kilosort) and [phy2](https://github.com/cortex-lab/phy/) into pprox files.
 
 ### other stuff
 
 - `scripts/extract_waveforms.py`: extracts spike waveforms from a raw recording (in ARF format) using spike times stored in a file (pprox format). This script is mostly only used to verify that spike sorting is working properly, because the `group-kilo-spikes` script has an option to store average waveforms.
```

### Comparing `melizalab-tools-2023.3.2/dlab/extracellular.py` & `melizalab-tools-2023.4.19/dlab/extracellular.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """ Utilities for extracellular experiments """
 import json
 import logging
 import re
 
-
-log = logging.getLogger("dlab")
+logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 def entry_time(entry):
     """Return the timestamp of an entry as a floating point number"""
     from arf import timestamp_to_float
 
     return timestamp_to_float(entry.attrs["timestamp"])
@@ -29,15 +28,15 @@
 
 
 def find_stim_dset(entry):
     """Returns the first dataset that matches 'Network_Events.*_TEXT'"""
     rex = re.compile(r"Network_Events-.*?TEXT")
     for name in entry:
         if rex.match(name) is not None:
-            log.debug("  - stim log dataset: %s", name)
+            logging.debug("  - stim log dataset: %s", name)
             return entry[name]
 
 
 def entry_metadata(entry):
     """Extracts metadata from an entry in an oeaudio-present experiment ARF file.
 
     Metadata are passed to open-ephys through the network events socket as a
```

### Comparing `melizalab-tools-2023.3.2/dlab/extract_waveforms.py` & `melizalab-tools-2023.4.19/dlab/extract_waveforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """ Commandline script to extract waveforms from extracellular recordings """
 import json
 import logging
 
 import h5py as h5
-import nbank
 import numpy as np
 import pandas as pd
 
-log = logging.getLogger("dlab")
+import nbank
 
 
 if __name__ == "__main__":
     import argparse
 
     from dlab.core import __version__, get_or_verify_datafile
-    from dlab.util import setup_log
 
     script_version = "2022.06.24"
 
     p = argparse.ArgumentParser(
         description="extract waveforms from extracellular recording based "
         "on spike times in pprox files. A csv file is generated"
         "for each pprox file"
@@ -64,31 +62,33 @@
     p.add_argument(
         "pprox",
         nargs="+",
         type=argparse.FileType("r", encoding="utf-8"),
         help="pprox files with spike times",
     )
     args = p.parse_args()
-    setup_log(log, args.debug)
+    logging.basicConfig(
+        format="%(message)s", level=logging.DEBUG if args.debug else logging.INFO
+    )
 
     datafile, arf_info = get_or_verify_datafile(args.recording, args.debug)
 
     with h5.File(datafile, "r") as arf:
         for spikefile in args.pprox:
-            log.info(" - processing spike times in '%s':", spikefile.name)
+            logging.info(" - processing spike times in '%s':", spikefile.name)
             spike_data = json.load(spikefile)
             # check that the recording matches the ARF file
-            log.info("   - source recording: %s", spike_data["recording"])
+            logging.info("   - source recording: %s", spike_data["recording"])
             dset_channel = spike_data["kilosort_source_channel"]
             # TODO verify that that index is 1-based
             dset_name = f"CH{dset_channel + 1}"
-            log.info("   - main channel: %s", dset_name)
+            logging.info("   - main channel: %s", dset_name)
             resource_info = nbank.describe(spike_data["recording"])
             if resource_info["sha1"] != arf_info["sha1"]:
-                log.warning(
+                logging.warning(
                     "   - warning: recording does not match the supplied ARF file, skipping"
                 )
                 continue
             # convert spike times to sample counts (relative to entry start)
             entry_metadata = spike_data["entry_metadata"]
             if len(set(e["sampling_rate"] for e in entry_metadata)) > 1:
                 raise ValueError("Not all entries have the same sampling rate")
@@ -128,15 +128,15 @@
             waveforms = np.zeros((nspikes, n_before + n_after), dtype="f8")
             for i, row in enumerate(selected.itertuples(index=False)):
                 waveforms[i, :] = dsets[row.entry][row.start : row.stop]
             # __import__("IPython").embed()
 
             #     spike_idx = (np.asarray(trial["events"]) * sampling_rate).astype("int64") + trial["recording"]["start"]
             #     nspikes = spike_idx.size
-            #     log.debug("    - trial %d: %d spikes from entry %d", trial["index"], nspikes, entry)
+            #     logging.debug("    - trial %d: %d spikes from entry %d", trial["index"], nspikes, entry)
             #     spike_times.append(spike_idx)
             #     spike_entries.append(np.ones(nspikes, dtype="int32") * entry)
             # all_spike_entries = np.concatenate(spike_entries)
             # all_spike_times = np.concatenate(spike_times)
             # nspikes = all_spike_times.size
 
             # TODO sort by entry to avoid looking up the dataset on every spike
```

### Comparing `melizalab-tools-2023.3.2/dlab/kilo.py` & `melizalab-tools-2023.4.19/dlab/kilo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
-""" Functions for using kilsort/phy data """
-import asyncio
-from aiohttp import ClientSession
-import re
+""" Functions for using kilosort/phy data """
 import json
 import logging
+import re
 from collections import namedtuple
-from pathlib import Path
 from functools import lru_cache
-from typing import Iterator, Dict
+from pathlib import Path
+from typing import Dict, Iterator
 
+import anyio
 import ewave
 import h5py as h5
 import numpy as np
 import pandas as pd
 import quickspikes as qs
+import toelis
+from httpx import AsyncClient
 
-from dlab import pprox, nbank
+from dlab import nbank, pprox
+from dlab.spikes import SpikeWaveforms, save_waveforms
 
-log = logging.getLogger("dlab.kilo")
+logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 Trial = namedtuple(
     "Trial",
     [
         "recording_entry",
         "recording_start",
         "recording_end",
@@ -66,35 +68,34 @@
         m = re_start.match(message)
         if m is not None:
             stim_name = Path(m.group(1)).stem
             yield Stimulus(stim_name, time)
 
 
 @lru_cache(maxsize=None)
-async def stim_duration(session: ClientSession, stim_name: str) -> float:
+async def stim_duration(session: AsyncClient, stim_name: str) -> float:
     """
     Returns the duration of a stimulus (in s). This can only really be done by
     downloading the stimulus from the registry, because the start/stop times are
     not reliable. We try to speed this up by memoizing the function and caching
     the downloaded files.
 
     """
     target = await nbank.find_resource(session, nbank.default_registry, stim_name)
     with ewave.wavfile(str(target)) as fp:
         return 1.0 * fp.nframes / fp.sampling_rate
 
 
 async def oeaudio_to_trials(
-    session: ClientSession,
+    session: AsyncClient,
     data_file: h5.File,
     sync_dset: str,
     sync_thresh: float = 1.0,
     prepad: float = 1.0,
 ) -> Iterator[Trial]:
-
     """Extracts trial information from an oeaudio-present experiment ARF file
 
     When using oeaudio-present, a single recording is made in response to all
     the stimuli. The stimulus presentation script sends network events to
     open-ephys to mark the start and stop of each stimulus. There is typically a
     significant lag between the 'start' event and the onset of the stimulus, due
     to buffering of the audio playback. However, the oeaudio-present script will
@@ -105,59 +106,60 @@
     The continuous recording is broken up into trials based on the stimulus
     presentation, such that each trial encompasses one and only one stimulus.
     The `prepad` parameter specifies, in seconds, when trials begin relative to
     stimulus onset. The default is 1.0 s.
 
     """
     from itertools import zip_longest
+
     from dlab.extracellular import (
-        entry_time,
         entry_datetime,
+        entry_time,
         find_stim_dset,
         iter_entries,
     )
 
     expt_start = None
     det = qs.detector(sync_thresh, 10)
     trials = []
     for entry_num, entry in iter_entries(data_file):
-        log.info(" - entry: '%s'", entry.name)
+        logging.info(" - entry: '%s'", entry.name)
         entry_start = entry_time(entry)
-        log.info("  - start time: %s", entry_datetime(entry))
+        logging.info("  - start time: %s", entry_datetime(entry))
         if expt_start is None:
             expt_start = entry_start
 
-        log.info("  - parsing stimulus log")
+        logging.info("  - parsing stimulus log")
         stims = list(oeaudio_stims(find_stim_dset(entry)))
-        log.info("    - detected %d stimuli", len(stims))
-        log.info("  - sync track: '%s'", sync_dset)
+        logging.info("    - detected %d stimuli", len(stims))
+        logging.info("  - sync track: '%s'", sync_dset)
         sync = entry[sync_dset]
         sync_data = sync[:].astype("d")
         det.scale_thresh(sync_data.mean(), sync_data.std())
         stim_onsets = np.asarray(det(sync_data))
-        log.info("    - detected %d clicks", stim_onsets.size)
+        logging.info("    - detected %d clicks", stim_onsets.size)
         dset_offset = sync.attrs["offset"]
         dset_end = sync.size
         sampling_rate = sync.attrs["sampling_rate"]
         stim_sample_offset = int(dset_offset * sampling_rate)
-        log.info("  - recording clock offset: %d", stim_sample_offset)
+        logging.info("  - recording clock offset: %d", stim_sample_offset)
 
         if len(stims) != stim_onsets.size:
-            log.warning(
+            logging.warning(
                 "  - WARNING: number of stimuli does not match number of clicks. This recording may need to be discarded"
             )
 
         padding_samples = int(prepad * sampling_rate)
         for stim, onset, offset in zip_longest(
             stims, stim_onsets, stim_onsets[1:], fillvalue=dset_end + padding_samples
         ):
             stim_seconds = await stim_duration(session, stim.name)
             stim_samples = int(stim_seconds * sampling_rate)
             if stim_samples > offset - onset:
-                log.warning(
+                logging.warning(
                     "  - WARNING: stimulus %s is longer than the duration of the trial",
                     stim,
                 )
             trials.append(
                 Trial(
                     entry_num,
                     onset - padding_samples,
@@ -170,26 +172,29 @@
     return trials
 
 
 def assign_events_flat(events: pd.DataFrame, sampling_rate: float):
     """Assign event_times to clusters, generating a large toelis object"""
     nevents, _ = events.shape
     nclusters = events.index.unique().size
-    log.info("- grouping %d spikes into %d clusters...", nevents, nclusters)
+    logging.info("- grouping %d spikes into %d clusters...", nevents, nclusters)
     return events.groupby("clust").apply(
         lambda df: df.time.sort_values().to_numpy() / sampling_rate * 1000.0
     )
 
 
 def trials_to_pprox(trials: pd.DataFrame, sampling_rate: float):
     """Convert pandas trials to pproc"""
     for trial in trials.itertuples():
-        # TODO need to handle empty trials
+        if isinstance(trial.events, float):
+            events = []
+        else:
+            events = (trial.events.astype("d") - trial.stimulus_start) / sampling_rate
         pproc = {
-            "events": (trial.events.astype("d") - trial.stimulus_start) / sampling_rate,
+            "events": events,
             "offset": trial.stimulus_start / sampling_rate,
             "index": trial.Index,
             "interval": (
                 (trial.recording_start - trial.stimulus_start) / sampling_rate,
                 (trial.recording_end - trial.stimulus_start) / sampling_rate,
             ),
             "stimulus": {
@@ -205,22 +210,22 @@
                 "end": trial.recording_end,
             },
         }
         yield pproc
 
 
 async def group_spikes_script(argv=None):
-    import os
     import argparse
+    import os
 
     from dlab.core import __version__
     from dlab.extracellular import entry_metadata, iter_entries
-    from dlab.util import json_serializable, setup_log
+    from dlab.util import json_serializable
 
-    version = "2023.02.22"
+    version = "2023.04.18"
 
     p = argparse.ArgumentParser(
         description="group kilosorted spikes into pprox files based on cluster and trial"
     )
     p.add_argument(
         "-v",
         "--version",
@@ -279,203 +284,191 @@
         "-n",
         help="base name of the unit (default is based on 'recording' field of trials pprox) ",
     )
     p.add_argument(
         "--save-waveforms",
         "-W",
         action="store_true",
-        help="save representative waveforms from each unit's main channel in npy format",
-    )
-    p.add_argument(
-        "--waveform-num-spikes",
-        type=int,
-        default=200,
-        help="maximum number of spikes to use for average waveform",
-    )
-    p.add_argument(
-        "--waveform-seed",
-        type=int,
-        default=12345,
-        help="random seed for selecting spikes",
+        help="save representative waveforms from each unit's main channel in an hdf5 file",
     )
     p.add_argument(
         "--waveform-pre-peak",
         type=float,
         default=2.0,
         help="samples before the spike to keep (default %(default).1f ms)",
     )
     p.add_argument(
         "--waveform-post-peak",
         type=float,
         default=5.0,
         help="samples after the spike to keep (default %(default).1f ms)",
     )
-    p.add_argument(
-        "--waveform-upsample",
-        type=int,
-        default=3,
-        help="factor to upsample spikes before aligning them (default %(default)0.1f)",
-    )
     p.add_argument("recording", type=Path, help="path of ARF recording file")
     p.add_argument(
         "sortdir",
         type=Path,
         help="kilosort output directory. Needs to contain 'spike_times.npy', 'spike_clusters.npy',"
         " 'cluster_info.tsv', and 'temp_wh.dat'",
     )
     args = p.parse_args(argv)
-    setup_log(log, args.debug)
+    logging.basicConfig(
+        format="%(message)s", level=logging.DEBUG if args.debug else logging.INFO
+    )
     os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"
+    logging.info("- %s version %s", p.prog, version)
 
-    async with ClientSession() as session:
+    async with AsyncClient(timeout=None) as session:
         resource_info = await nbank.fetch_metadata(
             session, nbank.default_registry, args.recording.stem
         )
         recording_name = resource_info["name"]
         resource_url = nbank.registry.full_url(nbank.default_registry, recording_name)
-        log.info("- kilosort output directory: %s", args.sortdir)
+        logging.info("- kilosort output directory: %s", args.sortdir)
         timefile = args.sortdir / "spike_times.npy"
         clustfile = args.sortdir / "spike_clusters.npy"
         infofile = args.sortdir / "cluster_info.tsv"
-        log.info("  - spike times: %s", timefile)
-        log.info("  - spike clusters: %s", clustfile)
+        logging.info("  - spike times: %s", timefile)
+        logging.info("  - spike clusters: %s", clustfile)
         events = pd.DataFrame(
             {"time": np.load(timefile).squeeze(), "clust": np.load(clustfile)},
         ).set_index("clust")
-        log.info("  - cluster info: %s", infofile)
+        logging.info("  - cluster info: %s", infofile)
         info = pd.read_csv(infofile, sep="\t", index_col=0)
         recfile = args.sortdir / "temp_wh.dat"
         params = read_kilo_params(args.sortdir / "params.py")
         recording = np.memmap(recfile, mode="c", dtype=params["dtype"])
         recording = np.reshape(
             recording, (recording.size // params["nchannels"], params["nchannels"])
         )
         nsamples, nchannels = recording.shape
-        log.info("  - filtered recording: %s", recfile)
-        log.info("    - %d samples, %d channels", nsamples, nchannels)
+        logging.info("  - filtered recording: %s", recfile)
+        logging.info("    - %d samples, %d channels", nsamples, nchannels)
         if args.cluster is not None:
-            log.info("- only analyzing clusters: %s", args.cluster)
+            logging.info("- only analyzing clusters: %s", args.cluster)
             events = events.loc[args.cluster]
 
         if args.toelis:
-            import toelis
-
             clusters = assign_events_flat(events, params["sampling_rate"])
             outfile = (args.output / recording_name).with_suffix(".toe_lis")
             if not args.dry_run:
                 with open(outfile, "wt") as ofp:
                     toelis.write(ofp, clusters)
-                log.info("- saved %d spikes to '%s'", toelis.count(clusters), outfile)
+                logging.info(
+                    "- saved %d spikes to '%s'", toelis.count(clusters), outfile
+                )
             return
 
-        if args.recording.exists():
+        if args.recording.is_file():
             datafile = args.recording
         else:
             datafile = await nbank.find_resource(
                 session, nbank.default_registry, str(args.recording)
             )
-        log.info("- splitting '%s' into trials:", datafile)
+        logging.info("- splitting '%s' into trials:", datafile)
         with h5.File(datafile, "r") as afp:
             trials = pd.DataFrame(
                 await oeaudio_to_trials(
                     session, afp, args.sync, args.sync_thresh, args.prepad
                 )
             )
             entry_attrs = tuple(entry_metadata(e) for _, e in iter_entries(afp))
 
         # this pandas magic sorts the events by cluster and trial
-        log.info("- sorting events into trials:")
+        logging.info("- sorting events into trials:")
         events["trial"] = (
             trials.recording_start.searchsorted(events.time, side="left") - 1
         )
-        clusters = (
-            events.groupby("clust")
-            .apply(lambda df: df.groupby("trial").apply(lambda x: x.time.to_numpy()))
-            .unstack("clust")
-            .unstack("clust")  # I have no idea why this is necessary
+        clusters = events.groupby("clust").apply(
+            lambda df: df.groupby("trial").apply(lambda x: x.time.to_numpy())
         )
+        # for some reason the trials end up in columns if we're only looking at
+        # a subset of clusters. This sort of undefined behavior in pandas is
+        # sure annoying.
+        if args.cluster is not None:
+            clusters = clusters.stack("trial")
 
         total_spikes = 0
         total_clusters = 0
-        for clust_id, cluster in clusters.items():
+        for clust_id, cluster in clusters.groupby("clust"):
             clust_info = info.loc[clust_id]
             clust_type = clust_info["group"]
-            clust_trials = trials.join(cluster.rename("events"))
-            n_spikes = clust_trials.events.apply(len).agg("sum")
+            n_spikes = cluster.apply(len).agg("sum")
+            # left join to trial information table - empty trials will be nan
+            clust_trials = trials.join(
+                cluster.reset_index(0, drop=True).rename("events")
+            )
             if clust_type == "noise" or (clust_type == "mua" and not args.mua):
-                log.info(
+                logging.info(
                     "  - cluster %d (%d spikes, %s) -> skipped",
                     clust_id,
                     n_spikes,
                     clust_type,
                 )
                 continue
             total_spikes += n_spikes
             total_clusters += 1
             outfile = args.output / f"{recording_name}_c{clust_id}.pprox"
-            log.info(
+            logging.info(
                 "  ✓ cluster %d (%d spikes, %s) -> %s",
                 clust_id,
                 n_spikes,
                 clust_type,
                 outfile,
             )
-
             clust_trials = pprox.from_trials(
                 trials_to_pprox(clust_trials, params["sampling_rate"]),
                 recording=resource_url,
                 processed_by=[f"{p.prog} {version}"],
                 kilosort_amplitude=clust_info["Amplitude"],
                 kilosort_contam_pct=clust_info["ContamPct"],
                 kilosort_source_channel=clust_info["ch"],
                 kilosort_probe_depth=clust_info["depth"],
                 kilosort_n_spikes=clust_info["n_spikes"],
                 entry_metadata=entry_attrs,
                 **resource_info["metadata"],
             )
-            log.info(
-                "    - computing average spike waveform from channel %d",
-                clust_info["ch"],
-            )
-            n_before = int(args.waveform_pre_peak * params["sampling_rate"] / 1000)
-            n_after = int(args.waveform_post_peak * params["sampling_rate"] / 1000)
-            spikes = events.loc[clust_id]
-            spikes = spikes[
-                (spikes.time > n_before) & (spikes.time < (nsamples - n_after))
-            ]
-            selected = spikes.sample(
-                min(args.waveform_num_spikes, n_spikes), random_state=args.waveform_seed
-            )
-            times = sorted(selected.time)
-            waveforms = qs.peaks(
-                recording[:, clust_info["ch"]], times, n_before, n_after
-            )
-            if args.waveform_upsample > 1:
-                # quick and dirty check for inverted signal
-                mean_spike = waveforms.mean(0)
-                flip = np.sign(mean_spike.min() + mean_spike.max())
-                _, waveforms = qs.realign_spikes(
-                    times,
-                    waveforms * flip,
-                    args.waveform_upsample,
-                    expected_peak=n_before * args.waveform_upsample,
-                )
-                waveforms *= flip
-            clust_trials["waveform"] = {
-                "mean": waveforms.mean(0),
-                "sampling_rate": params["sampling_rate"] * args.waveform_upsample,
-            }
-            if args.save_waveforms:
-                np.save(args.output / (outfile.stem + "_spikes.npy"), waveforms)
-
             if not args.dry_run:
                 with open(outfile, "wt") as ofp:
                     json.dump(clust_trials, ofp, default=json_serializable)
-        log.info(
+            if args.save_waveforms:
+                outfile = args.output / (outfile.stem + "_spikes.h5")
+                logging.info(
+                    "    - waveforms on channel %d -> %s",
+                    clust_info["ch"],
+                    outfile,
+                )
+                n_before = int(args.waveform_pre_peak * params["sampling_rate"] / 1000)
+                n_after = int(args.waveform_post_peak * params["sampling_rate"] / 1000)
+                spikes = events.loc[clust_id]
+                spikes = spikes[
+                    (spikes.time > n_before) & (spikes.time < (nsamples - n_after))
+                ]
+                waveforms = qs.peaks(
+                    recording[:, clust_info["ch"]],
+                    spikes.time,
+                    n_before,
+                    n_after,
+                )
+                if not args.dry_run:
+                    save_waveforms(
+                        outfile,
+                        SpikeWaveforms(
+                            waveforms.T, spikes.time, params["sampling_rate"], n_before
+                        ),
+                        recording=resource_url,
+                        processed_by=f"{p.prog} {version}",
+                        kilosort_amplitude=clust_info["Amplitude"],
+                        kilosort_contam_pct=clust_info["ContamPct"],
+                        kilosort_source_channel=clust_info["ch"],
+                        kilosort_probe_depth=clust_info["depth"],
+                        kilosort_n_spikes=clust_info["n_spikes"],
+                    )
+
+        logging.info(
             "- a total of %d spikes were assigned to %d clusters",
             total_spikes,
             total_clusters,
         )
 
 
 def run_group_spikes():
-    asyncio.run(group_spikes_script())
+    anyio.run(group_spikes_script)
```

### Comparing `melizalab-tools-2023.3.2/dlab/nbank.py` & `melizalab-tools-2023.4.19/dlab/nbank.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,133 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """Functions for interfacing with the neurobank repository """
-import asyncio
 import logging
 from typing import Dict, Union
+from urllib.parse import urlparse
+import json
 
-from aiohttp import ClientSession
-from aiopath import AsyncPath
-from nbank import registry, util
+from anyio import Path, create_task_group
+from httpx import AsyncClient, HTTPStatusError
 
-from dlab.util import setup_log
+from dlab import cache
+from nbank import registry, util
 
-log = logging.getLogger("dlab.nbank")
+logging.getLogger(__name__).addHandler(logging.NullHandler())
 default_registry = registry.default_registry()
 
 
 async def find_resource(
-    session: ClientSession,
+    session: AsyncClient,
     registry_url: str,
     resource_id: str,
-    alt_base: Union[AsyncPath, str, None] = None,
+    alt_base: Union[Path, str, None] = None,
     no_download: bool = False,
-) -> AsyncPath:
+) -> Path:
     """Locate a neurobank resource
 
     This function will try to locate resources from the following locations:
     - a local directory (alt_base, if set),
     - a local neurobank archive (using alt_base, if provided),
     - a local cache
     - a remote HTTP archive (caching the file for local access later)
 
     It will raise a ValueError if the resource does not exist and a
     FileNotFoundError if the resource cannot be located.
 
     """
     url, params = registry.get_locations(registry_url, resource_id)
     if alt_base is not None:
-        path = await resolve_local_path(alt_base)
+        stem = Path(alt_base) / resource_id
+        path = await resolve_local_path(stem)
         if path is not None:
+            logging.debug("%s: found in alt_base", resource_id)
             return path
-    async with session.get(url, params=params) as response:
-        if response.status == 404:
-            raise ValueError(f"{resource_id}: not a valid resource name")
-        response.raise_for_status()
-        locations = await response.json()
+    response = await session.get(url, params=params)
+    response.raise_for_status()
+    locations = response.json()
     # search for local files
     for loc in locations:
         if loc["scheme"] not in registry._local_schemes:
             continue
-        path = await resolve_local_path(AsyncPath(util.parse_location(loc, alt_base)))
+        path = await resolve_local_path(Path(util.parse_location(loc, alt_base)))
         if path is not None:
+            logging.debug("%s: found in local repository", resource_id)
             return path
     # search remote locations
     for loc in locations:
         if loc["scheme"] in registry._local_schemes:
             continue
         url = util.parse_location(loc)
         try:
             return await fetch_resource(session, url, resource_id, no_download)
         except FileNotFoundError:
             pass
     # all locations failed; raise an error
     raise FileNotFoundError(f"{resource_id}: unable to locate file")
 
 
-async def resolve_local_path(stem: AsyncPath) -> AsyncPath:
+async def resolve_local_path(stem: Path) -> Path:
     """Find a local resource based on a path or path stem.
 
     Because resource names often don't have extensions, a local filesystem
     search may be needed to resolve the full path.
 
     """
     if await stem.exists():
         return stem
     async for path in stem.parent.glob(f"{stem.name}.*"):
         return path
 
 
 async def fetch_resource(
-    session: ClientSession,
+    session: AsyncClient,
     url: str,
     resource_id: str,  # this could be parsed out of the url
-    chunk_size: int = 8192,
     no_download: bool = False,
-) -> AsyncPath:
+) -> Path:
     """Fetch a downloadable resource from the registry.
 
     The file will be cached locally. Returns the path of the file.
     """
-    from urllib.parse import urlparse
-    from dlab.core import user_cache_dir
-
-    parsed_url = urlparse(url)
-    cache_dir = AsyncPath(user_cache_dir()) / parsed_url.netloc
-    target = cache_dir / resource_id
+    target = await cache.locate(resource_id, urlparse(url).netloc)
     if await target.exists():
+        logging.debug("%s: found in local cache", resource_id)
         return target
     elif no_download:
         raise FileNotFoundError(f"{url}: resource not found in local cache")
-    await cache_dir.mkdir(parents=True, exist_ok=True)
-    log.debug("- fetching %s from registry", resource_id)
-    async with session.get(url) as response:
-        if response.status == 404:
+    logging.debug("%s: fetching from registry", resource_id)
+    async with session.stream("GET", url) as response:
+        if response.status_code == 404:
             raise FileNotFoundError(f"{url}: resource not found")
-        elif response.status == 415:
+        elif response.status_code == 415:
             # should be possible to get the error message from registry?
             raise FileNotFoundError(f"{url}: this data type is not downloadable")
-        async with target.open("wb") as fp:
-            async for data in response.content.iter_chunked(chunk_size):
+        async with await target.open("wb") as fp:
+            async for data in response.aiter_bytes():
                 await fp.write(data)
     return target
 
 
 async def fetch_metadata(
-    session: ClientSession, registry_url: str, resource_id: str
+    session: AsyncClient, registry_url: str, resource_id: str
 ) -> Dict:
-    """Fetch metadata for a resource"""
-    url, params = registry.get_resource(registry_url, resource_id)
-    async with session.get(url, params=params) as response:
+    """Fetch metadata for a resource. Results will be cached locally."""
+    target = await cache.locate(resource_id, urlparse(registry_url).netloc)
+    if await target.exists():
+        logging.debug("%s: metadata found in local cache", resource_id)
+        return json.loads(await target.read_text())
+    else:
+        logging.debug("%s: fetching metadata from registry", resource_id)
+        url, params = registry.get_resource(registry_url, resource_id)
+        response = await session.get(url, params=params)
         response.raise_for_status()
-        return await response.json()
+        data = response.json()
+        await target.write_text(json.dumps(data))
+        return data
 
 
 def add_registry_argument(parser, dest="registry_url"):
     """Add a registry argument to an argparse parser"""
     parser.add_argument(
         "-r",
         dest=dest,
@@ -138,32 +142,48 @@
 
     p = argparse.ArgumentParser(description="locate neurobank resources ")
     p.add_argument("--debug", help="show verbose log messages", action="store_true")
     add_registry_argument(p)
     p.add_argument(
         "-b",
         "--base",
-        type=AsyncPath,
+        type=Path,
         help="set an alternative base directory to search for local resources",
     )
-    p.add_argument("id", help="the identifier of the resource", nargs="+")
+    p.add_argument(
+        "--clear-cache",
+        action="store_true",
+        help="clear the contents of the local cache",
+    )
+    p.add_argument("id", help="identifier(s) of the resource(s) to locate", nargs="*")
     args = p.parse_args(argv)
-    setup_log(log, args.debug)
+    logging.basicConfig(
+        format="%(message)s", level=logging.DEBUG if args.debug else logging.INFO
+    )
+
+    if args.clear_cache:
+        await cache.clear(urlparse(args.registry_url).netloc)
 
-    async with ClientSession(headers={"Accept": "application/json"}) as session:
-        tasks = [
-            find_resource(session, args.registry_url, id, alt_base=args.base)
-            for id in args.id
-        ]
-        for id, task in zip(args.id, asyncio.as_completed(tasks)):
-            try:
-                path = await task
-            except ValueError:
-                log.info("%s: no such resource", id)
-            except FileNotFoundError:
-                log.info("%s: not found, unable to download", id)
-            else:
-                log.info("%s: %s", id, path)
+    async def _find_and_show(session, id):
+        try:
+            path = await find_resource(
+                session, args.registry_url, id, alt_base=args.base
+            )
+        except HTTPStatusError:
+            logging.info("%s: no such resource", id)
+        except FileNotFoundError:
+            logging.info("%s: not found, unable to download", id)
+        else:
+            logging.info("%s: %s", id, path)
+
+    headers = {"Accept": "application/json"}
+    async with AsyncClient(
+        timeout=None, headers=headers
+    ) as session, create_task_group() as tg:
+        for id in args.id:
+            tg.start_soon(_find_and_show, session, id)
 
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    from anyio import run
+
+    run(main)
```

### Comparing `melizalab-tools-2023.3.2/dlab/plotting.py` & `melizalab-tools-2023.4.19/dlab/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """Common functions for plotting things. 
 
 Functions in this module should take matplotlib axes as their first argument,
 but there is no direct import of matplotlib.
 
 """
 from typing import Tuple
+
 import numpy as np
 
 
 def spectrogram(
     ax,
     signal: np.ndarray,
     sampling_rate_hz: float,
@@ -19,16 +20,17 @@
     shift_s: float = 0.010,
     frequency_range: Tuple[float, float] = (700, 10000),
     compression: float = 0.1,
     **plot_kwargs
 ):
     """Plot a spectrogram of a signal, with some useful defaults for birdsong"""
     from math import ceil, log
+
     from ewave import rescale
-    from libtfr import mfft_precalc, fgrid, tgrid
+    from libtfr import fgrid, mfft_precalc, tgrid
 
     data = rescale(signal, np.float64)
     window_samples = int(window_s * sampling_rate_hz)
     nfft = 2 ** ceil(log(window_samples, 2))
     shift_samples = int(shift_s * sampling_rate_hz)
     mfft = mfft_precalc(nfft, np.hanning(window_samples))
     spec = mfft.mtspec(data, shift_samples)
```

### Comparing `melizalab-tools-2023.3.2/dlab/pprox.py` & `melizalab-tools-2023.4.19/dlab/pprox.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.3.2/dlab/signal.py` & `melizalab-tools-2023.4.19/dlab/signal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """ Signal processing functions """
-import numpy as np
 from typing import Tuple
 
+import numpy as np
+
 
 def kernel(name: str, bandwidth: float, dt: float) -> Tuple[np.ndarray, np.ndarray]:
     """
     Generate a smoothing kernel function with bandwidth.
 
     name:      the name of the kernel. can be anything supported
                by scipy.signal.get_window, plus the following functions:
```

### Comparing `melizalab-tools-2023.3.2/dlab/util.py` & `melizalab-tools-2023.4.19/dlab/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """ Utility functions for scripts and modules """
 import argparse
-import logging
 from functools import singledispatch
 
 import numpy as np
 
 
 def setup_log(log, debug=False):
     """Set up logging for a module.
 
     log: generate by calling e.g. `log = logging.getLogger("dlab.extracellular")`
     """
+    import logging
+
     ch = logging.StreamHandler()
     formatter = logging.Formatter("%(message)s")
     loglevel = logging.DEBUG if debug else logging.INFO
     log.setLevel(loglevel)
     ch.setLevel(loglevel)
     ch.setFormatter(formatter)
     log.addHandler(ch)
```

### Comparing `melizalab-tools-2023.3.2/melizalab_tools.egg-info/PKG-INFO` & `melizalab-tools-2023.4.19/melizalab_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melizalab-tools
-Version: 2023.3.2
+Version: 2023.4.19
 Summary: Meliza lab scripts and modules for auditory neurophysiology
 Home-page: https://github.com/melizalab/melizalab-tools
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
@@ -23,15 +23,13 @@
 
 ### modules
 
 - `dlab.pprox`: functions for working with [pprox](https://meliza.org/spec:2/pprox/) objects, a data format for storing multi-trial point process data (e.g. spike times evoked by stimulus presentation).
 
 ### console scripts
 
-- `song-detect`: This is a wrapper for the [quicksong](https://github.com/melizalab/quicksong/) package, an algorithm for automatically segmenting acoustic recordings into songs. 
-
-- `group-kilo-spikes`
+- `group-kilo-spikes`: sort spike times output from [kilosort](https://github.com/MouseLand/Kilosort) and [phy2](https://github.com/cortex-lab/phy/) into pprox files.
 
 ### other stuff
 
 - `scripts/extract_waveforms.py`: extracts spike waveforms from a raw recording (in ARF format) using spike times stored in a file (pprox format). This script is mostly only used to verify that spike sorting is working properly, because the `group-kilo-spikes` script has an option to store average waveforms.
```

### Comparing `melizalab-tools-2023.3.2/melizalab_tools.egg-info/SOURCES.txt` & `melizalab-tools-2023.4.19/melizalab_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 dlab/__init__.py
+dlab/cache.py
 dlab/core.py
 dlab/extracellular.py
 dlab/extract_waveforms.py
 dlab/kilo.py
 dlab/nbank.py
 dlab/plotting.py
 dlab/pprox.py
 dlab/signal.py
-dlab/song_detect.py
 dlab/spikes.py
 dlab/util.py
 melizalab_tools.egg-info/PKG-INFO
 melizalab_tools.egg-info/SOURCES.txt
 melizalab_tools.egg-info/dependency_links.txt
 melizalab_tools.egg-info/entry_points.txt
 melizalab_tools.egg-info/not-zip-safe
```

### Comparing `melizalab-tools-2023.3.2/setup.cfg` & `melizalab-tools-2023.4.19/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -27,30 +27,25 @@
 [options]
 zip_safe = false
 packages = dlab
 python_requires = >= 3.8
 setup_requires = 
 	setuptools >=58.1.0
 install_requires = 
-	aiopath >= 0.5.12
-	aiohttp >= 3.8.4
+	anyio >= 3.6.2
 	appdirs >= 1.4.4
 	arf >= 2.6.4
-	arfx >= 2.6.12
-	neurobank >= 0.10.2
-	numpy >= 1.23.1
-	pandas >= 1.4
-	PyYAML >= 5.4.1
+	neurobank >= 0.10.3
+	pandas >= 1.4.0
 	quickspikes >= 1.3.9
-	quicksong >= 0.2.0
-	scikit-learn >= 1.1.2
 	toelis >= 2.1.1
+	libtfr >= 2.1.7
+	ewave >= 1.0.7
 
 [options.entry_points]
 console_scripts = 
 	group-kilo-spikes = dlab.kilo:run_group_spikes
-	song-detect = dlab.song_detect:script
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `melizalab-tools-2023.3.2/tests/test_pprox.py` & `melizalab-tools-2023.4.19/tests/test_pprox.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.3.2/tests/test_spikes.py` & `melizalab-tools-2023.4.19/tests/test_spikes.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 def test_psth_clip():
     start = 1.1
     stop = 4.0
     binwidth = 0.01
     events = [1.1, 2.1, 2.9, 4.01]
-    counts, bins = spikes.psth(events, binwidth, start, stop)
+    counts, bins = spikes.psth(events, binwidth, start=start, stop=stop)
     assert counts.sum() == sum(1 for e in events if e >= start and e < 4.0)
     assert counts.size == bins.size
 
 
 def test_psth_multi_trial():
     """multi-trial data is fine as long as it can be flattened"""
     binwidth = 0.1
@@ -46,9 +46,9 @@
     """If kernel is scaled correctly, sum of rate over interval should be equal to N"""
     from dlab.signal import kernel
 
     binwidth = 0.01
     bandwidth = 0.1
     events = (1.1, 2.1, 2.9, 4.01)
     k, kt = kernel("gaussian", bandwidth, binwidth)
-    r, rt = spikes.rate(events, binwidth, k, 0.0, 5.0)
+    r, rt = spikes.rate(events, binwidth, k, start=0.0, stop=5.0)
     assert r.sum() * binwidth == pytest.approx(len(events))
```


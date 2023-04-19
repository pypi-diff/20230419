# Comparing `tmp/usody_sanitize-0.1.0b1.tar.gz` & `tmp/usody_sanitize-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usody_sanitize-0.1.0b1.tar", max compression
+gzip compressed data, was "usody_sanitize-0.1.0b3.tar", max compression
```

## Comparing `usody_sanitize-0.1.0b1.tar` & `usody_sanitize-0.1.0b3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    34523 2023-03-06 20:15:48.713049 usody_sanitize-0.1.0b1/LICENSE
--rwxr-xr-x   0        0        0     4653 2023-01-21 01:06:12.000000 usody_sanitize-0.1.0b1/README.md
--rwxr-xr-x   0        0        0      700 2023-03-06 07:17:40.375493 usody_sanitize-0.1.0b1/pyproject.toml
--rwxr-xr-x   0        0        0       28 2023-03-06 07:01:07.724756 usody_sanitize-0.1.0b1/usody_sanitize/__init__.py
--rwxr-xr-x   0        0        0     4606 2023-02-28 14:27:01.000000 usody_sanitize-0.1.0b1/usody_sanitize/commands.py
--rwxr-xr-x   0        0        0    10139 2023-03-06 18:38:21.242638 usody_sanitize-0.1.0b1/usody_sanitize/erasure.py
--rwxr-xr-x   0        0        0     1127 2023-03-06 07:15:36.742067 usody_sanitize-0.1.0b1/usody_sanitize/main.py
--rw-r--r--   0        0        0     3305 2023-02-23 03:02:46.000000 usody_sanitize-0.1.0b1/usody_sanitize/methods.py
--rw-r--r--   0        0        0      206 2023-02-21 01:32:23.000000 usody_sanitize-0.1.0b1/usody_sanitize/schemas/__init__.py
--rw-r--r--   0        0        0      716 2023-02-21 01:33:13.000000 usody_sanitize-0.1.0b1/usody_sanitize/schemas/devices.py
--rw-r--r--   0        0        0     5184 2023-02-20 23:55:13.000000 usody_sanitize-0.1.0b1/usody_sanitize/schemas/erasure.py
--rw-r--r--   0        0        0     3635 2023-02-03 16:48:51.000000 usody_sanitize-0.1.0b1/usody_sanitize/schemas/export_data.py
--rwxr-xr-x   0        0        0     5412 2023-02-23 03:09:07.000000 usody_sanitize-0.1.0b1/usody_sanitize/steps.py
--rw-r--r--   0        0        0     1487 2023-02-22 05:49:02.000000 usody_sanitize-0.1.0b1/usody_sanitize/utils.py
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 usody_sanitize-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-19 02:19:59.304629 usody_sanitize-0.1.0b3/LICENSE
+-rwxr-xr-x   0        0        0     4349 2023-04-19 05:21:38.796418 usody_sanitize-0.1.0b3/README.md
+-rwxr-xr-x   0        0        0      746 2023-04-19 05:43:02.732116 usody_sanitize-0.1.0b3/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2023-04-17 19:57:17.796161 usody_sanitize-0.1.0b3/usody_sanitize/__init__.py
+-rw-r--r--   0        0        0     2353 2023-04-19 05:37:39.768860 usody_sanitize-0.1.0b3/usody_sanitize/cmd_client.py
+-rwxr-xr-x   0        0        0     4785 2023-04-19 05:21:37.169737 usody_sanitize-0.1.0b3/usody_sanitize/commands.py
+-rwxr-xr-x   0        0        0    11345 2023-04-19 05:40:38.567324 usody_sanitize-0.1.0b3/usody_sanitize/erasure.py
+-rwxr-xr-x   0        0        0     1120 2023-04-17 03:46:30.428865 usody_sanitize-0.1.0b3/usody_sanitize/main.py
+-rw-r--r--   0        0        0     2975 2023-04-17 04:17:15.564592 usody_sanitize-0.1.0b3/usody_sanitize/methods.py
+-rw-r--r--   0        0        0      206 2023-02-21 01:32:23.532667 usody_sanitize-0.1.0b3/usody_sanitize/schemas/__init__.py
+-rw-r--r--   0        0        0      716 2023-02-21 01:33:13.740208 usody_sanitize-0.1.0b3/usody_sanitize/schemas/devices.py
+-rw-r--r--   0        0        0     5368 2023-04-17 03:38:26.941252 usody_sanitize-0.1.0b3/usody_sanitize/schemas/erasure.py
+-rw-r--r--   0        0        0     3635 2023-02-03 16:48:51.000000 usody_sanitize-0.1.0b3/usody_sanitize/schemas/export_data.py
+-rwxr-xr-x   0        0        0     5412 2023-02-23 03:09:07.516501 usody_sanitize-0.1.0b3/usody_sanitize/steps.py
+-rw-r--r--   0        0        0     1487 2023-02-22 05:49:02.035640 usody_sanitize-0.1.0b3/usody_sanitize/utils.py
+-rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 usody_sanitize-0.1.0b3/setup.py
+-rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 usody_sanitize-0.1.0b3/PKG-INFO
```

### Comparing `usody_sanitize-0.1.0b1/README.md` & `usody_sanitize-0.1.0b3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,52 @@
-# Usody Erasure
+# Usody Sanitize
 
 > Under development.
 
 This tool securely erases disks by performing a certificate-based validation of
 the wipe process. It ensures that the data on the disk is completely and 
 irrecoverably erased, protecting sensitive information from being recovered. 
 The tool uses industry-standard wiping methods to securely erase the data on 
 the disk, making it impossible to recover. The tool also generates a 
-certificate of erasure that can be used to verify the authenticity of the wipe
+certificate of sanitize process that can be used to verify the authenticity of the wipe
 process. This tool is perfect for businesses and individuals who need to
 securely and permanently remove sensitive data from their disks.
 
+## Todo
+
+- Test the command with more errors on erasures.
+- Better command output handler.
+- Improve the export of the erasures into json files.
 
 ## Installation
 
 Install the package from the official PyPi repository:
 
 <div class="termy">
 
 ```console
-$ pip install usody_erasure
+$ pip install usody_sanitize
 
 ---> 100%
 ```
 
 </div>
 
 ## Usage
 
 You can use this module via terminal or calling it from an external code.
 
 ### Terminal client
 
 Erase a single disk using the default method: 
-  
-```bash
-usody_erasure -v /dev/sda  
-```
-
-
-## Create new release
-  
-This project uses Poetry to create a new release and publish new releases.
-
-1. Create a new tag version using the poetry command.
 
 ```bash
-poetry self add poetry-bumpversion
+usody_sanitize -v /dev/sda  
 ```
 
-2. Set the new version with the
-[semantic versioning system](https://semver.org/spec/v1.0.0-beta.html) 
-and then build the new release.
-
-```bash
-poetry version <version>
-poetry build
-```
-
-3. Publish it to the PyPi repository.
-
-```bash
-poetry publish
-```
 
 ## Issues
 
 ### hdparm Error: The running kernel lacks CONFIG_IDE_TASK_IOCTL support for this device
 
 When trying to run the command 
 `hdparm --user-master u --security-erase UsodyPassword /dev/sdX`, an error
```

### Comparing `usody_sanitize-0.1.0b1/pyproject.toml` & `usody_sanitize-0.1.0b3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "usody-sanitize"
-version = "0.1.0-beta1"
+version = "0.1.0-beta3"
 
-description = "A tool to securely erasing data on disks HDD and SSD"
+description = "A tool to securely erase/wipe data on disks HDD and SSD with a proper sanitization process."
 repository = "https://github.com/usody/sanitize"
 authors = ["blkpws <me@blkpws.xyz>"]
 readme = "README.md"
 
 [tool.poetry_bumpversion.file."usody_sanitize/__init__.py"]
 
 [tool.poetry.dependencies]
@@ -17,13 +17,14 @@
 mkdocs = "^1.4.2"
 jinja2 = "^3.1.2"
 typer = "^0.7.0"
 mkdocs-material = "^9.0.6"
 mdx-include = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 
+
 [tool.poetry.scripts]
-sanitize-all = "usody_sanitize.main:run"
+sanitize = "usody_sanitize.cmd_client:run_cmd"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/commands.py` & `usody_sanitize-0.1.0b3/usody_sanitize/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,47 +12,52 @@
 
 async def list_blocks(
         dev_path: Optional[str] = None,
         children: bool = False,
 ) -> List[schemas.Block]:
     """Runs the command `lsblk` to get the information about devices.
 
+    Used maily to detect USB, live USB or disk attached.
+
     :param Optional[str] dev_path:
     :param bool children: Get partitions of each device.
 
     :return:
     """
     command = ["lsblk", "-JOa" if children else "-JOad"]
     logger.debug(f"Running command: `{command}`")
     if dev_path:
         command += [dev_path]
     output_text = subprocess.check_output(command, text=True)
 
     logger.debug(f"Processing `{command}` output.")
     devices_json = json.loads(output_text.strip()).get("blockdevices", [])
-    return [schemas.Block(**dev) for dev in devices_json]
+    return [schemas.Block.parse_obj(dev) for dev in devices_json]
 
 
 async def get_smart_info(dev_path: str) -> schemas.Smart:
     """Gets the information of the device with the `smartctl` command.
 
+    Used to detect when a disk is SSD or HDD correctly, as lsblk don't
+    detect this value correctly.
+
     :param str dev_path:
     :return:
     """
     command = ["smartctl", "-aj", dev_path]
     proc = await asyncio.create_subprocess_exec(
         *command,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     await proc.wait()
     output = await proc.stdout.read()
     smart_json = json.loads(output.decode('UTF-8').rstrip())
     logger.debug(f"Smart for {dev_path} is: {smart_json}")
-    return schemas.Smart(**smart_json)
+    return schemas.Smart.parse_obj(smart_json)
 
 
 async def get_total_sectors(dev_path: str) -> int:
     """Get the total
     """
     command = ["blockdev", "--getsz", dev_path]
     proc = await asyncio.create_subprocess_exec(
```

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/erasure.py` & `usody_sanitize-0.1.0b3/usody_sanitize/erasure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,126 @@
+import sys
 import json
 import logging
 import asyncio
 
-from typing import List, Optional
+from enum import Enum
 
-from pydantic.schema import schema
-
-from usody_sanitize import schemas, commands, steps, utils
-from usody_sanitize.methods import ErasureMethods
+from typing import List, Union, Optional
+from usody_sanitize import schemas, commands, steps, utils, __version__
+from usody_sanitize.methods import (
+    BASIC,
+    BASELINE,
+    ENHANCED,
+    CRYPTOGRAPHIC,
+)
 
 logger = logging.getLogger(__name__)
 
 
-async def auto_erase_all_disks() -> Optional[List[dict]]:
+class DefaultMethods(Enum):
+    """To easily convert strings to the method pre-defined. Used
+    when calling to the sanitize with string instead with method class.
+    """
+    BASIC = BASIC
+    BASELINE = BASELINE
+    ENHANCED = ENHANCED
+
+
+async def auto_erase_disks(
+        method: Optional[str] = None,
+        disks: Optional[List[str]] = None,
+) -> Optional[List[dict]]:
     """A main point to erase all disks unless disks mounted at root "/"
     then generates a certificate as JSON with all the information of
     the disk, erasure and the validation of the successful data wiped.
 
+    :param Optional[str] method: A string to select which pre-defined
+        methods to use, basic, baseline or enhanced. If none, Basic will
+        be selected.
+    :param Optional[List[str]] disks: A list of disks to be erased. If
+        none, all disks detected will be erased and sanitized.
+
     :return:
     """
+    # Select method.
+    if method:
+        try:
+            method = DefaultMethods[method.upper()].value
+        except ValueError:
+            sys.exit("Sanitize method not valid.")
+    else:
+        # Default method when not set by args.
+        method = DefaultMethods.BASIC.value
+    logger.info(f"Using sanitize method '{method.name}'.")
+
+    # Get disks.
     blocks: List[schemas.Block] = await commands.list_blocks(children=True)
     erasures: List[ErasureProcess] = []
     tasks: List[asyncio.Task] = []
 
+
     for blk in blocks:
 
         if blk.type != "disk":
             logger.debug(f"Skipping {blk.path}")
             continue  # Skip non disk volumes.
 
+        if disks is not None and blk.path in disks:
+            disks.remove(blk.path)
+        else:
+            continue
+
         # Detect if one of those drives has a mounted partition as root.
         if blk.children:
+
             if any([cld.mountpoint == "/" for cld in blk.children
                     if cld.mountpoint is not None]):
-                logger.warning(f"{blk.path} has a mounted partition as root.")
+                logger.warning(f"Skipping disk {blk.path} mounted as root.")
                 continue
 
         logger.debug(f"Processing disk {blk.path}.")
-        erasure = ErasureProcess(blk, method=None)
+        erasure = ErasureProcess(blk, method)
         erasures.append(erasure)
 
         # Start erasure task.
         tasks.append(asyncio.create_task(erasure.run()))
 
+    if disks:
+        logger.warning(f"Disks [{', '.join(disks)}] not found.")
+
     [await task for task in tasks]
-    return [erasure_finished.export() for erasure_finished in erasures]
+    logger.debug(f">>> {erasures}")
+    return [r.export() for r in erasures]
 
 
 class ErasureProcess:
     def __init__(
             self,
             block: schemas.Block,
-            method: schemas.ErasureMethod = None
+            method: Union[schemas.ErasureMethod, str] = None
     ):
-        logger.info(f"Start erasing process for device {block.path}.")
+        if isinstance(method, str):
+            # Todo: convert to schema.
+            pass
+
+        logger.info(f"Selected device {block.path} for sanitization.")
         self._device = schemas.Device(
             export_data=schemas.ExportData(
                 block=block,  # Data from `lsblk`
             )
         )
         validation = schemas.ErasureValidation()
         self._certificate = schemas.ErasureCertificate(
             device_info=self._device,
             validation=validation,
+            usody_sanitize=__version__
         )
         # --> HERE SELECT THE DEFAULT ERASURE METHOD <--
-        self._certificate.method = ErasureMethods.basic \
-            if method is None else method
+        self._certificate.method = BASIC if method is None else method
 
     @property
     def blk(self) -> Optional[schemas.Block]:
         return self._device.export_data.block
 
     @property
     def smart(self) -> Optional[schemas.Smart]:
@@ -81,21 +131,17 @@
 
     async def extract_device_info(self):
         """Get the basic info from the `lsblk` command and store it
         into the device schema. As the name of the function says,
 
         :return:
         """
-        # Check manufacturer names.
-        # Todo: Do a check if the device between
-        #  `smartctl` and `lsblk` matches.
-
         # Check if the device is SSD or HDD.
-        if self.smart.rotation_rate == 0:
-            if self.blk.rota == 1:
+        if self.smart.rotation_rate == 0:  # Is SSD.
+            if self.blk.rota == 1:  # `lsblk` says is a HDD.
                 logger.debug("SSD \n\t"
                              f"`lsblk` rotate = {self.blk.rota}\n\t"
                              "`smartctl` rotation_rate"
                              f" = {self.smart.rotation_rate}")
 
             self._device.storage_medium = "SSD"
 
@@ -152,16 +198,14 @@
         logger.debug(f"{self.blk.path}: Erasure finished, results:"
                      f" {json.dumps(self._certificate.dict(), indent=4)}")
 
     async def _pre_validation(self):
         """Check if the disk is not mounted and if it is not a
         read-only device.
 
-        Todo: Include validation commands on the final certification.
-
         :return:
         """
         bs = self.smart.logical_block_size
         max_sectors = await commands.get_total_sectors(self.blk.path)
         sectors = utils.get_spaced_numbers(max_sectors, 10)
 
         def _successful_command(
@@ -198,14 +242,15 @@
             cmd3 = await commands.read_from_sector(self.blk.path, s, bs)
             cmd3.description = "Check if new bytes has been written"
             if not _successful_command(cmd3):
                 return False
 
             elif self._certificate.validation.data[s] == cmd3.stdout:
                 logger.warning(
+                    f"{self.blk.path}: "
                     f"Validation failed: Sector {s} has not been changed")
                 return False
             # Successful write, update the sector with new value.
             self._certificate.validation.data[s] = cmd3.stdout
 
         logger.debug(f"{self.blk.path}: Pre validation step finished.")
         return True
@@ -237,34 +282,33 @@
         #   OR use dd to write a few bytes to the disk and check if
         #   they are still there after the erasure.
 
         current_method = self._certificate.method.program
 
         logger.debug(f"Using '{current_method}' for `{self.blk.path}`.")
         # Todo: Run the erasure as many steps as defined in the method.
-        # for n in range(self._certificate.method.overwriting_steps):
-
-        # Erasure steps.
-        if current_method == ErasureMethods.basic.program:
-            step = await steps.erase_hdd_shred(self.blk.path)
-            self._certificate.erasure_steps.append(step)
-        elif current_method == ErasureMethods.baseline_erasure.program:
-            step = await steps.erase_hdd_badblocks(self.blk.path)
-            self._certificate.erasure_steps.append(step)
-        else:
-            logger.error(
-                f"'{self._certificate.method.program}' not implemented.")
+        for n in range(self._certificate.method.overwriting_steps):
+            # Erasure steps.
+            if current_method == 'shred':
+                step = await steps.erase_hdd_shred(self.blk.path)
+                self._certificate.erasure_steps.append(step)
+            elif current_method == 'badblocks':
+                step = await steps.erase_hdd_badblocks(self.blk.path)
+                self._certificate.erasure_steps.append(step)
+            else:
+                logger.error(
+                    f"'{self._certificate.method.program}' not implemented.")
 
     async def _erase_ssd(self):
         """To erase an SSD, the only method allowed right now is the
         Baseline Cryptographic, so the method will be overwritten.
         :return:
         """
         # SSD can only be erased with method Cryptographic. Overwriting
         # erasures damages the disk.
-        self._certificate.method = ErasureMethods.baseline_cryptographic
+        self._certificate.method = CRYPTOGRAPHIC
 
         # Create the step schema and set initial values.
         logger.debug(f"Starting erasure step for {self.blk} as SSD.")
         self._certificate.erasure_steps.append(
             await steps.erase_ssd_hdparm(self.blk.path),
         )
```

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/main.py` & `usody_sanitize-0.1.0b3/usody_sanitize/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 def run():
     """Forces to run the function in a new async loop."""
     loop = asyncio.new_event_loop()
 
     try:
         logger.info("Starting sanitize main process.")
-        erasures = loop.run_until_complete(
-            erasure.auto_erase_all_disks()  # Start auto erasure process.
-        )
+        erasures = loop.run_until_complete(erasure.auto_erase_disks())
 
     finally:
         loop.close()
 
     return erasures
 
 
 if __name__ == '__main__':
+    # Run this one for development.
+    # Run it.
     logging.basicConfig(
         force=True,
         stream=sys.stdout,
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s %(name)s -"
                " [%(funcName)s at line %(lineno)d]: %(message)s"
     )
```

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/methods.py` & `usody_sanitize-0.1.0b3/usody_sanitize/methods.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,70 @@
+"""Pre-defined sanitize methods to erase disks securely."""
 from usody_sanitize import schemas
 
 
-class ErasureMethods:
-    """Defines and describes the erasure methods available."""
-    basic = schemas.ErasureMethod(
-        name="Basic Erasure",
-        # https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=917935
-        standard="",
-        description="A single-pass overwrite of the entire drive with"
-                    " zeros. This method is relatively fast and simple,"
-                    " but it may not be completely effective in destroying"
-                    " all traces of the original data.",
-        removal_process="Overwriting",
-        program="shred",
-        verification_enabled=True,
-        bad_sectors_enabled=False,
-        overwriting_steps=1,
-    )
-    baseline_erasure = schemas.ErasureMethod(
-        name="Baseline Erasure",
-        standard="NIST, Infosec HGM Baseline",
-        description="Method for securely erasing data in compliance"
-                    " with HMG Infosec Standard 5 guidelines includes"
-                    " a single step of a random write process on the"
-                    " full disk. This process overwrites all data with"
-                    " a randomized pattern, ensuring that it cannot be"
-                    " recovered. Built-in validation confirms that the"
-                    " data has been written correctly, and a final"
-                    " validation confirms that all data has been deleted.",
-        removal_process="Overwriting",
-        program="badblocks",
-        verification_enabled=True,  # Todo: Turn this `False` once tested.
-        bad_sectors_enabled=True,
-        overwriting_steps=1,
-    )
-    baseline_cryptographic = schemas.ErasureMethod(
-        name="Baseline Cryptographic",
-        standard="NIST, Infosec HGM Baseline",
-        description="Method for securely erasing data in compliance"
-                    " with HMG Infosec Standard 5 guidelines includes"
-                    " a single step of a random write process on the"
-                    " full disk. This process overwrites all data with"
-                    " a randomized pattern, ensuring that it cannot be"
-                    " recovered. Built-in validation confirms that the"
-                    " data has been written correctly, and a final"
-                    " validation confirms that all data has been deleted.",
-        removal_process="Overwriting",
-        program="hdparm",
-        verification_enabled=False,
-    )
-    enhanced = schemas.ErasureMethod(
-        name="Enhanced Erasure",
-        standard="HMG Infosec Standard 5",
-        description="Method for securely erasing data in compliance"
-                    " with HMG Infosec Standard 5 guidelines includes"
-                    " a single step of a random write process on the"
-                    " full disk. This process overwrites all data with"
-                    " a randomized pattern, ensuring that it cannot be"
-                    " recovered. Built-in validation confirms that the"
-                    " data has been written correctly, and a final"
-                    " validation confirms that all data has been deleted.",
-        removal_process="Overwriting",
-        program="badblocks",
-        verification_enabled=True,
-        bad_sectors_enabled=True,
-        overwriting_steps=3,
-    )
+BASIC = schemas.ErasureMethod(
+    name="Basic Erasure",
+    # https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=917935
+    standard="",
+    description="A single-pass overwrite of the entire drive with"
+                " zeros. This method is relatively fast and simple,"
+                " but it may not be completely effective in destroying"
+                " all traces of the original data.",
+    removal_process="Overwriting",
+    program="shred",
+    verification_enabled=True,
+    bad_sectors_enabled=False,
+    overwriting_steps=1,
+)
+
+BASELINE = schemas.ErasureMethod(
+    name="Baseline Erasure",
+    standard="NIST, Infosec HGM Baseline",
+    description="Method for securely erasing data in compliance"
+                " with HMG Infosec Standard 5 guidelines includes"
+                " a single step of a random write process on the"
+                " full disk. This process overwrites all data with"
+                " a randomized pattern, ensuring that it cannot be"
+                " recovered. Built-in validation confirms that the"
+                " data has been written correctly, and a final"
+                " validation confirms that all data has been deleted.",
+    removal_process="Overwriting",
+    program="badblocks",
+    verification_enabled=False,
+    bad_sectors_enabled=True,
+    overwriting_steps=1,
+)
+
+CRYPTOGRAPHIC = schemas.ErasureMethod(
+    name="Baseline Cryptographic",
+    standard="NIST, Infosec HGM Baseline",
+    description="Method for securely erasing data in compliance"
+                " with HMG Infosec Standard 5 guidelines includes"
+                " a single step of a random write process on the"
+                " full disk. This process overwrites all data with"
+                " a randomized pattern, ensuring that it cannot be"
+                " recovered. Built-in validation confirms that the"
+                " data has been written correctly, and a final"
+                " validation confirms that all data has been deleted.",
+    removal_process="Overwriting",
+    program="hdparm",
+    verification_enabled=False,
+)
+
+ENHANCED = schemas.ErasureMethod(
+    name="Enhanced Erasure",
+    standard="HMG Infosec Standard 5",
+    description="Method for securely erasing data in compliance"
+                " with HMG Infosec Standard 5 guidelines includes"
+                " a single step of a random write process on the"
+                " full disk. This process overwrites all data with"
+                " a randomized pattern, ensuring that it cannot be"
+                " recovered. Built-in validation confirms that the"
+                " data has been written correctly, and a final"
+                " validation confirms that all data has been deleted.",
+    removal_process="Overwriting",
+    program="badblocks",
+    verification_enabled=True,
+    bad_sectors_enabled=True,
+    overwriting_steps=3,
+)
```

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/schemas/devices.py` & `usody_sanitize-0.1.0b3/usody_sanitize/schemas/devices.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/schemas/erasure.py` & `usody_sanitize-0.1.0b3/usody_sanitize/schemas/erasure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, List
 from pydantic import BaseModel, Field
 
 from usody_sanitize.schemas.devices import Device
+from usody_sanitize import __version__ as app_version
 
 
 class ErasureCommand(BaseModel):
     """Main and base class to define a collection of steps to proceed.
     """
     description: Optional[str] = Field(
         default=None, description="Step description")
@@ -115,8 +116,12 @@
 
     result: bool = Field(
         default=False, description="True means erasure has been pass"
                                    " correctly, False means something"
                                    " failed and the data could not be"
                                    " erased/wipe.")
 
+    sanitize_version: str = Field(
+        default=app_version,
+        description="Version of usody_sanitize python package.")
+
```

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/schemas/export_data.py` & `usody_sanitize-0.1.0b3/usody_sanitize/schemas/export_data.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/steps.py` & `usody_sanitize-0.1.0b3/usody_sanitize/steps.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.0b1/usody_sanitize/utils.py` & `usody_sanitize-0.1.0b3/usody_sanitize/utils.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.0b1/PKG-INFO` & `usody_sanitize-0.1.0b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,67 @@
 Metadata-Version: 2.1
 Name: usody-sanitize
-Version: 0.1.0b1
-Summary: A tool to securely erasing data on disks HDD and SSD
+Version: 0.1.0b3
+Summary: A tool to securely erase/wipe data on disks HDD and SSD with a proper sanitization process.
 Home-page: https://github.com/usody/sanitize
 Author: blkpws
 Author-email: me@blkpws.xyz
 Requires-Python: >=3.9.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Project-URL: Repository, https://github.com/usody/sanitize
 Description-Content-Type: text/markdown
 
-# Usody Erasure
+# Usody Sanitize
 
 > Under development.
 
 This tool securely erases disks by performing a certificate-based validation of
 the wipe process. It ensures that the data on the disk is completely and 
 irrecoverably erased, protecting sensitive information from being recovered. 
 The tool uses industry-standard wiping methods to securely erase the data on 
 the disk, making it impossible to recover. The tool also generates a 
-certificate of erasure that can be used to verify the authenticity of the wipe
+certificate of sanitize process that can be used to verify the authenticity of the wipe
 process. This tool is perfect for businesses and individuals who need to
 securely and permanently remove sensitive data from their disks.
 
+## Todo
+
+- Test the command with more errors on erasures.
+- Better command output handler.
+- Improve the export of the erasures into json files.
 
 ## Installation
 
 Install the package from the official PyPi repository:
 
 <div class="termy">
 
 ```console
-$ pip install usody_erasure
+$ pip install usody_sanitize
 
 ---> 100%
 ```
 
 </div>
 
 ## Usage
 
 You can use this module via terminal or calling it from an external code.
 
 ### Terminal client
 
 Erase a single disk using the default method: 
-  
-```bash
-usody_erasure -v /dev/sda  
-```
-
-
-## Create new release
-  
-This project uses Poetry to create a new release and publish new releases.
-
-1. Create a new tag version using the poetry command.
 
 ```bash
-poetry self add poetry-bumpversion
+usody_sanitize -v /dev/sda  
 ```
 
-2. Set the new version with the
-[semantic versioning system](https://semver.org/spec/v1.0.0-beta.html) 
-and then build the new release.
-
-```bash
-poetry version <version>
-poetry build
-```
-
-3. Publish it to the PyPi repository.
-
-```bash
-poetry publish
-```
 
 ## Issues
 
 ### hdparm Error: The running kernel lacks CONFIG_IDE_TASK_IOCTL support for this device
 
 When trying to run the command 
 `hdparm --user-master u --security-erase UsodyPassword /dev/sdX`, an error
```


# Comparing `tmp/xerparser-0.9.3.tar.gz` & `tmp/xerparser-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerparser-0.9.3.tar", max compression
+gzip compressed data, was "xerparser-0.9.4.tar", max compression
```

## Comparing `xerparser-0.9.3.tar` & `xerparser-0.9.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35149 2022-12-03 05:25:25.921903 xerparser-0.9.3/LICENSE
--rw-r--r--   0        0        0     5352 2023-04-08 15:29:35.029582 xerparser-0.9.3/README.md
--rw-r--r--   0        0        0      743 2023-04-08 15:29:35.029582 xerparser-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      962 2023-04-08 15:29:35.029582 xerparser-0.9.3/xerparser/__init__.py
--rw-r--r--   0        0        0      465 2023-03-01 00:04:03.499449 xerparser-0.9.3/xerparser/schemas/__init__.py
--rw-r--r--   0        0        0     2643 2023-03-01 00:04:28.289431 xerparser-0.9.3/xerparser/schemas/account.py
--rw-r--r--   0        0        0     3247 2023-02-06 03:09:28.587242 xerparser-0.9.3/xerparser/schemas/actvcode.py
--rw-r--r--   0        0        0     1547 2023-01-25 01:32:05.201004 xerparser-0.9.3/xerparser/schemas/actvtype.py
--rw-r--r--   0        0        0    11154 2023-03-01 03:39:04.104780 xerparser-0.9.3/xerparser/schemas/calendars.py
--rw-r--r--   0        0        0      957 2023-03-01 00:04:28.289431 xerparser-0.9.3/xerparser/schemas/ermhdr.py
--rw-r--r--   0        0        0     1367 2023-01-25 01:32:05.211004 xerparser-0.9.3/xerparser/schemas/findates.py
--rw-r--r--   0        0        0      749 2023-01-16 21:15:50.835852 xerparser-0.9.3/xerparser/schemas/memotype.py
--rw-r--r--   0        0        0     1094 2023-02-26 04:48:17.672946 xerparser-0.9.3/xerparser/schemas/pcattype.py
--rw-r--r--   0        0        0     3227 2023-02-26 04:48:17.672946 xerparser-0.9.3/xerparser/schemas/pcatval.py
--rw-r--r--   0        0        0     8546 2023-03-17 20:28:16.137376 xerparser-0.9.3/xerparser/schemas/project.py
--rw-r--r--   0        0        0     2897 2023-03-01 00:04:03.499449 xerparser-0.9.3/xerparser/schemas/projwbs.py
--rw-r--r--   0        0        0     1103 2023-03-01 00:04:03.499449 xerparser-0.9.3/xerparser/schemas/rsrc.py
--rw-r--r--   0        0        0     2970 2023-03-01 00:04:28.289431 xerparser-0.9.3/xerparser/schemas/schedoptions.py
--rw-r--r--   0        0        0    16573 2023-03-17 20:28:16.137376 xerparser-0.9.3/xerparser/schemas/task.py
--rw-r--r--   0        0        0     1462 2023-03-06 00:43:40.451659 xerparser-0.9.3/xerparser/schemas/taskfin.py
--rw-r--r--   0        0        0      805 2022-12-26 20:40:30.667590 xerparser-0.9.3/xerparser/schemas/taskmemo.py
--rw-r--r--   0        0        0     2019 2023-01-25 01:32:05.211004 xerparser-0.9.3/xerparser/schemas/taskpred.py
--rw-r--r--   0        0        0     5063 2023-03-17 20:28:16.137376 xerparser-0.9.3/xerparser/schemas/taskrsrc.py
--rw-r--r--   0        0        0     1927 2023-01-25 01:32:05.211004 xerparser-0.9.3/xerparser/schemas/trsrcfin.py
--rw-r--r--   0        0        0     1524 2023-03-01 00:04:03.499449 xerparser-0.9.3/xerparser/schemas/udftype.py
--rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.3/xerparser/scripts/__init__.py
--rw-r--r--   0        0        0     1548 2022-12-30 22:42:20.878909 xerparser-0.9.3/xerparser/scripts/dates.py
--rw-r--r--   0        0        0      402 2023-01-25 01:32:05.211004 xerparser-0.9.3/xerparser/scripts/decorators.py
--rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.3/xerparser/src/__init__.py
--rw-r--r--   0        0        0     2851 2023-04-08 15:29:35.029582 xerparser-0.9.3/xerparser/src/errors.py
--rw-r--r--   0        0        0     2377 2023-04-08 15:29:35.029582 xerparser-0.9.3/xerparser/src/parser.py
--rw-r--r--   0        0        0      769 2023-04-08 15:29:35.029582 xerparser-0.9.3/xerparser/src/validators.py
--rw-r--r--   0        0        0    10693 2023-03-19 17:16:43.006985 xerparser-0.9.3/xerparser/src/xer.py
--rw-r--r--   0        0        0     6479 1970-01-01 00:00:00.000000 xerparser-0.9.3/setup.py
--rw-r--r--   0        0        0     6077 1970-01-01 00:00:00.000000 xerparser-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-03 05:25:25.921903 xerparser-0.9.4/LICENSE
+-rw-r--r--   0        0        0     5337 2023-04-19 13:53:53.195483 xerparser-0.9.4/README.md
+-rw-r--r--   0        0        0      743 2023-04-19 13:53:53.195483 xerparser-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-04-19 13:53:53.195483 xerparser-0.9.4/xerparser/__init__.py
+-rw-r--r--   0        0        0      465 2023-03-01 00:04:03.499449 xerparser-0.9.4/xerparser/schemas/__init__.py
+-rw-r--r--   0        0        0     2643 2023-03-01 00:04:28.289431 xerparser-0.9.4/xerparser/schemas/account.py
+-rw-r--r--   0        0        0     3247 2023-02-06 03:09:28.587242 xerparser-0.9.4/xerparser/schemas/actvcode.py
+-rw-r--r--   0        0        0     1547 2023-01-25 01:32:05.201004 xerparser-0.9.4/xerparser/schemas/actvtype.py
+-rw-r--r--   0        0        0    11154 2023-03-01 03:39:04.104780 xerparser-0.9.4/xerparser/schemas/calendars.py
+-rw-r--r--   0        0        0      957 2023-03-01 00:04:28.289431 xerparser-0.9.4/xerparser/schemas/ermhdr.py
+-rw-r--r--   0        0        0     1367 2023-01-25 01:32:05.211004 xerparser-0.9.4/xerparser/schemas/findates.py
+-rw-r--r--   0        0        0      749 2023-01-16 21:15:50.835852 xerparser-0.9.4/xerparser/schemas/memotype.py
+-rw-r--r--   0        0        0     1094 2023-02-26 04:48:17.672946 xerparser-0.9.4/xerparser/schemas/pcattype.py
+-rw-r--r--   0        0        0     3227 2023-02-26 04:48:17.672946 xerparser-0.9.4/xerparser/schemas/pcatval.py
+-rw-r--r--   0        0        0     8749 2023-04-19 13:53:53.195483 xerparser-0.9.4/xerparser/schemas/project.py
+-rw-r--r--   0        0        0     2897 2023-03-01 00:04:03.499449 xerparser-0.9.4/xerparser/schemas/projwbs.py
+-rw-r--r--   0        0        0     1103 2023-03-01 00:04:03.499449 xerparser-0.9.4/xerparser/schemas/rsrc.py
+-rw-r--r--   0        0        0     2970 2023-03-01 00:04:28.289431 xerparser-0.9.4/xerparser/schemas/schedoptions.py
+-rw-r--r--   0        0        0    16573 2023-03-17 20:28:16.137376 xerparser-0.9.4/xerparser/schemas/task.py
+-rw-r--r--   0        0        0     1462 2023-03-06 00:43:40.451659 xerparser-0.9.4/xerparser/schemas/taskfin.py
+-rw-r--r--   0        0        0      805 2022-12-26 20:40:30.667590 xerparser-0.9.4/xerparser/schemas/taskmemo.py
+-rw-r--r--   0        0        0     2019 2023-01-25 01:32:05.211004 xerparser-0.9.4/xerparser/schemas/taskpred.py
+-rw-r--r--   0        0        0     5063 2023-03-17 20:28:16.137376 xerparser-0.9.4/xerparser/schemas/taskrsrc.py
+-rw-r--r--   0        0        0     1927 2023-01-25 01:32:05.211004 xerparser-0.9.4/xerparser/schemas/trsrcfin.py
+-rw-r--r--   0        0        0     1524 2023-03-01 00:04:03.499449 xerparser-0.9.4/xerparser/schemas/udftype.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.4/xerparser/scripts/__init__.py
+-rw-r--r--   0        0        0     1548 2022-12-30 22:42:20.878909 xerparser-0.9.4/xerparser/scripts/dates.py
+-rw-r--r--   0        0        0      402 2023-01-25 01:32:05.211004 xerparser-0.9.4/xerparser/scripts/decorators.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.4/xerparser/src/__init__.py
+-rw-r--r--   0        0        0     2851 2023-04-08 15:29:35.029582 xerparser-0.9.4/xerparser/src/errors.py
+-rw-r--r--   0        0        0     2377 2023-04-08 15:29:35.029582 xerparser-0.9.4/xerparser/src/parser.py
+-rw-r--r--   0        0        0      769 2023-04-08 15:29:35.029582 xerparser-0.9.4/xerparser/src/validators.py
+-rw-r--r--   0        0        0    10693 2023-03-19 17:16:43.006985 xerparser-0.9.4/xerparser/src/xer.py
+-rw-r--r--   0        0        0     6464 1970-01-01 00:00:00.000000 xerparser-0.9.4/setup.py
+-rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 xerparser-0.9.4/PKG-INFO
```

### Comparing `xerparser-0.9.3/LICENSE` & `xerparser-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/README.md` & `xerparser-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # xerparser
 
-A simple Python package that reads the contents of a P6 .xer file and converts it into a Python object.  
+Read the contents of a P6 .xer file and convert it into a Python object.  
 
 *Disclaimers:  
 It's helpfull if you are already familiar with the mapping and schemas used by P6 during the export process.
 Refer to the [Oracle Documentation]( https://docs.oracle.com/cd/F25600_01/English/Mapping_and_Schema/xer_import_export_data_map_project/index.htm) for more information regarding how data is mapped to the XER format.  
 Tested on .xer files exported as versions 15.2 through 19.12.*  
 
 <br/>
@@ -117,15 +117,15 @@
 
 ## Error Checking
 
 Sometimes the xer file is corrupted during the export process. If this is the case, a `CorruptXerFile` Exception will be raised during initialization.  A list of the errors can be accessed from the `CorruptXerFile` Exception, or by using the `find_xer_errors` function.
 
 ### Option 1 - `errors` attribute of `CorruptXerFile` exception  (preferred)
 ```python
-from xerparser import Xer
+from xerparser import Xer, CorruptXerFile
 
 file = r"/path/to/file.xer"
 try:
     xer = Xer.reader(file)
 except CorruptXerFile as e:
     for error in e.errors:
         print(error)
```

### Comparing `xerparser-0.9.3/pyproject.toml` & `xerparser-0.9.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xerparser"
-version = "0.9.3"
+version = "0.9.4"
 description = "Parse a P6 .xer file to a Python object."
 authors = ["Jesse <code@seqmanagement.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 keywords = ["primavera", "p6", "xer", "schedule", "scheduling", "planning", "project management", "project controls"]
 repository = "https://github.com/jjCode01/xerparser"
```

### Comparing `xerparser-0.9.3/xerparser/__init__.py` & `xerparser-0.9.4/xerparser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 from xerparser.src.errors import find_xer_errors, CorruptXerFile
 from xerparser.src.parser import parser, file_reader
 from xerparser.src.xer import Xer
 from xerparser.schemas.actvcode import ACTVCODE
 from xerparser.schemas.actvtype import ACTVTYPE
 from xerparser.schemas.calendars import CALENDAR
```

### Comparing `xerparser-0.9.3/xerparser/schemas/account.py` & `xerparser-0.9.4/xerparser/schemas/account.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/actvcode.py` & `xerparser-0.9.4/xerparser/schemas/actvcode.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/actvtype.py` & `xerparser-0.9.4/xerparser/schemas/actvtype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/calendars.py` & `xerparser-0.9.4/xerparser/schemas/calendars.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/ermhdr.py` & `xerparser-0.9.4/xerparser/schemas/ermhdr.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/findates.py` & `xerparser-0.9.4/xerparser/schemas/findates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/memotype.py` & `xerparser-0.9.4/xerparser/schemas/memotype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/pcattype.py` & `xerparser-0.9.4/xerparser/schemas/pcattype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/pcatval.py` & `xerparser-0.9.4/xerparser/schemas/pcatval.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/project.py` & `xerparser-0.9.4/xerparser/schemas/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
     def __init__(
         self,
         sched_options: SCHEDOPTIONS,
         default_calendar: CALENDAR | None = None,
         **data,
     ) -> None:
-
         self.options: SCHEDOPTIONS = sched_options
 
         # table fields from .xer file
         self.uid: str = data["proj_id"]
         self.add_date: datetime = datetime.strptime(data["add_date"], date_format)
         self.default_calendar: CALENDAR | None = default_calendar
         self.data_date: datetime = datetime.strptime(
@@ -122,14 +121,19 @@
 
     @cached_property
     @rounded()
     def actual_cost(self) -> float:
         """Sum of task resource actual costs"""
         return sum(task.actual_cost for task in self.tasks)
 
+    @property
+    def actual_duration(self) -> int:
+        """Project actual duration in calendar days from start date to data date"""
+        return max((0, (self.data_date - self.actual_start).days))
+
     @cached_property
     def actual_start(self) -> datetime:
         """Earliest task start date"""
         if not self.tasks:
             return self.plan_start_date
         return min((task.start for task in self.tasks))
```

### Comparing `xerparser-0.9.3/xerparser/schemas/projwbs.py` & `xerparser-0.9.4/xerparser/schemas/projwbs.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/rsrc.py` & `xerparser-0.9.4/xerparser/schemas/rsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/schedoptions.py` & `xerparser-0.9.4/xerparser/schemas/schedoptions.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/task.py` & `xerparser-0.9.4/xerparser/schemas/task.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/taskfin.py` & `xerparser-0.9.4/xerparser/schemas/taskfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/taskmemo.py` & `xerparser-0.9.4/xerparser/schemas/taskmemo.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/taskpred.py` & `xerparser-0.9.4/xerparser/schemas/taskpred.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/taskrsrc.py` & `xerparser-0.9.4/xerparser/schemas/taskrsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/trsrcfin.py` & `xerparser-0.9.4/xerparser/schemas/trsrcfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/schemas/udftype.py` & `xerparser-0.9.4/xerparser/schemas/udftype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/scripts/dates.py` & `xerparser-0.9.4/xerparser/scripts/dates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/src/errors.py` & `xerparser-0.9.4/xerparser/src/errors.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/src/parser.py` & `xerparser-0.9.4/xerparser/src/parser.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/src/validators.py` & `xerparser-0.9.4/xerparser/src/validators.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/xerparser/src/xer.py` & `xerparser-0.9.4/xerparser/src/xer.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.3/setup.py` & `xerparser-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 entry_points = \
 {'console_scripts': ['calc_rem_hours_test = scripts:rem_hours_per_day_test',
                      'parse_test = scripts:parse_test',
                      'test = scripts:test']}
 
 setup_kwargs = {
     'name': 'xerparser',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Parse a P6 .xer file to a Python object.',
-    'long_description': '# xerparser\n\nA simple Python package that reads the contents of a P6 .xer file and converts it into a Python object.  \n\n*Disclaimers:  \nIt\'s helpfull if you are already familiar with the mapping and schemas used by P6 during the export process.\nRefer to the [Oracle Documentation]( https://docs.oracle.com/cd/F25600_01/English/Mapping_and_Schema/xer_import_export_data_map_project/index.htm) for more information regarding how data is mapped to the XER format.  \nTested on .xer files exported as versions 15.2 through 19.12.*  \n\n<br/>\n\n## Install\n\n**Windows**:\n\n```bash\npip install xerparser\n```\n\n**Linux/Mac**:\n\n```bash\npip3 install xerparser\n```\n\n<br/>  \n\n## Usage  \n\nImport the `Xer` class from `xerparser`  and pass the contents of a .xer file as an argument. Use the `Xer` class variable `CODEC` to set the proper encoding to decode the file.\n\n```python\nfrom xerparser import Xer\n\nfile = r"/path/to/file.xer"\nwith open(file, encoding=Xer.CODEC, errors="ignore") as f:\n    file_contents = f.read()\nxer = Xer(file_contents)\n```\n\nDo not pass the the .xer file directly as an argument to the `Xer` class. The file must be decoded and read into a string, which can then be passed as an argument. Or, pass the .xer file into the `Xer.reader` classmethod, which accepts:\n\n* str or pathlib.Path objects for files stored locally or on a server.\n* Binary files from requests, Flask, FastAPI, etc...\n\n```python\nfrom xerparser import Xer\n\nfile = r"/path/to/file.xer"\nxer = Xer.reader(file)\n```\n\n<br/>\n\n## Attributes\n\nThe tables stored in the .xer file are accessable as either Global, Project specific, Task specific, or Resource specific:\n\n### Global\n\n  ```python\n  xer.export_info           # export data\n  xer.activity_code_types   # dict of ACTVTYPE objects\n  xer.activity_code_values  # dict of ACTVCODE objects\n  xer.calendars             # dict of all CALENDAR objects\n  xer.financial_periods     # dict of FINDATES objects\n  xer.notebook_topics       # dict of MEMOTYPE objects\n  xer.projects              # dict of PROJECT objects\n  xer.project_code_types    # dict of PCATTYPE objects\n  xer.project_code_values   # dict of PCATVAL objects\n  xer.tasks                 # dict of all TASK objects\n  xer.relationships         # dict of all TASKPRED objects\n  xer.resources             # dict of RSRC objects\n  xer.udf_types             # dict of UDFTYPE objects\n  xer.wbs_nodes             # dict of all PROJWBS objects\n  ```  \n\n### Project Specific\n\n```python\n# Get first project\nproject = list(xer.projects.values())[0]\n\nproject.activity_codes        # list of project specific ACTVTYPE objects\nproject.calendars             # list of project specific CALENDAR objects\nproject.project_codes         # dict of PCATTYPE: PCATVAL objects\nproject.tasks                 # list of project specific TASK objects\nproject.relationships         # list of project specific TASKPRED objects\nproject.user_defined_fields   # dict of `UDFTYPE`: `UDF Value` pairs  \nproject.wbs_nodes             # list of project specific PROJWBS objects\n```\n\n### Task Specific\n\n```python\n# Get first task\ntask = project.tasks[0]\n\ntask.activity_codes       # dict of ACTVTYPE: ACTVCODE objects\ntask.memos                # list of TASKMEMO objects\ntask.periods              # list of TASKFIN objects\ntask.resources            # dict of TASKRSRC objects\ntask.user_defined_fields  # dict of `UDFTYPE`: `UDF Value` pairs \n```\n\n### Resource Specific\n\n```python\n# Get first task resource\nresource = list(task.resources.values())[0]\n\nresource.periods              # list of TRSRCFIN objects\nresource.user_defined_fields  # dict of `UDFTYPE`: `UDF Value` pairs \n```\n\n<br/>\n\n## Error Checking\n\nSometimes the xer file is corrupted during the export process. If this is the case, a `CorruptXerFile` Exception will be raised during initialization.  A list of the errors can be accessed from the `CorruptXerFile` Exception, or by using the `find_xer_errors` function.\n\n### Option 1 - `errors` attribute of `CorruptXerFile` exception  (preferred)\n```python\nfrom xerparser import Xer\n\nfile = r"/path/to/file.xer"\ntry:\n    xer = Xer.reader(file)\nexcept CorruptXerFile as e:\n    for error in e.errors:\n        print(error)\n```  \n\n### Option 2 - `find_xer_errors` function\n```python\nfrom xerparser import parser, file_reader, find_xer_errors\n\nfile = r"/path/to/file.xer"\nxer_data = parser(file_reader(file))\nfile_errors = find_xer_errors(xer_data)\nfor error in file_errors:\n    print(error)\n```\n\n### Errors\n\n- Minimum required tables - an error is recorded if one of the following tables is missing:\n  - CALENDAR\n  - PROJECT\n  - PROJWBS\n  - TASK\n  - TASKPRED  \n- Required table pairs - an error is recorded if Table 1 is included but not Table 2:  \n  \n  | Table 1       | Table 2       | Notes    |\n  | :----------- |:-------------|----------|\n  | TASKFIN | FINDATES | *Financial Period Data for Task* |\n  | TRSRCFIN | FINDATES | *Financial Period Data for Task Resource* |\n  | TASKRSRC | RSRC | *Resource Data* |\n  | TASKMEMO | MEMOTYPE | *Notebook Data* |\n  | ACTVCODE | ACTVTYPE | *Activity Code Data* |\n  | TASKACTV | ACTVCODE | *Activity Code Data* |\n  | PCATVAL | PCATTYPE | *Project Code Data* |\n  | PROJPCAT | PCATVAL | *Project Code Data* |\n  | UDFVALUE | UDFTYPE | *User Defined Field Data* |\n\n- Non-existent calendars assigned to tasks.\n- Non-existent resources assigned to task resources.\n',
+    'long_description': '# xerparser\n\nRead the contents of a P6 .xer file and convert it into a Python object.  \n\n*Disclaimers:  \nIt\'s helpfull if you are already familiar with the mapping and schemas used by P6 during the export process.\nRefer to the [Oracle Documentation]( https://docs.oracle.com/cd/F25600_01/English/Mapping_and_Schema/xer_import_export_data_map_project/index.htm) for more information regarding how data is mapped to the XER format.  \nTested on .xer files exported as versions 15.2 through 19.12.*  \n\n<br/>\n\n## Install\n\n**Windows**:\n\n```bash\npip install xerparser\n```\n\n**Linux/Mac**:\n\n```bash\npip3 install xerparser\n```\n\n<br/>  \n\n## Usage  \n\nImport the `Xer` class from `xerparser`  and pass the contents of a .xer file as an argument. Use the `Xer` class variable `CODEC` to set the proper encoding to decode the file.\n\n```python\nfrom xerparser import Xer\n\nfile = r"/path/to/file.xer"\nwith open(file, encoding=Xer.CODEC, errors="ignore") as f:\n    file_contents = f.read()\nxer = Xer(file_contents)\n```\n\nDo not pass the the .xer file directly as an argument to the `Xer` class. The file must be decoded and read into a string, which can then be passed as an argument. Or, pass the .xer file into the `Xer.reader` classmethod, which accepts:\n\n* str or pathlib.Path objects for files stored locally or on a server.\n* Binary files from requests, Flask, FastAPI, etc...\n\n```python\nfrom xerparser import Xer\n\nfile = r"/path/to/file.xer"\nxer = Xer.reader(file)\n```\n\n<br/>\n\n## Attributes\n\nThe tables stored in the .xer file are accessable as either Global, Project specific, Task specific, or Resource specific:\n\n### Global\n\n  ```python\n  xer.export_info           # export data\n  xer.activity_code_types   # dict of ACTVTYPE objects\n  xer.activity_code_values  # dict of ACTVCODE objects\n  xer.calendars             # dict of all CALENDAR objects\n  xer.financial_periods     # dict of FINDATES objects\n  xer.notebook_topics       # dict of MEMOTYPE objects\n  xer.projects              # dict of PROJECT objects\n  xer.project_code_types    # dict of PCATTYPE objects\n  xer.project_code_values   # dict of PCATVAL objects\n  xer.tasks                 # dict of all TASK objects\n  xer.relationships         # dict of all TASKPRED objects\n  xer.resources             # dict of RSRC objects\n  xer.udf_types             # dict of UDFTYPE objects\n  xer.wbs_nodes             # dict of all PROJWBS objects\n  ```  \n\n### Project Specific\n\n```python\n# Get first project\nproject = list(xer.projects.values())[0]\n\nproject.activity_codes        # list of project specific ACTVTYPE objects\nproject.calendars             # list of project specific CALENDAR objects\nproject.project_codes         # dict of PCATTYPE: PCATVAL objects\nproject.tasks                 # list of project specific TASK objects\nproject.relationships         # list of project specific TASKPRED objects\nproject.user_defined_fields   # dict of `UDFTYPE`: `UDF Value` pairs  \nproject.wbs_nodes             # list of project specific PROJWBS objects\n```\n\n### Task Specific\n\n```python\n# Get first task\ntask = project.tasks[0]\n\ntask.activity_codes       # dict of ACTVTYPE: ACTVCODE objects\ntask.memos                # list of TASKMEMO objects\ntask.periods              # list of TASKFIN objects\ntask.resources            # dict of TASKRSRC objects\ntask.user_defined_fields  # dict of `UDFTYPE`: `UDF Value` pairs \n```\n\n### Resource Specific\n\n```python\n# Get first task resource\nresource = list(task.resources.values())[0]\n\nresource.periods              # list of TRSRCFIN objects\nresource.user_defined_fields  # dict of `UDFTYPE`: `UDF Value` pairs \n```\n\n<br/>\n\n## Error Checking\n\nSometimes the xer file is corrupted during the export process. If this is the case, a `CorruptXerFile` Exception will be raised during initialization.  A list of the errors can be accessed from the `CorruptXerFile` Exception, or by using the `find_xer_errors` function.\n\n### Option 1 - `errors` attribute of `CorruptXerFile` exception  (preferred)\n```python\nfrom xerparser import Xer, CorruptXerFile\n\nfile = r"/path/to/file.xer"\ntry:\n    xer = Xer.reader(file)\nexcept CorruptXerFile as e:\n    for error in e.errors:\n        print(error)\n```  \n\n### Option 2 - `find_xer_errors` function\n```python\nfrom xerparser import parser, file_reader, find_xer_errors\n\nfile = r"/path/to/file.xer"\nxer_data = parser(file_reader(file))\nfile_errors = find_xer_errors(xer_data)\nfor error in file_errors:\n    print(error)\n```\n\n### Errors\n\n- Minimum required tables - an error is recorded if one of the following tables is missing:\n  - CALENDAR\n  - PROJECT\n  - PROJWBS\n  - TASK\n  - TASKPRED  \n- Required table pairs - an error is recorded if Table 1 is included but not Table 2:  \n  \n  | Table 1       | Table 2       | Notes    |\n  | :----------- |:-------------|----------|\n  | TASKFIN | FINDATES | *Financial Period Data for Task* |\n  | TRSRCFIN | FINDATES | *Financial Period Data for Task Resource* |\n  | TASKRSRC | RSRC | *Resource Data* |\n  | TASKMEMO | MEMOTYPE | *Notebook Data* |\n  | ACTVCODE | ACTVTYPE | *Activity Code Data* |\n  | TASKACTV | ACTVCODE | *Activity Code Data* |\n  | PCATVAL | PCATTYPE | *Project Code Data* |\n  | PROJPCAT | PCATVAL | *Project Code Data* |\n  | UDFVALUE | UDFTYPE | *User Defined Field Data* |\n\n- Non-existent calendars assigned to tasks.\n- Non-existent resources assigned to task resources.\n',
     'author': 'Jesse',
     'author_email': 'code@seqmanagement.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jjCode01/xerparser',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `xerparser-0.9.3/PKG-INFO` & `xerparser-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerparser
-Version: 0.9.3
+Version: 0.9.4
 Summary: Parse a P6 .xer file to a Python object.
 Home-page: https://github.com/jjCode01/xerparser
 License: GPL-3.0-only
 Keywords: primavera,p6,xer,schedule,scheduling,planning,project management,project controls
 Author: Jesse
 Author-email: code@seqmanagement.com
 Requires-Python: >=3.10,<4.0
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: html-sanitizer (>=1.9.3,<2.0.0)
 Project-URL: Repository, https://github.com/jjCode01/xerparser
 Description-Content-Type: text/markdown
 
 # xerparser
 
-A simple Python package that reads the contents of a P6 .xer file and converts it into a Python object.  
+Read the contents of a P6 .xer file and convert it into a Python object.  
 
 *Disclaimers:  
 It's helpfull if you are already familiar with the mapping and schemas used by P6 during the export process.
 Refer to the [Oracle Documentation]( https://docs.oracle.com/cd/F25600_01/English/Mapping_and_Schema/xer_import_export_data_map_project/index.htm) for more information regarding how data is mapped to the XER format.  
 Tested on .xer files exported as versions 15.2 through 19.12.*  
 
 <br/>
@@ -135,15 +135,15 @@
 
 ## Error Checking
 
 Sometimes the xer file is corrupted during the export process. If this is the case, a `CorruptXerFile` Exception will be raised during initialization.  A list of the errors can be accessed from the `CorruptXerFile` Exception, or by using the `find_xer_errors` function.
 
 ### Option 1 - `errors` attribute of `CorruptXerFile` exception  (preferred)
 ```python
-from xerparser import Xer
+from xerparser import Xer, CorruptXerFile
 
 file = r"/path/to/file.xer"
 try:
     xer = Xer.reader(file)
 except CorruptXerFile as e:
     for error in e.errors:
         print(error)
```


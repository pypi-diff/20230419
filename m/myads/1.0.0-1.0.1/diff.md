# Comparing `tmp/myads-1.0.0.tar.gz` & `tmp/myads-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myads-1.0.0.tar", last modified: Sun Apr  2 10:01:39 2023, max compression
+gzip compressed data, was "myads-1.0.1.tar", last modified: Wed Apr 19 21:51:55 2023, max compression
```

## Comparing `myads-1.0.0.tar` & `myads-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-02 10:01:39.204215 myads-1.0.0/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4442 2023-04-02 10:01:39.204215 myads-1.0.0/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4082 2023-04-02 09:58:52.000000 myads-1.0.0/README.md
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      732 2023-04-02 09:59:21.000000 myads-1.0.0/pyproject.toml
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-04-02 10:01:39.204215 myads-1.0.0/setup.cfg
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-02 10:01:39.200215 myads-1.0.0/src/
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-02 10:01:39.200215 myads-1.0.0/src/myads/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      769 2023-03-12 18:51:04.000000 myads-1.0.0/src/myads/__init__.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-02 10:01:39.204215 myads-1.0.0/src/myads/cite_tracker/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      595 2023-03-26 17:34:24.000000 myads-1.0.0/src/myads/cite_tracker/__init__.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     5989 2023-04-02 09:41:10.000000 myads-1.0.0/src/myads/cite_tracker/check.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2277 2023-04-02 09:39:57.000000 myads-1.0.0/src/myads/cite_tracker/report.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3256 2023-03-26 17:39:40.000000 myads-1.0.0/src/myads/cite_tracker/users.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     9849 2023-04-02 09:39:56.000000 myads-1.0.0/src/myads/query.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-02 10:01:39.204215 myads-1.0.0/src/myads/scripts/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     1684 2023-04-02 09:41:52.000000 myads-1.0.0/src/myads/scripts/myads.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-02 10:01:39.200215 myads-1.0.0/src/myads.egg-info/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4442 2023-04-02 10:01:39.000000 myads-1.0.0/src/myads.egg-info/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      424 2023-04-02 10:01:39.000000 myads-1.0.0/src/myads.egg-info/SOURCES.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-04-02 10:01:39.000000 myads-1.0.0/src/myads.egg-info/dependency_links.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-04-02 10:01:39.000000 myads-1.0.0/src/myads.egg-info/entry_points.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-04-02 10:01:39.000000 myads-1.0.0/src/myads.egg-info/requires.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-04-02 10:01:39.000000 myads-1.0.0/src/myads.egg-info/top_level.txt
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4612 2023-04-19 21:51:55.989712 myads-1.0.1/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4252 2023-04-19 21:50:51.000000 myads-1.0.1/README.md
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      732 2023-04-19 21:50:17.000000 myads-1.0.1/pyproject.toml
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-04-19 21:51:55.989712 myads-1.0.1/setup.cfg
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      769 2023-03-12 18:51:04.000000 myads-1.0.1/src/myads/__init__.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads/cite_tracker/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      595 2023-03-26 17:34:24.000000 myads-1.0.1/src/myads/cite_tracker/__init__.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     6611 2023-04-19 21:48:51.000000 myads-1.0.1/src/myads/cite_tracker/check.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2276 2023-04-19 21:46:53.000000 myads-1.0.1/src/myads/cite_tracker/report.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3256 2023-03-26 17:39:40.000000 myads-1.0.1/src/myads/cite_tracker/users.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     9957 2023-04-19 21:46:45.000000 myads-1.0.1/src/myads/query.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads/scripts/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     1684 2023-04-02 09:41:52.000000 myads-1.0.1/src/myads/scripts/myads.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-04-19 21:51:55.989712 myads-1.0.1/src/myads.egg-info/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4612 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      424 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/entry_points.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/requires.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-04-19 21:51:55.000000 myads-1.0.1/src/myads.egg-info/top_level.txt
```

### Comparing `myads-1.0.0/PKG-INFO` & `myads-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-Metadata-Version: 2.1
-Name: myads
-Version: 1.0.0
-Summary: Simple ADS API query package and citation tracker
-Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
-License: BSD 3-Clause License
-Keywords: nasa-ads,citations,astronomy,ads,python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+[![PyPI version](https://badge.fury.io/py/myads.svg)](https://badge.fury.io/py/myads)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/myads?logo=python)
 
 # myADS
 
 `myADS` is a simple package to keep track of citations to your (and other
 authors) papers.
 
 It both reports your current papers citation metrics, and
```

### Comparing `myads-1.0.0/README.md` & `myads-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: myads
+Version: 1.0.1
+Summary: Simple ADS API query package and citation tracker
+Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
+License: BSD 3-Clause License
+Keywords: nasa-ads,citations,astronomy,ads,python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+[![PyPI version](https://badge.fury.io/py/myads.svg)](https://badge.fury.io/py/myads)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/myads?logo=python)
+
 # myADS
 
 `myADS` is a simple package to keep track of citations to your (and other
 authors) papers.
 
 It both reports your current papers citation metrics, and
 checks for any new cites to your papers since the last time of checking.
```

### Comparing `myads-1.0.0/pyproject.toml` & `myads-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 dependencies = [
     'requests',
     'toml',
     'tabulate>=0.9.0'
 ]
 requires-python = ">=3.7"
-version = "1.0.0"
+version = "1.0.1"
 keywords = ["nasa-ads", "citations", "astronomy", "ads", "python"]
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 
 [project.scripts]
 myads = "myads.scripts.myads:main"
```

### Comparing `myads-1.0.0/src/myads/__init__.py` & `myads-1.0.1/src/myads/__init__.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.0/src/myads/cite_tracker/__init__.py` & `myads-1.0.1/src/myads/cite_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.0/src/myads/cite_tracker/check.py` & `myads-1.0.1/src/myads/cite_tracker/check.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 import toml
 from myads.query import ADSQueryWrapper
 from tabulate import tabulate
 
 
 def _refresh_database(data, query) -> dict:
     """
-    Get the most up-to-date cites to our papers.
+    Get the most up-to-date cites to the users' papers.
+
+    Parameters
+    ----------
+    data : 
+    query : ADSQueryWrapper object
 
     Returns
     -------
     database : dict
-        Details the up-to-date cites of our papers
-    query : ADSQueryWrapper object
+        Details the up-to-date cites of the users' papers
     """
 
     database = {}
 
     for paper in data.papers:
         tmp = query.citations(paper.bibcode)
         database[paper.bibcode] = {}
@@ -53,43 +57,52 @@
 
         if len(new) > 0:
 
             # Print new cites.
             print(
                 "\n",
                 f"{BOLD}{OKCYAN}{len(new)} new cite(s) for "
-                f"{database[bibcode]['title'][0]}{ENDC}",
+                f"{database[bibcode]['title']}{ENDC}",
             )
             table = []
             for paper in new:
                 table.append(
-                    [paper.title[0], paper.author, paper.date[:10], paper.link,]
+                    [paper.title, paper.author, paper.date[:10], paper.link,]
                 )
 
             print(
                 tabulate(
                     table,
                     tablefmt="grid",
                     maxcolwidths=[40, 40, None, 20],
                     headers=["Title", "Authors", "Date", "Bibcode"],
                 )
             )
 
 
 def _save_database(path, data):
-    """ Save the user database. """
+    """
+    Save the users cite database.
+
+    Parameters
+    ----------
+    path : str
+        Path to user database file
+    data : dict
+        Users' cite information
+    """
 
     with open(path, "w") as f:
         toml.dump(data, f)
 
 
 def check(verbose):
     """
-    Check against our personal database to see if there are any new cites to
-    our papers since the last call.
+    Check against each users' personal database to see if there are any new
+    cites to their papers since the last call.
 
     Parameters
     ----------
     verbose : bool  
         True for more output
     """
 
@@ -111,48 +124,58 @@
         FIRST_NAME = users[att]["first_name"]
         LAST_NAME = users[att]["last_name"]
         ORCID = users[att]["orcid"]
         print(f"\nChecking new cites for {FIRST_NAME} {LAST_NAME}...")
 
         # Query.
         if ORCID == "":
+            # Query just by first name last name.
             data = query.get(
                 q=f"first_author:{LAST_NAME},{FIRST_NAME}",
                 fl="title,citation_count,pubdate,bibcode",
             )
         else:
+            # Query also using the ORCID.
             q = (
                 f"orcid_pub:{ORCID} OR orcid_user:{ORCID} OR orcid_other:{ORCID} "
                 f"first_author:{LAST_NAME},{FIRST_NAME}"
             )
             data = query.get(q=q, fl="title,citation_count,pubdate,bibcode")
 
-        # Got a bad status code.
+        # Got a bad status code?
         if data is None:
             return
 
         if len(data.papers) == 0:
             print(f"No paper hits for {FIRST_NAME} {LAST_NAME}")
             continue
 
         # To store new cites.
         new_cite_list = {}
+        brand_new_paper = False
 
-        # Path to users database.
+        # Path to this users' database.
         user_database = cite_tracker.get_user_database_path(att)
 
-        # Does the user already have a database?
+        # Does this user already have a database?
         if os.path.isfile(user_database):
             # Load existing database.
             database = toml.load(user_database)
 
-            # Is there a new paper since last time thats not in the database?
-            for bibcode in data.get_all("bibcode"):
-                if bibcode not in database.keys():
-                    raise NotImplementedError(f"New paper {bibcode}, implement this")
+            # Is there a new paper for this user that's not in the database?
+            for tmp_paper in data.papers:
+                if tmp_paper.bibcode not in database.keys():
+                    brand_new_paper = True
+                    print(
+                        f"New paper for {FIRST_NAME} {LAST_NAME} ({bibcode})",
+                        f"adding to database...",
+                    )
+
+                    # Add new entry to database.
+                    database[bibcode] = {"title": tmp_paper.title, "citations": []}
 
             new_entry = False
 
             # Loop over each paper in database.
             for bibcode in database.keys():
                 if verbose:
                     print(f"Checking {bibcode}...")
@@ -181,15 +204,15 @@
                 # Update database.
                 database[bibcode]["citations"] = tmp_query_data.get_all("bibcode")
 
             # Report new cites.
             _print_new_cites(database, new_cite_list)
 
             # Update database with new entries.
-            if new_entry:
+            if new_entry or brand_new_paper:
                 _save_database(user_database, database)
             else:
                 print(f"No new cites for {FIRST_NAME} {LAST_NAME}")
         else:
             # Create new database (first time run).
             print(
                 f"First time run for {FIRST_NAME} {LAST_NAME}, "
```

### Comparing `myads-1.0.0/src/myads/cite_tracker/report.py` & `myads-1.0.1/src/myads/cite_tracker/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         FIRST_NAME = users[att]["first_name"]
         LAST_NAME = users[att]["last_name"]
         ORCID = users[att]["orcid"]
         print(f"\nReporting cites for {FIRST_NAME} {LAST_NAME}...")
 
         # Query.
         if ORCID == "":
-            q=f"first_author:{LAST_NAME},{FIRST_NAME}"
+            q = f"first_author:{LAST_NAME},{FIRST_NAME}"
         else:
             q = (
                 f"orcid_pub:{ORCID} OR orcid_user:{ORCID} OR orcid_other:{ORCID} "
                 f"first_author:{LAST_NAME},{FIRST_NAME}"
             )
 
         data = query.get(q=q, fl="title,citation_count,pubdate,bibcode")
@@ -52,15 +52,15 @@
             continue
 
         # Loop over each of my papers and print the number of cites.
         table = []
         for paper in data.papers:
             table.append(
                 [
-                    paper.title[0],
+                    paper.title,
                     f"{paper.citation_count} ({paper.citations_per_year:.1f})",
                     paper.pubdate,
                     paper.link,
                 ]
             )
 
         print(
```

### Comparing `myads-1.0.0/src/myads/cite_tracker/users.py` & `myads-1.0.1/src/myads/cite_tracker/users.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.0/src/myads/query.py` & `myads-1.0.1/src/myads/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         ----------
         paper_info : dict
             Data returned from the query for this paper
         """
 
         # Insert query data into this object.
         for att in paper_info.keys():
-            setattr(self, att, paper_info[att])
+            if att == "title":
+                setattr(self, att, paper_info[att][0])
+            else:
+                setattr(self, att, paper_info[att])
 
     def get_years_since_publication(self) -> float:
         """
         Return the number of years since publication for this paper.
 
         Requires to of had "pubdate" in the original query.
```

### Comparing `myads-1.0.0/src/myads/scripts/myads.py` & `myads-1.0.1/src/myads/scripts/myads.py`

 * *Files identical despite different names*

### Comparing `myads-1.0.0/src/myads.egg-info/PKG-INFO` & `myads-1.0.1/src/myads.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: myads
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple ADS API query package and citation tracker
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
 Keywords: nasa-ads,citations,astronomy,ads,python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/myads.svg)](https://badge.fury.io/py/myads)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/myads?logo=python)
+
 # myADS
 
 `myADS` is a simple package to keep track of citations to your (and other
 authors) papers.
 
 It both reports your current papers citation metrics, and
 checks for any new cites to your papers since the last time of checking.
```


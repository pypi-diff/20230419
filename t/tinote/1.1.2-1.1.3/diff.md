# Comparing `tmp/tinote-1.1.2.tar.gz` & `tmp/tinote-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-1.1.2.tar", last modified: Tue Apr 18 21:54:28 2023, max compression
+gzip compressed data, was "tinote-1.1.3.tar", last modified: Tue Apr 18 22:28:43 2023, max compression
```

## Comparing `tinote-1.1.2.tar` & `tinote-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:28.104280 tinote-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-18 21:54:28.104280 tinote-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-18 21:54:16.000000 tinote-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:54:28.104280 tinote-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 21:54:16.000000 tinote-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:28.104280 tinote-1.1.2/tinote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:16.000000 tinote-1.1.2/tinote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-18 21:54:16.000000 tinote-1.1.2/tinote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-18 21:54:16.000000 tinote-1.1.2/tinote/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:28.104280 tinote-1.1.2/tinote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:43.364165 tinote-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-18 22:28:43.364165 tinote-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-18 22:28:32.000000 tinote-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:28:43.364165 tinote-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 22:28:32.000000 tinote-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:43.364165 tinote-1.1.3/tinote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:32.000000 tinote-1.1.3/tinote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-18 22:28:32.000000 tinote-1.1.3/tinote/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-18 22:28:32.000000 tinote-1.1.3/tinote/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:43.364165 tinote-1.1.3/tinote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-18 22:28:43.000000 tinote-1.1.3/tinote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 22:28:43.000000 tinote-1.1.3/tinote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:28:43.000000 tinote-1.1.3/tinote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 22:28:43.000000 tinote-1.1.3/tinote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 22:28:43.000000 tinote-1.1.3/tinote.egg-info/top_level.txt
```

### Comparing `tinote-1.1.2/PKG-INFO` & `tinote-1.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.1.2
+Version: 1.1.3
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
+## No Thought Left Behind.
+
+#### Huh, that's a pretty good idea. I should write that down. 
+
+###### [proceeds to lose the paper]
+
+#### Wow, I should write down that task for later in Notepad!
+
+###### [proceeds not to save the file before computer restarts that night]
+
+#### Ugh.
+
 Tinote is light-weight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
+###### (made entirely for myself, but feel free to use it and contribute!)
+
 ## Installation
 
 Install Tinote using pip:
 
 ```bash
 pip install tinote
 ```
@@ -38,21 +52,34 @@
 ```bash
 ti add "a note to remember" <optional category> <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
 ```bash
-ti list [-v]
+ti list
+```
+
+```output
+IDEAS---------------------------------------------------------------------------
+[ ] 55 A dating app, but for hamster-owners ONLY
+[✔] 58 A sushi company that sell BEEF sushi! :O
+
+VAN-STUFF-----------------------------------------------------------------------
+[✔] 55 Fix the latch for the fridge
+[ ] 58 Install Solar
+    [ ] 60 Install roof-rack, hopefully easy
+    [ ] 61 Attach panels
+    [ ] 62 Run wiring
 ```
 
-List notes with filters (category or importance):
+List notes with filters (category or importance or marked) or higher verbosity:
 
 ```bash
-ti list -c <category> -i <importance>
+ti list -c <category> -i <importance> -m <is marked> -v
 ```
 
 Add a sub-note to a note (currently only supports one level)
 
 ```bash
 ti sub <parent_id> "Text of your sub-note" -i <importance>
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tinote-1.1.2/README.md` & `tinote-1.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 ![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
+## No Thought Left Behind.
+
+#### Huh, that's a pretty good idea. I should write that down. 
+
+###### [proceeds to lose the paper]
+
+#### Wow, I should write down that task for later in Notepad!
+
+###### [proceeds not to save the file before computer restarts that night]
+
+#### Ugh.
+
 Tinote is light-weight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
+###### (made entirely for myself, but feel free to use it and contribute!)
+
 ## Installation
 
 Install Tinote using pip:
 
 ```bash
 pip install tinote
 ```
@@ -17,21 +31,34 @@
 ```bash
 ti add "a note to remember" <optional category> <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
 ```bash
-ti list [-v]
+ti list
+```
+
+```output
+IDEAS---------------------------------------------------------------------------
+[ ] 55 A dating app, but for hamster-owners ONLY
+[✔] 58 A sushi company that sell BEEF sushi! :O
+
+VAN-STUFF-----------------------------------------------------------------------
+[✔] 55 Fix the latch for the fridge
+[ ] 58 Install Solar
+    [ ] 60 Install roof-rack, hopefully easy
+    [ ] 61 Attach panels
+    [ ] 62 Run wiring
 ```
 
-List notes with filters (category or importance):
+List notes with filters (category or importance or marked) or higher verbosity:
 
 ```bash
-ti list -c <category> -i <importance>
+ti list -c <category> -i <importance> -m <is marked> -v
 ```
 
 Add a sub-note to a note (currently only supports one level)
 
 ```bash
 ti sub <parent_id> "Text of your sub-note" -i <importance>
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tinote-1.1.2/setup.py` & `tinote-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `tinote-1.1.2/tinote/main.py` & `tinote-1.1.3/tinote/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,28 +88,31 @@
 def format_note(note_text, sub=False):
     bullet_indent = "\t\t" if sub else "\t"
     lines = note_text.split("*")
     formatted_lines = [lines[0]] + [f"{bullet_indent}* {line.strip()}" for line in lines[1:]]
     return "\n".join(formatted_lines)
 
 
-def list_notes(category=None, importance=None, verbose=None):
+def list_notes(category=None, importance=None, verbose=None, marked=None):
     notes, _, _ = load_notes()
 
     if not category:
         sorted_notes = sorted(notes, key=lambda x: x['category'])
     else:
         sorted_notes = [note for note in notes if note['category'] == category]
 
     def display_notes(notes_list, indent=0):
         for note in notes_list:
             if importance and note["importance"] != importance:
                 continue
 
-            checked_symbol = "✔" if note["checked"] else "✘"
+            if marked is not None and note["checked"] != marked:
+                continue
+
+            checked_symbol = "[✔]" if note["checked"] else "[ ]"
             importance_symbol = f"[{note['importance']}]" if note["importance"] is not None and verbose else ""
             created_timestamp = f'(Created {note["created_timestamp"]})' if verbose else ""
             marked_timestamp = f'(Mark Updated {note["marked_timestamp"]})' if verbose and note["marked_timestamp"] is not None else ""
 
             lines = textwrap.wrap(note['note'], width=80 - indent)
             first_line = lines.pop(0)
 
@@ -218,14 +221,15 @@
     # Add subparser for 'list' command
     list_parser = subparsers.add_parser("list", help="List all notes.")
     list_parser.add_argument("-c", "--category", type=str, default=None, help="List notes from a specific category.")
     list_parser.add_argument("-i", "--importance", type=int, default=None,
                              help="List notes with a specific importance level.")
     list_parser.add_argument("-v", "--verbose", action="store_true",
                              help="Show importance and timestamp with each note.")
+    list_parser.add_argument("-m", "--marked", type=bool, default=None, help="Filter on marked (no filter by default, true or false for marked/unmarked)")
 
     mark_parser = subparsers.add_parser("mark", help="Mark a note as checked or unchecked.")
     mark_parser.add_argument("id", type=int, help="The ID of the note to mark.")
     mark_parser.add_argument("-u", "--uncheck", action="store_true", help="Unmark the note instead of marking it.")
 
     delete_parser = subparsers.add_parser("delete", help="Delete a note.")
     delete_parser.add_argument("id", type=int, help="The ID of the note to delete.")
@@ -236,15 +240,15 @@
     args = parser.parse_args()
 
     if args.subcommand == "add":
         category = args.category_keyword if args.category_keyword is not None else args.category
         importance = args.importance_keyword if args.importance_keyword is not None else args.importance
         create_note(args.note, category, importance)
     elif args.subcommand == "list":
-        list_notes(args.category, args.importance, args.verbose)
+        list_notes(args.category, args.importance, args.verbose, args.marked)
     elif args.subcommand == "mark":
         mark_note(args.id, not args.uncheck)
     elif args.subcommand == "delete":
         delete_note(args.id)
     elif args.subcommand == 'clear':
         clear_notes(args.category)
     elif args.subcommand == 'sub':
```

### Comparing `tinote-1.1.2/tinote/update.py` & `tinote-1.1.3/tinote/update.py`

 * *Files identical despite different names*

### Comparing `tinote-1.1.2/tinote.egg-info/PKG-INFO` & `tinote-1.1.3/tinote.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.1.2
+Version: 1.1.3
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
+## No Thought Left Behind.
+
+#### Huh, that's a pretty good idea. I should write that down. 
+
+###### [proceeds to lose the paper]
+
+#### Wow, I should write down that task for later in Notepad!
+
+###### [proceeds not to save the file before computer restarts that night]
+
+#### Ugh.
+
 Tinote is light-weight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
+###### (made entirely for myself, but feel free to use it and contribute!)
+
 ## Installation
 
 Install Tinote using pip:
 
 ```bash
 pip install tinote
 ```
@@ -38,21 +52,34 @@
 ```bash
 ti add "a note to remember" <optional category> <optional importance>
 ```
 
 List all notes (verbose list will include importance and timestamp):
 
 ```bash
-ti list [-v]
+ti list
+```
+
+```output
+IDEAS---------------------------------------------------------------------------
+[ ] 55 A dating app, but for hamster-owners ONLY
+[✔] 58 A sushi company that sell BEEF sushi! :O
+
+VAN-STUFF-----------------------------------------------------------------------
+[✔] 55 Fix the latch for the fridge
+[ ] 58 Install Solar
+    [ ] 60 Install roof-rack, hopefully easy
+    [ ] 61 Attach panels
+    [ ] 62 Run wiring
 ```
 
-List notes with filters (category or importance):
+List notes with filters (category or importance or marked) or higher verbosity:
 
 ```bash
-ti list -c <category> -i <importance>
+ti list -c <category> -i <importance> -m <is marked> -v
 ```
 
 Add a sub-note to a note (currently only supports one level)
 
 ```bash
 ti sub <parent_id> "Text of your sub-note" -i <importance>
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


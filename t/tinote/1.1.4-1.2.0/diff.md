# Comparing `tmp/tinote-1.1.4.tar.gz` & `tmp/tinote-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-1.1.4.tar", last modified: Tue Apr 18 22:39:36 2023, max compression
+gzip compressed data, was "tinote-1.2.0.tar", last modified: Wed Apr 19 04:02:16 2023, max compression
```

## Comparing `tinote-1.1.4.tar` & `tinote-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:39:36.546078 tinote-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-18 22:39:36.546078 tinote-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-18 22:39:25.000000 tinote-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:39:36.546078 tinote-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 22:39:25.000000 tinote-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:39:36.546078 tinote-1.1.4/tinote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:39:25.000000 tinote-1.1.4/tinote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-18 22:39:25.000000 tinote-1.1.4/tinote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-18 22:39:25.000000 tinote-1.1.4/tinote/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:39:36.546078 tinote-1.1.4/tinote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-18 22:39:36.000000 tinote-1.1.4/tinote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 22:39:36.000000 tinote-1.1.4/tinote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:39:36.000000 tinote-1.1.4/tinote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 22:39:36.000000 tinote-1.1.4/tinote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 22:39:36.000000 tinote-1.1.4/tinote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:16.224665 tinote-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-19 04:02:16.224665 tinote-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-19 04:02:05.000000 tinote-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 04:02:16.224665 tinote-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-19 04:02:05.000000 tinote-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:16.224665 tinote-1.2.0/tinote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:05.000000 tinote-1.2.0/tinote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-19 04:02:05.000000 tinote-1.2.0/tinote/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-19 04:02:05.000000 tinote-1.2.0/tinote/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:02:16.224665 tinote-1.2.0/tinote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 04:02:16.000000 tinote-1.2.0/tinote.egg-info/top_level.txt
```

### Comparing `tinote-1.1.4/PKG-INFO` & `tinote-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.1.4
+Version: 1.2.0
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -64,37 +64,40 @@
 [ ] 55 A dating app, but for hamster-owners ONLY
 [✔] 58 A sushi company that sell BEEF sushi! :O
 
 VAN-STUFF-----------------------------------------------------------------------
 [✔] 55 Fix the latch for the fridge
 [ ] 58 Install Solar
     [ ] 60 Install roof-rack, hopefully easy
+        * How hard could it be
+        * Hahaha
     [ ] 61 Attach panels
     [ ] 62 Run wiring
 ```
+As you can see, using * in a message (no newline necessary) will cause that to be indented on the next line down.
 
 List notes with filters (category or importance or marked) or higher verbosity:
 
 ```bash
 ti list -c <category> -i <importance> -m -u -v
 ```
 
-Add a sub-note to a note (currently only supports one level)
+Add a sub-note to a note (can be as recursive as you can dream)
 
 ```bash
 ti sub <parent_id> "Text of your sub-note" -i <importance>
 ```
 
-Mark a note as checked/unchecked:
+Mark a note as checked/unchecked (-u indicates to unmark):
 
 ```bash
-ti mark <note_id>
+ti mark <note_id> -u 
 ```
 
-Delete a note:
+Delete a note (deletes all children notes):
 
 ```bash
 ti delete <note_id>
 ```
 
 Clear all notes or notes within a specified category:
```

### Comparing `tinote-1.1.4/README.md` & `tinote-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -43,37 +43,40 @@
 [ ] 55 A dating app, but for hamster-owners ONLY
 [✔] 58 A sushi company that sell BEEF sushi! :O
 
 VAN-STUFF-----------------------------------------------------------------------
 [✔] 55 Fix the latch for the fridge
 [ ] 58 Install Solar
     [ ] 60 Install roof-rack, hopefully easy
+        * How hard could it be
+        * Hahaha
     [ ] 61 Attach panels
     [ ] 62 Run wiring
 ```
+As you can see, using * in a message (no newline necessary) will cause that to be indented on the next line down.
 
 List notes with filters (category or importance or marked) or higher verbosity:
 
 ```bash
 ti list -c <category> -i <importance> -m -u -v
 ```
 
-Add a sub-note to a note (currently only supports one level)
+Add a sub-note to a note (can be as recursive as you can dream)
 
 ```bash
 ti sub <parent_id> "Text of your sub-note" -i <importance>
 ```
 
-Mark a note as checked/unchecked:
+Mark a note as checked/unchecked (-u indicates to unmark):
 
 ```bash
-ti mark <note_id>
+ti mark <note_id> -u 
 ```
 
-Delete a note:
+Delete a note (deletes all children notes):
 
 ```bash
 ti delete <note_id>
 ```
 
 Clear all notes or notes within a specified category:
```

### Comparing `tinote-1.1.4/setup.py` & `tinote-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tinote-1.1.4/tinote/main.py` & `tinote-1.2.0/tinote/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,49 +48,54 @@
     notes.append(new_note)
     save_notes(notes, new_id, category)  # Update max_id
 
     print("Note added successfully.")
 
 
 def create_sub_note(note, parent_id, importance):
-    notes, max_id, last_category = load_notes()
-
-    for n in notes:
-        if n["id"] == parent_id:
-            parent_note = n
-            break
-    else:
-        print("Parent does not exist.")
-        return
-
+    all_notes, max_id, last_category = load_notes()
     new_id = max_id + 1
 
-    new_note = {
-        "id": new_id,  # Use the new ID
-        "parent": parent_id,
-        "note": note,
-        "category": parent_note["category"],
-        "importance": importance,
-        "created_timestamp": datetime.now().isoformat(),
-        "marked_timestamp": None,
-        "checked": False,
-    }
-
-    try:
-        parent_note["subs"].append(new_note)
-    except KeyError:
-        parent_note["subs"] = [new_note]
-
-    save_notes(notes, new_id, last_category)
-
-    print("Sub-note added successfully.")
+    def find_and_add_sub_note(notes):
+        for n in notes:
+            if n["id"] == parent_id:
+                parent_note = n
+                break
+            elif find_and_add_sub_note(n["subs"]):
+                return True
+        else:
+            return False
+
+        new_note = {
+            "id": new_id,
+            "parent": parent_id,
+            "note": note,
+            "category": parent_note["category"],
+            "importance": importance,
+            "created_timestamp": datetime.now().isoformat(),
+            "marked_timestamp": None,
+            "subs": [],
+            "checked": False,
+        }
+
+        try:
+            parent_note["subs"].append(new_note)
+        except KeyError:
+            parent_note["subs"] = [new_note]
+        return True
+
+    if find_and_add_sub_note(all_notes):
+        save_notes(all_notes, new_id, last_category)
+        print("Sub-note added successfully.")
+    else:
+        print("Parent id does not exist.")
 
 
-def format_note(note_text, sub=False):
-    bullet_indent = "\t\t" if sub else "\t"
+def format_note(note_text, indent):
+    bullet_indent = (indent * " ") + "\t"
     lines = note_text.split("*")
     formatted_lines = [lines[0]] + [f"{bullet_indent}* {line.strip()}" for line in lines[1:]]
     return "\n".join(formatted_lines)
 
 
 def list_notes(category=None, importance=None, verbose=None, marked=None, unmarked=None):
     notes, _, _ = load_notes()
@@ -113,59 +118,60 @@
 
             checked_symbol = "[✔]" if note["checked"] else "[ ]"
             importance_symbol = f"[{note['importance']}]" if note["importance"] is not None and verbose else ""
             created_timestamp = f'(Created {note["created_timestamp"]})' if verbose else ""
             marked_timestamp = f'(Mark Updated {note["marked_timestamp"]})' if verbose and note["marked_timestamp"] is not None else ""
 
             lines = textwrap.wrap(note['note'], width=80 - indent)
-            first_line = lines.pop(0)
 
+            first_line = format_note(lines.pop(0), indent)
             print(
                 f"{indent * ' '}{checked_symbol} {note['id']} {first_line} "
                 f"{importance_symbol} {created_timestamp} {marked_timestamp}"
             )
 
             for line in lines:
                 print(f"{indent * ' '}   {line}")
 
             try:
                 if note["subs"]:
                     display_notes(note["subs"], indent + 4)
-            except KeyError:
-                pass
+            except KeyError as e:
+                print(e)
 
     grouped_notes = {}
     for note in sorted_notes:
         grouped_notes.setdefault(note['category'], []).append(note)
 
     for category, cat_notes in grouped_notes.items():
         print(f"\n{category.upper()}{'-' * (80 - len(category))}")
         display_notes(cat_notes)
 
 
 def mark_note(note_id, checked=True):
-    notes, max_id, last_category = load_notes()
+    all_notes, max_id, last_category = load_notes()
 
-    for note in notes:
-        if note["id"] == note_id:
-            note["checked"] = checked
-            note["marked_timestamp"] = datetime.now().isoformat()
-            save_notes(notes, max_id, last_category)
-            print(f"Note {'marked' if checked else 'unmarked'} successfully.")
-            return
-
-        for index, sub in enumerate(note["subs"]):
-            if sub["id"] == note_id:
-                sub["checked"] = checked
+    def find_and_mark_note(notes):
+        for note in notes:
+            if note["id"] == note_id:
+                note["checked"] = checked
                 note["marked_timestamp"] = datetime.now().isoformat()
-                save_notes(notes, max_id, last_category)
                 print(f"Note {'marked' if checked else 'unmarked'} successfully.")
-                return
+                return True
+            elif find_and_mark_note(note["subs"]):
+                return True
+        else:
+            return False
+
+    note_marked = find_and_mark_note(all_notes)
+
+    if note_marked:
+        save_notes(all_notes, max_id, last_category)
     else:
-        print("Invalid note ID.")
+        print("Invalid note id.")
 
 
 def delete_note(note_id):
     notes, max_id, last_category = load_notes()
 
     for index, note in enumerate(notes):
         if note["id"] == note_id:
```

### Comparing `tinote-1.1.4/tinote/update.py` & `tinote-1.2.0/tinote/update.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,16 @@
         data = json.load(f)
 
     # Get the current version from the data
     current_version = data.get("version", "1.0.x")
 
     # Define a dictionary of update actions keyed by the version they should be applied to
     update_actions = [
-        ("1.1.0", update_1_0_x_to_1_1_x)
+        ("1.1.0", update_1_0_x_to_1_1_x),
+        ("1.2.0", update_1_1_x_to_1_2_x)
     ]
 
     # Apply the update actions in order
     for version, update_action in update_actions:
         if current_version < version:
             print(f"Updating user data file from {current_version} to {version}")
             data = update_action(data)
@@ -38,14 +39,36 @@
 def update_1_0_x_to_1_1_x(data):
     notes = data.get("notes", [])
 
     for note in notes:
         try:
             note["created_timestamp"] = note["timestamp"]
             note["marked_timestamp"] = None
-            note["subs"] = [] if "subs" not in note.keys() else note["subs"]
+            note["subs"] = [] if "subs" not in note.keys() or note["subs"] is None else note["subs"]
 
             del note["timestamp"]
         except KeyError:
             pass
 
     return data
+
+
+def update_1_1_x_to_1_2_x(data):
+    all_notes = data.get("notes", [])
+
+    def update_notes(notes):
+        for note in notes:
+            try:
+                if "timestamp" in note.keys():
+                    note["created_timestamp"] = note["timestamp"]
+                    del note["timestamp"]
+
+                note["marked_timestamp"] = None
+                note["subs"] = [] if "subs" not in note.keys() or note["subs"] is None else note["subs"]
+            except KeyError:
+                pass
+
+            update_notes(note["subs"])
+
+    update_notes(all_notes)
+
+    return data
```

### Comparing `tinote-1.1.4/tinote.egg-info/PKG-INFO` & `tinote-1.2.0/tinote.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.1.4
+Version: 1.2.0
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -64,37 +64,40 @@
 [ ] 55 A dating app, but for hamster-owners ONLY
 [✔] 58 A sushi company that sell BEEF sushi! :O
 
 VAN-STUFF-----------------------------------------------------------------------
 [✔] 55 Fix the latch for the fridge
 [ ] 58 Install Solar
     [ ] 60 Install roof-rack, hopefully easy
+        * How hard could it be
+        * Hahaha
     [ ] 61 Attach panels
     [ ] 62 Run wiring
 ```
+As you can see, using * in a message (no newline necessary) will cause that to be indented on the next line down.
 
 List notes with filters (category or importance or marked) or higher verbosity:
 
 ```bash
 ti list -c <category> -i <importance> -m -u -v
 ```
 
-Add a sub-note to a note (currently only supports one level)
+Add a sub-note to a note (can be as recursive as you can dream)
 
 ```bash
 ti sub <parent_id> "Text of your sub-note" -i <importance>
 ```
 
-Mark a note as checked/unchecked:
+Mark a note as checked/unchecked (-u indicates to unmark):
 
 ```bash
-ti mark <note_id>
+ti mark <note_id> -u 
 ```
 
-Delete a note:
+Delete a note (deletes all children notes):
 
 ```bash
 ti delete <note_id>
 ```
 
 Clear all notes or notes within a specified category:
```


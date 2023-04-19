# Comparing `tmp/remindmail-2023.4.2.1.tar.gz` & `tmp/remindmail-2023.4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.4.2.1.tar", last modified: Sun Apr  2 16:45:12 2023, max compression
+gzip compressed data, was "remindmail-2023.4.2.2.tar", last modified: Sun Apr  2 17:25:21 2023, max compression
```

## Comparing `remindmail-2023.4.2.1.tar` & `remindmail-2023.4.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 16:45:12.539947 remindmail-2023.4.2.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.4.2.1/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11896 2023-04-02 16:45:12.539947 remindmail-2023.4.2.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11548 2023-04-02 03:55:21.000000 remindmail-2023.4.2.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.4.2.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-04-02 16:45:12.539947 remindmail-2023.4.2.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 16:45:12.539947 remindmail-2023.4.2.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 16:45:12.539947 remindmail-2023.4.2.1/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2022-10-19 22:48:49.000000 remindmail-2023.4.2.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2022-10-19 22:48:49.000000 remindmail-2023.4.2.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    27067 2023-04-02 16:44:36.000000 remindmail-2023.4.2.1/src/remind/remind.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 16:45:12.539947 remindmail-2023.4.2.1/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11896 2023-04-02 16:45:12.000000 remindmail-2023.4.2.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      305 2023-04-02 16:45:12.000000 remindmail-2023.4.2.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-02 16:45:12.000000 remindmail-2023.4.2.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       46 2023-04-02 16:45:12.000000 remindmail-2023.4.2.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-04-02 16:45:12.000000 remindmail-2023.4.2.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 17:25:21.693085 remindmail-2023.4.2.2/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.4.2.2/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-04-02 17:25:21.693085 remindmail-2023.4.2.2/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-02 17:14:09.000000 remindmail-2023.4.2.2/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.4.2.2/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-04-02 17:25:21.693085 remindmail-2023.4.2.2/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 17:25:21.689084 remindmail-2023.4.2.2/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 17:25:21.693085 remindmail-2023.4.2.2/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2022-10-19 22:48:49.000000 remindmail-2023.4.2.2/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2022-10-19 22:48:49.000000 remindmail-2023.4.2.2/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    27775 2023-04-02 17:24:34.000000 remindmail-2023.4.2.2/src/remind/remind.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-02 17:25:21.693085 remindmail-2023.4.2.2/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11997 2023-04-02 17:25:21.000000 remindmail-2023.4.2.2/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      305 2023-04-02 17:25:21.000000 remindmail-2023.4.2.2/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-02 17:25:21.000000 remindmail-2023.4.2.2/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       46 2023-04-02 17:25:21.000000 remindmail-2023.4.2.2/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-04-02 17:25:21.000000 remindmail-2023.4.2.2/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.4.2.1/LICENSE.md` & `remindmail-2023.4.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.2.1/PKG-INFO` & `remindmail-2023.4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.4.2.1
+Version: 2023.4.2.2
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -81,14 +81,15 @@
 # usage
 
 - `-h` (or `--help`): Displays usage information.
 - `-ls` (or `-l` or `--list`): Lists all current reminders in `remind.md`.
 - `-g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab (see [generate](##generate))
 - `--later`: Emails reminders that are marked with `[any]`
+- `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
 
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
```

### Comparing `remindmail-2023.4.2.1/README.md` & `remindmail-2023.4.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 # usage
 
 - `-h` (or `--help`): Displays usage information.
 - `-ls` (or `-l` or `--list`): Lists all current reminders in `remind.md`.
 - `-g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab (see [generate](##generate))
 - `--later`: Emails reminders that are marked with `[any]`
+- `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
 
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
```

### Comparing `remindmail-2023.4.2.1/setup.cfg` & `remindmail-2023.4.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.04.02.1
+version = 2023.04.02.2
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.4.2.1/src/remind/remind.py` & `remindmail-2023.4.2.2/src/remind/remind.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,24 @@
 from cabinet import Cabinet, mail
 
 cab = Cabinet()
 
 TODAY = str(datetime.today().strftime('%Y-%m-%d'))
 WEEKDAYS = ['sunday', 'monday', 'tuesday',
             'wednesday', 'thursday', 'friday', 'saturday']
-TODAY_INDEX = datetime.today().day
 PATH_REMIND_FILE = cab.get(
     'path', 'remindmail', 'file')
 QUERY_TRACE = []
 
 
 def _months_since_epoch(epoch):
     epoch_time = time.localtime(epoch)
     return ((epoch_time.tm_year - 1970) * 12) + epoch_time.tm_mon
 
 
-def _strip_to(query):
-    if query.startswith(' to ') or query.startswith('to ') or query.startswith('day to '):
-        return ''.join(query.split('to')[1:]).strip()
-
-    return query.strip()
-
-
 def parse_date(query):
     """
     Parses a date from the input query
     """
 
     # handle 'tomorrow'
     if 'tomorrow' in query:
@@ -94,20 +86,14 @@
         mail.send(f"Reminder - {subject}", body or "", is_quiet=is_quiet)
         print("\nSent! Check your inbox.")
     else:
         log_msg(
             f"In test mode- mail would send subject '{subject}' and body '{body}'", level="debug")
 
 
-def _larger(string_a, string_b):
-    """A helper function to return the larger string between string_a and string_b"""
-
-    return string_a if len(string_a) > len(string_b) else string_b
-
-
 def list_reminders(param=None):
     """
     Displays the scheduled reminders in remind.py, formatted with line numbers
     Usage: remindmail ls
     Parameters:
     - param: string; currently unused
 
@@ -149,22 +135,24 @@
 
 def generate(force=False, dry_run=False):
     """
     Mails reminders from the remind.md file in {PATH_LOCAL}.
     Intended to be run from crontab (try 'remindmail generate force' to run immediately)
     """
 
+    today_index = datetime.today().day
+
     day_of_month_reminders_generated = cab.get(
         "remindmail", "day_generated")
 
     if day_of_month_reminders_generated == '':
         day_of_month_reminders_generated = 0
 
     # do not generate more than once in one day unless `remind generate force`
-    if not (TODAY_INDEX != day_of_month_reminders_generated
+    if not (today_index != day_of_month_reminders_generated
             and datetime.today().hour > 3) and not force and not dry_run:
         log_msg(
             "Reminders have already been generated in the past 12 hours.", level="debug")
         return
 
     log_msg("Generating reminders")
 
@@ -257,15 +245,15 @@
             split_types = ['d', 'w', 'm', 'sun', 'mon',
                            'tue', 'wed', 'thu', 'fri', 'sat']
             if split_type in split_types and any(is_epoch_equal_offset):
                 if split_type == 'd':
                     is_match = True
                 elif split_type == 'w' and today_dayw == 'Sun':
                     is_match = True
-                elif split_type == 'm' and TODAY_INDEX == 1:
+                elif split_type == 'm' and today_index == 1:
                     is_match = True
                 elif (split_type in ['sun', 'mon', 'tue', 'wed', 'thu', 'fri', 'sat']
                       and today_dayw.lower() == split_type):
                     is_match = True
 
         # handle deletion and decrementing
         if is_match:
@@ -296,19 +284,19 @@
                     log_msg(f"(in test mode- not executing {item})",
                             level="debug")
 
     cab.write_file("remind.md", "notes",
                    '\n'.join(remindmd_file), is_quiet=True)
 
     if not dry_run:
-        log_msg(f"Setting remindmail -> day_generated to {TODAY_INDEX}")
-        cab.put("remindmail", "day_generated", TODAY_INDEX)
+        log_msg(f"Setting remindmail -> day_generated to {today_index}")
+        cab.put("remindmail", "day_generated", today_index)
     else:
         log_msg(
-            f"In test mode- would set remindmail -> day_generated to {TODAY_INDEX}", level="debug")
+            f"In test mode- would set remindmail -> day_generated to {today_index}", level="debug")
 
     log_msg("Generated tasks")
 
 
 def offset(args):
     """
     Calculates the offset for a certain date (today by default)
@@ -392,25 +380,51 @@
                         "value", f"{PATH_REMIND_FILE}/remind.md")
                 print((f"\n\nSet. Open {cab.path_cabinet}/settings.json"
                        f" and set path -> edit -> remind -> sync to true"
                        f" to enable cloud syncing."))
     sys.exit()
 
 
+def show_tomorrow():
+    """
+    Prints reminders from remind.md tagged with tomorow's date in YYYY-MM-DD format
+    """
+
+    tomorrow = str((datetime.today() + timedelta(days=1)).strftime('%Y-%m-%d'))
+    remindmd_file = cab.get_file_as_array("remind.md", "notes") or []
+
+    for item in remindmd_file:
+        if f"[{tomorrow}]" in item:
+            print(item)
+
+
 def parse_query(query=None, manual_message='', manual_date='', noconfirm=False):
     """
     Parses arguments to determine what to email or what to write to a file for later.
 
     Args:
         query (str): The query string to parse (default: None).
         manual_message (str): The manual message to use if query is None (default: '').
         manual_date (str): The manual date to use (default: '').
         noconfirm (bool, optional): If True, bypass the confirmation screen.
     """
 
+    # helper functions
+    def get_larger(string_a, string_b):
+        """A helper function to return the larger string between string_a and string_b"""
+
+        return string_a if len(string_a) > len(string_b) else string_b
+
+    def strip_to(query):
+        """A helper function to remove the portion after 'to' or 'day to'"""
+        if query.startswith(' to ') or query.startswith('to ') or query.startswith('day to '):
+            return ''.join(query.split('to')[1:]).strip()
+
+        return query.strip()
+
     query = query or manual_message
     query_original = query
     QUERY_TRACE.append(query)
     query_time_token = ''  # the 'meat' between [] in remind.md
     query_notes = ''
     query_time_formatted = ''
     query_notes_formatted = ''
@@ -467,15 +481,15 @@
                          query, flags=re.IGNORECASE)
 
     if _months:
         _number_of_months = int(re.search(r'\d+', _months[0]).group())
         _newdate = (datetime.now().date() +
                     relativedelta(months=_number_of_months))
         _query_match = query.split(_months[0])
-        query = _larger(_query_match[0], _query_match[1])
+        query = get_larger(_query_match[0], _query_match[1])
 
         if is_recurring:
             query_time_token = f"M%{_number_of_months}"
             _frequency = (f"{f'{_number_of_months} ' if _number_of_months > 1 else ''}"
                           f"{'month' if _number_of_months == 1 else 'months'}")
             query_time_formatted = f"every {_frequency} starting {_newdate.strftime('%B %d')}"
         else:
@@ -495,15 +509,15 @@
         query = re.sub(_weeks[0], f"in {_number_of_weeks * 7} days", query)
 
     # handle "in n days"
     _days = re.findall("in [0-9]+ days|in 1 day", query, flags=re.IGNORECASE)
     if _days:
         _number_of_days = int(re.search(r'\d+', _days[0]).group())
         _query_match = query.split(_days[0])
-        query = _larger(_query_match[0], _query_match[1])
+        query = get_larger(_query_match[0], _query_match[1])
 
         _newdate = datetime.now().date() + timedelta(days=_number_of_days)
         if is_recurring:
             query_time_token = f"D%{_number_of_days}"
             query_time_formatted = (f"every {_number_of_days} days"
                                     f" starting {_newdate.strftime('%B %d')}")
         else:
@@ -519,15 +533,15 @@
 
         # ['on sun', ... , 'on sat', 'next sun', ... , 'next sat']
         for day in [f"on {day[:3]}" for day in WEEKDAYS] + [f"next {day[:3]}" for day in WEEKDAYS]:
 
             if re.search(day, query, flags=re.IGNORECASE):
 
                 _query_match = re.split(day, query, flags=re.IGNORECASE)
-                query = _larger(_query_match[0], _query_match[1])
+                query = get_larger(_query_match[0], _query_match[1])
 
                 query_time_token = re.sub(
                     'on|next|day', '', day, flags=re.IGNORECASE).strip()
 
                 query_time_formatted = {
                     'sun': 'Sunday',
                     'mon': 'Monday',
@@ -546,15 +560,15 @@
 
     # handle other dates
     parsed_date = parse_date(query)
 
     # handle "tomorrow"
     if not query_time_token and re.search("tomorrow", query, flags=re.IGNORECASE):
         _query_match = re.split("tomorrow", query, flags=re.IGNORECASE)
-        query = _strip_to(_larger(_query_match[0], _query_match[1]))
+        query = strip_to(get_larger(_query_match[0], _query_match[1]))
 
     # handle manual time
     if manual_date:
         parsed_date = parse_date(manual_date)
 
     # handle specific dates (found or specified)
     if parsed_date and (not query_time_token or manual_date):
@@ -571,27 +585,27 @@
         if manual_message:
             query = manual_message
         else:
             if len(parsed_date[1]) > 1:
                 _join_operator = ''
                 if len(parsed_date[1]) > 1:
                     _join_operator = parsed_date[1][1]
-                query = ''.join(_larger(parsed_date[1][0], _join_operator))
-                query = _strip_to(''.join(query.rsplit(' on ', 1)) or query)
+                query = ''.join(get_larger(parsed_date[1][0], _join_operator))
+                query = strip_to(''.join(query.rsplit(' on ', 1)) or query)
             elif len(parsed_date) > 1:
-                parsed_date_formatted = _strip_to(''.join(parsed_date[1]))
+                parsed_date_formatted = strip_to(''.join(parsed_date[1]))
                 if parsed_date_formatted:
                     query = parsed_date_formatted
 
     # confirmation
     if query_notes:
         query_notes_formatted = f"\nNotes: {query_notes.strip()}\n"
 
     response = ''
-    query = _strip_to(query.strip())
+    query = strip_to(query.strip())
 
     if manual_message:
         query = manual_message
 
     while response not in ['y', 'n', 'r', 'l', 'm']:
         options = "(y)es\n(n)o\n(p)arse entire query\n(r)eport\n(l)ater\n(t)omorrow\n(m)anual"
 
@@ -722,28 +736,32 @@
                         help='Print generated reminders without sending them. Only used with -g.')
     parser.add_argument('--later', action='store_true',
                         help='Mail reminders for later')
     parser.add_argument('-o', '--offset', nargs='?',
                         help=help_offset)
     parser.add_argument('-e', '--edit', action='store_true',
                         help='Edits remind.md through the terminal')
+    parser.add_argument('--show-tomorrow', action='store_true',
+                        help='Shows a list of reminders scheduled for tomorrow')
     parser.add_argument('manual_reminder_args', nargs='*')
 
     args = parser.parse_args()
 
     if args.list:
         list_reminders()
     elif args.generate:
         generate(force=args.force, dry_run=args.dry_run)
     elif args.later:
         mail_reminders_for_later()
     elif args.offset is not None:
         offset(args.offset.split(" "))
     elif args.edit:
         edit()
+    elif args.show_tomorrow:
+        show_tomorrow()
     elif args.manual_reminder_args:
         parse_query(query=' '.join(args.manual_reminder_args),
                     noconfirm=args.noconfirm)
     else:
         manual_reminder(manual_message=args.message or '',
                         manual_date=args.date or '', noconfirm=args.noconfirm)
```

### Comparing `remindmail-2023.4.2.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.4.2.2/src/remindmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.4.2.1
+Version: 2023.4.2.2
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -81,14 +81,15 @@
 # usage
 
 - `-h` (or `--help`): Displays usage information.
 - `-ls` (or `-l` or `--list`): Lists all current reminders in `remind.md`.
 - `-g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab (see [generate](##generate))
 - `--later`: Emails reminders that are marked with `[any]`
+- `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
 
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
```


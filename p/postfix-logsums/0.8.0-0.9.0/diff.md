# Comparing `tmp/postfix_logsums-0.8.0.tar.gz` & `tmp/postfix_logsums-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfix_logsums-0.8.0.tar", last modified: Mon Mar 27 12:05:48 2023, max compression
+gzip compressed data, was "postfix_logsums-0.9.0.tar", last modified: Wed Apr 19 16:24:37 2023, max compression
```

## Comparing `postfix_logsums-0.8.0.tar` & `postfix_logsums-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:05:48.305743 postfix_logsums-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2225 2023-03-27 12:05:48.305743 postfix_logsums-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      987 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1091 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/postfix-logsums
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:05:48.305743 postfix_logsums-0.8.0/postfix_logsums/
--rw-r--r--   0 root         (0) root         (0)    63145 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/postfix_logsums/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71967 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/postfix_logsums/app.py
--rw-r--r--   0 root         (0) root         (0)     7622 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/postfix_logsums/errors.py
--rw-r--r--   0 root         (0) root         (0)     7965 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/postfix_logsums/results.py
--rw-r--r--   0 root         (0) root         (0)    31612 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/postfix_logsums/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:05:48.305743 postfix_logsums-0.8.0/postfix_logsums.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2225 2023-03-27 12:05:48.000000 postfix_logsums-0.8.0/postfix_logsums.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-27 12:05:48.000000 postfix_logsums-0.8.0/postfix_logsums.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 12:05:48.000000 postfix_logsums-0.8.0/postfix_logsums.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-27 12:05:48.000000 postfix_logsums-0.8.0/postfix_logsums.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1125 2023-03-27 12:05:48.305743 postfix_logsums-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4364 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:05:48.305743 postfix_logsums-0.8.0/test/
--rwxr-xr-x   0 root         (0) root         (0)     7285 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    13220 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/test/test_05_stats_collections.py
--rwxr-xr-x   0 root         (0) root         (0)     2411 2023-03-27 12:05:24.000000 postfix_logsums-0.8.0/test/test_10_results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1091 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix-logsums
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.093709 postfix_logsums-0.9.0/postfix_logsums/
+-rw-r--r--   0 root         (0) root         (0)    63893 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74500 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/app.py
+-rw-r--r--   0 root         (0) root         (0)     7699 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/results.py
+-rw-r--r--   0 root         (0) root         (0)    31716 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/stats.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/postfix_logsums/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/postfix_logsums.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-19 16:24:37.000000 postfix_logsums-0.9.0/postfix_logsums.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:24:37.097709 postfix_logsums-0.9.0/test/
+-rwxr-xr-x   0 root         (0) root         (0)     7285 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    13220 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/test/test_05_stats_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)     2411 2023-04-19 16:24:15.000000 postfix_logsums-0.9.0/test/test_10_results.py
```

### Comparing `postfix_logsums-0.8.0/LICENSE` & `postfix_logsums-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/PKG-INFO` & `postfix_logsums-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix_logsums
-Version: 0.8.0
+Version: 0.9.0
 Summary: Produce Postfix MTA logfile summary
 Home-page: https://github.com/pixelpark/postfix-logsums
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `postfix_logsums-0.8.0/README.md` & `postfix_logsums-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/postfix-logsums` & `postfix_logsums-0.9.0/postfix-logsums`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/postfix_logsums/__init__.py` & `postfix_logsums-0.9.0/postfix_logsums/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,29 +25,33 @@
 # Own modules
 from .errors import PostfixLogsumsError
 
 from .results import PostfixLogSums
 
 from .stats import MessageStats, MessageStatsPerDay, SmtpdStats
 
-__version__ = '0.8.0'
+from .xlate import XLATOR
+
+__version__ = '0.9.0'
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
 __copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 DEFAULT_TERMINAL_WIDTH = 99
 DEFAULT_TERMINAL_HEIGHT = 40
 MAX_TERMINAL_WIDTH = 150
 
 UTF8_ENCODING = 'utf-8'
 DEFAULT_ENCODING = UTF8_ENCODING
 DEFAULT_SYSLOG_NAME = 'postfix'
 DEFAULT_MAX_TRIM_LENGTH = 66
 
 LOG = logging.getLogger(__name__)
 
+_ = XLATOR.gettext
+
 
 # =============================================================================
 def pp(value, indent=4, width=None, depth=None):
     """
     Return a pretty print string of the given value.
 
     @return: pretty print string
@@ -138,14 +142,16 @@
     re_said1 = re.compile(r'^.*: *')
 
     utc = datetime.timezone(datetime.timedelta(0), 'UTC')
 
     default_encoding = DEFAULT_ENCODING
     default_max_trim_length = DEFAULT_MAX_TRIM_LENGTH
 
+    min_max_len = 4
+
     # -------------------------------------------------------------------------
     def __init__(
             self, appname=None, verbose=0, day=None, syslog_name=DEFAULT_SYSLOG_NAME,
             zero_fill=False, detail_verbose_msg=False, detail_reject=True,
             detail_deferral=False, detail_bounce=False, detail_smtp=True,
             detail_smtpd_warning=True, ignore_case=False, rej_add_from=False,
             smtpd_stats=False, extended=False, no_no_message_size=False,
@@ -185,21 +191,30 @@
         self._rcvd_msgs_qid = {}
         self._connection_times = {}
         self._message_size = {}
         self._message_deferred_qid = {}
         self.date_str = None
 
         if day:
-            t_diff = datetime.timedelta(days=1)
-            used_date = copy.copy(self.today)
-            if day == 'yesterday':
+
+            if isinstance(day, datetime.datetime):
+                used_date = day.date()
+            elif isinstance(day, datetime.date):
+                used_date = day
+            elif day.lower() == 'yesterday':
+                t_diff = datetime.timedelta(days=1)
                 used_date = self.today - t_diff
-            elif day != 'today':
-                msg = "Wrong day {d!r} given. Valid values are {n}, {y!r} and {t!r}.".format(
-                    d=day, n='None', y='yesterday', t='today')
+            elif day.lower() == 'today':
+                used_date = copy.copy(self.today)
+            else:
+                msg = _(
+                    "Wrong day {d!r} given. Valid values are {n}, {y!r} and {t!r} or a valid "
+                    "{dt} or {dd} object.").format(
+                        d=day, n='None', y='yesterday', t='today',
+                        dt='datetime.datetime', dd='datetime.date')
                 raise PostfixLogsumsError(msg)
             self.date_str = used_date.isoformat()
             filter_pattern = r"^{m} {d:02d}\s".format(
                 m=self.month_names[used_date.month - 1], d=used_date.day)
             self.re_date_filter = re.compile(filter_pattern, re.IGNORECASE)
             filter_rfc3339_pattern = r"^{y:04d}-{m:02d}-{d:02d}[T\s]".format(
                 y=used_date.year, m=used_date.month, d=used_date.day)
@@ -349,16 +364,17 @@
         if not max_len:
             max_len = cls.default_max_trim_length
 
         trimmed = str(message).strip()
         if do_not_trim:
             return trimmed
 
-        if max_len < 4:
-            msg = "Invalid max. length {} of a string, must be >= 4.".format(max_len)
+        if max_len < cls.min_max_len:
+            msg = _("Invalid max. length {max} of a string, must be >= {min}.").format(
+                max=max_len, min=cls.min_max_len)
             raise ValueError(msg)
 
         ml = int(max_len) - 3
         if len(trimmed) > ml:
             trimmed = trimmed[0:ml] + '...'
 
         return trimmed
@@ -406,15 +422,15 @@
 
     @verbose.setter
     def verbose(self, value):
         v = int(value)
         if v >= 0:
             self._verbose = v
         else:
-            LOG.warning("Wrong verbose level {!r}, must be >= 0".format(value))
+            LOG.warning(_("Wrong verbose level {!r}, must be >= 0").format(value))
 
     # -----------------------------------------------------------
     @property
     def initialized(self):
         """The initialisation of this object is complete."""
         return getattr(self, '_initialized', False)
 
@@ -423,19 +439,19 @@
     def syslog_name(self):
         """The name, which is used by syslog for entries in logfiles."""
         return self._syslog_name
 
     @syslog_name.setter
     def syslog_name(self, value):
         if value is None:
-            msg = "The syslog name must not be None."
+            msg = _("The syslog name must not be {}.").format('None')
             raise TypeError(msg)
         v = str(value).strip()
         if v == '':
-            msg = "The syslog name must not be empty."
+            msg = _("The syslog name must not be empty.")
             raise ValueError(msg)
         self._syslog_name = v
 
     # -----------------------------------------------------------
     @property
     def compression(self):
         """The compression explicitely to use for all logfiles and the input stream."""
@@ -444,15 +460,15 @@
     @compression.setter
     def compression(self, value):
         if value is None:
             self._compression = None
             return
         v = str(value).strip().lower()
         if v not in self.valid_compressions:
-            msg = "Invalid compression {!r} given.".format(value)
+            msg = _("Invalid compression {!r} given.").format(value)
             raise PostfixLogsumsError(msg)
         if v == 'xz':
             self._compression = 'lzma'
         else:
             self._compression = v
 
     # -------------------------------------------------------------------------
@@ -577,15 +593,16 @@
     def encoding(self):
         """Return the default encoding used to read config files."""
         return self._encoding
 
     @encoding.setter
     def encoding(self, value):
         if not isinstance(value, str):
-            msg = "Encoding {v!r} must be a {s!r} object, but is a {c!r} object instead.".format(
+            msg = _(
+                "Encoding {v!r} must be a {s!r} object, but is a {c!r} object instead.").format(
                 v=value, s='str', c=value.__class__.__name__)
             raise TypeError(msg)
 
         encoder = codecs.lookup(value)
         self._encoding = encoder.name
 
     # -------------------------------------------------------------------------
@@ -684,24 +701,27 @@
     # -------------------------------------------------------------------------
     def parse(self, *files):
         """Main entry point of this class."""
 
         self.results.reset()
 
         if not files:
-            LOG.debug("Parsing from STDIN ...")
+            LOG.debug(_("Parsing from {} ...").format('STDIN'))
             self.results.start_logfile('STDIN')
             return self.parse_fh(sys.stdin, 'STDIN', self.compression)
 
         for logfile in files:
-            LOG.debug("Parsing logfile {!r} ...".format(str(logfile)))
+            LOG.debug(_("Parsing logfile {!r} ...").format(str(logfile)))
             self.results.start_logfile(logfile)
             if not self.parse_file(logfile):
                 return False
 
+        if self.date_str:
+            LOG.debug(_("Filtering log messages for date {} ...").format(self.date_str))
+
         return True
 
     # -------------------------------------------------------------------------
     def parse_file(self, logfile):
         """Parsing a particular logfile."""
 
         open_opts = {
@@ -730,37 +750,37 @@
 
     # -------------------------------------------------------------------------
     def parse_fh(self, fh, filename, compression=None):
 
         line = None
 
         if not compression:
-            LOG.debug("Reading uncompressed file {!r} ...".format(filename))
+            LOG.debug(_("Reading uncompressed file {!r} ...").format(filename))
             line = fh.readline()
             while line:
                 self.eval_line(line)
                 line = fh.readline()
             return True
 
         cdata = fh.read()
 
         if compression == 'gzip':
-            LOG.debug("Reading {w} compressed file {f!r} ...".format(
+            LOG.debug(_("Reading {w} compressed file {f!r} ...").format(
                 w='GZIP', f=filename))
             self.read_gzip(cdata)
             return True
 
         if compression == 'bzip2':
-            LOG.debug("Reading {w} compressed file {f!r} ...".format(
+            LOG.debug(_("Reading {w} compressed file {f!r} ...").format(
                 w='BZIP2', f=filename))
             self.read_bzip2(cdata)
             return True
 
         if compression == 'lzma':
-            LOG.debug("Reading {w} compressed file {f!r} ...".format(
+            LOG.debug(_("Reading {w} compressed file {f!r} ...").format(
                 w='LZMA', f=filename))
             self.read_lzma(cdata)
             return True
 
     # -------------------------------------------------------------------------
     def read_gzip(self, cdata):
 
@@ -818,15 +838,16 @@
 
         result = self._eval_pf_command(self._cur_msg)
         if result:
             self._cur_pf_command = result[0]
             self._cur_qid = result[1]
         else:
             if self.verbose > 1:
-                LOG.debug("Did not found Postfix command and QID from: {}".format(self._cur_msg))
+                LOG.debug(_("Did not found Postfix command and QID from: {}").format(
+                    self._cur_msg))
             return
         if self.verbose > 3:
             LOG.debug("Postfix command {cmd!r}, qid {qid!r}, message: {msg}".format(
                 cmd=self._cur_pf_command, qid=self._cur_qid, msg=self._cur_msg))
 
         self.results.incr_lines_considered()
 
@@ -1203,15 +1224,15 @@
         if cmd_msg not in counter[cmd][part]:
             counter[cmd][part][cmd_msg] = 0
         counter[cmd][part][cmd_msg] += 1
 
     # -------------------------------------------------------------------------
     def _eval_cleanup_cmd(self, subtype, part, cmd_msg):
         if self.verbose > 2:
-            LOG.debug("Evaluating 'cleanup' command message.")
+            LOG.debug(_("Evaluating {!r} command message.").format('cleanup'))
 
         if not self.detail_verbose_msg:
             cmd_msg = self.re_clean_from.sub('', cmd_msg)
             cmd_msg = self.string_trimmer(cmd_msg, do_not_trim=self.detail_verbose_msg)
 
         hour = self._cur_ts.hour
         self.results.rejected_messages_per_hour[hour] += 1
@@ -1626,15 +1647,15 @@
             self.results.rcpt_user[addr].size += size
             self.results.msgs_total.bytes_delivered += size
         else:
             self.results.rcpt_domain[domain].size += 0
             self.results.rcpt_user[addr].size += 0
             if not self.no_no_message_size:
                 self.results.no_message_size[qid] = addr
-            self._add_ext_msg_detail(qid, '(sender not in log)')
+            self._add_ext_msg_detail(qid, '({})'.format('sender not in log'))
 
         self._add_ext_msg_detail(qid, addr)
 
     # -------------------------------------------------------------------------
     def _eval_pickup_msgs(self):
         hour = self._cur_ts.hour
         qid = self._cur_qid
@@ -1703,15 +1724,15 @@
             m = self.re_connected_to_port.search(self._cur_msg)
             if m:
                 smtp_target = m.group(1).lower()
                 smtp_msg = m.group(2)
 
         if not smtp_target:
             if self.verbose > 1:
-                msg = "Unhandled SMTP message: {msg!r}".format(msg=self._cur_msg)
+                msg = _("Unhandled SMTP message: {msg!r}").format(msg=self._cur_msg)
                 LOG.debug(msg)
             return
 
         if smtp_target not in self.results.smtp_messages:
             self.results.smtp_messages[smtp_target] = {}
         if smtp_msg not in self.results.smtp_messages[smtp_target]:
             self.results.smtp_messages[smtp_target] = 0
```

### Comparing `postfix_logsums-0.8.0/postfix_logsums/app.py` & `postfix_logsums-0.9.0/postfix_logsums/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,40 +45,80 @@
 
 from . import __version__ as GLOBAL_VERSION
 from . import pp, to_bytes, MAX_TERMINAL_WIDTH
 from . import DEFAULT_TERMINAL_WIDTH, DEFAULT_TERMINAL_HEIGHT
 from . import get_generic_appname, get_smh
 from . import PostfixLogParser
 
+from .xlate import XLATOR, format_list
+
 from .stats import HOURS_PER_DAY
 
-__version__ = '0.7.10'
+__version__ = '0.8.4'
+_ = XLATOR.gettext
+ngettext = XLATOR.ngettext
 
 
 # =============================================================================
 class NonNegativeItegerOptionAction(argparse.Action):
 
     # -------------------------------------------------------------------------
     def __call__(self, parser, namespace, value, option_string=None):
 
         try:
             val = int(value)
         except Exception as e:
-            msg = "Got a {c} for converting {v!r} into an integer value: {e}".format(
+            msg = _("Got a {c} for converting {v!r} into an integer value: {e}").format(
                 c=e.__class__.__name__, v=value, e=e)
             raise argparse.ArgumentError(self, msg)
 
         if val < 0:
-            msg = "The option must not be negative (given: {}).".format(value)
+            msg = _("The option must not be negative (given: {}).").format(value)
             raise argparse.ArgumentError(self, msg)
 
         setattr(namespace, self.dest, val)
 
 
 # =============================================================================
+class FilterDayOptionAction(argparse.Action):
+
+    # -------------------------------------------------------------------------
+    def __init__(self, option_strings, *args, **kwargs):
+        """Initialise a FilterDayOptionAction object."""
+        super(FilterDayOptionAction, self).__init__(
+            option_strings=option_strings, *args, **kwargs)
+
+    # -------------------------------------------------------------------------
+    def __call__(self, parser, namespace, value, option_string=None):
+
+        val = str(value)
+        used_day = None
+        if val.lower() == 'today':
+            used_day = datetime.date.today()
+        elif val.lower() == 'yesterday':
+            t_diff = datetime.timedelta(days=1)
+            used_day = datetime.date.today() - t_diff
+        else:
+            pattern = r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2})$'
+            m = re.match(pattern, val)
+            if m:
+                try:
+                    used_day = datetime.date(int(m['year']), int(m['month']), int(m['day']))
+                except Exception as e:
+                    msg = _("Invalid date as day {!r} given").format(value)
+                    msg += ': ' + str(e)
+                    raise argparse.ArgumentError(self, msg)
+            else:
+                msg = _("Invalid date as day {!r} given").format(value) + '.'
+                raise argparse.ArgumentError(self, msg)
+
+        setattr(namespace, self.dest, used_day)
+
+
+# =============================================================================
 class LogFilesOptionAction(argparse.Action):
     """An argparse action for logfiles."""
 
     # -------------------------------------------------------------------------
     def __init__(self, option_strings, *args, **kwargs):
         """Initialise a LogFilesOptionAction object."""
         super(LogFilesOptionAction, self).__init__(
@@ -97,23 +137,23 @@
             all_files = [values]
 
         logfiles = []
         for logfile in all_files:
 
             path = Path(logfile)
             if not path.exists():
-                msg = "Logfile {!r} does not exists.".format(logfile)
+                msg = _("Logfile {!r} does not exists.").format(logfile)
                 raise argparse.ArgumentError(self, msg)
 
             if not path.is_file():
-                msg = "File {!r} is not a regular file.".format(logfile)
+                msg = _("File {!r} is not a regular file.").format(logfile)
                 raise argparse.ArgumentError(self, msg)
 
             if not os.access(str(path), os.R_OK):
-                msg = "File {!r} is not readable.".format(logfile)
+                msg = _("File {!r} is not readable.").format(logfile)
                 raise argparse.ArgumentError(self, msg)
 
             logfiles.append(path.resolve())
 
         setattr(namespace, self.dest, logfiles)
 
 # =============================================================================
@@ -312,15 +352,15 @@
         """Wrap the given message to the max terminal width ..."""
         if width is None:
             width = cls.max_width
         return textwrap.fill(message, width)
 
     # -------------------------------------------------------------------------
     def __init__(self):
-
+        """The constructor method."""
         self._appname = get_generic_appname()
         self._version = __version__
         self._verbose = 0
         self._quiet = False
         self._initialized = False
         self.parser = None
 
@@ -388,15 +428,15 @@
 
     @verbose.setter
     def verbose(self, value):
         v = int(value)
         if v >= 0:
             self._verbose = v
         else:
-            LOG.warning("Wrong verbose level {!r}, must be >= 0".format(value))
+            LOG.warning(_("Wrong verbose level {!r}, must be >= 0").format(value))
 
     # -----------------------------------------------------------
     @property
     def quiet(self):
         """Don't print headings for empty reports."""
         return self._quiet
 
@@ -586,299 +626,305 @@
 
         """
 
         appname = self.appname_capitalized
         arg_width = self.max_width - 24
 
         desc = []
-        desc.append('{} is a log analyzer/summarizer for the Postfix MTA.'.format(appname))
-        desc.append(
+        desc.append(_('{} is a log analyzer/summarizer for the Postfix MTA.').format(appname))
+        desc.append(_(
             'It is designed to provide an over-view of Postfix activity, with just enough '
-            'detail to give the administrator a "heads up" for potential trouble spots.')
-        desc.append((
+            'detail to give the administrator a "heads up" for potential trouble spots.'))
+        desc.append(_(
             '{} generates summaries and, in some cases, detailed reports of mail server traffic '
             'volumes, rejected and bounced email, and server warnings, '
             'errors and panics.').format(appname))
 
         description = ''
         for des in desc:
             des = self.wrap_msg(des)
             if description:
                 description += '\n\n'
             description += des
 
-        day_values = ('today', 'yesterday')
-
         self.arg_parser = argparse.ArgumentParser(
             prog=self.appname,
             description=description,
             formatter_class=RawTextHelpFormatter,
             add_help=False,
         )
 
-        logfile_group = self.arg_parser.add_argument_group('Options for scanning Postfix logfiles')
+        logfile_group = self.arg_parser.add_argument_group(_(
+            'Options for scanning Postfix logfiles'))
 
         # --day
-        desc = 'Generate report for just today or yesterday.'
+        desc = self.wrap_msg(_(
+            'Generate report for just today, yesterday or a date in ISO format (YYY-mm-dd).'))
         desc = self.wrap_msg(desc, arg_width)
         logfile_group.add_argument(
-            '-d', '--day', metavar='|'.join(day_values), dest='day', choices=day_values,
-            help=desc)
+            '-d', '--day', metavar=_('DAY'), dest='day',
+            action=FilterDayOptionAction, help=desc)
 
         # --extended
-        desc = 'Extended (extreme? excessive?) detail.\n'
-        desc += self.wrap_msg(
+        desc = _('Extended (extreme? excessive?) detail.') + '\n'
+        desc += self.wrap_msg(_(
             'At present, this includes only a per-message report, sorted by sender domain, '
-            'then user-in-domain, then by queue i.d.', arg_width) + '\n'
-        desc += self.wrap_msg(
+            'then user-in-domain, then by queue i.d.'), arg_width) + '\n'
+        desc += self.wrap_msg(_(
             'WARNING: the data built to generate this report can quickly consume very large '
-            'amounts of memory if a ot of log entries are processed!', arg_width)
+            'amounts of memory if a lot of log entries are processed!'), arg_width)
         logfile_group.add_argument(
             '-e', '--extended', dest='extended', action="store_true", help=desc)
 
         # --ignore-case
-        desc = self.wrap_msg(
-            'Handle complete email address in a case-insensitive manner.', arg_width)
+        desc = self.wrap_msg(_(
+            'Handle complete email address in a case-insensitive manner.'), arg_width)
         desc += '\n'
-        desc += self.wrap_msg(
+        desc += self.wrap_msg(_(
             'Normally {} lower-cases only the host and domain parts, leaving the user part alone. '
-            'This option causes the entire email address to be lower-cased.'.format(appname),
+            'This option causes the entire email address to be lower-cased.').format(appname),
             arg_width)
         logfile_group.add_argument(
             '-i', '--ignore-case', dest='ignore_case', action="store_true", help=desc)
 
         # --no-no-msg-size
-        desc = self.wrap_msg('Do not emit report on "Messages with no size data".', arg_width)
+        desc = self.wrap_msg(_('Do not emit report on "Messages with no size data".'), arg_width)
         desc += '\n'
-        desc += self.wrap_msg((
+        desc += self.wrap_msg(_(
             'Message size is reported only by the queue manager. The message may be delivered '
             'long-enough after the (last) qmgr log entry that the information is not in '
             'the log(s) processed by a particular run of {a}. This throws off "Recipients by '
             'message size" and the total for "bytes delivered." These are normally reported by '
-            '{a} as "Messages with nosize data.').format(a=appname), arg_width)
+            '{a} as "Messages with nosize data".').format(a=appname), arg_width)
         logfile_group.add_argument(
             '--no-no-msg-size', dest='nono_msgsize', action="store_true", help=desc)
 
         # --rej-add-from
-        desc = self.wrap_msg(
+        desc = self.wrap_msg(_(
             'For those reject reports that list IP addresses or host/domain names: append the '
             'email from address to each listing. (Does not apply to "Improper use of '
-            'SMTP command pipelining" report.)', arg_width)
+            'SMTP command pipelining" report.)'), arg_width)
         logfile_group.add_argument(
             '--rej-add-from', dest='rej_add_from', action="store_true", help=desc)
 
         # --smtpd-stats
-        desc = self.wrap_msg('Generate smtpd connection statistics.', arg_width) + '\n'
-        desc += self.wrap_msg(
+        desc = self.wrap_msg(_('Generate smtpd connection statistics.'), arg_width) + '\n'
+        desc += self.wrap_msg(_(
             'The "per-day" report is not generated for single-day reports. For multiple-day '
             'reports: "per-hour" numbers are daily averages (reflected in the report '
-            'heading).', arg_width)
+            'heading).'), arg_width)
         logfile_group.add_argument(
             '--smtpd-stats', dest='smtpd_stats', action="store_true", help=desc)
 
         # --verp-mung
-        desc = self.wrap_msg(
+        desc = self.wrap_msg(_(
             'Do "VERP" generated address (?) munging. Convert sender addresses of the form '
-            '"list-return-NN-someuser=some.dom@host.sender.dom" to'
-            '"list-return-ID-someuser=some.dom@host.sender.dom".', arg_width) + '\n'
-        desc += self.wrap_msg(
-            'In other words: replace the numeric value with "ID".', arg_width) + '\n'
-        desc += self.wrap_msg(
+            '"list-return-NN-someuser=some.dom@host.sender.dom" to '
+            '"list-return-ID-someuser=some.dom@host.sender.dom".'), arg_width) + '\n'
+        desc += self.wrap_msg(_(
+            'In other words: replace the numeric value with "ID".'), arg_width) + '\n'
+        desc += self.wrap_msg(_(
             'By specifying the optional "=2" (second form), the munging is more "aggressive", '
-            'converting the address to something like: "list-return@host.sender.dom".',
+            'converting the address to something like: "list-return@host.sender.dom".'),
             arg_width) + '\n'
-        desc += self.wrap_msg(
+        desc += self.wrap_msg(_(
             'Actually: specifying anything less than 2 does the "simple" munging and anything '
-            'greater than 1 results in the more "aggressive" hack being applied.', arg_width)
+            'greater than 1 results in the more "aggressive" hack being applied.'), arg_width)
         logfile_group.add_argument(
             '--verp-mung', type=int, metavar='1|2', const=0, dest='verp_mung', nargs='?',
             action=NonNegativeItegerOptionAction, help=desc)
 
         #######
         # Select compression
-        compression_section = self.arg_parser.add_argument_group('Logfile compression options')
+        compression_section = self.arg_parser.add_argument_group(_('Logfile compression options'))
 
         compression_group = compression_section.add_mutually_exclusive_group()
 
         # --gzip
-        desc = self.wrap_msg(
-            'Assume, that stdin stream or the given files are gzip compressed.', arg_width) + '\n'
-        desc += self.wrap_msg(
+        desc = self.wrap_msg(_(
+            'Assume, that stdin stream or the given files are gzip compressed.'), arg_width) + '\n'
+        desc += self.wrap_msg(_(
             'If not given, filenames with the extension ".gz" are assumed to be compressed with '
-            'the gzip compression.', arg_width)
+            'the gzip compression.'), arg_width)
         compression_group.add_argument(
             '-z', '--gzip', dest='gzip', action="store_true", help=desc)
 
         # --bzip2
-        desc = self.wrap_msg(
-            'Assume, that stdin stream or the given files are bzip2 compressed.', arg_width) + '\n'
-        desc += self.wrap_msg(
+        desc = self.wrap_msg(_(
+            'Assume, that stdin stream or the given files are bzip2 '
+            'compressed.'), arg_width) + '\n'
+        desc += self.wrap_msg(_(
             'If not given, filenames with the extensions ".bz2" or ".bzip2" are assumed to be '
-            'compressed with the bzip2 compression.', arg_width)
+            'compressed with the bzip2 compression.'), arg_width)
         compression_group.add_argument(
             '-j', '--bzip2', dest='bzip2', action="store_true", help=desc)
 
         # --xz
-        desc = self.wrap_msg(
-            'Assume, that stdin stream or the given files are xz or lzma compressed.',
+        desc = self.wrap_msg(_(
+            'Assume, that stdin stream or the given files are xz or lzma compressed.'),
             arg_width) + '\n'
-        desc += self.wrap_msg(
+        desc += self.wrap_msg(_(
             'If not given, filenames with the extensions ".xz" or ".lzma" are assumed to be '
-            'compressed with the xz or lzma compression.', arg_width)
+            'compressed with the xz or lzma compression.'), arg_width)
         compression_group.add_argument(
             '-J', '--xz', '--lzma', dest='xz', action="store_true", help=desc)
 
         # last parse option
-        desc = 'The logfile(s) to analyze. If no file(s) specified, reads from stdin.'
+        desc = _('The logfile(s) to analyze. If no file(s) specified, reads from stdin.')
         desc = self.wrap_msg(desc, arg_width)
         logfile_group.add_argument(
-            'logfiles', metavar='FILE', nargs='*', action=LogFilesOptionAction, help=desc)
+            'logfiles', metavar=_('FILE'), nargs='*', action=LogFilesOptionAction, help=desc)
 
         #######
         # Output
-        output_options = self.arg_parser.add_argument_group('Output options')
+        output_options = self.arg_parser.add_argument_group(_('Output options'))
 
-        desc = 'Output format. Valid options are: ' + ', '.join(
-            map(lambda x: repr(x), self.output_formats)) + '. '
-        desc += "Default: 'txt'."
+        desc = _('Output format. Valid options are:') + ' ' + format_list(
+            self.output_formats, True) + '. '
+        desc += _("Default: '{}'.").format('txt')
         desc = self.wrap_msg(desc, arg_width)
         output_options.add_argument(
-            '-O', '--output-format', choices=self.output_formats, metavar='FMT',
+            '-O', '--output-format', choices=self.output_formats, metavar=_('FORMAT'),
             dest='output_format', help=desc)
 
         # --detail
-        desc = self.wrap_msg(
+        desc = self.wrap_msg(_(
             'Sets all --*-detail, -h and -u to COUNT. Is over-ridden by '
-            'individual settings.', arg_width) + '\n'
-        desc += self.wrap_msg('--detail 0 suppresses *all* detail.', arg_width)
+            'individual settings.'), arg_width) + '\n'
+        desc += self.wrap_msg(_('--detail 0 suppresses *all* detail.'), arg_width)
         output_options.add_argument(
-            '-D', '--detail', type=int, metavar='COUNT', dest='detail',
+            '-D', '--detail', type=int, metavar=_('COUNT'), dest='detail',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --bounce-detail
-        desc = self.wrap_msg(
-            'Limit detailed bounce reports to the top COUNT.', arg_width) + '\n'
-        desc += self.wrap_msg('0 to suppress entirely.', arg_width)
+        desc = self.wrap_msg(_(
+            'Limit detailed bounce reports to the top {}.').format(_('COUNT')), arg_width) + '\n'
+        desc += self.wrap_msg(_('0 to suppress entirely.'), arg_width)
         output_options.add_argument(
-            '--bounce-detail', type=int, metavar='COUNT', dest='detail_bounce',
+            '--bounce-detail', type=int, metavar=_('COUNT'), dest='detail_bounce',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --deferral-detail
-        desc = self.wrap_msg(
-            'Limit detailed deferral reports to the top COUNT.', arg_width) + '\n'
-        desc += self.wrap_msg('0 to suppress entirely.', arg_width)
+        desc = self.wrap_msg(_(
+            'Limit detailed deferral reports to the top {}.').format(_('COUNT')), arg_width) + '\n'
+        desc += self.wrap_msg(_('0 to suppress entirely.'), arg_width)
         output_options.add_argument(
-            '--deferral-detail', type=int, metavar='COUNT', dest='detail_deferral',
+            '--deferral-detail', type=int, metavar=_('COUNT'), dest='detail_deferral',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --reject-detail
-        desc = self.wrap_msg(
-            'Limit detailed smtpd reject, warn, hold and discard reports to the top '
-            'COUNT.', arg_width) + '\n'
-        desc += self.wrap_msg('0 to suppress entirely.', arg_width)
+        desc = self.wrap_msg(_(
+            'Limit detailed smtpd reject, warn, hold and discard reports to the '
+            'top {}.').format(_('COUNT')), arg_width) + '\n'
+        desc += self.wrap_msg(_('0 to suppress entirely.'), arg_width)
         output_options.add_argument(
-            '--reject-detail', type=int, metavar='COUNT', dest='detail_reject',
+            '--reject-detail', type=int, metavar=_('COUNT'), dest='detail_reject',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --smtp-detail
-        desc = self.wrap_msg(
-            'Limit detailed smtp delivery reports to the top COUNT.', arg_width) + '\n'
-        desc += self.wrap_msg('0 to suppress entirely.', arg_width)
+        desc = self.wrap_msg(_(
+            'Limit detailed smtp delivery reports to the '
+            'top {}.').format(_('COUNT')), arg_width) + '\n'
+        desc += self.wrap_msg(_('0 to suppress entirely.'), arg_width)
         output_options.add_argument(
-            '--smtp-detail', type=int, metavar='COUNT', dest='detail_smtp',
+            '--smtp-detail', type=int, metavar=_('COUNT'), dest='detail_smtp',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --smtpd-warning-detail
-        desc = self.wrap_msg(
-            'Limit detailed smtpd warnings reports to the top COUNT.', arg_width) + '\n'
-        desc += self.wrap_msg('0 to suppress entirely.', arg_width)
+        desc = self.wrap_msg(_(
+            'Limit detailed smtpd warnings reports to the '
+            'top {}.').format(_('COUNT')), arg_width) + '\n'
+        desc += self.wrap_msg(_('0 to suppress entirely.'), arg_width)
         output_options.add_argument(
-            '--smtpd-warning-detail', type=int, metavar='COUNT', dest='detail_smtpd_warning',
+            '--smtpd-warning-detail', type=int, metavar=_('COUNT'), dest='detail_smtpd_warning',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --host
-        desc = self.wrap_msg('Top COUNT to display in host/domain reports.', arg_width)
-        desc += '\n0 = none.\n'
-        desc += self.wrap_msg(
-            'See also: "-u" and "--*-detail" options for further report-limiting options.',
+        desc = self.wrap_msg(_(
+            'Top {} to display in host/domain reports.').format(_('COUNT')), arg_width)
+        desc += '\n0 = {}.\n'.format(_('none'))
+        desc += self.wrap_msg(_(
+            'See also: "-u" and "--*-detail" options for further report-limiting options.'),
             arg_width)
         output_options.add_argument(
-            '-h', '--host', type=int, metavar='COUNT', dest='detail_host',
+            '-h', '--host', type=int, metavar=_('COUNT'), dest='detail_host',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --user
-        desc = self.wrap_msg('Top COUNT to display in user reports.', arg_width) + '\n'
-        desc += '0 = none.'
+        desc = self.wrap_msg(_(
+            'Top {} to display in user reports.').format(_('COUNT')), arg_width) + '\n'
+        desc += '0 = {}.'.format(_('none'))
         output_options.add_argument(
-            '-u', '--user', type=int, metavar='COUNT', dest='detail_user',
+            '-u', '--user', type=int, metavar=_('COUNT'), dest='detail_user',
             action=NonNegativeItegerOptionAction, help=desc)
 
         # --problems-first
-        desc = self.wrap_msg(
-            'Emit "problems" reports (bounces, defers, warnings, etc.) before "normal" stats.',
+        desc = self.wrap_msg(_(
+            'Emit "problems" reports (bounces, defers, warnings, etc.) before "normal" stats.'),
             arg_width)
         output_options.add_argument(
             '--pf', '--problems-first', dest='problems_first', action="store_true", help=desc)
 
         # --iso-date-time
-        desc = self.wrap_msg(
+        desc = self.wrap_msg(_(
             'For summaries that contain date or time information, use ISO 8601 standard formats '
-            '(CCYY-MM-DD and HH:MM), rather than "Mon DD CCYY" and "HHMM".', arg_width)
+            '(CCYY-MM-DD and HH:MM), rather than "Mon DD CCYY" and "HHMM".'), arg_width)
         output_options.add_argument(
             '--iso-date-time', dest='iso_date', action="store_true", help=desc)
 
         # --verbose-msg-detail
-        desc = self.wrap_msg(
+        desc = self.wrap_msg(_(
             'For the message deferral, bounce and reject summaries: display the full "reason", '
-            'rather than a truncated one.', arg_width) + '\n'
-        desc += self.wrap_msg(
-            'NOTE: this can result in quite long lines in the report.', arg_width)
+            'rather than a truncated one.'), arg_width) + '\n'
+        desc += self.wrap_msg(_(
+            'NOTE: this can result in quite long lines in the report.'), arg_width)
         output_options.add_argument(
             '--verbose-msg-detail', dest='detail_verbose_msg', action="store_true", help=desc)
 
         # --zero-fill
-        desc = self.wrap_msg(
+        desc = self.wrap_msg(_(
             '"Zero-fill" certain arrays so reports come out with data in columns that might '
-            'otherwise be blank.', arg_width)
+            'otherwise be blank.'), arg_width)
         output_options.add_argument(
             '--zero-fill', dest='zero_fill', action="store_true", help=desc)
 
         #######
         # General stuff
-        general_group = self.arg_parser.add_argument_group('General_options')
+        general_group = self.arg_parser.add_argument_group(_('General options'))
 
         verbose_group = general_group.add_mutually_exclusive_group()
 
-        desc = 'Increase the verbosity level.'
+        desc = self.wrap_msg(_(
+            'Enabling debug messages and increase their verbosity level if used multiple times.'))
         verbose_group.add_argument(
             "-v", "--verbose", action="count", dest='verbose', help=desc)
 
         # --quiet
-        desc = self.wrap_msg("quiet - don't print headings for empty reports.", arg_width)
+        desc = self.wrap_msg(_("quiet - don't print headings for empty reports."), arg_width)
         desc += '\n'
-        desc += self.wrap_msg(
-            'NOTE: headings for warning, fatal, and "master"  messages will always be '
-            'printed.', arg_width)
+        desc += self.wrap_msg(_(
+            'NOTE: headings for warning, fatal, and "master" messages will always be '
+            'printed.'), arg_width)
         verbose_group.add_argument(
             '-q', '--quiet', dest='quiet', action="store_true", help=desc)
 
         general_group.add_argument(
             "--help", action='help', dest='help',
-            help='Show this help message and exit.'
+            help=_('Show this help message and exit.')
         )
 
         general_group.add_argument(
             "--usage", action='store_true', dest='usage',
-            help="Display brief usage message and exit."
+            help=_("Display brief usage message and exit.")
         )
 
-        v_msg = "Version of %(prog)s: {}".format(GLOBAL_VERSION)
+        v_msg = _("Version of %(prog)s: {}").format(GLOBAL_VERSION)
         general_group.add_argument(
             "-V", '--version', action='version', version=v_msg,
-            help="Show program's version number and exit."
+            help=_("Show program's version number and exit.")
         )
 
     # -------------------------------------------------------------------------
     def perform_arg_parser(self):
 
         self.args = self.arg_parser.parse_args()
 
@@ -932,24 +978,24 @@
 
     # -------------------------------------------------------------------------
     def handle_error(
             self, error_message=None, exception_name=None, do_traceback=False):
 
         msg = str(error_message).strip()
         if not msg:
-            msg = 'undefined error.'
+            msg = _('undefined error.')
         title = None
 
         if isinstance(error_message, Exception):
             title = error_message.__class__.__name__
         else:
             if exception_name is not None:
                 title = exception_name.strip()
             else:
-                title = 'Exception happened'
+                title = _('Exception happened')
         msg = title + ': ' + msg
 
         root_log = logging.getLogger()
         has_handlers = False
         if root_log.handlers:
             has_handlers = True
 
@@ -973,41 +1019,41 @@
     # -------------------------------------------------------------------------
     def __call__(self):
         return self.run()
 
     # -------------------------------------------------------------------------
     def run(self):
 
-        LOG.debug("And here wo go ...")
+        LOG.debug(_("And here wo go ..."))
 
         locale.setlocale(locale.LC_ALL, '')
 
         self.parser.parse(*self.args.logfiles)
         self.results = self.parser.results
         self.nr_days = len(self.results.messages_per_day.keys())
 
         if self.verbose > 2:
-            LOG.info('Result of parsing:' + '\n' + pp(self.results.as_dict()))
+            LOG.info(_('Result of parsing:') + '\n' + pp(self.results.as_dict()))
         elif self.verbose > 1:
-            LOG.info('Result of parsing:' + '\n' + pp(self.results.dict()))
+            LOG.info(_('Result of parsing:') + '\n' + pp(self.results.dict()))
 
         if self.args.output_format == 'json':
             print(json.dumps(self.results.dict(), indent=4, sort_keys=True))
             return
         elif self.args.output_format == 'yaml':
             print(yaml.safe_dump(
                 self.results.dict(), allow_unicode=True, explicit_start=True, canonical=False,
                 sort_keys=True, indent=4, width=self.max_width, default_style=None))
             return
 
         print()
         if self.parser.date_str:
-            msg = "Postfix log summaries for {}".format(self.parser.date_str)
+            msg = _("Postfix log summaries for {}").format(self.parser.date_str)
         else:
-            msg = "Postfix log summaries"
+            msg = _("Postfix log summaries")
         print(msg)
         print('=' * len(msg))
 
         self.print_grand_totals()
 
         if self.args.smtpd_stats:
             self.print_smtpd_stats()
@@ -1023,51 +1069,52 @@
 
         if self.args.smtpd_stats:
             if self.nr_days > 1:
                 self.print_per_day_smtpd()
             self.print_per_hour_smtpd()
             self.print_domain_smtpd_summary()
 
-        self.print_user_data(self.results.sending_user_data, "Senders by message count", 'count')
-        self.print_user_data(self.results.rcpt_user, "Recipients by message count", 'count')
-        self.print_user_data(self.results.sending_user_data, "Senders by message size", 'size')
-        self.print_user_data(self.results.rcpt_user, "Recipients by message size", 'size')
+        self.print_user_data(
+            self.results.sending_user_data, _("Senders by message count"), 'count')
+        self.print_user_data(self.results.rcpt_user, _("Recipients by message count"), 'count')
+        self.print_user_data(self.results.sending_user_data, _("Senders by message size"), 'size')
+        self.print_user_data(self.results.rcpt_user, _("Recipients by message size"), 'size')
 
         self.print_hash_by_key(
-            self.results.no_message_size, 'Messages with no size data', self.detail)
+            self.results.no_message_size, _('Messages with no size data'), self.detail)
 
         if not self.args.problems_first:
             self.print_problems_reports()
 
         if self.args.extended:
             self.print_detailed_msg_data()
 
         print()
 
     # -------------------------------------------------------------------------
     def print_grand_totals(self):
         """Printing the grand total numbers and data."""
-        self.print_subsect_title('Grand Totals')
+        self.print_subsect_title(_('Grand Totals'))
 
         if self.results.logdate_oldest or self.results.logdate_latest:
-            lbl_oldest = 'Date of oldest log entry:'
-            lbl_latest = 'Date of latest log entry:'
+            lbl_oldest = _('Date of oldest log entry:')
+            lbl_latest = _('Date of latest log entry:')
             max_len = len(lbl_oldest)
             if len(lbl_latest) > max_len:
                 max_len = len(lbl_latest)
             print()
             if self.results.logdate_oldest:
                 dt = self.results.logdate_oldest.isoformat(' ')
                 print("{m:<{lng}}  {dt}".format(m=lbl_oldest, lng=max_len, dt=dt))
             if self.results.logdate_latest:
                 dt = self.results.logdate_latest.isoformat(' ')
                 print("{m:<{lng}}  {dt}".format(m=lbl_latest, lng=max_len, dt=dt))
 
         print()
-        print('Messages:')
+        print(_('Messages:'))
         print()
 
         # Variable renamings:
         #  - self.results.bounced_total => self.results.msgs_total.bounced
         #  - self.results.deferrals_total => self.results.msgs_total.deferrals
         #  - self.results.deferred_messages_total => self.results.msgs_total.deferred
         #  - self.results.messages_delivered => self.results.msgs_total.delivered
@@ -1082,78 +1129,78 @@
 
         msgs_received = self.results.msgs_total.received
         msgs_delivered = self.results.msgs_total.delivered
         msgs_rejected = self.results.msgs_total.rejected
         msgs_discarded = self.results.msgs_total.discarded
         msgs_total = msgs_delivered + msgs_rejected + msgs_discarded
 
-        msgs_rejected_pct = 0
-        msgs_discarded_pct = 0
+        msgs_rejected_pct = 0.0
+        msgs_discarded_pct = 0.0
         if msgs_total:
             msgs_rejected_pct = msgs_rejected / msgs_total * 100
             msgs_discarded_pct = msgs_discarded / msgs_total * 100
 
         nr = adj_int_units_localized(msgs_received)
-        print(tpl_loc.format(val=nr, lbl='received'))
+        print(tpl_loc.format(val=nr, lbl=_('received')))
         nr = adj_int_units_localized(msgs_delivered)
-        print(tpl_loc.format(val=nr, lbl='delivered'))
+        print(tpl_loc.format(val=nr, lbl=_('delivered')))
         nr = adj_int_units_localized(self.results.msgs_total.forwarded)
-        print(tpl_loc.format(val=nr, lbl='forwarded'))
+        print(tpl_loc.format(val=nr, lbl=_('forwarded')))
         nr = adj_int_units_localized(self.results.msgs_total.deferred)
-        print(tpl_loc.format(val=nr, lbl='deferred'), end='')
+        print(tpl_loc.format(val=nr, lbl=_('deferred')), end='')
         if self.results.msgs_total.deferrals:
             nr = adj_int_units_localized(self.results.msgs_total.deferrals)
-            val = '  ({val} {lbl})'.format(lbl='deferrals', val=nr)
+            val = '  ({val} {lbl})'.format(lbl=_('deferrals'), val=nr)
             print(val, end='')
         print()
         nr = adj_int_units_localized(self.results.msgs_total.bounced)
-        print(tpl_loc.format(val=nr, lbl='bounced'))
+        print(tpl_loc.format(val=nr, lbl=_('bounced')))
         nr = adj_int_units_localized(self.results.msgs_total.rejected)
-        print(tpl_loc.format(val=nr, lbl='rejected'), end='')
-        print(' ({:0.1n}%)'.format(msgs_rejected_pct))
+        print(tpl_loc.format(val=nr, lbl=_('rejected')), end='')
+        print(' ({:0.1f}%)'.format(msgs_rejected_pct))
         nr = adj_int_units_localized(self.results.msgs_total.reject_warning)
-        print(tpl_loc.format(val=nr, lbl='reject warnings'))
+        print(tpl_loc.format(val=nr, lbl=_('reject warnings')))
         nr = adj_int_units_localized(self.results.msgs_total.held)
-        print(tpl_loc.format(val=nr, lbl='held'))
+        print(tpl_loc.format(val=nr, lbl=_('held')))
         nr = adj_int_units_localized(self.results.msgs_total.discarded)
-        print(tpl_loc.format(val=nr, lbl='discarded'), end='')
+        print(tpl_loc.format(val=nr, lbl=_('discarded')), end='')
         print(' ({:0.1f}%)'.format(msgs_discarded_pct))
         print()
 
         nr = adj_int_units_localized(self.results.msgs_total.bytes_received)
-        print(tpl_loc.format(val=nr, lbl='bytes received'))
+        print(tpl_loc.format(val=nr, lbl=_('bytes received')))
         nr = adj_int_units_localized(self.results.msgs_total.bytes_delivered)
-        print(tpl_loc.format(val=nr, lbl='bytes delivered'))
+        print(tpl_loc.format(val=nr, lbl=_('bytes delivered')))
         nr = adj_int_units_localized(self.results.msgs_total.sending_users)
-        print(tpl_loc.format(val=nr, lbl='senders'))
+        print(tpl_loc.format(val=nr, lbl=_('senders')))
         nr = adj_int_units_localized(self.results.msgs_total.sending_domains)
-        print(tpl_loc.format(val=nr, lbl='sending hosts/domains'))
+        print(tpl_loc.format(val=nr, lbl=_('sending hosts/domains')))
         nr = adj_int_units_localized(self.results.msgs_total.rcpt_users)
-        print(tpl_loc.format(val=nr, lbl='recipients'))
+        print(tpl_loc.format(val=nr, lbl=_('recipients')))
         nr = adj_int_units_localized(self.results.msgs_total.rcpt_domains)
-        print(tpl_loc.format(val=nr, lbl='recipients hosts/domains'))
+        print(tpl_loc.format(val=nr, lbl=_('recipients hosts/domains')))
 
         print()
 
     # -------------------------------------------------------------------------
     def print_subsect_title(self, title, nr_items=1, count=None, quiet=None):
         """Printing the title of a sub section."""
         msg = str(title)
         if quiet is None:
             quiet = self.quiet
         print()
 
         if not nr_items:
             if not quiet:
-                msg += ': None'
+                msg += ': ' + _('None')
                 print(msg)
             return False
 
         if count:
-            msg += ' ({lbl}: {c})'.format(lbl='top', c=count)
+            msg += ' ({lbl}: {c})'.format(lbl=_('top'), c=count)
 
         print(msg)
         print('-' * len(msg))
 
         return True
 
     # -------------------------------------------------------------------------
@@ -1168,29 +1215,29 @@
             avg_time = (time_conn / total_conn) + 0.5
         total_time_splitted = get_smh(time_conn)
 
         print()
         print('Smtpd:')
         print()
 
-        print(tpl_loc.format(val=adj_int_units_localized(total_conn), lbl='connections'))
-        print(tpl_loc.format(val=adj_int_units_localized(count_domains), lbl='hosts/domains'))
+        print(tpl_loc.format(val=adj_int_units_localized(total_conn), lbl=_('connections')))
+        print(tpl_loc.format(val=adj_int_units_localized(count_domains), lbl=_('hosts/domains')))
         print(tpl_loc.format(
-            val=adj_int_units_localized(avg_time, no_unit=True), lbl='connections'))
+            val=adj_int_units_localized(avg_time, no_unit=True), lbl=_('connections')))
         print('  {h:d}:{m:02d}:{s:02.0f}  {lbl}'.format(
             h=total_time_splitted[2], m=total_time_splitted[1],
-            s=total_time_splitted[0], lbl='total connect time'))
+            s=total_time_splitted[0], lbl=_('total connect time')))
         print()
 
     # -------------------------------------------------------------------------
     def print_nested_hash(self, data, label, count):
         if not len(data.keys()):
             if self.quiet:
                 return
-            print('\n{lbl}: {n}'.format(lbl=label, n='none'))
+            print('\n{lbl}: {n}'.format(lbl=label, n=_('none')))
             return
         print('\n{lbl}'.format(lbl=label))
         print('-' * len(label))
         self.walk_nested_hash(data, count)
 
     # -------------------------------------------------------------------------
     def walk_nested_hash(self, data, count, level=0):
@@ -1206,35 +1253,35 @@
         if isinstance(first_value, dict):
             for key in sorted_keys:
                 print('{i}{k}'.format(i=indent, k=key), end='')
                 first_key2 = sorted(data[key].keys(), key=str.lower)[0]
                 first_value2 = data[key][first_key2]
                 if not isinstance(first_value2, dict):
                     if count is not None and count > 0:
-                        print(' ({lbl}: {c})'.format(lbl='top', c=count), end='')
+                        print(' ({lbl}: {c})'.format(lbl=_('top'), c=count), end='')
                     total_count = 0
                     for key2 in data[key].keys():
                         total_count += data[key][key2]
                     val = adj_int_units_localized(total_count, no_unit=True).rstrip()
-                    print(' ({lbl}: {c})'.format(lbl='total', c=val), end='')
+                    print(' ({lbl}: {c})'.format(lbl=_('total'), c=val), end='')
                 print()
                 self.walk_nested_hash(data[key], count, level)
         else:
             self.really_print_hash_by_cnt_vals(data, count, indent)
 
     # -------------------------------------------------------------------------
     def print_hash_by_cnt_vals(self, data, title, count):
         """Print hash contents sorted by numeric values in descending
         order (i.e.: highest first)."""
         if count:
             title = "{top} {c} ".format(top="top", c=count) + title
         if not len(data.keys()):
             if self.quiet:
                 return
-            print('\n{lbl}: {n}'.format(lbl=title, n='none'))
+            print('\n{lbl}: {n}'.format(lbl=title, n=_('none')))
             return
 
         print('\n{lbl}'.format(lbl=title))
         print('-' * len(title))
 
         self.really_print_hash_by_cnt_vals(data, count, ' ')
 
@@ -1275,63 +1322,63 @@
                 break
 
     # -------------------------------------------------------------------------
     def print_problems_reports(self):
         """Print "problems" reports."""
         if self.detail_deferral != 0:
             self.print_nested_hash(
-                data=self.results.deferred, label="Message deferral detail",
+                data=self.results.deferred, label=_("Message deferral detail"),
                 count=self.detail_deferral)
 
         if self.detail_bounce != 0:
             self.print_nested_hash(
-                data=self.results.bounced, label="Message bounce detail (by relay)",
+                data=self.results.bounced, label=_("Message bounce detail (by relay)"),
                 count=self.detail_bounce)
 
         if self.detail_reject != 0:
             self.print_nested_hash(
-                data=self.results.rejects, label="Message reject detail",
+                data=self.results.rejects, label=_("Message reject detail"),
                 count=self.detail_reject)
             self.print_nested_hash(
-                data=self.results.warnings, label="Message reject warning detail",
+                data=self.results.warnings, label=_("Message reject warning detail"),
                 count=self.detail_reject)
             self.print_nested_hash(
-                data=self.results.holds, label="Message hold detail",
+                data=self.results.holds, label=_("Message hold detail"),
                 count=self.detail_reject)
             self.print_nested_hash(
-                data=self.results.discards, label="Message discard detail",
+                data=self.results.discards, label=_("Message discard detail"),
                 count=self.detail_reject)
 
         if self.detail_smtp != 0:
             self.print_nested_hash(
-                data=self.results.smtp_messages, label="SMTP delivery failures",
+                data=self.results.smtp_messages, label=_("SMTP delivery failures"),
                 count=self.detail_smtp)
 
         if self.detail_smtpd_warning != 0:
             self.print_nested_hash(
-                data=self.results.warnings, label="Warnings", count=self.detail_smtpd_warning)
+                data=self.results.warnings, label=_("Warnings"), count=self.detail_smtpd_warning)
 
-        self.print_nested_hash(data=self.results.fatals, label="Fatal Errors", count=0)
-        self.print_nested_hash(data=self.results.panics, label="Panics", count=0)
+        self.print_nested_hash(data=self.results.fatals, label=_("Fatal Errors"), count=0)
+        self.print_nested_hash(data=self.results.panics, label=_("Panics"), count=0)
         self.print_hash_by_cnt_vals(
-            data=self.results.master_msgs, title='Master daemon messages', count=0)
+            data=self.results.master_msgs, title=_('Master daemon messages'), count=0)
 
     # -------------------------------------------------------------------------
     def print_per_day_summary(self):
         """Print "per-day" traffic summary."""
-        self.print_subsect_title("Per-Day Traffic Summary")
+        self.print_subsect_title(_("Per-Day Traffic Summary"))
         indent = '  '
 
         labels = {
-            'date': 'Date',
-            'received': 'Received',
-            'sent': 'Delivered',
-            'deferred': 'Deferred',
-            'bounced': 'Bounced',
-            'rejected': 'Rejected',
+            'date': _('Date'),
+            'received': _('Received'),
+            'sent': _('Delivered'),
+            'deferred': _('Deferred'),
+            'bounced': _('Bounced'),
+            'rejected': _('Rejected'),
         }
         widths = {
             'date': 12,
             'received': 11,
             'sent': 11,
             'deferred': 11,
             'bounced': 11,
@@ -1376,27 +1423,28 @@
 
     # -------------------------------------------------------------------------
     def print_per_hour_summary(self):
         """Print "per-hour" traffic summary."""
         indent = '  '
 
         if self.nr_days == 1:
-            title = 'Per-Hour Traffic Summary'
+            title = _('Per-Hour Traffic Summary')
         else:
-            title = 'Per-Hour Traffic Daily Average'
+            title = _('Per-Hour Traffic Daily Average')
         self.print_subsect_title(title)
 
         labels = {
-            'hour': 'Hour',
-            'received': 'Received',
-            'sent': 'Delivered',
-            'deferred': 'Deferred',
-            'bounced': 'Bounced',
-            'rejected': 'Rejected',
+            'hour': _('Hour'),
+            'received': _('Received'),
+            'sent': _('Delivered'),
+            'deferred': _('Deferred'),
+            'bounced': _('Bounced'),
+            'rejected': _('Rejected'),
         }
+
         widths = {
             'hour': 13,
             'received': 11,
             'sent': 11,
             'deferred': 11,
             'bounced': 11,
             'rejected': 11,
@@ -1472,26 +1520,26 @@
     def print_recip_domain_summary(self):
         """Print "per-recipient-domain" traffic summary."""
         indent = '  '
         count = self.detail_host
         if count == 0:
             return
 
-        title = 'Host/Domain Summary: Message Delivery'
+        title = _('Host/Domain Summary: Message Delivery')
         nr_items = len(self.results.rcpt_domain.keys())
         if not self.print_subsect_title(title, nr_items=nr_items, count=count):
             return
 
         labels = {
-            'sent': 'Sent count',
-            'bytes': 'Bytes',
-            'defers': 'Defers',
-            'avg_delay': 'Avg. delay',
-            'max_delay': 'Max. delay',
-            'domain': 'Host/Domain',
+            'sent': _('Sent count'),
+            'bytes': _('Bytes'),
+            'defers': _('Defers'),
+            'avg_delay': _('Avg. delay'),
+            'max_delay': _('Max. delay'),
+            'domain': _('Host/Domain'),
         }
         widths = {
             'sent': 8,
             'bytes': 8,
             'defers': 8,
             'avg_delay': 8,
             'max_delay': 8,
@@ -1542,23 +1590,23 @@
     def print_sending_domain_summary(self):
         """Print "per-sender-domain" traffic summary."""
         indent = '  '
         count = self.detail_host
         if count == 0:
             return
 
-        title = 'Host/Domain Summary: Messages Received'
+        title = _('Host/Domain Summary: Messages Received')
         nr_items = len(self.results.sending_domain_data.keys())
         if not self.print_subsect_title(title, nr_items=nr_items, count=count):
             return
 
         labels = {
-            'received': 'Message count',
-            'bytes': 'Bytes',
-            'domain': 'Host/Domain',
+            'received': _('Message count'),
+            'bytes': _('Bytes'),
+            'domain': _('Host/Domain'),
         }
         widths = {
             'received': 8,
             'bytes': 8,
             'domain': 20,
         }
 
@@ -1590,27 +1638,27 @@
             i += 1
             if count is not None and i >= count:
                 break
 
     # -------------------------------------------------------------------------
     def print_per_day_smtpd(self):
         """print "per-day" smtpd connection summary"""
-        title = 'Per-Day SMTPD Connection Summary'
+        title = _('Per-Day SMTPD Connection Summary')
         indent = '  '
 
         nr_items = len(self.results.smtpd_per_day.keys())
         if not self.print_subsect_title(title, nr_items=nr_items):
             return
 
         labels = {
-            'date': 'Date',
-            'connections': 'Connections',
-            'time_conn': 'Time connections total',
-            'avg_time': 'Avg. time connection',
-            'max_time': 'Max. time connection',
+            'date': _('Date'),
+            'connections': _('Connections'),
+            'time_conn': _('Time connections total'),
+            'avg_time': _('Avg. time connection'),
+            'max_time': _('Max. time connection'),
         }
         widths = {
             'date': 12,
             'connections': 11,
             'time_conn': 11,
             'avg_time': 11,
             'max_time': 11,
@@ -1657,31 +1705,31 @@
             print(indent + line)
 
     # -------------------------------------------------------------------------
     def print_per_hour_smtpd(self):
         """print 'per-hour' smtpd connection summary"""
         indent = '  '
         if self.nr_days == 1:
-            title = 'Per-Hour SMTPD Connection Summary'
+            title = _('Per-Hour SMTPD Connection Summary')
         else:
-            title = 'Per-Hour SMTPD Connection Daily Average'
+            title = _('Per-Hour SMTPD Connection Daily Average')
 
         conns_total = 0
         for stat in self.results.smtpd_messages_per_hour:
             conns_total += stat.count
 
         if not self.print_subsect_title(title, nr_items=conns_total):
             return
 
         labels = {
-            'hour': 'Hour',
-            'conn': 'Connections',
-            'time_total': 'Time total',
-            'time_avg': 'Time avg.',
-            'time_max': 'Time max.',
+            'hour': _('Hour'),
+            'conn': _('Connections'),
+            'time_total': _('Time total'),
+            'time_avg': _('Time avg.'),
+            'time_max': _('Time max.'),
         }
 
         widths = {
             'hour': 13,
             'conn': 11,
             'time_total': 11,
             'time_avg': 11,
@@ -1750,25 +1798,25 @@
     def print_domain_smtpd_summary(self):
         """print 'per-domain-smtpd' connection summary"""
         indent = '  '
         count = self.detail_host
         if count == 0:
             return
 
-        title = 'Host/Domain Summary: SMTPD Connections'
+        title = _('Host/Domain Summary: SMTPD Connections')
         nr_items = len(self.results.smtpd_per_domain.keys())
         if not self.print_subsect_title(title, nr_items=nr_items, count=count):
             return
 
         labels = {
-            'conn': 'Connections',
-            'time_total': 'Time total',
-            'time_avg': 'Time avg.',
-            'time_max': 'Time max.',
-            'domain': 'Host/Domain',
+            'conn': _('Connections'),
+            'time_total': _('Time total'),
+            'time_avg': _('Time avg.'),
+            'time_max': _('Time max.'),
+            'domain': _('Host/Domain'),
         }
 
         widths = {
             'conn': 11,
             'time_total': 11,
             'time_avg': 11,
             'time_max': 11,
@@ -1797,15 +1845,15 @@
             time_total = self.results.smtpd_per_domain[domain].connect_time_total
             max_time = self.results.smtpd_per_domain[domain].connect_time_max
 
             total_time_splitted = get_smh(time_total)
             avg = time_total / nr
 
             if domain is None:
-                domain = '<None>'
+                domain = _('<None>')
 
             values = {
                 'conn': 0,
                 'time_total': 0,
                 'time_avg': 0,
                 'time_max': 0,
                 'domain': domain,
```

### Comparing `postfix_logsums-0.8.0/postfix_logsums/errors.py` & `postfix_logsums-0.9.0/postfix_logsums/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 @summary: a module for all error (exception) classes used in this package
 
 @author: Frank Brehm
 @contact: frank@brehm-online.com
 @copyright: © 2023 by Frank Brehm, Berlin
 """
 
-__version__ = '0.4.0'
+from .xlate import XLATOR
+
+__version__ = '0.5.0'
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
 __copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
+_ = XLATOR.gettext
+
 
 # =============================================================================
 class PostfixLogsumsError(Exception):
     """Base error class for all exceptions in this package."""
 
     pass
 
@@ -38,17 +42,17 @@
         self.err_msg = err_msg
         super(WrongDateKeyError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
         if self.err_msg:
-            msg = "Invalid key {k!r} for a {what}, must be valid date: {e}"
+            msg = _("Invalid key {k!r} for a {what}, must be valid date: {e}")
         else:
-            msg = "Invalid key {k!r} for a {what}, must be valid date."
+            msg = _("Invalid key {k!r} for a {what}, must be valid date.")
         return msg.format(k=self.key, what='DailyStatsDict', e=self.err_msg)
 
 # =============================================================================
 class WrongDailyKeyError(StatsError, KeyError):
     """Error class for a invalid key for a DailyStatsDict."""
 
     # -------------------------------------------------------------------------
@@ -58,17 +62,17 @@
         self.err_msg = err_msg
         super(WrongDailyKeyError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
         if self.err_msg:
-            msg = "Key error for key {k!r} for a {what}: {e}"
+            msg = _("Key error for key {k!r} for a {what}: {e}")
         else:
-            msg = "Key error for {k!r} for a {what}."
+            msg = _("Key error for {k!r} for a {what}.")
         return msg.format(k=self.key, what='DailyStatsDict', e=self.err_msg)
 
 # =============================================================================
 class WrongMsgStatsAttributeError(StatsError, AttributeError):
     """Error class for a wrong attribute in a MessageStats object."""
 
     # -------------------------------------------------------------------------
@@ -77,15 +81,15 @@
         self.attribute = attribute
         self.class_name = class_name
         super(WrongMsgStatsAttributeError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Invalid attribute {attr!r} for a {w} object."
+        msg = _("Invalid attribute {attr!r} for a {w} object.")
         return msg.format(attr=self.attribute, w=self.class_name)
 
 
 # =============================================================================
 class WrongMsgStatsValueError(StatsError, ValueError):
     """Error class for a wrong value for a MessageStats value."""
 
@@ -103,15 +107,15 @@
         self.key = key
         self.obj_type = obj_type
         super(WrongMsgStatsKeyError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Invalid key {k!r} for a {w} object."
+        msg = _("Invalid key {k!r} for a {w} object.")
         return msg.format(k=self.key, w=self.obj_type)
 
 
 # =============================================================================
 class WrongMsgPerDayKeyError(StatsError, KeyError):
     """Error class for a wrong key for the MessageStatsPerDay object."""
 
@@ -122,15 +126,15 @@
         self.key = key
         self.obj_type = obj_type
         super(WrongMsgPerDayKeyError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Invalid key {k!r} for a {w} object."
+        msg = _("Invalid key {k!r} for a {w} object.")
         return msg.format(k=self.key, w=self.obj_type)
 
 
 # =============================================================================
 class WrongMsgStatsHourError(StatsError, KeyError):
     """Error class for a wrong hour for the HourlyStats object."""
 
@@ -141,15 +145,15 @@
         self.hour = hour
         self.obj_type = obj_type
         super(WrongMsgStatsHourError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Invalid hour {h!r} for a {w} object."
+        msg = _("Invalid hour {h!r} for a {w} object.")
         return msg.format(h=self.hour, w=self.obj_type)
 
 
 # =============================================================================
 class MsgStatsHourValNotfoundError(StatsError, ValueError):
     """Error class for a value not found error in the HourlyStats class."""
 
@@ -160,15 +164,15 @@
         self.value = value
         self.obj_type = obj_type
         super(MsgStatsHourValNotfoundError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Value {v!r} not found in the {w} object."
+        msg = _("Value {v!r} not found in the {w} object.")
         return msg.format(v=self.value, w=self.obj_type)
 
 
 # =============================================================================
 class MsgStatsHourInvalidMethodError(StatsError, RuntimeError):
     """Error class for an invalid method used with a HourlyStats class object."""
 
@@ -179,15 +183,15 @@
         self.method = method
         self.obj_type = obj_type
         super(MsgStatsHourInvalidMethodError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Invalid method {m}() for a {w} object."
+        msg = _("Invalid method {m}() for a {w} object.")
         return msg.format(m=self.method, w=self.obj_type)
 
 
 # =============================================================================
 
 if __name__ == "__main__":
```

### Comparing `postfix_logsums-0.8.0/postfix_logsums/results.py` & `postfix_logsums-0.9.0/postfix_logsums/results.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/postfix_logsums/stats.py` & `postfix_logsums-0.9.0/postfix_logsums/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,23 @@
     from collections import MutableMapping, Mapping, MutableSequence, Sequence
 
 # Own modules
 from .errors import StatsError, WrongDateKeyError, WrongMsgStatsKeyError, WrongDailyKeyError
 from .errors import MsgStatsHourValNotfoundError, MsgStatsHourInvalidMethodError
 from .errors import WrongMsgStatsAttributeError, WrongMsgStatsValueError
 
-__version__ = '0.7.1'
+from .xlate import XLATOR
+
+__version__ = '0.8.0'
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
 __copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 HOURS_PER_DAY = 24
 LOG = logging.getLogger(__name__)
+_ = XLATOR.gettext
 
 # =============================================================================
 def is_sequence(arg):
     """Return, whether the given value is a sequential object, but nat a str."""
     if not isinstance(arg, Sequence):
         return False
 
@@ -61,15 +64,15 @@
             #     t=type(first_param), p=first_param))
 
             if isinstance(first_param, Mapping):
                 self._update_from_mapping(first_param)
             elif first_param.__class__.__name__ == 'zip':
                 self._update_from_mapping(dict(first_param))
             else:
-                msg = "Object is not a {m} object, but a {w} object instead.".format(
+                msg = _("Object is not a {m} object, but a {w} object instead.").format(
                     m='Mapping', w=first_param.__class__.__qualname__)
                 raise StatsError(msg)
 
         if kwargs:
             self._update_from_mapping(kwargs)
 
     # -------------------------------------------------------------------------
@@ -92,29 +95,29 @@
 
         if name not in self.valid_keys:
             raise WrongMsgStatsAttributeError(name, self.__class__.__name__)
 
         try:
             v = int(value)
         except ValueError as e:
-            msg = "Wrong value {v!r} for a {w} value: {e}".format(
+            msg = _("Wrong value {v!r} for a {w} value: {e}").format(
                 v=value, w=self.__class__.__name__, e=e)
             raise WrongMsgStatsValueError(msg)
 
         if v < 0:
-            msg = "Wrong value {v!r} for a {w} value: must be >= 0".format(
+            msg = _("Wrong value {v!r} for a {w} value: must be >= 0").format(
                 v=value, w=self.__class__.__name__)
             raise WrongMsgStatsValueError(msg)
 
         self._values[name] = v
 
     # -------------------------------------------------------------------------
     def __delattr__(self, name):
         """Called, if an attribute should be deleted."""
-        msg = "Deleting attribute {a!r} of a {w} is not allowed.".format(
+        msg = _("Deleting attribute {a!r} of a {w} is not allowed.").format(
             a=name, w=self.__class__.__name__)
         raise StatsError(msg)
 
     # -------------------------------------------------------------------------
     def _update_from_mapping(self, mapping):
 
         for key in mapping.keys():
@@ -376,29 +379,30 @@
 
     # -------------------------------------------------------------------------
     def __init__(self, stats_class=BaseMessageStats, first_param=None, **kwargs):
         """Constructor."""
 
         self._stats = {}
         if not issubclass(stats_class, BaseMessageStats):
-            msg = "Wrong class {c} for using as an item class, must be a subclas of {sc}.".format(
+            msg = _(
+                "Wrong class {c} for using as an item class, must be a subclas of {sc}.").format(
                 c=stats_class.__name__, sc='BaseMessageStats')
             raise TypeError(msg)
         self._stats_class = stats_class
 
         if first_param is not None:
 
             if isinstance(first_param, self.__class__):
                 self._update_from_other(first_param)
             elif isinstance(first_param, Mapping):
                 self._update_from_mapping(first_param)
             elif first_param.__class__.__name__ == 'zip':
                 self._update_from_mapping(dict(first_param))
             else:
-                msg = "Object is not a {m} object, but a {w} object instead.".format(
+                msg = _("Object is not a {m} object, but a {w} object instead.").format(
                     m='Mapping', w=first_param.__class__.__qualname__)
                 raise StatsError(msg)
 
         if kwargs:
             self._update_from_mapping(kwargs)
 
     # -------------------------------------------------------------------------
@@ -576,15 +580,15 @@
 
     # -------------------------------------------------------------------------
     def pop(self, key, *args):
         """Remove and return an arbitrary element from the dict."""
         used_key = self.key_to_date(key)
 
         if len(args) > 1:
-            msg = "The method {met}() expected at most {max} arguments, got {got}.".format(
+            msg = _("The method {met}() expected at most {max} arguments, got {got}.").format(
                 met='pop', max=2, got=(len(args) + 1))
             raise TypeError(msg)
 
         if used_key not in self._stats:
             if args:
                 return args[0]
             raise WrongDailyKeyError(key)
@@ -627,15 +631,15 @@
         if isinstance(other, self.__class__):
             self._update_from_other(other)
         elif isinstance(other, Mapping):
             self._update_from_mapping(other)
         elif other.__class__.__name__ == 'zip':
             self._update_from_mapping(dict(other))
         else:
-            msg = "Object is not a {m} object, but a {w} object instead.".format(
+            msg = _("Object is not a {m} object, but a {w} object instead.").format(
                 m='Mapping', w=other.__class__.__qualname__)
             raise StatsError(msg)
 
     # -------------------------------------------------------------------------
     def _update_from_other(self, other):
         if not isinstance(other, self.__class__):
             raise StatsError("Wtf, not a {} class?!?".format(self.__class__.__name__))
@@ -659,15 +663,15 @@
 
         self._list = []
         for hour in range(self.hours_per_day):
             self._list.append(0)
 
         if args:
             if len(args) > self.hours_per_day:
-                msg = "Invalid number {} of statistics per hour give.".format(len(args))
+                msg = _("Invalid number {} of statistics per hour given.").format(len(args))
                 raise StatsError(msg)
             index = 0
             for value in args:
                 self[index] = value
                 index += 1
 
     # -------------------------------------------------------------------------
@@ -744,18 +748,18 @@
 
     # -------------------------------------------------------------------------
     def __setitem__(self, hour, value):
         """Setting the value for the given hour."""
         try:
             v = int(value)
         except ValueError as e:
-            msg = "Wrong value {v!r} for a per hour stat: {e}".format(v=value, e=e)
+            msg = _("Wrong value {v!r} for a per hour stat: {e}").format(v=value, e=e)
             raise WrongMsgStatsValueError(msg)
         if v < 0:
-            msg = "Wrong value {v!r} for a per hour stat: must be >= 0".format(v=value)
+            msg = _("Wrong value {v!r} for a per hour stat: must be >= 0").format(v=value)
             raise WrongMsgStatsValueError(msg)
         self._list[hour] = int(value)
 
     # -------------------------------------------------------------------------
     def __delitem__(self, hour):
         """Deleting an item in the list - invalid action."""
 
@@ -765,15 +769,15 @@
     def insert(self, hour, value):
         """Insert an item in the list - invalid action."""
 
         raise MsgStatsHourInvalidMethodError('insert')
 
     # -------------------------------------------------------------------------
     def append(self, value):
-        """iAppending the given value to the current list - invalid action."""
+        """Appending the given value to the current list - invalid action."""
 
         raise MsgStatsHourInvalidMethodError('append')
 
     # -------------------------------------------------------------------------
     def reverse(self):
         """Reverses the values of the current list in place."""
 
@@ -816,15 +820,15 @@
 
         self._list = []
         for hour in range(self.hours_per_day):
             self._list.append(SmtpdStatsPerHour())
 
         if args:
             if len(args) > self.hours_per_day:
-                msg = "Invalid number {} of statistics per hour give.".format(len(args))
+                msg = _("Invalid number {} of statistics per hour given.").format(len(args))
                 raise StatsError(msg)
             index = 0
             for value in args:
                 if value is not None:
                     self[index] = value
                 index += 1
 
@@ -833,15 +837,15 @@
         """Setting the value for the given hour."""
         if isinstance(value, SmtpdStatsPerHour):
             self._list[hour] = value
             return
 
         if isinstance(value, (list, tuple)):
             if len(value) != 3:
-                msg = (
+                msg = _(
                     "Wrong value {v!r} for a per hour stat of smtp - "
                     "must have three numbers.").format(v=value)
                 raise WrongMsgStatsValueError(msg)
             v = SmtpdStatsPerHour()
             v[0] = value[0]
             v[1] = value[1]
             v[2] = value[2]
@@ -849,15 +853,15 @@
             return
 
         if isinstance(value, dict):
             v = SmtpdStatsPerHour(**value)
             self._list[hour] = v
             return
 
-        msg = "Wrong value {v!r} for a per hour stat.".format(v=value)
+        msg = _("Wrong value {v!r} for a per hour stat.").format(v=value)
         raise WrongMsgStatsValueError(msg)
 
     # -------------------------------------------------------------------------
     def as_list(self, pure=False):
         """Typecasting into a simple list."""
         vals = []
         for stat in self:
```

### Comparing `postfix_logsums-0.8.0/postfix_logsums.egg-info/PKG-INFO` & `postfix_logsums-0.9.0/postfix_logsums.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix-logsums
-Version: 0.8.0
+Version: 0.9.0
 Summary: Produce Postfix MTA logfile summary
 Home-page: https://github.com/pixelpark/postfix-logsums
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `postfix_logsums-0.8.0/setup.cfg` & `postfix_logsums-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/setup.py` & `postfix_logsums-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/test/test_00_errors.py` & `postfix_logsums-0.9.0/test/test_00_errors.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/test/test_05_stats_collections.py` & `postfix_logsums-0.9.0/test/test_05_stats_collections.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.8.0/test/test_10_results.py` & `postfix_logsums-0.9.0/test/test_10_results.py`

 * *Files identical despite different names*


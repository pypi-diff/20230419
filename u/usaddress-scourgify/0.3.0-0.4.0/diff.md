# Comparing `tmp/usaddress-scourgify-0.3.0.tar.gz` & `tmp/usaddress-scourgify-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fable/CodeProjects/GBR/usaddress-scourgify/dist/tmpx4fit9ef/usaddress-scourgify-0.3.0.tar", last modified: Tue Apr 18 17:00:11 2023, max compression
+gzip compressed data, was "/home/fable/CodeProjects/GBR/usaddress-scourgify/dist/tmp7eec17wl/usaddress-scourgify-0.4.0.tar", last modified: Wed Apr 19 18:17:29 2023, max compression
```

## Comparing `usaddress-scourgify-0.3.0.tar` & `usaddress-scourgify-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:59:14.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      803 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/scourgify/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/scourgify/tests/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/tests/test_cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/scourgify/tests/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/tests/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27406 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/tests/test_address_normalization.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4243 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/validations.py
--rw-r--r--   0 root         (0) root         (0)     8940 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/cleaning.py
--rw-r--r--   0 root         (0) root         (0)    33262 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/normalize.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16206 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/address_constants.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5242 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:59:14.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      803 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/scourgify/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/scourgify/tests/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/tests/test_cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/scourgify/tests/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/tests/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28157 2023-04-19 18:10:27.000000 usaddress-scourgify-0.4.0/scourgify/tests/test_address_normalization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4717 2023-04-19 18:09:29.000000 usaddress-scourgify-0.4.0/scourgify/validations.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/cleaning.py
+-rw-r--r--   0 root         (0) root         (0)    33255 2023-04-19 17:21:34.000000 usaddress-scourgify-0.4.0/scourgify/normalize.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-18 16:58:50.000000 usaddress-scourgify-0.4.0/scourgify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16206 2023-04-18 16:58:50.000000 usaddress-scourgify-0.4.0/scourgify/address_constants.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5591 2023-04-19 17:55:25.000000 usaddress-scourgify-0.4.0/README.rst
```

### Comparing `usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/SOURCES.txt` & `usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/PKG-INFO` & `usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.3.0
+Version: 0.4.0
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
```

### Comparing `usaddress-scourgify-0.3.0/LICENSE` & `usaddress-scourgify-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.3.0/scourgify/exceptions.py` & `usaddress-scourgify-0.4.0/scourgify/exceptions.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.3.0/scourgify/tests/test_cleaning.py` & `usaddress-scourgify-0.4.0/scourgify/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.3.0/scourgify/tests/test_address_normalization.py` & `usaddress-scourgify-0.4.0/scourgify/tests/test_address_normalization.py`

 * *Files 3% similar despite different names*

```diff
@@ -575,32 +575,52 @@
         with self.assertRaises(IncompleteAddressError):
             validate_address_components(minus_city_state_zip)
 
     def test_validate_postal_code(self):
         """Test validate_us_postal_code_format"""
 
         with self.assertRaises(AddressValidationError):
-            zip_plus = '97219-0001-00'
-            validate_us_postal_code_format(zip_plus, self.address_dict)
+            zip_five = 'AAAAA'
+            validate_us_postal_code_format(zip_five, self.address_dict)
+
+        with self.assertRaises(AddressValidationError):
+            zip_five = '97219-AAAA'
+            validate_us_postal_code_format(zip_five, self.address_dict)
 
         with self.assertRaises(AddressValidationError):
-            zip_plus = '97219-00'
+            zip_plus = '97219-000100'
             validate_us_postal_code_format(zip_plus, self.address_dict)
 
         with self.assertRaises(AddressValidationError):
-            zip_plus = '972-0001'
+            zip_plus = '97219-0001-00'
             validate_us_postal_code_format(zip_plus, self.address_dict)
 
         with self.assertRaises(AddressValidationError):
             zip_five = '9721900'
             validate_us_postal_code_format(zip_five, self.address_dict)
 
-        with self.assertRaises(AddressValidationError):
-            zip_five = '972'
-            validate_us_postal_code_format(zip_five, self.address_dict)
+        zip_five = '972'
+        expected = '00972'
+        result = validate_us_postal_code_format(zip_five, self.address_dict)
+        self.assertEqual(expected, result)
+
+        zip_plus = '97219-00'
+        expected = '97219-0000'
+        result = validate_us_postal_code_format(zip_plus, self.address_dict)
+        self.assertEqual(expected, result)
+
+        zip_plus = '972-0001'
+        expected = '00972-0001'
+        result = validate_us_postal_code_format(zip_plus, self.address_dict)
+        self.assertEqual(expected, result)
+
+        zip_plus = '972190001'
+        expected = '97219-0001'
+        result = validate_us_postal_code_format(zip_plus, self.address_dict)
+        self.assertEqual(expected, result)
 
         expected = '97219'
         result = validate_us_postal_code_format(expected, self.address_dict)
         self.assertEqual(expected, result)
 
     def test_get_addr_line_str(self):
         """Test get_addr_line_str function."""
```

### Comparing `usaddress-scourgify-0.3.0/scourgify/validations.py` & `usaddress-scourgify-0.4.0/scourgify/validations.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,22 +93,36 @@
     :rtype: str
     """
     error = None
     msg = (
         'US Postal Codes must conform to five-digit Zip or Zip+4 standards.'
     )
     postal_code = post_clean_addr_str(postal_code)
-    if '-' in postal_code:
-        plus_four_code = postal_code.split('-')
-        if len(plus_four_code) != 2:
+    plus_four_code = postal_code.split('-')
+    for code in plus_four_code:
+        try:
+            int(code)
+        except ValueError:
             error = True
-        elif len(plus_four_code[0]) != 5 or len(plus_four_code[1]) != 4:
+    if not error:
+        if '-' in postal_code:
+            if len(postal_code.replace('-', '')) > 9:
+                error = True
+            elif len(plus_four_code) != 2:
+                error = True
+            else:
+                postal_code = '-'.join([
+                    plus_four_code[0].zfill(5), plus_four_code[1].zfill(4)
+                ])
+        elif len(postal_code) == 9:
+            postal_code = '-'.join([postal_code[:5], postal_code[5:]])
+        elif len(postal_code) > 5:
             error = True
-    elif len(postal_code) != 5:
-        error = True
+        else:
+            postal_code = postal_code.zfill(5)
 
     if error:
         raise AddressValidationError(msg, None, address)
     else:
         return postal_code
```

### Comparing `usaddress-scourgify-0.3.0/scourgify/cleaning.py` & `usaddress-scourgify-0.4.0/scourgify/cleaning.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.3.0/scourgify/normalize.py` & `usaddress-scourgify-0.4.0/scourgify/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         addr_str.
     :type state: str
     :param zipcode: optional str postal code that does not need to be parsed
         from addr_str.
     :type zipcode: str
     :param addtl_funcs: optional sequence of funcs that take string for further
         processing and return line1 and line2 strings
-    :type addtl_funcs: Sequence[Callable[str, (str, str)]]
+    :type addtl_funcs: Sequence[Callable[str, (str)]]
     :return: address dict with uppercase parsed and normalized address values.
     :rtype: Mapping[str, str]
     """
     # get address parsed into usaddress components.
     error = None
     parsed_addr = None
     addr_str = pre_clean_addr_str(addr_str, normalize_state(state))
@@ -237,15 +237,15 @@
             parsed_addr, LINE1_USADDRESS_LABELS
         )
         validate_parens_groups_parsed(line1)
     else:
         # line1 is set to addr_str so complete dict can be passed to error.
         line1 = addr_str
 
-    addr_rec = dict(
+    addr_rec = OrderedDict(
         address_line_1=line1, address_line_2=line2, city=city,
         state=state, postal_code=zipcode
     )
     if error:
         raise UnParseableAddressError(None, None, addr_rec)
     else:
         return addr_rec
@@ -413,15 +413,19 @@
     :return: str | None
     """
     val_from_parse = parsed_addr.get(val_label)
     orig_val = post_clean_addr_str(orig_val)
     val_from_parse = post_clean_addr_str(val_from_parse)
     non_null_val_set = {orig_val, val_from_parse} - {None}
     if len(non_null_val_set) > 1:
-        raise AmbiguousAddressError(None, None, orig_addr_str)
+        msg = (
+            f'Parsed {val_label} does not align with submitted value: '
+            f'Parsed: {val_from_parse}. Original: {orig_val}'
+        )
+        raise AmbiguousAddressError(None, msg, orig_addr_str)
     else:
         return non_null_val_set.pop() if non_null_val_set else None
 
 
 def normalize_address_components(parsed_addr):
     # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
     """Normalize parsed sections of address as appropriate.
@@ -694,36 +698,40 @@
     post_clean_addr_str = staticmethod(post_clean_addr_str)
     format_address_record = staticmethod(format_address_record)
     normalize_address_components = staticmethod(normalize_address_components)
     get_parsed_values = staticmethod(get_parsed_values)
 
     def __init__(self, address, addr_map=None, addtl_funcs=None, strict=None):
         self.address = address
-        self.addr_map = addr_map
         self.addtl_funcs = addtl_funcs
         self.strict = True if strict is None else strict
+        if addr_map and not isinstance(self.address, str):
+            self.address = {
+                key: self.address.get(val) for key, val in addr_map.items()
+            }
+
+    @staticmethod
+    def get_normalized_line_1(parsed_addr, line_labels=LINE1_USADDRESS_LABELS):
+        return get_normalized_line_segment(parsed_addr, line_labels)
+
+    @staticmethod
+    def get_normalized_line_2(parsed_addr, line_labels=LINE2_USADDRESS_LABELS):
+        return get_normalized_line_segment(parsed_addr, line_labels)
 
     def normalize(self):
         if isinstance(self.address, str):
-            return self.normalize_addr_str(
-                self.address, addtl_funcs=self.addtl_funcs
-            )
+            return self.normalize_addr_str(self.address)
         else:
-            return self.normalize_addr_dict(
-                self.address, addr_map=self.addr_map,
-                addtl_funcs=self.addtl_funcs, strict=self.strict
-            )
+            return self.normalize_addr_dict()
 
     def normalize_addr_str(self, addr_str,  # type: str
                            line2=None,  # type: Optional[str]
                            city=None,  # type: Optional[str]
                            state=None,  # type: Optional[str]
                            zipcode=None,  # type: Optional[str]
-                           addtl_funcs=None
-                           # type: Sequence[Callable[[str,str], str]]  # noqa
                            ):  # noqa
         # get address parsed into usaddress components.
         error = None
         parsed_addr = None
         addr_str = self.pre_clean_addr_str(addr_str, normalize_state(state))
         try:
             parsed_addr = self.parse_address_string(addr_str)
@@ -770,60 +778,54 @@
                 parsed_addr, state, 'StateName', addr_str
             )
             state = normalize_state(state)
 
             # assumes if line2 is passed in that it need not be parsed from
             # addr_str. Primarily used to allow advanced processing of
             # otherwise unparsable addresses.
-            line2 = line2 if line2 else get_normalized_line_segment(
-                parsed_addr, LINE2_USADDRESS_LABELS
-            )
+            line2 = line2 if line2 else self.get_normalized_line_2(parsed_addr)
             line2 = self.post_clean_addr_str(line2)
             # line 1 is fully post cleaned in get_normalized_line_segment.
-            line1 = get_normalized_line_segment(
-                parsed_addr, LINE1_USADDRESS_LABELS
-            )
+            line1 = self.get_normalized_line_1(parsed_addr)
             validate_parens_groups_parsed(line1)
         else:
             # line1 is set to addr_str so complete dict can be passed to error.
             line1 = addr_str
 
-        addr_rec = dict(
+        addr_rec = OrderedDict(
             address_line_1=line1, address_line_2=line2, city=city,
             state=state, postal_code=zipcode
         )
         if error:
             raise UnParseableAddressError(None, None, addr_rec)
         else:
             return addr_rec
 
-    def normalize_addr_dict(self, addr_dict, addr_map=None, addtl_funcs=None,
-                            strict=True):
-        if addr_map:
-            addr_dict = {key: addr_dict.get(val) for key, val in
-                         addr_map.items()}
-        addr_dict = validate_address_components(addr_dict, strict=strict)
+    def normalize_addr_dict(self):
+        addr_dict = validate_address_components(
+            self.address, strict=self.strict
+        )
 
         # line 1 and line 2 elements are combined to ensure consistent
         # processing whether the line 2 elements are pre-parsed or
         # included in line 1
         addr_str = get_addr_line_str(addr_dict, comma_separate=True)
         postal_code = addr_dict.get('postal_code')
         zipcode = validate_us_postal_code_format(
             postal_code, addr_dict
         ) if postal_code else None
         city = addr_dict.get('city')
         state = addr_dict.get('state')
         try:
             address = self.normalize_addr_str(
                 addr_str, city=city, state=state,
-                zipcode=zipcode, addtl_funcs=addtl_funcs
+                zipcode=zipcode
             )
         except AddressNormalizationError:
             addr_str = get_addr_line_str(
                 addr_dict, comma_separate=True, addr_parts=ADDRESS_KEYS
             )
             address = self.normalize_addr_str(
                 addr_str, city=city, state=state,
-                zipcode=zipcode, addtl_funcs=addtl_funcs
+                zipcode=zipcode
             )
         return address
```

### Comparing `usaddress-scourgify-0.3.0/scourgify/address_constants.py` & `usaddress-scourgify-0.4.0/scourgify/address_constants.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.3.0/setup.cfg` & `usaddress-scourgify-0.4.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = usaddress-scourgify
-version = 0.3.0
+version = 0.4.0
 description = Clean US addresses following USPS pub 28 and RESO guidelines
 author = Fable Turas
 author_email = fable@rainsoftware.tech
 maintainer = GreenBuildingRegistry
 maintainer_email = admin@greenbuildingregistry.com
 keywords = usaddress, normalization, address
 url = https://github.com/GreenBuildingRegistry/usaddress-scourgify
```

### Comparing `usaddress-scourgify-0.3.0/PKG-INFO` & `usaddress-scourgify-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.3.0
+Version: 0.4.0
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
```

### Comparing `usaddress-scourgify-0.3.0/README.rst` & `usaddress-scourgify-0.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,17 @@
             'postal_code': '97203'
         }
 
 normalized_address_record() uses the included processing functions to remove unacceptable special characters, extra spaces, predictable abnormal character sub-strings and phrases. It also abbreviates directional indicators and street types according to the abbreviation mappings found in address_constants.  If applicable, line 2 address elements (ie: Apt, Unit) are separated from line 1 inputs and standard occupancy type abbreviations are applied.
 
 You may supply additional additional processing functions as a list of callable supplied to the addtl_funcs parameter. Any additional functions should take a string address and return a tuple of strings (line1, line2).
 
+Postal codes are normalized to US zip or zip+4 and zero padded as applicable.  ie: `2129 => 02129`, `02129-44 => 02129-0044`, `021290044 => 02129-0044`.
+However, postal codes that cannot be effectively normalized, such as invalid length or invalid characters, will raise AddressValidationError. ie `12345678901 or 02129- or 02129-0044-123, etc`
+
 Alternately, you may extend the `NormalizeAddress` class to customize the normalization behavior by overriding any of the class' methods.
 
 If your address is in the form of a dict that does not use the keys address_line_1, address_line_2, city, state, and postal_code, you must supply a key map to the addr_map parameter in the format {standard_key: custom_key}
 
 
 .. code-block:: python
```


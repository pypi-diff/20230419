# Comparing `tmp/email_validator-2.0.0.dev4.tar.gz` & `tmp/email_validator-2.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_validator-2.0.0.dev4.tar", last modified: Mon Mar 13 12:56:33 2023, max compression
+gzip compressed data, was "email_validator-2.0.0.post1.tar", last modified: Sun Apr 16 20:15:04 2023, max compression
```

## Comparing `email_validator-2.0.0.dev4.tar` & `email_validator-2.0.0.post1.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/
--rw-rw-r--   0 user      (1000) user      (1000)     7048 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev4/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       53 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev4/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    22815 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21857 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev4/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-13 12:56:33.961168 email_validator-2.0.0.dev4/email_validator/
--rw-rw-r--   0 user      (1000) user      (1000)     4133 2023-03-13 12:54:36.000000 email_validator-2.0.0.dev4/email_validator/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev4/email_validator/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5749 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/deliverability.py
--rw-rw-r--   0 user      (1000) user      (1000)     4835 2023-03-13 12:53:03.000000 email_validator-2.0.0.dev4/email_validator/exceptions_types.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/py.typed
--rw-rw-r--   0 user      (1000) user      (1000)     1802 2023-03-10 16:29:14.000000 email_validator-2.0.0.dev4/email_validator/rfc_constants.py
--rw-rw-r--   0 user      (1000) user      (1000)    17571 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/syntax.py
--rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-03-10 16:29:23.000000 email_validator-2.0.0.dev4/email_validator/validate_email.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/email_validator.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    22815 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      543 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       29 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-13 12:56:33.000000 email_validator-2.0.0.dev4/email_validator.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       96 2023-02-04 18:50:03.000000 email_validator-2.0.0.dev4/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)     1367 2023-03-13 12:56:33.965168 email_validator-2.0.0.dev4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)       37 2021-11-17 12:22:14.000000 email_validator-2.0.0.dev4/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-16 20:15:04.413253 email_validator-2.0.0.post1/
+-rw-rw-r--   0 user      (1001) user      (1001)     7048 2018-11-18 15:32:44.000000 email_validator-2.0.0.post1/LICENSE
+-rw-rw-r--   0 user      (1001) user      (1001)       62 2023-04-16 13:11:30.000000 email_validator-2.0.0.post1/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)    25348 2023-04-16 20:15:04.413253 email_validator-2.0.0.post1/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)    24389 2023-04-16 01:18:22.000000 email_validator-2.0.0.post1/README.md
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-16 20:15:04.409253 email_validator-2.0.0.post1/email_validator/
+-rw-rw-r--   0 user      (1001) user      (1001)     4189 2023-04-15 21:26:20.000000 email_validator-2.0.0.post1/email_validator/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2146 2023-04-15 21:26:20.000000 email_validator-2.0.0.post1/email_validator/__main__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     5749 2023-04-16 00:27:55.000000 email_validator-2.0.0.post1/email_validator/deliverability.py
+-rw-rw-r--   0 user      (1001) user      (1001)     5524 2023-04-16 01:18:22.000000 email_validator-2.0.0.post1/email_validator/exceptions_types.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2720 2023-04-16 01:18:22.000000 email_validator-2.0.0.post1/email_validator/rfc_constants.py
+-rw-rw-r--   0 user      (1001) user      (1001)    23969 2023-04-15 21:26:36.000000 email_validator-2.0.0.post1/email_validator/syntax.py
+-rw-rw-r--   0 user      (1001) user      (1001)     9037 2023-04-16 01:18:22.000000 email_validator-2.0.0.post1/email_validator/validate_email.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-16 20:15:04.413253 email_validator-2.0.0.post1/email_validator.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)    25348 2023-04-16 20:15:04.000000 email_validator-2.0.0.post1/email_validator.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      631 2023-04-16 20:15:04.000000 email_validator-2.0.0.post1/email_validator.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-04-16 20:15:04.000000 email_validator-2.0.0.post1/email_validator.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       66 2023-04-16 20:15:04.000000 email_validator-2.0.0.post1/email_validator.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       29 2023-04-16 20:15:04.000000 email_validator-2.0.0.post1/email_validator.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       16 2023-04-16 20:15:04.000000 email_validator-2.0.0.post1/email_validator.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)     1348 2023-04-16 20:15:04.413253 email_validator-2.0.0.post1/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)       37 2021-05-09 18:39:53.000000 email_validator-2.0.0.post1/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-16 20:15:04.413253 email_validator-2.0.0.post1/tests/
+-rw-rw-r--   0 user      (1001) user      (1001)     1569 2023-02-11 14:49:29.000000 email_validator-2.0.0.post1/tests/mocked-dns-answers.json
+-rw-rw-r--   0 user      (1001) user      (1001)     4297 2023-03-04 18:27:39.000000 email_validator-2.0.0.post1/tests/mocked_dns_response.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2934 2023-04-16 00:27:55.000000 email_validator-2.0.0.post1/tests/test_deliverability.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2354 2023-04-16 01:18:22.000000 email_validator-2.0.0.post1/tests/test_main.py
+-rw-rw-r--   0 user      (1001) user      (1001)    36749 2023-04-16 01:18:22.000000 email_validator-2.0.0.post1/tests/test_syntax.py
```

### Comparing `email_validator-2.0.0.dev4/LICENSE` & `email_validator-2.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev4/PKG-INFO` & `email_validator-2.0.0.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email_validator
-Version: 2.0.0.dev4
+Version: 2.0.0.post1
 Summary: A robust email address syntax and deliverability validation library.
 Home-page: https://github.com/JoshData/python-email-validator
 Author: Joshua Tauberer
 Author-email: jt@occams.info
 License: CC0 (copyright waived)
 Keywords: email address validator
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,29 +33,31 @@
 users by their email address like on a registration/login form (but not
 necessarily for composing an email message, see below).
 
 Key features:
 
 * Checks that an email address has the correct syntax --- good for
   registration/login forms or other uses related to identifying users.
-  Rejects obsolete email address syntax that you'd find unexpected.
 * Gives friendly English error messages when validation fails that you
   can display to end-users.
 * Checks deliverability (optional): Does the domain name resolve?
   (You can override the default DNS resolver to add query caching.)
 * Supports internationalized domain names and internationalized local parts.
-  Blocks unsafe characters for your safety.
+* Rejects addresses with unsafe Unicode characters, obsolete email address
+  syntax that you'd find unexpected, special use domain names like
+  `@localhost`, and domains without a dot by default. This is an
+  opinionated library!
 * Normalizes email addresses (important for internationalized
-  addresses! see below).
+  and quoted-string addresses! see below).
+* Python type annotations are used.
 
-This library does NOT permit obsolete forms of email addresses, so
-if you need strict validation against the email specs exactly, use
-[pyIsEmail](https://github.com/michaelherold/pyIsEmail) or try
-[flanker](https://github.com/mailgun/flanker) if you are parsing the
-To: line of an email.
+This is an opinionated library. You should definitely also consider using
+the less-opinionated [pyIsEmail](https://github.com/michaelherold/pyIsEmail) and
+[flanker](https://github.com/mailgun/flanker) if they are better for your
+use case.
 
 [![Build Status](https://github.com/JoshData/python-email-validator/actions/workflows/test_and_build.yaml/badge.svg)](https://github.com/JoshData/python-email-validator/actions/workflows/test_and_build.yaml)
 
 View the [CHANGELOG / Release Notes](CHANGELOG.md) for the version history of changes in the library. Occasionally this README is ahead of the latest published package --- see the CHANGELOG for details.
 
 ---
 
@@ -75,29 +77,31 @@
 
 If you're validating a user's email address before creating a user
 account in your application, you might do this:
 
 ```python
 from email_validator import validate_email, EmailNotValidError
 
-email = "my+address@mydomain.tld"
-is_new_account = True # False for login pages
+email = "my+address@example.org"
 
 try:
-  # Check that the email address is valid.
-  validation = validate_email(email, check_deliverability=is_new_account)
 
-  # Take the normalized form of the email address
-  # for all logic beyond this point (especially
-  # before going to a database query where equality
-  # may not take into account Unicode normalization).  
-  email = validation.email
+  # Check that the email address is valid. Turn on check_deliverability
+  # for first-time validations like on account creation pages (but not
+  # login pages).
+  emailinfo = validate_email(email, check_deliverability=False)
+
+  # After this point, use only the normalized form of the email address,
+  # especially before going to a database query.
+  email = emailinfo.normalized
+
 except EmailNotValidError as e:
-  # Email is not valid.
-  # The exception message is human-readable.
+
+  # The exception message is human-readable explanation of why it's
+  # not a valid (or deliverable) email address.
   print(str(e))
 ```
 
 This validates the address and gives you its normalized form. You should
 **put the normalized form in your database** and always normalize before
 checking if an address is in your database. When using this in a login form,
 set `check_deliverability` to `False` to avoid unnecessary DNS queries.
@@ -121,76 +125,83 @@
 exception classes are subclasses of `EmailNotValidError`, which in turn
 is a subclass of `ValueError`.
 
 But when an email address is valid, an object is returned containing
 a normalized form of the email address (which you should use!) and
 other information.
 
-The validator doesn't permit obsoleted forms of email addresses that no
-one uses anymore even though they are still valid and deliverable, since
+The validator doesn't, by default, permit obsoleted forms of email addresses
+that no one uses anymore even though they are still valid and deliverable, since
 they will probably give you grief if you're using email for login. (See
-later in the document about that.)
+later in the document about how to allow some obsolete forms.)
 
-The validator checks that the domain name in the email address has a
-DNS MX record (except a NULL MX record) indicating that it can receive
-email (or a fallback A-record, see below).
-There is nothing to be gained by trying to actually contact an SMTP
-server, so that's not done here. For privacy, security, and practicality
-reasons servers are good at not giving away whether an address is
+The validator optionally checks that the domain name in the email address has
+a DNS MX record indicating that it can receive email. (Except a Null MX record.
+If there is no MX record, a fallback A/AAAA-record is permitted, unless
+a reject-all SPF record is present.) DNS is slow and sometimes unavailable or
+unreliable, so consider whether these checks are useful for your use case and
+turn them off if they aren't.
+There is nothing to be gained by trying to actually contact an SMTP server, so
+that's not done here. For privacy, security, and practicality reasons, servers
+are good at not giving away whether an address is
 deliverable or not: email addresses that appear to accept mail at first
 can bounce mail after a delay, and bounced mail may indicate a temporary
 failure of a good email address (sometimes an intentional failure, like
 greylisting).
 
 ### Options
 
 The `validate_email` function also accepts the following keyword arguments
 (defaults are as shown below):
 
-`check_deliverability=True`: If true, a DNS query is made to check that a non-null MX record is present for the domain-part of the email address (or if not, an A/AAAA record as an MX fallback can be present but in that case a reject-all SPF record must not be present). Set to `False` to skip this DNS-based check. DNS is slow and sometimes unavailable, so consider whether these checks are useful for your use case. It is recommended to pass `False` when performing validation for login pages (but not account creation pages) since re-validation of a previously validated domain in your database by querying DNS at every login is probably undesirable. You can also set `email_validator.CHECK_DELIVERABILITY` to `False` to turn this off for all calls by default.
+`check_deliverability=True`: If true, DNS queries are made to check that the domain name in the email address (the part after the @-sign) can receive mail, as described above. Set to `False` to skip this DNS-based check. It is recommended to pass `False` when performing validation for login pages (but not account creation pages) since re-validation of a previously validated domain in your database by querying DNS at every login is probably undesirable. You can also set `email_validator.CHECK_DELIVERABILITY` to `False` to turn this off for all calls by default.
 
-`dns_resolver=None`: Pass an instance of [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to control the DNS resolver including setting a timeout and [a cache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html). The `caching_resolver` function shown above is a helper function to construct a dns.resolver.Resolver with a [LRUCache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html#dns.resolver.LRUCache). Reuse the same resolver instance across calls to `validate_email` to make use of the cache.
+`dns_resolver=None`: Pass an instance of [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to control the DNS resolver including setting a timeout and [a cache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html). The `caching_resolver` function shown below is a helper function to construct a dns.resolver.Resolver with a [LRUCache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html#dns.resolver.LRUCache). Reuse the same resolver instance across calls to `validate_email` to make use of the cache.
 
-`test_environment=False`: DNS-based deliverability checks are disabled and  `test` and `subdomain.test` domain names are permitted (see below). You can also set `email_validator.TEST_ENVIRONMENT` to `True` to turn it on for all calls by default.
+`test_environment=False`: If `True`, DNS-based deliverability checks are disabled and  `test` and `**.test` domain names are permitted (see below). You can also set `email_validator.TEST_ENVIRONMENT` to `True` to turn it on for all calls by default.
 
 `allow_smtputf8=True`: Set to `False` to prohibit internationalized addresses that would
     require the
     [SMTPUTF8](https://tools.ietf.org/html/rfc6531) extension. You can also set `email_validator.ALLOW_SMTPUTF8` to `False` to turn it off for all calls by default.
 
+`allow_quoted_local=False`: Set to `True` to allow obscure and potentially problematic email addresses in which the part of the address before the @-sign contains spaces, @-signs, or other surprising characters when the local part is surrounded in quotes (so-called quoted-string local parts). In the object returned by `validate_email`, the normalized local part removes any unnecessary backslash-escaping and even removes the surrounding quotes if the address would be valid without them. You can also set `email_validator.ALLOW_QUOTED_LOCAL` to `True` to turn this on for all calls by default.
+
+`allow_domain_literal=False`: Set to `True` to allow bracketed IPv4 and "IPv6:"-prefixd IPv6 addresses in the domain part of the email address. No deliverability checks are performed for these addresses. In the object returned by `validate_email`, the normalized domain will use the condensed IPv6 format, if applicable. The object's `domain_address` attribute will hold the parsed `ipaddress.IPv4Address` or `ipaddress.IPv6Address` object if applicable. You can also set `email_validator.ALLOW_DOMAIN_LITERAL` to `True` to turn this on for all calls by default.
+
 `allow_empty_local=False`: Set to `True` to allow an empty local part (i.e.
     `@example.com`), e.g. for validating Postfix aliases.
     
 
 ### DNS timeout and cache
 
 When validating many email addresses or to control the timeout (the default is 15 seconds), create a caching [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to reuse in each call. The `caching_resolver` function returns one easily for you:
 
 ```python
 from email_validator import validate_email, caching_resolver
 
 resolver = caching_resolver(timeout=10)
 
 while True:
-  email = validate_email(email, dns_resolver=resolver).email
+  validate_email(email, dns_resolver=resolver)
 ```
 
 ### Test addresses
 
-This library rejects email addresess that use the [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml) `invalid`, `localhost`, `test`, and some others by raising `EmailSyntaxError`. This is to protect your system from abuse: You probably don't want a user to be able to cause an email to be sent to `localhost`. However, in your non-production test environments you may want to use `@test` or `@myname.test` email addresses. There are three ways you can allow this:
+This library rejects email addresess that use the [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml) `invalid`, `localhost`, `test`, and some others by raising `EmailSyntaxError`. This is to protect your system from abuse: You probably don't want a user to be able to cause an email to be sent to `localhost` (although they might be able to still do so via a malicious MX record). However, in your non-production test environments you may want to use `@test` or `@myname.test` email addresses. There are three ways you can allow this:
 
 1. Add `test_environment=True` to the call to `validate_email` (see above).
-2. Set `email_validator.TEST_ENVIRONMENT` to `True`.
-3. Remove the special-use domain name that you want to use from `email_validator.SPECIAL_USE_DOMAIN_NAMES`:
+2. Set `email_validator.TEST_ENVIRONMENT` to `True` globally.
+3. Remove the special-use domain name that you want to use from `email_validator.SPECIAL_USE_DOMAIN_NAMES`, e.g.:
 
 ```python
 import email_validator
 email_validator.SPECIAL_USE_DOMAIN_NAMES.remove("test")
 ```
 
-It is tempting to use `@example.com/net/org` in tests. These domains are reserved to IANA for use in documentation so there is no risk of accidentally emailing someone at those domains. But beware that this library will reject these domain names if DNS-based deliverability checks are not disabled because these domains do not resolve to domains that accept email. In tests, consider using your own domain name or `@test` or `@myname.test` instead.
+It is tempting to use `@example.com/net/org` in tests. They are *not* in this library's `SPECIAL_USE_DOMAIN_NAMES` list so you can, but shouldn't, use them. These domains are reserved to IANA for use in documentation so there is no risk of accidentally emailing someone at those domains. But beware that this library will nevertheless reject these domain names if DNS-based deliverability checks are not disabled because these domains do not resolve to domains that accept email. In tests, consider using your own domain name or `@test` or `@myname.test` instead.
 
 Internationalized email addresses
 ---------------------------------
 
 The email protocol SMTP and the domain name system DNS have historically
 only allowed English (ASCII) characters in email addresses and domain names,
 respectively. Each has adapted to internationalization in a separate
@@ -219,16 +230,17 @@
 local parts, a wider range of Unicode characters are allowed.
 
 A surprisingly large number of Unicode characters are not safe to display,
 especially when the email address is concatenated with other text, so this
 library tries to protect you by not permitting resvered, non-, private use,
 formatting (which can be used to alter the display order of characters),
 whitespace, and control characters, and combining characters
-as the first character (so that they cannot combine with something outside
-of the email address string). See https://qntm.org/safe and https://trojansource.codes/
+as the first character of the local part and the domain name (so that they
+cannot combine with something outside of the email address string or with
+the @-sign). See https://qntm.org/safe and https://trojansource.codes/
 for relevant prior work. (Other than whitespace, these are checks that
 you should be applying to nearly all user inputs in a security-sensitive
 context.)
 
 These character checks are performed after Unicode normalization (see below),
 so you are only fully protected if you replace all user-provided email addresses
 with the normalized email address string returned by this library. This does not
@@ -256,38 +268,44 @@
 If your mail submission library doesn't support Unicode at all --- even
 in the domain part of the address --- then immediately prior to mail
 submission you must replace the email address with its ASCII-ized form.
 This library gives you back the ASCII-ized form in the `ascii_email`
 field in the returned object, which you can get like this:
 
 ```python
-valid = validate_email(email, allow_smtputf8=False)
-email = valid.ascii_email
+emailinfo = validate_email(email, allow_smtputf8=False)
+email = emailinfo.ascii_email
 ```
 
 The local part is left alone (if it has internationalized characters
 `allow_smtputf8=False` will force validation to fail) and the domain
 part is converted to [IDNA ASCII](https://tools.ietf.org/html/rfc5891).
 (You probably should not do this at account creation time so you don't
 change the user's login information without telling them.)
 
 Normalization
 -------------
 
+### Unicode Normalization
+
 The use of Unicode in email addresses introduced a normalization
 problem. Different Unicode strings can look identical and have the same
-semantic meaning to the user. The `email` field returned on successful
+semantic meaning to the user. The `normalized` field returned on successful
 validation provides the correctly normalized form of the given email
-address:
+address.
+
+For example, the CJK fullwidth Latin letters are considered semantically
+equivalent in domain names to their ASCII counterparts. This library
+normalizes them to their ASCII counterparts:
 
 ```python
-valid = validate_email("me@Ｄｏｍａｉｎ.com")
-email = valid.ascii_email
-print(email)
-# prints: me@domain.com
+emailinfo = validate_email("me@Ｄｏｍａｉｎ.com")
+print(emailinfo.normalized)
+print(emailinfo.ascii_email)
+# prints "me@domain.com" twice
 ```
 
 Because an end-user might type their email address in different (but
 equivalent) un-normalized forms at different times, you ought to
 replace what they enter with the normalized form immediately prior to
 going into your database (during account creation), querying your database
 (during login), or sending outbound mail. Normalization may also change
@@ -306,87 +324,96 @@
 [UTS46](http://unicode.org/reports/tr46) mappings on the domain part,
 and conversion from Punycode to Unicode characters.
 
 (See [RFC 6532 (internationalized email) section
 3.1](https://tools.ietf.org/html/rfc6532#section-3.1) and [RFC 5895
 (IDNA 2008) section 2](http://www.ietf.org/rfc/rfc5895.txt).)
 
+### Other Normalization
+
+Normalization is also applied to quoted-string local parts and domain
+literal IPv6 addresses if you have allowed them by the `allow_quoted_local`
+and `allow_domain_literal` options. In quoted-string local parts, unnecessary
+backslash escaping is removed and even the surrounding quotes are removed if
+they are unnecessary. For IPv6 domain literals, the IPv6 address is
+normalized to condensed form. [RFC 2142](https://datatracker.ietf.org/doc/html/rfc2142)
+also requires lowercase normalization for some specific mailbox names like `postmaster@`.
+
 Examples
 --------
 
 For the email address `test@joshdata.me`, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='test@joshdata.me',
+  normalized='test@joshdata.me',
   local_part='test',
   domain='joshdata.me',
   ascii_email='test@joshdata.me',
   ascii_local_part='test',
   ascii_domain='joshdata.me',
   smtputf8=False)
 ```
 
 For the fictitious but valid address `example@ツ.ⓁⒾⒻⒺ`, which has an
 internationalized domain but ASCII local part, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='example@ツ.life',
+  normalized='example@ツ.life',
   local_part='example',
   domain='ツ.life',
   ascii_email='example@xn--bdk.life',
   ascii_local_part='example',
   ascii_domain='xn--bdk.life',
   smtputf8=False)
 
 ```
 
-Note that the `email` and `domain` fields provide a normalized form of the
+Note that `normalized` and other fields provide a normalized form of the
 email address, domain name, and (in other cases) local part (see earlier
 discussion of normalization), which you should use in your database.
 
 Calling `validate_email` with the ASCII form of the above email address,
 `example@xn--bdk.life`, returns the exact same information (i.e., the
-`email` field always will contain Unicode characters, not Punycode).
+`normalized` field always will contain Unicode characters, not Punycode).
 
 For the fictitious address `ツ-test@joshdata.me`, which has an
 internationalized local part, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='ツ-test@joshdata.me',
+  normalized='ツ-test@joshdata.me',
   local_part='ツ-test',
   domain='joshdata.me',
   ascii_email=None,
   ascii_local_part=None,
   ascii_domain='joshdata.me',
   smtputf8=True)
 ```
 
 Now `smtputf8` is `True` and `ascii_email` is `None` because the local
-part of the address is internationalized. The `local_part` and `email` fields
-return the normalized form of the address: certain Unicode characters
-(such as angstrom and ohm) may be replaced by other equivalent code
-points (a-with-ring and omega).
+part of the address is internationalized. The `local_part` and `normalized` fields
+return the normalized form of the address.
 
 Return value
 ------------
 
 When an email address passes validation, the fields in the returned object
 are:
 
 | Field | Value |
 | -----:|-------|
-| `email` | The normalized form of the email address that you should put in your database. This merely combines the `local_part` and `domain` fields (see below). |
-| `ascii_email` | If set, an ASCII-only form of the email address by replacing the domain part with [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt). This field will be present when an ASCII-only form of the email address exists (including if the email address is already ASCII). If the local part of the email address contains internationalized characters, `ascii_email` will be `None`. If set, it merely combines `ascii_local_part` and `ascii_domain`. |
-| `local_part` | The local part of the given email address (before the @-sign) with Unicode NFC normalization applied. |
+| `normalized` | The normalized form of the email address that you should put in your database. This combines the `local_part` and `domain` fields (see below). |
+| `ascii_email` | If set, an ASCII-only form of the normalized email address by replacing the domain part with [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt). This field will be present when an ASCII-only form of the email address exists (including if the email address is already ASCII). If the local part of the email address contains internationalized characters, `ascii_email` will be `None`. If set, it merely combines `ascii_local_part` and `ascii_domain`. |
+| `local_part` | The normalized local part of the given email address (before the @-sign). Normalization includes Unicode NFC normalization and removing unnecessary quoted-string quotes and backslashes. If `allow_quoted_local` is True and the surrounding quotes are necessary, the quotes _will_ be present in this field. |
 | `ascii_local_part` | If set, the local part, which is composed of ASCII characters only. |
 | `domain` | The canonical internationalized Unicode form of the domain part of the email address. If the returned string contains non-ASCII characters, either the [SMTPUTF8](https://tools.ietf.org/html/rfc6531) feature of your mail relay will be required to transmit the message or else the email address's domain part must be converted to IDNA ASCII first: Use `ascii_domain` field instead. |
 | `ascii_domain` | The [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt)-encoded form of the domain part of the given email address, as it would be transmitted on the wire. |
+| `domain_address` | If domain literals are allowed and if the email address contains one, an `ipaddress.IPv4Address` or `ipaddress.IPv6Address` object. |
 | `smtputf8` | A boolean indicating that the [SMTPUTF8](https://tools.ietf.org/html/rfc6531) feature of your mail relay will be required to transmit messages to this address because the local part of the address has non-ASCII characters (the local part cannot be IDNA-encoded). If `allow_smtputf8=False` is passed as an argument, this flag will always be false because an exception is raised if it would have been true. |
 | `mx` | A list of (priority, domain) tuples of MX records specified in the DNS for the domain (see [RFC 5321 section 5](https://tools.ietf.org/html/rfc5321#section-5)). May be `None` if the deliverability check could not be completed because of a temporary issue like a timeout. |
 | `mx_fallback_type` | `None` if an `MX` record is found. If no MX records are actually specified in DNS and instead are inferred, through an obsolete mechanism, from A or AAAA records, the value is the type of DNS record used instead (`A` or `AAAA`). May be `None` if the deliverability check could not be completed because of a temporary issue like a timeout. |
 | `spf` | Any SPF record found while checking deliverability. Only set if the SPF record is queried. |
 
 Assumptions
 -----------
@@ -400,21 +427,20 @@
   of the email address must be a resolvable domain name
   (see the deliverability checks described above).
   Most [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml)
   and their subdomains, as well as
   domain names without a `.`, are rejected as a syntax error
   (except see the `test_environment` parameter above).
 * Obsolete email syntaxes are rejected:
-  The "quoted string" form of the local part of the email address (RFC
-  5321 4.1.2) is not permitted.
-  Quoted forms allow multiple @-signs, space characters, and other
-  troublesome conditions. The unusual [(comment) syntax](https://github.com/JoshData/python-email-validator/issues/77)
-  is also rejected. The "literal" form for the domain part of an email address (an
-  IP address in brackets) is rejected. Other obsolete and deprecated syntaxes are
-  rejected. No one uses these forms anymore.
+  The unusual ["(comment)" syntax](https://github.com/JoshData/python-email-validator/issues/77)
+  is rejected. Extremely old obsolete syntaxes are
+  rejected. Quoted-string local parts and domain-literal addresses
+  are rejected by default, but there are options to allow them (see above).
+  No one uses these forms anymore, and I can't think of any reason why anyone
+  using this library would need to accept them.
 
 
 Testing
 -------
 
 Tests can be run using
 
@@ -430,20 +456,17 @@
 
 The package is distributed as a universal wheel and as a source package.
 
 To release:
 
 * Update CHANGELOG.md.
 * Update the version number in setup.cfg.
-* Make & push a commit with the new version number.
-* Make & push a tag (`git tag v... && git push --tags`).
+* Make & push a commit with the new version number and make sure tests pass.
+* Make & push a tag (see command below).
 * Make a release at https://github.com/JoshData/python-email-validator/releases/new.
-* Follow the steps below to publish source and a universal wheel to pypi.
+* Publish a source and wheel distribution to pypi (see command below).
 
 ```sh
-./release_to_pypi.sh
 git tag v$(grep version setup.cfg | sed "s/.*= //")
 git push --tags
+./release_to_pypi.sh
 ```
-
-Notes: The wheel is specified as universal in the file `setup.cfg` by the `universal = 1` key in the
-`[bdist_wheel]` section.
```

### Comparing `email_validator-2.0.0.dev4/README.md` & `email_validator-2.0.0.post1/email_validator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: email-validator
+Version: 2.0.0.post1
+Summary: A robust email address syntax and deliverability validation library.
+Home-page: https://github.com/JoshData/python-email-validator
+Author: Joshua Tauberer
+Author-email: jt@occams.info
+License: CC0 (copyright waived)
+Keywords: email address validator
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 email-validator: Validate Email Addresses
 =========================================
 
 A robust email address syntax and deliverability validation library for
 Python 3.7+ by [Joshua Tauberer](https://joshdata.me).
 
 This library validates that a string is of the form `name@example.com`
@@ -10,29 +33,31 @@
 users by their email address like on a registration/login form (but not
 necessarily for composing an email message, see below).
 
 Key features:
 
 * Checks that an email address has the correct syntax --- good for
   registration/login forms or other uses related to identifying users.
-  Rejects obsolete email address syntax that you'd find unexpected.
 * Gives friendly English error messages when validation fails that you
   can display to end-users.
 * Checks deliverability (optional): Does the domain name resolve?
   (You can override the default DNS resolver to add query caching.)
 * Supports internationalized domain names and internationalized local parts.
-  Blocks unsafe characters for your safety.
+* Rejects addresses with unsafe Unicode characters, obsolete email address
+  syntax that you'd find unexpected, special use domain names like
+  `@localhost`, and domains without a dot by default. This is an
+  opinionated library!
 * Normalizes email addresses (important for internationalized
-  addresses! see below).
+  and quoted-string addresses! see below).
+* Python type annotations are used.
 
-This library does NOT permit obsolete forms of email addresses, so
-if you need strict validation against the email specs exactly, use
-[pyIsEmail](https://github.com/michaelherold/pyIsEmail) or try
-[flanker](https://github.com/mailgun/flanker) if you are parsing the
-To: line of an email.
+This is an opinionated library. You should definitely also consider using
+the less-opinionated [pyIsEmail](https://github.com/michaelherold/pyIsEmail) and
+[flanker](https://github.com/mailgun/flanker) if they are better for your
+use case.
 
 [![Build Status](https://github.com/JoshData/python-email-validator/actions/workflows/test_and_build.yaml/badge.svg)](https://github.com/JoshData/python-email-validator/actions/workflows/test_and_build.yaml)
 
 View the [CHANGELOG / Release Notes](CHANGELOG.md) for the version history of changes in the library. Occasionally this README is ahead of the latest published package --- see the CHANGELOG for details.
 
 ---
 
@@ -52,29 +77,31 @@
 
 If you're validating a user's email address before creating a user
 account in your application, you might do this:
 
 ```python
 from email_validator import validate_email, EmailNotValidError
 
-email = "my+address@mydomain.tld"
-is_new_account = True # False for login pages
+email = "my+address@example.org"
 
 try:
-  # Check that the email address is valid.
-  validation = validate_email(email, check_deliverability=is_new_account)
 
-  # Take the normalized form of the email address
-  # for all logic beyond this point (especially
-  # before going to a database query where equality
-  # may not take into account Unicode normalization).  
-  email = validation.email
+  # Check that the email address is valid. Turn on check_deliverability
+  # for first-time validations like on account creation pages (but not
+  # login pages).
+  emailinfo = validate_email(email, check_deliverability=False)
+
+  # After this point, use only the normalized form of the email address,
+  # especially before going to a database query.
+  email = emailinfo.normalized
+
 except EmailNotValidError as e:
-  # Email is not valid.
-  # The exception message is human-readable.
+
+  # The exception message is human-readable explanation of why it's
+  # not a valid (or deliverable) email address.
   print(str(e))
 ```
 
 This validates the address and gives you its normalized form. You should
 **put the normalized form in your database** and always normalize before
 checking if an address is in your database. When using this in a login form,
 set `check_deliverability` to `False` to avoid unnecessary DNS queries.
@@ -98,76 +125,83 @@
 exception classes are subclasses of `EmailNotValidError`, which in turn
 is a subclass of `ValueError`.
 
 But when an email address is valid, an object is returned containing
 a normalized form of the email address (which you should use!) and
 other information.
 
-The validator doesn't permit obsoleted forms of email addresses that no
-one uses anymore even though they are still valid and deliverable, since
+The validator doesn't, by default, permit obsoleted forms of email addresses
+that no one uses anymore even though they are still valid and deliverable, since
 they will probably give you grief if you're using email for login. (See
-later in the document about that.)
+later in the document about how to allow some obsolete forms.)
 
-The validator checks that the domain name in the email address has a
-DNS MX record (except a NULL MX record) indicating that it can receive
-email (or a fallback A-record, see below).
-There is nothing to be gained by trying to actually contact an SMTP
-server, so that's not done here. For privacy, security, and practicality
-reasons servers are good at not giving away whether an address is
+The validator optionally checks that the domain name in the email address has
+a DNS MX record indicating that it can receive email. (Except a Null MX record.
+If there is no MX record, a fallback A/AAAA-record is permitted, unless
+a reject-all SPF record is present.) DNS is slow and sometimes unavailable or
+unreliable, so consider whether these checks are useful for your use case and
+turn them off if they aren't.
+There is nothing to be gained by trying to actually contact an SMTP server, so
+that's not done here. For privacy, security, and practicality reasons, servers
+are good at not giving away whether an address is
 deliverable or not: email addresses that appear to accept mail at first
 can bounce mail after a delay, and bounced mail may indicate a temporary
 failure of a good email address (sometimes an intentional failure, like
 greylisting).
 
 ### Options
 
 The `validate_email` function also accepts the following keyword arguments
 (defaults are as shown below):
 
-`check_deliverability=True`: If true, a DNS query is made to check that a non-null MX record is present for the domain-part of the email address (or if not, an A/AAAA record as an MX fallback can be present but in that case a reject-all SPF record must not be present). Set to `False` to skip this DNS-based check. DNS is slow and sometimes unavailable, so consider whether these checks are useful for your use case. It is recommended to pass `False` when performing validation for login pages (but not account creation pages) since re-validation of a previously validated domain in your database by querying DNS at every login is probably undesirable. You can also set `email_validator.CHECK_DELIVERABILITY` to `False` to turn this off for all calls by default.
+`check_deliverability=True`: If true, DNS queries are made to check that the domain name in the email address (the part after the @-sign) can receive mail, as described above. Set to `False` to skip this DNS-based check. It is recommended to pass `False` when performing validation for login pages (but not account creation pages) since re-validation of a previously validated domain in your database by querying DNS at every login is probably undesirable. You can also set `email_validator.CHECK_DELIVERABILITY` to `False` to turn this off for all calls by default.
 
-`dns_resolver=None`: Pass an instance of [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to control the DNS resolver including setting a timeout and [a cache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html). The `caching_resolver` function shown above is a helper function to construct a dns.resolver.Resolver with a [LRUCache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html#dns.resolver.LRUCache). Reuse the same resolver instance across calls to `validate_email` to make use of the cache.
+`dns_resolver=None`: Pass an instance of [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to control the DNS resolver including setting a timeout and [a cache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html). The `caching_resolver` function shown below is a helper function to construct a dns.resolver.Resolver with a [LRUCache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html#dns.resolver.LRUCache). Reuse the same resolver instance across calls to `validate_email` to make use of the cache.
 
-`test_environment=False`: DNS-based deliverability checks are disabled and  `test` and `subdomain.test` domain names are permitted (see below). You can also set `email_validator.TEST_ENVIRONMENT` to `True` to turn it on for all calls by default.
+`test_environment=False`: If `True`, DNS-based deliverability checks are disabled and  `test` and `**.test` domain names are permitted (see below). You can also set `email_validator.TEST_ENVIRONMENT` to `True` to turn it on for all calls by default.
 
 `allow_smtputf8=True`: Set to `False` to prohibit internationalized addresses that would
     require the
     [SMTPUTF8](https://tools.ietf.org/html/rfc6531) extension. You can also set `email_validator.ALLOW_SMTPUTF8` to `False` to turn it off for all calls by default.
 
+`allow_quoted_local=False`: Set to `True` to allow obscure and potentially problematic email addresses in which the part of the address before the @-sign contains spaces, @-signs, or other surprising characters when the local part is surrounded in quotes (so-called quoted-string local parts). In the object returned by `validate_email`, the normalized local part removes any unnecessary backslash-escaping and even removes the surrounding quotes if the address would be valid without them. You can also set `email_validator.ALLOW_QUOTED_LOCAL` to `True` to turn this on for all calls by default.
+
+`allow_domain_literal=False`: Set to `True` to allow bracketed IPv4 and "IPv6:"-prefixd IPv6 addresses in the domain part of the email address. No deliverability checks are performed for these addresses. In the object returned by `validate_email`, the normalized domain will use the condensed IPv6 format, if applicable. The object's `domain_address` attribute will hold the parsed `ipaddress.IPv4Address` or `ipaddress.IPv6Address` object if applicable. You can also set `email_validator.ALLOW_DOMAIN_LITERAL` to `True` to turn this on for all calls by default.
+
 `allow_empty_local=False`: Set to `True` to allow an empty local part (i.e.
     `@example.com`), e.g. for validating Postfix aliases.
     
 
 ### DNS timeout and cache
 
 When validating many email addresses or to control the timeout (the default is 15 seconds), create a caching [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to reuse in each call. The `caching_resolver` function returns one easily for you:
 
 ```python
 from email_validator import validate_email, caching_resolver
 
 resolver = caching_resolver(timeout=10)
 
 while True:
-  email = validate_email(email, dns_resolver=resolver).email
+  validate_email(email, dns_resolver=resolver)
 ```
 
 ### Test addresses
 
-This library rejects email addresess that use the [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml) `invalid`, `localhost`, `test`, and some others by raising `EmailSyntaxError`. This is to protect your system from abuse: You probably don't want a user to be able to cause an email to be sent to `localhost`. However, in your non-production test environments you may want to use `@test` or `@myname.test` email addresses. There are three ways you can allow this:
+This library rejects email addresess that use the [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml) `invalid`, `localhost`, `test`, and some others by raising `EmailSyntaxError`. This is to protect your system from abuse: You probably don't want a user to be able to cause an email to be sent to `localhost` (although they might be able to still do so via a malicious MX record). However, in your non-production test environments you may want to use `@test` or `@myname.test` email addresses. There are three ways you can allow this:
 
 1. Add `test_environment=True` to the call to `validate_email` (see above).
-2. Set `email_validator.TEST_ENVIRONMENT` to `True`.
-3. Remove the special-use domain name that you want to use from `email_validator.SPECIAL_USE_DOMAIN_NAMES`:
+2. Set `email_validator.TEST_ENVIRONMENT` to `True` globally.
+3. Remove the special-use domain name that you want to use from `email_validator.SPECIAL_USE_DOMAIN_NAMES`, e.g.:
 
 ```python
 import email_validator
 email_validator.SPECIAL_USE_DOMAIN_NAMES.remove("test")
 ```
 
-It is tempting to use `@example.com/net/org` in tests. These domains are reserved to IANA for use in documentation so there is no risk of accidentally emailing someone at those domains. But beware that this library will reject these domain names if DNS-based deliverability checks are not disabled because these domains do not resolve to domains that accept email. In tests, consider using your own domain name or `@test` or `@myname.test` instead.
+It is tempting to use `@example.com/net/org` in tests. They are *not* in this library's `SPECIAL_USE_DOMAIN_NAMES` list so you can, but shouldn't, use them. These domains are reserved to IANA for use in documentation so there is no risk of accidentally emailing someone at those domains. But beware that this library will nevertheless reject these domain names if DNS-based deliverability checks are not disabled because these domains do not resolve to domains that accept email. In tests, consider using your own domain name or `@test` or `@myname.test` instead.
 
 Internationalized email addresses
 ---------------------------------
 
 The email protocol SMTP and the domain name system DNS have historically
 only allowed English (ASCII) characters in email addresses and domain names,
 respectively. Each has adapted to internationalization in a separate
@@ -196,16 +230,17 @@
 local parts, a wider range of Unicode characters are allowed.
 
 A surprisingly large number of Unicode characters are not safe to display,
 especially when the email address is concatenated with other text, so this
 library tries to protect you by not permitting resvered, non-, private use,
 formatting (which can be used to alter the display order of characters),
 whitespace, and control characters, and combining characters
-as the first character (so that they cannot combine with something outside
-of the email address string). See https://qntm.org/safe and https://trojansource.codes/
+as the first character of the local part and the domain name (so that they
+cannot combine with something outside of the email address string or with
+the @-sign). See https://qntm.org/safe and https://trojansource.codes/
 for relevant prior work. (Other than whitespace, these are checks that
 you should be applying to nearly all user inputs in a security-sensitive
 context.)
 
 These character checks are performed after Unicode normalization (see below),
 so you are only fully protected if you replace all user-provided email addresses
 with the normalized email address string returned by this library. This does not
@@ -233,38 +268,44 @@
 If your mail submission library doesn't support Unicode at all --- even
 in the domain part of the address --- then immediately prior to mail
 submission you must replace the email address with its ASCII-ized form.
 This library gives you back the ASCII-ized form in the `ascii_email`
 field in the returned object, which you can get like this:
 
 ```python
-valid = validate_email(email, allow_smtputf8=False)
-email = valid.ascii_email
+emailinfo = validate_email(email, allow_smtputf8=False)
+email = emailinfo.ascii_email
 ```
 
 The local part is left alone (if it has internationalized characters
 `allow_smtputf8=False` will force validation to fail) and the domain
 part is converted to [IDNA ASCII](https://tools.ietf.org/html/rfc5891).
 (You probably should not do this at account creation time so you don't
 change the user's login information without telling them.)
 
 Normalization
 -------------
 
+### Unicode Normalization
+
 The use of Unicode in email addresses introduced a normalization
 problem. Different Unicode strings can look identical and have the same
-semantic meaning to the user. The `email` field returned on successful
+semantic meaning to the user. The `normalized` field returned on successful
 validation provides the correctly normalized form of the given email
-address:
+address.
+
+For example, the CJK fullwidth Latin letters are considered semantically
+equivalent in domain names to their ASCII counterparts. This library
+normalizes them to their ASCII counterparts:
 
 ```python
-valid = validate_email("me@Ｄｏｍａｉｎ.com")
-email = valid.ascii_email
-print(email)
-# prints: me@domain.com
+emailinfo = validate_email("me@Ｄｏｍａｉｎ.com")
+print(emailinfo.normalized)
+print(emailinfo.ascii_email)
+# prints "me@domain.com" twice
 ```
 
 Because an end-user might type their email address in different (but
 equivalent) un-normalized forms at different times, you ought to
 replace what they enter with the normalized form immediately prior to
 going into your database (during account creation), querying your database
 (during login), or sending outbound mail. Normalization may also change
@@ -283,87 +324,96 @@
 [UTS46](http://unicode.org/reports/tr46) mappings on the domain part,
 and conversion from Punycode to Unicode characters.
 
 (See [RFC 6532 (internationalized email) section
 3.1](https://tools.ietf.org/html/rfc6532#section-3.1) and [RFC 5895
 (IDNA 2008) section 2](http://www.ietf.org/rfc/rfc5895.txt).)
 
+### Other Normalization
+
+Normalization is also applied to quoted-string local parts and domain
+literal IPv6 addresses if you have allowed them by the `allow_quoted_local`
+and `allow_domain_literal` options. In quoted-string local parts, unnecessary
+backslash escaping is removed and even the surrounding quotes are removed if
+they are unnecessary. For IPv6 domain literals, the IPv6 address is
+normalized to condensed form. [RFC 2142](https://datatracker.ietf.org/doc/html/rfc2142)
+also requires lowercase normalization for some specific mailbox names like `postmaster@`.
+
 Examples
 --------
 
 For the email address `test@joshdata.me`, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='test@joshdata.me',
+  normalized='test@joshdata.me',
   local_part='test',
   domain='joshdata.me',
   ascii_email='test@joshdata.me',
   ascii_local_part='test',
   ascii_domain='joshdata.me',
   smtputf8=False)
 ```
 
 For the fictitious but valid address `example@ツ.ⓁⒾⒻⒺ`, which has an
 internationalized domain but ASCII local part, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='example@ツ.life',
+  normalized='example@ツ.life',
   local_part='example',
   domain='ツ.life',
   ascii_email='example@xn--bdk.life',
   ascii_local_part='example',
   ascii_domain='xn--bdk.life',
   smtputf8=False)
 
 ```
 
-Note that the `email` and `domain` fields provide a normalized form of the
+Note that `normalized` and other fields provide a normalized form of the
 email address, domain name, and (in other cases) local part (see earlier
 discussion of normalization), which you should use in your database.
 
 Calling `validate_email` with the ASCII form of the above email address,
 `example@xn--bdk.life`, returns the exact same information (i.e., the
-`email` field always will contain Unicode characters, not Punycode).
+`normalized` field always will contain Unicode characters, not Punycode).
 
 For the fictitious address `ツ-test@joshdata.me`, which has an
 internationalized local part, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='ツ-test@joshdata.me',
+  normalized='ツ-test@joshdata.me',
   local_part='ツ-test',
   domain='joshdata.me',
   ascii_email=None,
   ascii_local_part=None,
   ascii_domain='joshdata.me',
   smtputf8=True)
 ```
 
 Now `smtputf8` is `True` and `ascii_email` is `None` because the local
-part of the address is internationalized. The `local_part` and `email` fields
-return the normalized form of the address: certain Unicode characters
-(such as angstrom and ohm) may be replaced by other equivalent code
-points (a-with-ring and omega).
+part of the address is internationalized. The `local_part` and `normalized` fields
+return the normalized form of the address.
 
 Return value
 ------------
 
 When an email address passes validation, the fields in the returned object
 are:
 
 | Field | Value |
 | -----:|-------|
-| `email` | The normalized form of the email address that you should put in your database. This merely combines the `local_part` and `domain` fields (see below). |
-| `ascii_email` | If set, an ASCII-only form of the email address by replacing the domain part with [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt). This field will be present when an ASCII-only form of the email address exists (including if the email address is already ASCII). If the local part of the email address contains internationalized characters, `ascii_email` will be `None`. If set, it merely combines `ascii_local_part` and `ascii_domain`. |
-| `local_part` | The local part of the given email address (before the @-sign) with Unicode NFC normalization applied. |
+| `normalized` | The normalized form of the email address that you should put in your database. This combines the `local_part` and `domain` fields (see below). |
+| `ascii_email` | If set, an ASCII-only form of the normalized email address by replacing the domain part with [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt). This field will be present when an ASCII-only form of the email address exists (including if the email address is already ASCII). If the local part of the email address contains internationalized characters, `ascii_email` will be `None`. If set, it merely combines `ascii_local_part` and `ascii_domain`. |
+| `local_part` | The normalized local part of the given email address (before the @-sign). Normalization includes Unicode NFC normalization and removing unnecessary quoted-string quotes and backslashes. If `allow_quoted_local` is True and the surrounding quotes are necessary, the quotes _will_ be present in this field. |
 | `ascii_local_part` | If set, the local part, which is composed of ASCII characters only. |
 | `domain` | The canonical internationalized Unicode form of the domain part of the email address. If the returned string contains non-ASCII characters, either the [SMTPUTF8](https://tools.ietf.org/html/rfc6531) feature of your mail relay will be required to transmit the message or else the email address's domain part must be converted to IDNA ASCII first: Use `ascii_domain` field instead. |
 | `ascii_domain` | The [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt)-encoded form of the domain part of the given email address, as it would be transmitted on the wire. |
+| `domain_address` | If domain literals are allowed and if the email address contains one, an `ipaddress.IPv4Address` or `ipaddress.IPv6Address` object. |
 | `smtputf8` | A boolean indicating that the [SMTPUTF8](https://tools.ietf.org/html/rfc6531) feature of your mail relay will be required to transmit messages to this address because the local part of the address has non-ASCII characters (the local part cannot be IDNA-encoded). If `allow_smtputf8=False` is passed as an argument, this flag will always be false because an exception is raised if it would have been true. |
 | `mx` | A list of (priority, domain) tuples of MX records specified in the DNS for the domain (see [RFC 5321 section 5](https://tools.ietf.org/html/rfc5321#section-5)). May be `None` if the deliverability check could not be completed because of a temporary issue like a timeout. |
 | `mx_fallback_type` | `None` if an `MX` record is found. If no MX records are actually specified in DNS and instead are inferred, through an obsolete mechanism, from A or AAAA records, the value is the type of DNS record used instead (`A` or `AAAA`). May be `None` if the deliverability check could not be completed because of a temporary issue like a timeout. |
 | `spf` | Any SPF record found while checking deliverability. Only set if the SPF record is queried. |
 
 Assumptions
 -----------
@@ -377,21 +427,20 @@
   of the email address must be a resolvable domain name
   (see the deliverability checks described above).
   Most [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml)
   and their subdomains, as well as
   domain names without a `.`, are rejected as a syntax error
   (except see the `test_environment` parameter above).
 * Obsolete email syntaxes are rejected:
-  The "quoted string" form of the local part of the email address (RFC
-  5321 4.1.2) is not permitted.
-  Quoted forms allow multiple @-signs, space characters, and other
-  troublesome conditions. The unusual [(comment) syntax](https://github.com/JoshData/python-email-validator/issues/77)
-  is also rejected. The "literal" form for the domain part of an email address (an
-  IP address in brackets) is rejected. Other obsolete and deprecated syntaxes are
-  rejected. No one uses these forms anymore.
+  The unusual ["(comment)" syntax](https://github.com/JoshData/python-email-validator/issues/77)
+  is rejected. Extremely old obsolete syntaxes are
+  rejected. Quoted-string local parts and domain-literal addresses
+  are rejected by default, but there are options to allow them (see above).
+  No one uses these forms anymore, and I can't think of any reason why anyone
+  using this library would need to accept them.
 
 
 Testing
 -------
 
 Tests can be run using
 
@@ -407,20 +456,17 @@
 
 The package is distributed as a universal wheel and as a source package.
 
 To release:
 
 * Update CHANGELOG.md.
 * Update the version number in setup.cfg.
-* Make & push a commit with the new version number.
-* Make & push a tag (`git tag v... && git push --tags`).
+* Make & push a commit with the new version number and make sure tests pass.
+* Make & push a tag (see command below).
 * Make a release at https://github.com/JoshData/python-email-validator/releases/new.
-* Follow the steps below to publish source and a universal wheel to pypi.
+* Publish a source and wheel distribution to pypi (see command below).
 
 ```sh
-./release_to_pypi.sh
 git tag v$(grep version setup.cfg | sed "s/.*= //")
 git push --tags
+./release_to_pypi.sh
 ```
-
-Notes: The wheel is specified as universal in the file `setup.cfg` by the `universal = 1` key in the
-`[bdist_wheel]` section.
```

### Comparing `email_validator-2.0.0.dev4/email_validator/__init__.py` & `email_validator-2.0.0.post1/email_validator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 
 # These global attributes are a part of the library's API and can be
 # changed by library users.
 
 # Default values for keyword arguments.
 
 ALLOW_SMTPUTF8 = True
+ALLOW_QUOTED_LOCAL = False
+ALLOW_DOMAIN_LITERAL = False
+GLOBALLY_DELIVERABLE = True
 CHECK_DELIVERABILITY = True
 TEST_ENVIRONMENT = False
-GLOBALLY_DELIVERABLE = True
 DEFAULT_TIMEOUT = 15  # secs
 
 # IANA Special Use Domain Names
 # Last Updated 2021-09-21
 # https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.txt
 #
 # The domain names without dots would be caught by the check that the domain
```

### Comparing `email_validator-2.0.0.dev4/email_validator/deliverability.py` & `email_validator-2.0.0.post1/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `email_validator-2.0.0.dev4/email_validator/exceptions_types.py` & `email_validator-2.0.0.post1/email_validator/exceptions_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Optional
 
 
 class EmailNotValidError(ValueError):
     """Parent class of all exceptions raised by this module."""
     pass
 
@@ -17,29 +18,32 @@
 
 
 class ValidatedEmail(object):
     """The validate_email function returns objects of this type holding the normalized form of the email address
     and other information."""
 
     """The email address that was passed to validate_email. (If passed as bytes, this will be a string.)"""
-    original_email: str
+    original: str
 
     """The normalized email address, which should always be used in preferance to the original address.
     The normalized address converts an IDNA ASCII domain name to Unicode, if possible, and performs
     Unicode normalization on the local part and on the domain (if originally Unicode). It is the
     concatenation of the local_part and domain attributes, separated by an @-sign."""
-    email: str
+    normalized: str
 
     """The local part of the email address after Unicode normalization."""
     local_part: str
 
     """The domain part of the email address after Unicode normalization or conversion to
     Unicode from IDNA ascii."""
     domain: str
 
+    """If the domain part is a domain literal, the IPv4Address or IPv6Address object."""
+    domain_address: object
+
     """If not None, a form of the email address that uses 7-bit ASCII characters only."""
     ascii_email: Optional[str]
 
     """If not None, the local part of the email address using 7-bit ASCII characters only."""
     ascii_local_part: Optional[str]
 
     """A form of the domain name that uses 7-bit ASCII characters only."""
@@ -60,21 +64,30 @@
 
     """Tests use this constructor."""
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def __repr__(self):
-        return f"<ValidatedEmail {self.email}>"
+        return f"<ValidatedEmail {self.normalized}>"
+
+    """For backwards compatibility, support old field names."""
+    def __getattr__(self, key):
+        if key == "original_email":
+            return self.original
+        if key == "email":
+            return self.normalized
+        raise AttributeError()
 
     """For backwards compatibility, some fields are also exposed through a dict-like interface. Note
     that some of the names changed when they became attributes."""
     def __getitem__(self, key):
+        warnings.warn("dict-like access to the return value of validate_email is deprecated and may not be supported in the future.", DeprecationWarning, stacklevel=2)
         if key == "email":
-            return self.email
+            return self.normalized
         if key == "email_ascii":
             return self.ascii_email
         if key == "local":
             return self.local_part
         if key == "domain":
             return self.ascii_domain
         if key == "domain_i18n":
@@ -88,15 +101,15 @@
         raise KeyError()
 
     """Tests use this."""
     def __eq__(self, other):
         if not isinstance(other, ValidatedEmail):
             return False
         return (
-            self.email == other.email
+            self.normalized == other.normalized
             and self.local_part == other.local_part
             and self.domain == other.domain
             and getattr(self, 'ascii_email', None) == getattr(other, 'ascii_email', None)
             and getattr(self, 'ascii_local_part', None) == getattr(other, 'ascii_local_part', None)
             and getattr(self, 'ascii_domain', None) == getattr(other, 'ascii_domain', None)
             and self.smtputf8 == other.smtputf8
             and repr(sorted(self.mx) if getattr(self, 'mx', None) else None)
@@ -114,8 +127,11 @@
                                    'ascii_email', 'ascii_local_part', 'ascii_domain',
                                    'smtputf8', 'mx', 'mx_fallback_type')
                        ) \
             + ")"
 
     """Convenience method for accessing ValidatedEmail as a dict"""
     def as_dict(self):
-        return self.__dict__
+        d = self.__dict__
+        if d.get('domain_address'):
+            d['domain_address'] = repr(d['domain_address'])
+        return d
```

### Comparing `email_validator-2.0.0.dev4/email_validator/syntax.py` & `email_validator-2.0.0.post1/email_validator/syntax.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,212 @@
 from .exceptions_types import EmailSyntaxError
 from .rfc_constants import EMAIL_MAX_LENGTH, LOCAL_PART_MAX_LENGTH, DOMAIN_MAX_LENGTH, \
-    DOT_ATOM_TEXT, DOT_ATOM_TEXT_INTL, ATEXT_RE, ATEXT_INTL_RE, ATEXT_HOSTNAME_INTL, DNS_LABEL_LENGTH_LIMIT, DOT_ATOM_TEXT_HOSTNAME, DOMAIN_NAME_REGEX
+    DOT_ATOM_TEXT, DOT_ATOM_TEXT_INTL, ATEXT_RE, ATEXT_INTL_RE, ATEXT_HOSTNAME_INTL, QTEXT_INTL, \
+    DNS_LABEL_LENGTH_LIMIT, DOT_ATOM_TEXT_HOSTNAME, DOMAIN_NAME_REGEX, DOMAIN_LITERAL_CHARS
 
 import re
 import unicodedata
 import idna  # implements IDNA 2008; Python's codec is only IDNA 2003
+import ipaddress
+from typing import Optional
 
 
 def get_length_reason(addr, utf8=False, limit=EMAIL_MAX_LENGTH):
     """Helper function to return an error message related to invalid length."""
     diff = len(addr) - limit
     prefix = "at least " if utf8 else ""
     suffix = "s" if diff > 1 else ""
     return f"({prefix}{diff} character{suffix} too many)"
 
 
 def safe_character_display(c):
     # Return safely displayable characters in quotes.
+    if c == '\\':
+        return f"\"{c}\""  # can't use repr because it escapes it
     if unicodedata.category(c)[0] in ("L", "N", "P", "S"):
         return repr(c)
 
     # Construct a hex string in case the unicode name doesn't exist.
     if ord(c) < 0xFFFF:
         h = f"U+{ord(c):04x}".upper()
     else:
         h = f"U+{ord(c):08x}".upper()
 
     # Return the character name or, if it has no name, the hex string.
     return unicodedata.name(c, h)
 
 
-def validate_email_local_part(local: str, allow_smtputf8: bool = True, allow_empty_local: bool = False):
+def validate_email_local_part(local: str, allow_smtputf8: bool = True, allow_empty_local: bool = False,
+                              quoted_local_part: bool = False):
     """Validates the syntax of the local part of an email address."""
 
     if len(local) == 0:
         if not allow_empty_local:
             raise EmailSyntaxError("There must be something before the @-sign.")
         else:
             # The caller allows an empty local part. Useful for validating certain
             # Postfix aliases.
             return {
                 "local_part": local,
                 "ascii_local_part": local,
                 "smtputf8": False,
             }
 
-    # Check the length of the local part by couting characters.
+    # Check the length of the local part by counting characters.
     # (RFC 5321 4.5.3.1.1)
     # We're checking the number of characters here. If the local part
     # is ASCII-only, then that's the same as bytes (octets). If it's
     # internationalized, then the UTF-8 encoding may be longer, but
     # that may not be relevant. We will check the total address length
     # instead.
     if len(local) > LOCAL_PART_MAX_LENGTH:
         reason = get_length_reason(local, limit=LOCAL_PART_MAX_LENGTH)
         raise EmailSyntaxError(f"The email address is too long before the @-sign {reason}.")
 
     # Check the local part against the non-internationalized regular expression.
     # Most email addresses match this regex so it's probably fastest to check this first.
-    # (RFC 2822 3.2.4)
+    # (RFC 5322 3.2.3)
+    # All local parts matching the dot-atom rule are also valid as a quoted string
+    # so if it was originally quoted (quoted_local_part is True) and this regex matches,
+    # it's ok.
+    # (RFC 5321 4.1.2 / RFC 5322 3.2.4).
     m = DOT_ATOM_TEXT.match(local)
     if m:
-        # It's valid.
+        # It's valid. And since it's just the permitted ASCII characters,
+        # it's normalized and safe. If the local part was originally quoted,
+        # the quoting was unnecessary and it'll be returned as normalized to
+        # non-quoted form.
 
-        # Return the local part unchanged and flag that SMTPUTF8 is not needed.
+        # Return the local part and flag that SMTPUTF8 is not needed.
         return {
             "local_part": local,
             "ascii_local_part": local,
             "smtputf8": False,
         }
 
-    # The local part failed the ASCII check. Try the extended character set
+    # The local part failed the basic dot-atom check. Try the extended character set
     # for internationalized addresses. It's the same pattern but with additional
     # characters permitted.
+    # RFC 6531 section 3.3.
+    valid: Optional[str] = None
+    requires_smtputf8 = False
     m = DOT_ATOM_TEXT_INTL.match(local)
     if m:
-        # It's valid.
-
         # But international characters in the local part may not be permitted.
         if not allow_smtputf8:
             # Check for invalid characters against the non-internationalized
             # permitted character set.
-            # (RFC 2822 Section 3.2.4 / RFC 5322 Section 3.2.3)
+            # (RFC 5322 3.2.3)
             bad_chars = set(
                 safe_character_display(c)
                 for c in local
                 if not ATEXT_RE.match(c)
             )
             if bad_chars:
                 raise EmailSyntaxError("Internationalized characters before the @-sign are not supported: " + ", ".join(sorted(bad_chars)) + ".")
 
             # Although the check above should always find something, fall back to this just in case.
             raise EmailSyntaxError("Internationalized characters before the @-sign are not supported.")
 
-        # RFC 6532 section 3.1 also says that Unicode NFC normalization should be applied,
+        # It's valid.
+        valid = "dot-atom"
+        requires_smtputf8 = True
+
+    # There are no syntactic restrictions on quoted local parts, so if
+    # it was originally quoted, it is probably valid. More characters
+    # are allowed, like @-signs, spaces, and quotes, and there are no
+    # restrictions on the placement of dots, as in dot-atom local parts.
+    elif quoted_local_part:
+        # Check for invalid characters in a quoted string local part.
+        # (RFC 5321 4.1.2. RFC 5322 lists additional permitted *obsolete*
+        # characters which are *not* allowed here. RFC 6531 section 3.3
+        # extends the range to UTF8 strings.)
+        bad_chars = set(
+            safe_character_display(c)
+            for c in local
+            if not QTEXT_INTL.match(c)
+        )
+        if bad_chars:
+            raise EmailSyntaxError("The email address contains invalid characters in quotes before the @-sign: " + ", ".join(sorted(bad_chars)) + ".")
+
+        # See if any characters are outside of the ASCII range.
+        bad_chars = set(
+            safe_character_display(c)
+            for c in local
+            if not (32 <= ord(c) <= 126)
+        )
+        if bad_chars:
+            requires_smtputf8 = True
+
+            # International characters in the local part may not be permitted.
+            if not allow_smtputf8:
+                raise EmailSyntaxError("Internationalized characters before the @-sign are not supported: " + ", ".join(sorted(bad_chars)) + ".")
+
+        # It's valid.
+        valid = "quoted"
+
+    # If the local part matches the internationalized dot-atom form or was quoted,
+    # perform normalization and additional checks for Unicode strings.
+    if valid:
+        # RFC 6532 section 3.1 says that Unicode NFC normalization should be applied,
         # so we'll return the normalized local part in the return value.
         local = unicodedata.normalize("NFC", local)
 
-        # Check for unsafe characters.
+        # Check that the local part is a valid, safe, and sensible Unicode string.
         # Some of this may be redundant with the range U+0080 to U+10FFFF that is checked
-        # by DOT_ATOM_TEXT_INTL. Other characters may be permitted by the email specs, but
-        # they may not be valid, safe, or sensible Unicode strings.
-        check_unsafe_chars(local)
+        # by DOT_ATOM_TEXT_INTL and QTEXT_INTL. Other characters may be permitted by the
+        # email specs, but they may not be valid, safe, or sensible Unicode strings.
+        # See the function for rationale.
+        check_unsafe_chars(local, allow_space=(valid == "quoted"))
 
         # Try encoding to UTF-8. Failure is possible with some characters like
         # surrogate code points, but those are checked above. Still, we don't
         # want to have an unhandled exception later.
         try:
             local.encode("utf8")
         except ValueError:
             raise EmailSyntaxError("The email address contains an invalid character.")
 
-        # Flag that SMTPUTF8 will be required for deliverability.
+        # If this address passes only by the quoted string form, re-quote it
+        # and backslash-escape quotes and backslashes (removing any unnecessary
+        # escapes). Per RFC 5321 4.1.2, "all quoted forms MUST be treated as equivalent,
+        # and the sending system SHOULD transmit the form that uses the minimum quoting possible."
+        if valid == "quoted":
+            local = '"' + re.sub(r'(["\\])', r'\\\1', local) + '"'
+
         return {
             "local_part": local,
-            "ascii_local_part": None,  # no ASCII form is possible
-            "smtputf8": True,
+            "ascii_local_part": local if not requires_smtputf8 else None,
+            "smtputf8": requires_smtputf8,
         }
 
-    # It's not a valid local part either non-internationalized or internationalized.
-    # Let's find out why.
+    # It's not a valid local part. Let's find out why.
+    # (Since quoted local parts are all valid or handled above, these checks
+    # don't apply in those cases.)
 
     # Check for invalid characters.
-    # (RFC 2822 Section 3.2.4 / RFC 5322 Section 3.2.3, plus RFC 6531 section 3.3)
+    # (RFC 5322 3.2.3, plus RFC 6531 3.3)
     bad_chars = set(
         safe_character_display(c)
         for c in local
         if not ATEXT_INTL_RE.match(c)
     )
     if bad_chars:
         raise EmailSyntaxError("The email address contains invalid characters before the @-sign: " + ", ".join(sorted(bad_chars)) + ".")
 
     # Check for dot errors imposted by the dot-atom rule.
-    # (RFC 2822 3.2.4)
+    # (RFC 5322 3.2.3)
     check_dot_atom(local, 'An email address cannot start with a {}.', 'An email address cannot have a {} immediately before the @-sign.', is_hostname=False)
 
     # All of the reasons should already have been checked, but just in case
     # we have a fallback message.
     raise EmailSyntaxError("The email address contains invalid characters before the @-sign.")
 
 
-def check_unsafe_chars(s):
+def check_unsafe_chars(s, allow_space=False):
     # Check for unsafe characters or characters that would make the string
     # invalid or non-sensible Unicode.
     bad_chars = set()
     for i, c in enumerate(s):
         category = unicodedata.category(c)
         if category[0] in ("L", "N", "P", "S"):
             # Letters, numbers, punctuation, and symbols are permitted.
@@ -152,21 +214,33 @@
         elif category[0] == "M":
             # Combining character in first position would combine with something
             # outside of the email address if concatenated, so they are not safe.
             # We also check if this occurs after the @-sign, which would not be
             # sensible.
             if i == 0:
                 bad_chars.add(c)
+        elif category == "Zs":
+            # Spaces outside of the ASCII range are not specifically disallowed in
+            # internationalized addresses as far as I can tell, but they violate
+            # the spirit of the non-internationalized specification that email
+            # addresses do not contain ASCII spaces when not quoted. Excluding
+            # ASCII spaces when not quoted is handled directly by the atom regex.
+            #
+            # In quoted-string local parts, spaces are explicitly permitted, and
+            # the ASCII space has category Zs, so we must allow it here, and we'll
+            # allow all Unicode spaces to be consistent.
+            if not allow_space:
+                bad_chars.add(c)
         elif category[0] == "Z":
-            # Spaces and line/paragraph characters (Z) outside of the ASCII range
-            # are not specifically disallowed as far as I can tell, but they
-            # violate the spirit of the non-internationalized specification that
-            # email addresses do not contain spaces or line breaks when not quoted.
+            # The two line and paragraph separator characters (in categories Zl and Zp)
+            # are not specifically disallowed in internationalized addresses
+            # as far as I can tell, but they violate the spirit of the non-internationalized
+            # specification that email addresses do not contain line breaks when not quoted.
             bad_chars.add(c)
-        elif category[0] == "C":
+        elif category[0] in ("C", "Z"):
             # Control, format, surrogate, private use, and unassigned code points (C)
             # are all unsafe in various ways. Control and format characters can affect
             # text rendering if the email address is concatenated with other text.
             # Bidirectional format characters are unsafe, even if used properly, because
             # they cause an email address to render as a different email address.
             # Private use characters do not make sense for publicly deliverable
             # email addresses.
@@ -177,15 +251,15 @@
             bad_chars.add(c)
     if bad_chars:
         raise EmailSyntaxError("The email address contains unsafe characters: "
                                + ", ".join(safe_character_display(c) for c in sorted(bad_chars)) + ".")
 
 
 def check_dot_atom(label, start_descr, end_descr, is_hostname):
-    # RFC 2822 3.2.4
+    # RFC 5322 3.2.3
     if label.endswith("."):
         raise EmailSyntaxError(end_descr.format("period"))
     if label.startswith("."):
         raise EmailSyntaxError(start_descr.format("period"))
     if ".." in label:
         raise EmailSyntaxError("An email address cannot have two periods in a row.")
 
@@ -195,21 +269,17 @@
             raise EmailSyntaxError(end_descr.format("hyphen"))
         if label.startswith("-"):
             raise EmailSyntaxError(start_descr.format("hyphen"))
         if ".-" in label or "-." in label:
             raise EmailSyntaxError("An email address cannot have a period and a hyphen next to each other.")
 
 
-def validate_email_domain_part(domain, test_environment=False, globally_deliverable=True):
+def validate_email_domain_name(domain, test_environment=False, globally_deliverable=True):
     """Validates the syntax of the domain part of an email address."""
 
-    # Empty?
-    if len(domain) == 0:
-        raise EmailSyntaxError("There must be something after the @-sign.")
-
     # Check for invalid characters before normalization.
     # (RFC 952 plus RFC 6531 section 3.3 for internationalized addresses)
     bad_chars = set(
         safe_character_display(c)
         for c in domain
         if not ATEXT_HOSTNAME_INTL.match(c)
     )
@@ -234,15 +304,15 @@
 
     # The domain part is made up period-separated "labels." Each label must
     # have at least one character and cannot start or end with dashes, which
     # means there are some surprising restrictions on periods and dashes.
     # Check that before we do IDNA encoding because the IDNA library gives
     # unfriendly errors for these cases, but after UTS-46 normalization because
     # it can insert periods and hyphens (from fullwidth characters).
-    # (RFC 952, RFC 2822 3.2.4)
+    # (RFC 952, RFC 1123 2.1, RFC 5322 3.2.3)
     check_dot_atom(domain, 'An email address cannot have a {} immediately after the @-sign.', 'An email address cannot end with a {}.', is_hostname=True)
 
     # Check for RFC 5890's invalid R-LDH labels, which are labels that start
     # with two characters other than "xn" and two dashes.
     for label in domain.split("."):
         if re.match(r"(?!xn)..--", label, re.I):
             raise EmailSyntaxError("An email address cannot have two letters followed by two dashes immediately after the @-sign or after a period, except Punycode.")
@@ -355,7 +425,67 @@
     # which is better for display purposes. This should also take care
     # of RFC 6532 section 3.1's suggestion to apply Unicode NFC
     # normalization to addresses.
     return {
         "ascii_domain": ascii_domain,
         "domain": domain_i18n,
     }
+
+
+def validate_email_domain_literal(domain_literal, allow_domain_literal=False):
+    # This is obscure domain-literal syntax. Parse it and return
+    # a compressed/normalized address.
+    # RFC 5321 4.1.3 and RFC 5322 3.4.1.
+
+    # Try to parse the domain literal as an IPv4 address.
+    # There is no tag for IPv4 addresses, so we can never
+    # be sure if the user intends an IPv4 address.
+    if re.match(r"^[0-9\.]+$", domain_literal):
+        try:
+            addr = ipaddress.IPv4Address(domain_literal)
+        except ValueError as e:
+            raise EmailSyntaxError(f"The address in brackets after the @-sign is not valid: It is not an IPv4 address ({e}) or is missing an address literal tag.")
+        if not allow_domain_literal:
+            raise EmailSyntaxError("A bracketed IPv4 address after the @-sign is not allowed here.")
+
+        # Return the IPv4Address object and the domain back unchanged.
+        return {
+            "domain_address": addr,
+            "domain": f"[{addr}]",
+        }
+
+    # If it begins with "IPv6:" it's an IPv6 address.
+    if domain_literal.startswith("IPv6:"):
+        try:
+            addr = ipaddress.IPv6Address(domain_literal[5:])
+        except ValueError as e:
+            raise EmailSyntaxError(f"The IPv6 address in brackets after the @-sign is not valid ({e}).")
+        if not allow_domain_literal:
+            raise EmailSyntaxError("A bracketed IPv6 address after the @-sign is not allowed here.")
+
+        # Return the IPv6Address object and construct a normalized
+        # domain literal.
+        return {
+            "domain_address": addr,
+            "domain": f"[IPv6:{addr.compressed}]",
+        }
+
+    if ":" not in domain_literal:
+        raise EmailSyntaxError("The part after the @-sign in brackets is not an IPv4 address and has no address literal tag.")
+
+    # The tag (the part before the colon) has character restrictions,
+    # but since it must come from a registry of tags (in which only "IPv6" is defined),
+    # there's no need to check the syntax of the tag. See RFC 5321 4.1.2.
+
+    # Check for permitted ASCII characters. This actually doesn't matter
+    # since there will be an exception after anyway.
+    bad_chars = set(
+        safe_character_display(c)
+        for c in domain_literal
+        if not DOMAIN_LITERAL_CHARS.match(c)
+    )
+    if bad_chars:
+        raise EmailSyntaxError("The part after the @-sign contains invalid characters in brackets: " + ", ".join(sorted(bad_chars)) + ".")
+
+    # There are no other domain literal tags.
+    # https://www.iana.org/assignments/address-literal-tags/address-literal-tags.xhtml
+    raise EmailSyntaxError("The part after the @-sign contains an invalid address literal tag in brackets.")
```

### Comparing `email_validator-2.0.0.dev4/email_validator/validate_email.py` & `email_validator-2.0.0.post1/email_validator/validate_email.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from typing import Optional, Union
 
 from .exceptions_types import EmailSyntaxError, ValidatedEmail
-from .syntax import validate_email_local_part, validate_email_domain_part, get_length_reason
-from .rfc_constants import EMAIL_MAX_LENGTH
+from .syntax import validate_email_local_part, validate_email_domain_name, validate_email_domain_literal, get_length_reason
+from .rfc_constants import EMAIL_MAX_LENGTH, QUOTED_LOCAL_PART_ADDR, CASE_INSENSITIVE_MAILBOX_NAMES
 
 
 def validate_email(
     email: Union[str, bytes],
     # /, # not supported in Python 3.6, 3.7
     *,
     allow_smtputf8: Optional[bool] = None,
     allow_empty_local: bool = False,
+    allow_quoted_local: Optional[bool] = None,
+    allow_domain_literal: Optional[bool] = None,
     check_deliverability: Optional[bool] = None,
     test_environment: Optional[bool] = None,
     globally_deliverable: Optional[bool] = None,
     timeout: Optional[int] = None,
     dns_resolver: Optional[object] = None
 ) -> ValidatedEmail:
     """
     Validates an email address, raising an EmailNotValidError if the address is not valid or returning a dict of
     information when the address is valid. The email argument can be a str or a bytes instance,
     but if bytes it must be ASCII-only. This is the main method of this library.
     """
 
     # Fill in default values of arguments.
-    from . import ALLOW_SMTPUTF8, CHECK_DELIVERABILITY, TEST_ENVIRONMENT, GLOBALLY_DELIVERABLE, DEFAULT_TIMEOUT
+    from . import ALLOW_SMTPUTF8, ALLOW_QUOTED_LOCAL, ALLOW_DOMAIN_LITERAL, \
+        GLOBALLY_DELIVERABLE, CHECK_DELIVERABILITY, TEST_ENVIRONMENT, DEFAULT_TIMEOUT
     if allow_smtputf8 is None:
         allow_smtputf8 = ALLOW_SMTPUTF8
+    if allow_quoted_local is None:
+        allow_quoted_local = ALLOW_QUOTED_LOCAL
+    if allow_domain_literal is None:
+        allow_domain_literal = ALLOW_DOMAIN_LITERAL
     if check_deliverability is None:
         check_deliverability = CHECK_DELIVERABILITY
     if test_environment is None:
         test_environment = TEST_ENVIRONMENT
     if globally_deliverable is None:
         globally_deliverable = GLOBALLY_DELIVERABLE
     if timeout is None:
@@ -41,38 +48,85 @@
     # on the wire with SMTP.
     if not isinstance(email, str):
         try:
             email = email.decode("ascii")
         except ValueError:
             raise EmailSyntaxError("The email address is not valid ASCII.")
 
-    # At-sign.
-    parts = email.split('@')
-    if len(parts) != 2:
-        raise EmailSyntaxError("The email address is not valid. It must have exactly one @-sign.")
+    # Typical email addresses have a single @-sign, but the
+    # awkward "quoted string" local part form (RFC 5321 4.1.2)
+    # allows @-signs (and escaped quotes) to appear in the local
+    # part if the local part is quoted. If the address is quoted,
+    # split it at a non-escaped @-sign and unescape the escaping.
+    quoted_local_part = False
+    m = QUOTED_LOCAL_PART_ADDR.match(email)
+    if m:
+        quoted_local_part = True
+        local_part, domain_part = m.groups()
+
+        # Remove backslashes.
+        import re
+        local_part = re.sub(r"\\(.)", "\\1", local_part)
+
+    else:
+        # Split at the one and only at-sign.
+        parts = email.split('@')
+        if len(parts) != 2:
+            raise EmailSyntaxError("The email address is not valid. It must have exactly one @-sign.")
+        local_part, domain_part = parts
 
     # Collect return values in this instance.
     ret = ValidatedEmail()
-    ret.original_email = email
+    ret.original = email
 
     # Validate the email address's local part syntax and get a normalized form.
-    local_part_info = validate_email_local_part(parts[0],
+    # If the original address was quoted and the decoded local part is a valid
+    # unquoted local part, then we'll get back a normalized (unescaped) local
+    # part.
+    local_part_info = validate_email_local_part(local_part,
                                                 allow_smtputf8=allow_smtputf8,
-                                                allow_empty_local=allow_empty_local)
+                                                allow_empty_local=allow_empty_local,
+                                                quoted_local_part=quoted_local_part)
+    if quoted_local_part and not allow_quoted_local:
+        raise EmailSyntaxError("Quoting the part before the @-sign is not allowed here.")
     ret.local_part = local_part_info["local_part"]
     ret.ascii_local_part = local_part_info["ascii_local_part"]
     ret.smtputf8 = local_part_info["smtputf8"]
 
+    # Some local parts are required to be case-insensitive, so we should normalize
+    # to lowercase.
+    # RFC 2142
+    if ret.ascii_local_part is not None \
+       and ret.ascii_local_part.lower() in CASE_INSENSITIVE_MAILBOX_NAMES \
+       and ret.local_part is not None:
+        ret.ascii_local_part = ret.ascii_local_part.lower()
+        ret.local_part = ret.local_part.lower()
+
     # Validate the email address's domain part syntax and get a normalized form.
-    domain_part_info = validate_email_domain_part(parts[1], test_environment=test_environment, globally_deliverable=globally_deliverable)
-    ret.domain = domain_part_info["domain"]
-    ret.ascii_domain = domain_part_info["ascii_domain"]
+    is_domain_literal = False
+    if len(domain_part) == 0:
+        raise EmailSyntaxError("There must be something after the @-sign.")
+
+    elif domain_part.startswith("[") and domain_part.endswith("]"):
+        # Parse the address in the domain literal and get back a normalized domain.
+        domain_part_info = validate_email_domain_literal(domain_part[1:-1], allow_domain_literal=allow_domain_literal)
+        ret.domain = domain_part_info["domain"]
+        ret.ascii_domain = domain_part_info["domain"]  # Domain literals are always ASCII.
+        ret.domain_address = domain_part_info["domain_address"]
+        is_domain_literal = True  # Prevent deliverability checks.
+
+    else:
+        # Check the syntax of the domain and get back a normalized
+        # internationalized and ASCII form.
+        domain_part_info = validate_email_domain_name(domain_part, test_environment=test_environment, globally_deliverable=globally_deliverable)
+        ret.domain = domain_part_info["domain"]
+        ret.ascii_domain = domain_part_info["ascii_domain"]
 
     # Construct the complete normalized form.
-    ret.email = ret.local_part + "@" + ret.domain
+    ret.normalized = ret.local_part + "@" + ret.domain
 
     # If the email address has an ASCII form, add it.
     if not ret.smtputf8:
         if not ret.ascii_domain:
             raise Exception("Missing ASCII domain.")
         ret.ascii_email = (ret.ascii_local_part or "") + "@" + ret.ascii_domain
     else:
@@ -95,38 +149,42 @@
     # form, I don't think the internationalized form can be longer, and so the ASCII
     # form length check would be sufficient. If there is no ASCII form, then we have
     # to check the UTF-8 encoding. The UTF-8 encoding could be up to about four times
     # longer than the number of characters.
     #
     # See the length checks on the local part and the domain.
     if ret.ascii_email and len(ret.ascii_email) > EMAIL_MAX_LENGTH:
-        if ret.ascii_email == ret.email:
+        if ret.ascii_email == ret.normalized:
             reason = get_length_reason(ret.ascii_email)
-        elif len(ret.email) > EMAIL_MAX_LENGTH:
+        elif len(ret.normalized) > EMAIL_MAX_LENGTH:
             # If there are more than 254 characters, then the ASCII
             # form is definitely going to be too long.
-            reason = get_length_reason(ret.email, utf8=True)
+            reason = get_length_reason(ret.normalized, utf8=True)
         else:
             reason = "(when converted to IDNA ASCII)"
         raise EmailSyntaxError(f"The email address is too long {reason}.")
-    if len(ret.email.encode("utf8")) > EMAIL_MAX_LENGTH:
-        if len(ret.email) > EMAIL_MAX_LENGTH:
+    if len(ret.normalized.encode("utf8")) > EMAIL_MAX_LENGTH:
+        if len(ret.normalized) > EMAIL_MAX_LENGTH:
             # If there are more than 254 characters, then the UTF-8
             # encoding is definitely going to be too long.
-            reason = get_length_reason(ret.email, utf8=True)
+            reason = get_length_reason(ret.normalized, utf8=True)
         else:
             reason = "(when encoded in bytes)"
         raise EmailSyntaxError(f"The email address is too long {reason}.")
 
     if check_deliverability and not test_environment:
         # Validate the email address's deliverability using DNS
         # and update the return dict with metadata.
 
+        if is_domain_literal:
+            # There is nothing to check --- skip deliverability checks.
+            return ret
+
         # Lazy load `deliverability` as it is slow to import (due to dns.resolver)
         from .deliverability import validate_email_deliverability
         deliverability_info = validate_email_deliverability(
-            ret["domain"], ret["domain_i18n"], timeout, dns_resolver
+            ret.ascii_domain, ret.domain, timeout, dns_resolver
         )
         for key, value in deliverability_info.items():
             setattr(ret, key, value)
 
     return ret
```

### Comparing `email_validator-2.0.0.dev4/email_validator.egg-info/PKG-INFO` & `email_validator-2.0.0.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: email-validator
-Version: 2.0.0.dev4
-Summary: A robust email address syntax and deliverability validation library.
-Home-page: https://github.com/JoshData/python-email-validator
-Author: Joshua Tauberer
-Author-email: jt@occams.info
-License: CC0 (copyright waived)
-Keywords: email address validator
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 email-validator: Validate Email Addresses
 =========================================
 
 A robust email address syntax and deliverability validation library for
 Python 3.7+ by [Joshua Tauberer](https://joshdata.me).
 
 This library validates that a string is of the form `name@example.com`
@@ -33,29 +10,31 @@
 users by their email address like on a registration/login form (but not
 necessarily for composing an email message, see below).
 
 Key features:
 
 * Checks that an email address has the correct syntax --- good for
   registration/login forms or other uses related to identifying users.
-  Rejects obsolete email address syntax that you'd find unexpected.
 * Gives friendly English error messages when validation fails that you
   can display to end-users.
 * Checks deliverability (optional): Does the domain name resolve?
   (You can override the default DNS resolver to add query caching.)
 * Supports internationalized domain names and internationalized local parts.
-  Blocks unsafe characters for your safety.
+* Rejects addresses with unsafe Unicode characters, obsolete email address
+  syntax that you'd find unexpected, special use domain names like
+  `@localhost`, and domains without a dot by default. This is an
+  opinionated library!
 * Normalizes email addresses (important for internationalized
-  addresses! see below).
+  and quoted-string addresses! see below).
+* Python type annotations are used.
 
-This library does NOT permit obsolete forms of email addresses, so
-if you need strict validation against the email specs exactly, use
-[pyIsEmail](https://github.com/michaelherold/pyIsEmail) or try
-[flanker](https://github.com/mailgun/flanker) if you are parsing the
-To: line of an email.
+This is an opinionated library. You should definitely also consider using
+the less-opinionated [pyIsEmail](https://github.com/michaelherold/pyIsEmail) and
+[flanker](https://github.com/mailgun/flanker) if they are better for your
+use case.
 
 [![Build Status](https://github.com/JoshData/python-email-validator/actions/workflows/test_and_build.yaml/badge.svg)](https://github.com/JoshData/python-email-validator/actions/workflows/test_and_build.yaml)
 
 View the [CHANGELOG / Release Notes](CHANGELOG.md) for the version history of changes in the library. Occasionally this README is ahead of the latest published package --- see the CHANGELOG for details.
 
 ---
 
@@ -75,29 +54,31 @@
 
 If you're validating a user's email address before creating a user
 account in your application, you might do this:
 
 ```python
 from email_validator import validate_email, EmailNotValidError
 
-email = "my+address@mydomain.tld"
-is_new_account = True # False for login pages
+email = "my+address@example.org"
 
 try:
-  # Check that the email address is valid.
-  validation = validate_email(email, check_deliverability=is_new_account)
 
-  # Take the normalized form of the email address
-  # for all logic beyond this point (especially
-  # before going to a database query where equality
-  # may not take into account Unicode normalization).  
-  email = validation.email
+  # Check that the email address is valid. Turn on check_deliverability
+  # for first-time validations like on account creation pages (but not
+  # login pages).
+  emailinfo = validate_email(email, check_deliverability=False)
+
+  # After this point, use only the normalized form of the email address,
+  # especially before going to a database query.
+  email = emailinfo.normalized
+
 except EmailNotValidError as e:
-  # Email is not valid.
-  # The exception message is human-readable.
+
+  # The exception message is human-readable explanation of why it's
+  # not a valid (or deliverable) email address.
   print(str(e))
 ```
 
 This validates the address and gives you its normalized form. You should
 **put the normalized form in your database** and always normalize before
 checking if an address is in your database. When using this in a login form,
 set `check_deliverability` to `False` to avoid unnecessary DNS queries.
@@ -121,76 +102,83 @@
 exception classes are subclasses of `EmailNotValidError`, which in turn
 is a subclass of `ValueError`.
 
 But when an email address is valid, an object is returned containing
 a normalized form of the email address (which you should use!) and
 other information.
 
-The validator doesn't permit obsoleted forms of email addresses that no
-one uses anymore even though they are still valid and deliverable, since
+The validator doesn't, by default, permit obsoleted forms of email addresses
+that no one uses anymore even though they are still valid and deliverable, since
 they will probably give you grief if you're using email for login. (See
-later in the document about that.)
+later in the document about how to allow some obsolete forms.)
 
-The validator checks that the domain name in the email address has a
-DNS MX record (except a NULL MX record) indicating that it can receive
-email (or a fallback A-record, see below).
-There is nothing to be gained by trying to actually contact an SMTP
-server, so that's not done here. For privacy, security, and practicality
-reasons servers are good at not giving away whether an address is
+The validator optionally checks that the domain name in the email address has
+a DNS MX record indicating that it can receive email. (Except a Null MX record.
+If there is no MX record, a fallback A/AAAA-record is permitted, unless
+a reject-all SPF record is present.) DNS is slow and sometimes unavailable or
+unreliable, so consider whether these checks are useful for your use case and
+turn them off if they aren't.
+There is nothing to be gained by trying to actually contact an SMTP server, so
+that's not done here. For privacy, security, and practicality reasons, servers
+are good at not giving away whether an address is
 deliverable or not: email addresses that appear to accept mail at first
 can bounce mail after a delay, and bounced mail may indicate a temporary
 failure of a good email address (sometimes an intentional failure, like
 greylisting).
 
 ### Options
 
 The `validate_email` function also accepts the following keyword arguments
 (defaults are as shown below):
 
-`check_deliverability=True`: If true, a DNS query is made to check that a non-null MX record is present for the domain-part of the email address (or if not, an A/AAAA record as an MX fallback can be present but in that case a reject-all SPF record must not be present). Set to `False` to skip this DNS-based check. DNS is slow and sometimes unavailable, so consider whether these checks are useful for your use case. It is recommended to pass `False` when performing validation for login pages (but not account creation pages) since re-validation of a previously validated domain in your database by querying DNS at every login is probably undesirable. You can also set `email_validator.CHECK_DELIVERABILITY` to `False` to turn this off for all calls by default.
+`check_deliverability=True`: If true, DNS queries are made to check that the domain name in the email address (the part after the @-sign) can receive mail, as described above. Set to `False` to skip this DNS-based check. It is recommended to pass `False` when performing validation for login pages (but not account creation pages) since re-validation of a previously validated domain in your database by querying DNS at every login is probably undesirable. You can also set `email_validator.CHECK_DELIVERABILITY` to `False` to turn this off for all calls by default.
 
-`dns_resolver=None`: Pass an instance of [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to control the DNS resolver including setting a timeout and [a cache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html). The `caching_resolver` function shown above is a helper function to construct a dns.resolver.Resolver with a [LRUCache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html#dns.resolver.LRUCache). Reuse the same resolver instance across calls to `validate_email` to make use of the cache.
+`dns_resolver=None`: Pass an instance of [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to control the DNS resolver including setting a timeout and [a cache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html). The `caching_resolver` function shown below is a helper function to construct a dns.resolver.Resolver with a [LRUCache](https://dnspython.readthedocs.io/en/latest/resolver-caching.html#dns.resolver.LRUCache). Reuse the same resolver instance across calls to `validate_email` to make use of the cache.
 
-`test_environment=False`: DNS-based deliverability checks are disabled and  `test` and `subdomain.test` domain names are permitted (see below). You can also set `email_validator.TEST_ENVIRONMENT` to `True` to turn it on for all calls by default.
+`test_environment=False`: If `True`, DNS-based deliverability checks are disabled and  `test` and `**.test` domain names are permitted (see below). You can also set `email_validator.TEST_ENVIRONMENT` to `True` to turn it on for all calls by default.
 
 `allow_smtputf8=True`: Set to `False` to prohibit internationalized addresses that would
     require the
     [SMTPUTF8](https://tools.ietf.org/html/rfc6531) extension. You can also set `email_validator.ALLOW_SMTPUTF8` to `False` to turn it off for all calls by default.
 
+`allow_quoted_local=False`: Set to `True` to allow obscure and potentially problematic email addresses in which the part of the address before the @-sign contains spaces, @-signs, or other surprising characters when the local part is surrounded in quotes (so-called quoted-string local parts). In the object returned by `validate_email`, the normalized local part removes any unnecessary backslash-escaping and even removes the surrounding quotes if the address would be valid without them. You can also set `email_validator.ALLOW_QUOTED_LOCAL` to `True` to turn this on for all calls by default.
+
+`allow_domain_literal=False`: Set to `True` to allow bracketed IPv4 and "IPv6:"-prefixd IPv6 addresses in the domain part of the email address. No deliverability checks are performed for these addresses. In the object returned by `validate_email`, the normalized domain will use the condensed IPv6 format, if applicable. The object's `domain_address` attribute will hold the parsed `ipaddress.IPv4Address` or `ipaddress.IPv6Address` object if applicable. You can also set `email_validator.ALLOW_DOMAIN_LITERAL` to `True` to turn this on for all calls by default.
+
 `allow_empty_local=False`: Set to `True` to allow an empty local part (i.e.
     `@example.com`), e.g. for validating Postfix aliases.
     
 
 ### DNS timeout and cache
 
 When validating many email addresses or to control the timeout (the default is 15 seconds), create a caching [dns.resolver.Resolver](https://dnspython.readthedocs.io/en/latest/resolver-class.html) to reuse in each call. The `caching_resolver` function returns one easily for you:
 
 ```python
 from email_validator import validate_email, caching_resolver
 
 resolver = caching_resolver(timeout=10)
 
 while True:
-  email = validate_email(email, dns_resolver=resolver).email
+  validate_email(email, dns_resolver=resolver)
 ```
 
 ### Test addresses
 
-This library rejects email addresess that use the [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml) `invalid`, `localhost`, `test`, and some others by raising `EmailSyntaxError`. This is to protect your system from abuse: You probably don't want a user to be able to cause an email to be sent to `localhost`. However, in your non-production test environments you may want to use `@test` or `@myname.test` email addresses. There are three ways you can allow this:
+This library rejects email addresess that use the [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml) `invalid`, `localhost`, `test`, and some others by raising `EmailSyntaxError`. This is to protect your system from abuse: You probably don't want a user to be able to cause an email to be sent to `localhost` (although they might be able to still do so via a malicious MX record). However, in your non-production test environments you may want to use `@test` or `@myname.test` email addresses. There are three ways you can allow this:
 
 1. Add `test_environment=True` to the call to `validate_email` (see above).
-2. Set `email_validator.TEST_ENVIRONMENT` to `True`.
-3. Remove the special-use domain name that you want to use from `email_validator.SPECIAL_USE_DOMAIN_NAMES`:
+2. Set `email_validator.TEST_ENVIRONMENT` to `True` globally.
+3. Remove the special-use domain name that you want to use from `email_validator.SPECIAL_USE_DOMAIN_NAMES`, e.g.:
 
 ```python
 import email_validator
 email_validator.SPECIAL_USE_DOMAIN_NAMES.remove("test")
 ```
 
-It is tempting to use `@example.com/net/org` in tests. These domains are reserved to IANA for use in documentation so there is no risk of accidentally emailing someone at those domains. But beware that this library will reject these domain names if DNS-based deliverability checks are not disabled because these domains do not resolve to domains that accept email. In tests, consider using your own domain name or `@test` or `@myname.test` instead.
+It is tempting to use `@example.com/net/org` in tests. They are *not* in this library's `SPECIAL_USE_DOMAIN_NAMES` list so you can, but shouldn't, use them. These domains are reserved to IANA for use in documentation so there is no risk of accidentally emailing someone at those domains. But beware that this library will nevertheless reject these domain names if DNS-based deliverability checks are not disabled because these domains do not resolve to domains that accept email. In tests, consider using your own domain name or `@test` or `@myname.test` instead.
 
 Internationalized email addresses
 ---------------------------------
 
 The email protocol SMTP and the domain name system DNS have historically
 only allowed English (ASCII) characters in email addresses and domain names,
 respectively. Each has adapted to internationalization in a separate
@@ -219,16 +207,17 @@
 local parts, a wider range of Unicode characters are allowed.
 
 A surprisingly large number of Unicode characters are not safe to display,
 especially when the email address is concatenated with other text, so this
 library tries to protect you by not permitting resvered, non-, private use,
 formatting (which can be used to alter the display order of characters),
 whitespace, and control characters, and combining characters
-as the first character (so that they cannot combine with something outside
-of the email address string). See https://qntm.org/safe and https://trojansource.codes/
+as the first character of the local part and the domain name (so that they
+cannot combine with something outside of the email address string or with
+the @-sign). See https://qntm.org/safe and https://trojansource.codes/
 for relevant prior work. (Other than whitespace, these are checks that
 you should be applying to nearly all user inputs in a security-sensitive
 context.)
 
 These character checks are performed after Unicode normalization (see below),
 so you are only fully protected if you replace all user-provided email addresses
 with the normalized email address string returned by this library. This does not
@@ -256,38 +245,44 @@
 If your mail submission library doesn't support Unicode at all --- even
 in the domain part of the address --- then immediately prior to mail
 submission you must replace the email address with its ASCII-ized form.
 This library gives you back the ASCII-ized form in the `ascii_email`
 field in the returned object, which you can get like this:
 
 ```python
-valid = validate_email(email, allow_smtputf8=False)
-email = valid.ascii_email
+emailinfo = validate_email(email, allow_smtputf8=False)
+email = emailinfo.ascii_email
 ```
 
 The local part is left alone (if it has internationalized characters
 `allow_smtputf8=False` will force validation to fail) and the domain
 part is converted to [IDNA ASCII](https://tools.ietf.org/html/rfc5891).
 (You probably should not do this at account creation time so you don't
 change the user's login information without telling them.)
 
 Normalization
 -------------
 
+### Unicode Normalization
+
 The use of Unicode in email addresses introduced a normalization
 problem. Different Unicode strings can look identical and have the same
-semantic meaning to the user. The `email` field returned on successful
+semantic meaning to the user. The `normalized` field returned on successful
 validation provides the correctly normalized form of the given email
-address:
+address.
+
+For example, the CJK fullwidth Latin letters are considered semantically
+equivalent in domain names to their ASCII counterparts. This library
+normalizes them to their ASCII counterparts:
 
 ```python
-valid = validate_email("me@Ｄｏｍａｉｎ.com")
-email = valid.ascii_email
-print(email)
-# prints: me@domain.com
+emailinfo = validate_email("me@Ｄｏｍａｉｎ.com")
+print(emailinfo.normalized)
+print(emailinfo.ascii_email)
+# prints "me@domain.com" twice
 ```
 
 Because an end-user might type their email address in different (but
 equivalent) un-normalized forms at different times, you ought to
 replace what they enter with the normalized form immediately prior to
 going into your database (during account creation), querying your database
 (during login), or sending outbound mail. Normalization may also change
@@ -306,87 +301,96 @@
 [UTS46](http://unicode.org/reports/tr46) mappings on the domain part,
 and conversion from Punycode to Unicode characters.
 
 (See [RFC 6532 (internationalized email) section
 3.1](https://tools.ietf.org/html/rfc6532#section-3.1) and [RFC 5895
 (IDNA 2008) section 2](http://www.ietf.org/rfc/rfc5895.txt).)
 
+### Other Normalization
+
+Normalization is also applied to quoted-string local parts and domain
+literal IPv6 addresses if you have allowed them by the `allow_quoted_local`
+and `allow_domain_literal` options. In quoted-string local parts, unnecessary
+backslash escaping is removed and even the surrounding quotes are removed if
+they are unnecessary. For IPv6 domain literals, the IPv6 address is
+normalized to condensed form. [RFC 2142](https://datatracker.ietf.org/doc/html/rfc2142)
+also requires lowercase normalization for some specific mailbox names like `postmaster@`.
+
 Examples
 --------
 
 For the email address `test@joshdata.me`, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='test@joshdata.me',
+  normalized='test@joshdata.me',
   local_part='test',
   domain='joshdata.me',
   ascii_email='test@joshdata.me',
   ascii_local_part='test',
   ascii_domain='joshdata.me',
   smtputf8=False)
 ```
 
 For the fictitious but valid address `example@ツ.ⓁⒾⒻⒺ`, which has an
 internationalized domain but ASCII local part, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='example@ツ.life',
+  normalized='example@ツ.life',
   local_part='example',
   domain='ツ.life',
   ascii_email='example@xn--bdk.life',
   ascii_local_part='example',
   ascii_domain='xn--bdk.life',
   smtputf8=False)
 
 ```
 
-Note that the `email` and `domain` fields provide a normalized form of the
+Note that `normalized` and other fields provide a normalized form of the
 email address, domain name, and (in other cases) local part (see earlier
 discussion of normalization), which you should use in your database.
 
 Calling `validate_email` with the ASCII form of the above email address,
 `example@xn--bdk.life`, returns the exact same information (i.e., the
-`email` field always will contain Unicode characters, not Punycode).
+`normalized` field always will contain Unicode characters, not Punycode).
 
 For the fictitious address `ツ-test@joshdata.me`, which has an
 internationalized local part, the returned object is:
 
 ```python
 ValidatedEmail(
-  email='ツ-test@joshdata.me',
+  normalized='ツ-test@joshdata.me',
   local_part='ツ-test',
   domain='joshdata.me',
   ascii_email=None,
   ascii_local_part=None,
   ascii_domain='joshdata.me',
   smtputf8=True)
 ```
 
 Now `smtputf8` is `True` and `ascii_email` is `None` because the local
-part of the address is internationalized. The `local_part` and `email` fields
-return the normalized form of the address: certain Unicode characters
-(such as angstrom and ohm) may be replaced by other equivalent code
-points (a-with-ring and omega).
+part of the address is internationalized. The `local_part` and `normalized` fields
+return the normalized form of the address.
 
 Return value
 ------------
 
 When an email address passes validation, the fields in the returned object
 are:
 
 | Field | Value |
 | -----:|-------|
-| `email` | The normalized form of the email address that you should put in your database. This merely combines the `local_part` and `domain` fields (see below). |
-| `ascii_email` | If set, an ASCII-only form of the email address by replacing the domain part with [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt). This field will be present when an ASCII-only form of the email address exists (including if the email address is already ASCII). If the local part of the email address contains internationalized characters, `ascii_email` will be `None`. If set, it merely combines `ascii_local_part` and `ascii_domain`. |
-| `local_part` | The local part of the given email address (before the @-sign) with Unicode NFC normalization applied. |
+| `normalized` | The normalized form of the email address that you should put in your database. This combines the `local_part` and `domain` fields (see below). |
+| `ascii_email` | If set, an ASCII-only form of the normalized email address by replacing the domain part with [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt). This field will be present when an ASCII-only form of the email address exists (including if the email address is already ASCII). If the local part of the email address contains internationalized characters, `ascii_email` will be `None`. If set, it merely combines `ascii_local_part` and `ascii_domain`. |
+| `local_part` | The normalized local part of the given email address (before the @-sign). Normalization includes Unicode NFC normalization and removing unnecessary quoted-string quotes and backslashes. If `allow_quoted_local` is True and the surrounding quotes are necessary, the quotes _will_ be present in this field. |
 | `ascii_local_part` | If set, the local part, which is composed of ASCII characters only. |
 | `domain` | The canonical internationalized Unicode form of the domain part of the email address. If the returned string contains non-ASCII characters, either the [SMTPUTF8](https://tools.ietf.org/html/rfc6531) feature of your mail relay will be required to transmit the message or else the email address's domain part must be converted to IDNA ASCII first: Use `ascii_domain` field instead. |
 | `ascii_domain` | The [IDNA](https://tools.ietf.org/html/rfc5891) [Punycode](https://www.rfc-editor.org/rfc/rfc3492.txt)-encoded form of the domain part of the given email address, as it would be transmitted on the wire. |
+| `domain_address` | If domain literals are allowed and if the email address contains one, an `ipaddress.IPv4Address` or `ipaddress.IPv6Address` object. |
 | `smtputf8` | A boolean indicating that the [SMTPUTF8](https://tools.ietf.org/html/rfc6531) feature of your mail relay will be required to transmit messages to this address because the local part of the address has non-ASCII characters (the local part cannot be IDNA-encoded). If `allow_smtputf8=False` is passed as an argument, this flag will always be false because an exception is raised if it would have been true. |
 | `mx` | A list of (priority, domain) tuples of MX records specified in the DNS for the domain (see [RFC 5321 section 5](https://tools.ietf.org/html/rfc5321#section-5)). May be `None` if the deliverability check could not be completed because of a temporary issue like a timeout. |
 | `mx_fallback_type` | `None` if an `MX` record is found. If no MX records are actually specified in DNS and instead are inferred, through an obsolete mechanism, from A or AAAA records, the value is the type of DNS record used instead (`A` or `AAAA`). May be `None` if the deliverability check could not be completed because of a temporary issue like a timeout. |
 | `spf` | Any SPF record found while checking deliverability. Only set if the SPF record is queried. |
 
 Assumptions
 -----------
@@ -400,21 +404,20 @@
   of the email address must be a resolvable domain name
   (see the deliverability checks described above).
   Most [Special Use Domain Names](https://www.iana.org/assignments/special-use-domain-names/special-use-domain-names.xhtml)
   and their subdomains, as well as
   domain names without a `.`, are rejected as a syntax error
   (except see the `test_environment` parameter above).
 * Obsolete email syntaxes are rejected:
-  The "quoted string" form of the local part of the email address (RFC
-  5321 4.1.2) is not permitted.
-  Quoted forms allow multiple @-signs, space characters, and other
-  troublesome conditions. The unusual [(comment) syntax](https://github.com/JoshData/python-email-validator/issues/77)
-  is also rejected. The "literal" form for the domain part of an email address (an
-  IP address in brackets) is rejected. Other obsolete and deprecated syntaxes are
-  rejected. No one uses these forms anymore.
+  The unusual ["(comment)" syntax](https://github.com/JoshData/python-email-validator/issues/77)
+  is rejected. Extremely old obsolete syntaxes are
+  rejected. Quoted-string local parts and domain-literal addresses
+  are rejected by default, but there are options to allow them (see above).
+  No one uses these forms anymore, and I can't think of any reason why anyone
+  using this library would need to accept them.
 
 
 Testing
 -------
 
 Tests can be run using
 
@@ -430,20 +433,17 @@
 
 The package is distributed as a universal wheel and as a source package.
 
 To release:
 
 * Update CHANGELOG.md.
 * Update the version number in setup.cfg.
-* Make & push a commit with the new version number.
-* Make & push a tag (`git tag v... && git push --tags`).
+* Make & push a commit with the new version number and make sure tests pass.
+* Make & push a tag (see command below).
 * Make a release at https://github.com/JoshData/python-email-validator/releases/new.
-* Follow the steps below to publish source and a universal wheel to pypi.
+* Publish a source and wheel distribution to pypi (see command below).
 
 ```sh
-./release_to_pypi.sh
 git tag v$(grep version setup.cfg | sed "s/.*= //")
 git push --tags
+./release_to_pypi.sh
 ```
-
-Notes: The wheel is specified as universal in the file `setup.cfg` by the `universal = 1` key in the
-`[bdist_wheel]` section.
```

### Comparing `email_validator-2.0.0.dev4/setup.cfg` & `email_validator-2.0.0.post1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = email_validator
-version = 2.0.0-dev4
+version = 2.0.0.post1
 description = A robust email address syntax and deliverability validation library.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JoshData/python-email-validator
 author = Joshua Tauberer
 author_email = jt@occams.info
 license = CC0 (copyright waived)
@@ -30,18 +30,15 @@
 python_requires = >=3.7
 
 [options.package_data]
 * = py.typed
 
 [options.entry_points]
 console_scripts = 
-	email_validator=email_validator:main
-
-[bdist_wheel]
-universal = 1
+	email_validator=email_validator.__main__:main
 
 [flake8]
 max-line-length = 120
 
 [tool:pytest]
 testpaths = tests
 filterwarnings =
```


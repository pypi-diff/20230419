# Comparing `tmp/mail_devel-0.1.0-py3-none-any.whl.zip` & `tmp/mail_devel-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,19 @@
-Zip file size: 17509 bytes, number of entries: 19
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-17 17:53 mail_devel/__init__.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Feb-24 15:00 mail_devel/__main__.py
--rw-r--r--  2.0 unx     7875 b- defN 23-Feb-23 18:22 mail_devel/http.py
--rw-r--r--  2.0 unx      410 b- defN 23-Feb-18 12:03 mail_devel/mailbox.py
--rw-r--r--  2.0 unx     1929 b- defN 23-Feb-23 18:28 mail_devel/smtp.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Feb-20 16:43 mail_devel/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-18 17:37 mail_devel/resources/__init__.py
--rw-r--r--  2.0 unx     2356 b- defN 23-Feb-20 15:27 mail_devel/resources/index.html
--rw-r--r--  2.0 unx     2681 b- defN 23-Feb-20 15:27 mail_devel/resources/main.css
--rw-r--r--  2.0 unx     6395 b- defN 23-Feb-20 16:10 mail_devel/resources/main.js
--rw-r--r--  2.0 unx     2356 b- defN 23-Feb-20 15:27 mail_devel-0.1.0.data/data/index.html
--rw-r--r--  2.0 unx     2681 b- defN 23-Feb-20 15:27 mail_devel-0.1.0.data/data/main.css
--rw-r--r--  2.0 unx     6395 b- defN 23-Feb-20 16:10 mail_devel-0.1.0.data/data/main.js
--rw-r--r--  2.0 unx     1085 b- defN 23-Feb-24 15:04 mail_devel-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1477 b- defN 23-Feb-24 15:04 mail_devel-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 15:04 mail_devel-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-Feb-24 15:04 mail_devel-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-24 15:04 mail_devel-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1579 b- defN 23-Feb-24 15:04 mail_devel-0.1.0.dist-info/RECORD
-19 files, 47767 bytes uncompressed, 14917 bytes compressed:  68.8%
+Zip file size: 14520 bytes, number of entries: 17
+-rw-r--r--  2.0 unx       48 b- defN 23-Apr-19 09:55 mail_devel/__init__.py
+-rw-r--r--  2.0 unx     1251 b- defN 23-Apr-19 09:55 mail_devel/__main__.py
+-rw-r--r--  2.0 unx     8195 b- defN 23-Apr-19 09:55 mail_devel/http.py
+-rw-r--r--  2.0 unx      410 b- defN 23-Apr-19 09:55 mail_devel/mailbox.py
+-rw-r--r--  2.0 unx     8249 b- defN 23-Apr-19 09:55 mail_devel/service.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Apr-19 09:55 mail_devel/smtp.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-Apr-19 09:55 mail_devel/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 09:55 mail_devel/resources/__init__.py
+-rw-r--r--  2.0 unx     2356 b- defN 23-Apr-19 09:55 mail_devel/resources/index.html
+-rw-r--r--  2.0 unx     2681 b- defN 23-Apr-19 09:55 mail_devel/resources/main.css
+-rw-r--r--  2.0 unx     6395 b- defN 23-Apr-19 09:55 mail_devel/resources/main.js
+-rw-r--r--  2.0 unx     1085 b- defN 23-Apr-19 09:56 mail_devel-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1454 b- defN 23-Apr-19 09:56 mail_devel-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 09:56 mail_devel-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Apr-19 09:56 mail_devel-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-19 09:56 mail_devel-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Apr-19 09:56 mail_devel-0.2.0.dist-info/RECORD
+17 files, 38301 bytes uncompressed, 12250 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: mail_devel/http.py
 Comment: 
 
 Filename: mail_devel/mailbox.py
 Comment: 
 
+Filename: mail_devel/service.py
+Comment: 
+
 Filename: mail_devel/smtp.py
 Comment: 
 
 Filename: mail_devel/utils.py
 Comment: 
 
 Filename: mail_devel/resources/__init__.py
@@ -24,35 +27,26 @@
 
 Filename: mail_devel/resources/main.css
 Comment: 
 
 Filename: mail_devel/resources/main.js
 Comment: 
 
-Filename: mail_devel-0.1.0.data/data/index.html
-Comment: 
-
-Filename: mail_devel-0.1.0.data/data/main.css
-Comment: 
-
-Filename: mail_devel-0.1.0.data/data/main.js
-Comment: 
-
-Filename: mail_devel-0.1.0.dist-info/LICENSE
+Filename: mail_devel-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: mail_devel-0.1.0.dist-info/METADATA
+Filename: mail_devel-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: mail_devel-0.1.0.dist-info/WHEEL
+Filename: mail_devel-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: mail_devel-0.1.0.dist-info/entry_points.txt
+Filename: mail_devel-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mail_devel-0.1.0.dist-info/top_level.txt
+Filename: mail_devel-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mail_devel-0.1.0.dist-info/RECORD
+Filename: mail_devel-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mail_devel/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 6672 6f6d 202e 7365 7276 6963 6520 696d  from .service im
+00000010: 706f 7274 2053 6572 7669 6365 0a0a 5645  port Service..VE
+00000020: 5253 494f 4e20 3d20 2230 2e32 2e30 220a  RSION = "0.2.0".
```

## mail_devel/__main__.py

```diff
@@ -1,273 +1,52 @@
-import argparse
 import asyncio
 import logging
-import os
 import signal
 from argparse import Namespace
-from contextlib import AsyncExitStack, suppress
+from contextlib import suppress
 
-from aiosmtpd.controller import Controller
-from pymap.backend.dict import DictBackend, FilterSet
-from pymap.imap import IMAPService
 from pymap.parsing.specials.searchkey import SearchKey
 
 from . import utils
-from .http import Frontend
-from .mailbox import TestMailboxSet
-from .smtp import Authenticator, MemoryHandler
+from .service import Service
 
 _logger = logging.getLogger(__name__)
 
 
 # Manual patch for https://github.com/icgood/pymap/pull/138
 original_func = SearchKey.__init__
 
 
 def patched_searchkey(self, key, filter_=None, inverse=False):
     if isinstance(filter_, list):
-        filter_ = frozenset(filter_)
+        filter_ = tuple(filter_)
     return original_func(self, key, filter_, inverse)
 
 
 SearchKey.__init__ = patched_searchkey
 
 
 async def sleep_forever() -> None:
     with suppress(asyncio.CancelledError):
         while True:
             await asyncio.sleep(60)
 
 
-async def imap_context(args: Namespace) -> Namespace:
-    return Namespace(
-        demo_data=False,
-        demo_user=args.user,
-        demo_password=args.password,
-        host=args.imap_host or args.host,
-        port=args.imap_port,
-        debug=args.debug,
-        cert=args.cert,
-        key=args.key,
-        tls=False,
-        proxy_protocol=None,
-        inherited_sockets=None,
-    )
-
-
-def log_connection_info(args: Namespace) -> None:
-    tls = bool(args.cert and args.key)
-    if args.http:
-        _logger.info(f"HTTP service [{args.http_port}]")
-
-    _logger.info(f"IMAP service [{args.imap_port}]")
-    if tls:
-        _logger.info(f"IMAP/STARTTLS service [{args.imap_port}]")
-
-    if not args.starttls_required:
-        _logger.info(f"SMTP service [{args.smtp_port}]")
-    if tls:
-        _logger.info(f"SMTP/STARTTLS service [{args.smtp_port}]")
-        _logger.info(f"SMTPS service [{args.smtps_port}]")
-
-
 async def run(args: Namespace) -> None:
-    loop = asyncio.get_running_loop()
-
-    if args.cert and args.key:
-        ssl_context = utils.generate_ssl_context(cert=args.cert, key=args.key)
-    else:
-        ssl_context = None
-
-    # Create the mailbox
-    mailbox_set = TestMailboxSet()
-    filter_set = FilterSet()
-    inbox = await mailbox_set.get_mailbox("INBOX")
-
-    # Create the IMAP and optionally IMAPS service
-    backend_args = await imap_context(args)
-    backend, config = await DictBackend.init(backend_args)
-    config.set_cache[args.user] = mailbox_set, filter_set
-    imap = IMAPService(backend, config)
-
-    # Create the SMTP and optionally SMTPS service
-    handler = MemoryHandler(inbox, args.flagged_seen)
-    smtp = Controller(
-        handler,
-        hostname=args.smtp_host or args.host,
-        port=args.smtp_port,
-        tls_context=ssl_context,
-        auth_required=args.auth_required,
-        auth_require_tls=args.auth_require_tls,
-        require_starttls=args.starttls_required,
-        authenticator=Authenticator(args.user, args.password),
-    )
-
-    if ssl_context:
-        smtps = Controller(
-            handler,
-            hostname=args.smtp_host or args.host,
-            port=args.smtps_port,
-            ssl_context=ssl_context,
-            auth_required=args.auth_required,
-            auth_require_tls=args.auth_require_tls,
-            authenticator=Authenticator(args.user, args.password),
-        )
-    else:
-        smtps = None
-
-    # Create the HTTP service
-    if args.http:
-        frontend = Frontend(
-            mailbox_set,
-            host=args.http_host or args.host,
-            port=args.http_port,
-            devel=args.devel,
-        )
-    else:
-        frontend = None
-
-    # Start the services
-    async with AsyncExitStack() as stack:
-        await backend.start(stack)
-        await imap.start(stack)
-
-        smtp.start()
-        if smtps:
-            smtps.start()
-
-        if frontend:
-            asyncio.create_task(frontend.start())
-
-        log_connection_info(args)
-
+    loop = asyncio.get_event_loop()
+    service = await Service.init(args)
+    async with service.start():
         forever = asyncio.create_task(sleep_forever())
         loop.add_signal_handler(signal.SIGINT, forever.cancel)
         loop.add_signal_handler(signal.SIGTERM, forever.cancel)
         await forever
 
 
 def main() -> None:
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--host",
-        default=os.environ.get("MAIL_HOST", ""),
-        help="The IP to bind the listening server ports. Default is %(default)s",
-    )
-    parser.add_argument(
-        "--user",
-        default=os.environ.get("MAIL_USER", "test@example.org"),
-        help="The user account for SMTP and IMAP. Default is %(default)s",
-    )
-    pw = parser.add_argument(
-        "--password",
-        default=os.environ.get("MAIL_PASSWORD"),
-        help="The password for SMTP and IMAP",
-    )
-
-    group = parser.add_argument_group("IMAP")
-    parser.add_argument(
-        "--imap-host",
-        default=False,
-        help="Overrules the IP binding specifically for IMAP",
-    )
-    group.add_argument(
-        "--imap-port",
-        metavar="PORT",
-        default=4143,
-        help="The port of the IMAP interface. Default is %(default)s",
-    )
-
-    group = parser.add_argument_group("HTTP")
-    parser.add_argument(
-        "--http-host",
-        default=False,
-        help="Overrules the IP binding specifically for HTTP",
-    )
-    group.add_argument(
-        "--http-port",
-        metavar="PORT",
-        default=4080,
-        help="The port of the HTTP interface. Default is %(default)s",
-    )
-    group.add_argument(
-        "--no-http",
-        dest="http",
-        action="store_false",
-        help="Disable the HTTP server",
-    )
-
-    group = parser.add_argument_group("SMTP")
-    parser.add_argument(
-        "--smtp-host",
-        default=False,
-        help="Overrules the IP binding specifically for smtp",
-    )
-    group.add_argument(
-        "--smtp-port",
-        metavar="PORT",
-        default=4025,
-        help="The port of the SMTP interface. Default is %(default)s",
-    )
-    group.add_argument(
-        "--smtps-port",
-        metavar="PORT",
-        default=4465,
-        help="The port of the SMTPS interface. Requires --cert and --key. "
-        "Default is %(default)s",
-    )
-    group.add_argument(
-        "--auth-required",
-        action="store_true",
-        help="Required SMTP AUTH",
-    )
-    group.add_argument(
-        "--auth-require-tls",
-        action="store_true",
-        help="Require TLS for SMTP AUTH",
-    )
-    group.add_argument(
-        "--starttls-required",
-        action="store_true",
-        help="Require STARTTLS",
-    )
-    group.add_argument(
-        "--flagged-seen",
-        action="store_true",
-        help="Flag messages in the INBOX as seen if they arrive via SMTP",
-    )
-
-    group = parser.add_argument_group("Options")
-    group.add_argument("--debug", action="store_true", help="Verbose logging")
-    group.add_argument(
-        "--devel",
-        action="store_true",
-        help="Use files from the working directory instead of the resources for "
-        "the HTTP frontend. Useful for own frontends or development",
-    )
-
-    group = parser.add_argument_group("Security")
-    group.add_argument(
-        "--cert",
-        default=None,
-        metavar="FILE",
-        type=utils.valid_file,
-        help="TLS certificate file",
-    )
-    group.add_argument(
-        "--key",
-        default=None,
-        metavar="FILE",
-        type=utils.valid_file,
-        help="TLS key file",
-    )
-    args = parser.parse_args()
-
-    if not args.password:
-        raise argparse.ArgumentError(pw, "Missing argument `password`")
+    args = Service.parse()
 
     utils.configure_logging(level="DEBUG" if args.debug else "INFO")
     asyncio.run(run(args))
 
 
 if __name__ == "__main__":
     main()
```

## mail_devel/http.py

```diff
@@ -58,20 +58,21 @@
                 web.get(r"/api", self._api_index),
                 web.get(r"/api/{mailbox}", self._api_mailbox),
                 web.get(r"/api/{mailbox}/{uid:\d+}", self._api_message),
                 web.get(
                     r"/api/{mailbox}/{uid:\d+}/attachment/{attachment}",
                     self._api_attachment,
                 ),
+                web.get(r"/api/{mailbox}/{uid:\d+}/flags", self._api_flag),
                 web.put(r"/api/{mailbox}/{uid:\d+}/flags/{flag}", self._api_flag),
                 web.delete(r"/api/{mailbox}/{uid:\d+}/flags/{flag}", self._api_flag),
             ]
         )
 
-        await web._run_app(
+        return await web._run_app(
             self.api,
             host=self.host,
             port=self.port,
             access_log_format='%a "%r" %s %b "%{Referer}i" "%{User-Agent}i"',
             reuse_address=True,
             reuse_port=True,
             print=None,
@@ -80,28 +81,30 @@
     async def _page_index(self, request: Request) -> Response:  # pylint: disable=W0613
         try:
             return Response(
                 body=self.load_resource("index.html"),
                 content_type="text/html",
             )
         except FileNotFoundError as e:
+            _logger.error("File 'index.html' not in resources")
             raise web.HTTPNotFound() from e
 
     async def _page_static(self, request: Request) -> Response:
         static = request.match_info["static"]
         if static.endswith(".js"):
             mimetype = "text/javascript"
         elif static.endswith(".css"):
             mimetype = "text/css"
         else:
             raise web.HTTPNotFound()
 
         try:
             return Response(body=self.load_resource(static), content_type=mimetype)
         except FileNotFoundError as e:
+            _logger.error(f"File {static!r} not in resources")
             raise web.HTTPNotFound() from e
 
     async def _convert_message(self, msg: Message, full: bool = False) -> dict:
         content = bytes((await msg.load_content([])).content)
 
         message = message_from_bytes(content)
         result = {
@@ -197,28 +200,30 @@
                 )
 
         raise web.HTTPNotFound()
 
     async def _api_flag(self, request: Request) -> Response:
         try:
             name = request.match_info["mailbox"]
-            uid = int(request.match_info["uid"])
-            flag = request.match_info["flag"].title()
             mailbox = await self.mailbox_set.get_mailbox(name)
+            uid = int(request.match_info["uid"])
+
+            if request.method in ("DELETE", "PUT"):
+                flag = request.match_info["flag"].title()
+                flag = Flag(b"\\" + flag.encode())
+            else:
+                flag = None
         except (IndexError, KeyError) as e:
             raise web.HTTPNotFound() from e
 
-        remove = request.method == "DELETE"
-
-        flag = Flag(b"\\" + flag.encode())
         async for msg in mailbox.messages():
             if msg.uid != uid:
                 continue
 
-            if remove:
+            if request.method == "DELETE":
                 msg.permanent_flags = msg.permanent_flags.difference([flag])
-            else:
+            elif request.method == "PUT":
                 msg.permanent_flags = msg.permanent_flags.union([flag])
 
             return web.json_response(flags_to_api(msg.permanent_flags))
 
         raise web.HTTPNotFound()
```

## Comparing `mail_devel-0.1.0.dist-info/LICENSE` & `mail_devel-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mail_devel-0.1.0.dist-info/METADATA` & `mail_devel-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: mail-devel
-Version: 0.1.0
+Version: 0.2.0
 Summary: IMAP and SMTP in memory test server
 Home-page: https://github.com/fkantelberg/mail-devel
 Author: Florian Kantelberg
 Author-email: florian.kantelberg@mailbox.org
 License: MIT
 Keywords: imap smtp development
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp
 Requires-Dist: aiohttp-jinja2
 Requires-Dist: aiosmtpd
 Requires-Dist: pymap
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mail-devel)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

## Comparing `mail_devel-0.1.0.dist-info/RECORD` & `mail_devel-0.2.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-mail_devel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mail_devel/__main__.py,sha256=5O13OI1mqISPh06CZGFvvvQi9EbrpMKEogXIMtXmodg,7681
-mail_devel/http.py,sha256=UGh9V2QgSq9QEKSjhU94dH1-v6yRX1Ed0uLFFCXz-ck,7875
+mail_devel/__init__.py,sha256=bJUeFKTUbMmplQNEaAIH--FKEVIDXiv6ZWMtSk1Clw4,48
+mail_devel/__main__.py,sha256=xLaUehNg3Fk2m7tGUfiAPbZv1mxCGOqFyRIDOnSO-6c,1251
+mail_devel/http.py,sha256=sjEviniFcQu2S7OwEDM22wnywy2jaorDaMS911R93jM,8195
 mail_devel/mailbox.py,sha256=CFzG8nQLbEgKWrFblwxg9-dDSvWfkuogkD-Aua33bD0,410
+mail_devel/service.py,sha256=dSm0_PcEuoctSxc86CSGnqiX9Ax8ajHsBqqkUhE0OZM,8249
 mail_devel/smtp.py,sha256=DArwHAH9JSF7r5tWeHg5d2WyO8YOzmrONFraXllrPeo,1929
 mail_devel/utils.py,sha256=DI8LJPoRxhWgZkhysMGLYhAI4cwDr4YgRR6xpkJM5KA,2708
 mail_devel/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mail_devel/resources/index.html,sha256=1U1prOQKz8VlKcNrIK_kb-b4T9QyHlPGkOm1TYx8QQk,2356
 mail_devel/resources/main.css,sha256=MDjCkNKGp_mmn4MKvdN1l0Z_wotHIRYDJE4wmSmS90s,2681
 mail_devel/resources/main.js,sha256=3HG3ci7ZQmcsWut_6KQEN-_pEfCERnFsYKja8gGY26g,6395
-mail_devel-0.1.0.data/data/index.html,sha256=1U1prOQKz8VlKcNrIK_kb-b4T9QyHlPGkOm1TYx8QQk,2356
-mail_devel-0.1.0.data/data/main.css,sha256=MDjCkNKGp_mmn4MKvdN1l0Z_wotHIRYDJE4wmSmS90s,2681
-mail_devel-0.1.0.data/data/main.js,sha256=3HG3ci7ZQmcsWut_6KQEN-_pEfCERnFsYKja8gGY26g,6395
-mail_devel-0.1.0.dist-info/LICENSE,sha256=2uv3FXpGSeGfn8IfQfoIC6H2ERGw0jizs1HaWgYDMP4,1085
-mail_devel-0.1.0.dist-info/METADATA,sha256=OHAx14VkwL_4DM8dzldJgVCv6fG_m41uf1tj37FNJvU,1477
-mail_devel-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mail_devel-0.1.0.dist-info/entry_points.txt,sha256=msOFnZ8G-RwKfWNoenhoUXRX9UOkFNf-KVNSL2IQseg,56
-mail_devel-0.1.0.dist-info/top_level.txt,sha256=Q649zJRj-7u22745fgJO6Otc4d8q03ZINA6GR61x-KM,11
-mail_devel-0.1.0.dist-info/RECORD,,
+mail_devel-0.2.0.dist-info/LICENSE,sha256=2uv3FXpGSeGfn8IfQfoIC6H2ERGw0jizs1HaWgYDMP4,1085
+mail_devel-0.2.0.dist-info/METADATA,sha256=Zv2NK7KZH5X8EzU_awvm61umSGGRJuxbTZ5x9sO1Two,1454
+mail_devel-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mail_devel-0.2.0.dist-info/entry_points.txt,sha256=msOFnZ8G-RwKfWNoenhoUXRX9UOkFNf-KVNSL2IQseg,56
+mail_devel-0.2.0.dist-info/top_level.txt,sha256=Q649zJRj-7u22745fgJO6Otc4d8q03ZINA6GR61x-KM,11
+mail_devel-0.2.0.dist-info/RECORD,,
```


# Comparing `tmp/pscrape-0.0.2.tar.gz` & `tmp/pscrape-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pscrape-0.0.2.tar", last modified: Fri Feb 24 09:37:01 2023, max compression
+gzip compressed data, was "pscrape-0.0.3.tar", last modified: Wed Apr 19 15:04:41 2023, max compression
```

## Comparing `pscrape-0.0.2.tar` & `pscrape-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-02-24 09:37:01.632119 pscrape-0.0.2/
--rw-r--r--   0 lbirch     (501) staff       (20)     1074 2023-02-24 09:22:28.000000 pscrape-0.0.2/LICENSE.txt
--rw-r--r--   0 lbirch     (501) staff       (20)     2279 2023-02-24 09:37:01.632205 pscrape-0.0.2/PKG-INFO
--rw-r--r--   0 lbirch     (501) staff       (20)     1911 2023-02-24 09:22:28.000000 pscrape-0.0.2/README.md
-drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-02-24 09:37:01.631295 pscrape-0.0.2/pscrape/
--rw-r--r--   0 lbirch     (501) staff       (20)       28 2023-02-24 09:22:28.000000 pscrape-0.0.2/pscrape/__init__.py
--rw-r--r--   0 lbirch     (501) staff       (20)     4638 2023-02-24 09:22:28.000000 pscrape-0.0.2/pscrape/scraper.py
-drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-02-24 09:37:01.632018 pscrape-0.0.2/pscrape.egg-info/
--rw-r--r--   0 lbirch     (501) staff       (20)     2279 2023-02-24 09:37:01.000000 pscrape-0.0.2/pscrape.egg-info/PKG-INFO
--rw-r--r--   0 lbirch     (501) staff       (20)      282 2023-02-24 09:37:01.000000 pscrape-0.0.2/pscrape.egg-info/SOURCES.txt
--rw-r--r--   0 lbirch     (501) staff       (20)        1 2023-02-24 09:37:01.000000 pscrape-0.0.2/pscrape.egg-info/dependency_links.txt
--rw-r--r--   0 lbirch     (501) staff       (20)       49 2023-02-24 09:37:01.000000 pscrape-0.0.2/pscrape.egg-info/entry_points.txt
--rw-r--r--   0 lbirch     (501) staff       (20)       24 2023-02-24 09:37:01.000000 pscrape-0.0.2/pscrape.egg-info/requires.txt
--rw-r--r--   0 lbirch     (501) staff       (20)        8 2023-02-24 09:37:01.000000 pscrape-0.0.2/pscrape.egg-info/top_level.txt
--rw-r--r--   0 lbirch     (501) staff       (20)       93 2023-02-24 09:22:28.000000 pscrape-0.0.2/pyproject.toml
--rw-r--r--   0 lbirch     (501) staff       (20)      556 2023-02-24 09:37:01.632457 pscrape-0.0.2/setup.cfg
--rw-r--r--   0 lbirch     (501) staff       (20)       68 2023-02-24 09:22:28.000000 pscrape-0.0.2/setup.py
+drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-04-19 15:04:41.238213 pscrape-0.0.3/
+-rw-r--r--   0 lbirch     (501) staff       (20)     1074 2023-04-19 14:55:53.000000 pscrape-0.0.3/LICENSE.txt
+-rw-r--r--   0 lbirch     (501) staff       (20)     2284 2023-04-19 15:04:41.238296 pscrape-0.0.3/PKG-INFO
+-rw-r--r--   0 lbirch     (501) staff       (20)     1917 2023-04-19 15:02:39.000000 pscrape-0.0.3/README.md
+drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-04-19 15:04:41.237329 pscrape-0.0.3/pscrape/
+-rw-r--r--   0 lbirch     (501) staff       (20)       28 2023-04-19 15:03:04.000000 pscrape-0.0.3/pscrape/__init__.py
+-rw-r--r--   0 lbirch     (501) staff       (20)     4150 2023-04-19 15:00:15.000000 pscrape-0.0.3/pscrape/scraper.py
+drwxr-xr-x   0 lbirch     (501) staff       (20)        0 2023-04-19 15:04:41.238095 pscrape-0.0.3/pscrape.egg-info/
+-rw-r--r--   0 lbirch     (501) staff       (20)     2284 2023-04-19 15:04:41.000000 pscrape-0.0.3/pscrape.egg-info/PKG-INFO
+-rw-r--r--   0 lbirch     (501) staff       (20)      282 2023-04-19 15:04:41.000000 pscrape-0.0.3/pscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 lbirch     (501) staff       (20)        1 2023-04-19 15:04:41.000000 pscrape-0.0.3/pscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 lbirch     (501) staff       (20)       49 2023-04-19 15:04:41.000000 pscrape-0.0.3/pscrape.egg-info/entry_points.txt
+-rw-r--r--   0 lbirch     (501) staff       (20)       24 2023-04-19 15:04:41.000000 pscrape-0.0.3/pscrape.egg-info/requires.txt
+-rw-r--r--   0 lbirch     (501) staff       (20)        8 2023-04-19 15:04:41.000000 pscrape-0.0.3/pscrape.egg-info/top_level.txt
+-rw-r--r--   0 lbirch     (501) staff       (20)       93 2023-04-19 14:55:53.000000 pscrape-0.0.3/pyproject.toml
+-rw-r--r--   0 lbirch     (501) staff       (20)      556 2023-04-19 15:04:41.238538 pscrape-0.0.3/setup.cfg
+-rw-r--r--   0 lbirch     (501) staff       (20)       68 2023-04-19 14:55:53.000000 pscrape-0.0.3/setup.py
```

### Comparing `pscrape-0.0.2/LICENSE.txt` & `pscrape-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pscrape-0.0.2/PKG-INFO` & `pscrape-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pscrape
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quickly generate a list of free and working proxies
 Home-page: https://github.com/lbirchler/pscrape
 Author: lbirchler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,16 +15,16 @@
 quickly generate a list of free and working proxies
 
 ---
 
 
 ## Installation
 
-```bash
-pip install pscrape 
+```
+python3 -m pip install pscrape 
 ```
 
 ---
 
 ## Usage
 
 ```
@@ -41,15 +41,15 @@
     anonymous, elite, or transparent.
 - **https** (bool, optional): Https only. Defaults to False.
 - **debug** (bool, optional): Display scraped and validated proxies. Defaults to False.
 
 
 ### CLI
 ```
-usage: pscraper [-h] [-c COUNTRY] [-a {anonymous,elite,transparent}] [--https]
+usage: pscrape [-h] [-c COUNTRY] [-a {anonymous,elite,transparent}] [--https]
                     [-o OUTPUT_FILE]
 
 optional arguments:
 -h, --help            show this help message and exit
 -c COUNTRY, --country COUNTRY
                     Country ISO Code
 -a {anonymous,elite,transparent}, --anon {anonymous,elite,transparent}
@@ -58,15 +58,15 @@
 -o OUTPUT_FILE, --output_file OUTPUT_FILE
                     Save list of proxies to file.
 ```
 
 Example:
 
 ```
-$ pscraper -c US --https -o /tmp/proxies.txt
+$ pscrape -c US --https -o /tmp/proxies.txt
 ```
 
 ```
 + Total scraped proxies:  12
 > 20.241.236.196:3128    | US  | anonymous    | https
 > 204.2.218.145:8080     | US  | elite proxy  | https
 > 104.223.135.178:10000  | US  | elite proxy  | https
```

### Comparing `pscrape-0.0.2/README.md` & `pscrape-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 quickly generate a list of free and working proxies
 
 ---
 
 
 ## Installation
 
-```bash
-pip install pscrape 
+```
+python3 -m pip install pscrape 
 ```
 
 ---
 
 ## Usage
 
 ```
@@ -29,15 +29,15 @@
     anonymous, elite, or transparent.
 - **https** (bool, optional): Https only. Defaults to False.
 - **debug** (bool, optional): Display scraped and validated proxies. Defaults to False.
 
 
 ### CLI
 ```
-usage: pscraper [-h] [-c COUNTRY] [-a {anonymous,elite,transparent}] [--https]
+usage: pscrape [-h] [-c COUNTRY] [-a {anonymous,elite,transparent}] [--https]
                     [-o OUTPUT_FILE]
 
 optional arguments:
 -h, --help            show this help message and exit
 -c COUNTRY, --country COUNTRY
                     Country ISO Code
 -a {anonymous,elite,transparent}, --anon {anonymous,elite,transparent}
@@ -46,15 +46,15 @@
 -o OUTPUT_FILE, --output_file OUTPUT_FILE
                     Save list of proxies to file.
 ```
 
 Example:
 
 ```
-$ pscraper -c US --https -o /tmp/proxies.txt
+$ pscrape -c US --https -o /tmp/proxies.txt
 ```
 
 ```
 + Total scraped proxies:  12
 > 20.241.236.196:3128    | US  | anonymous    | https
 > 204.2.218.145:8080     | US  | elite proxy  | https
 > 104.223.135.178:10000  | US  | elite proxy  | https
@@ -72,8 +72,8 @@
 ```
 20.241.236.196:3128
 204.2.218.145:8080
 104.223.135.178:10000
 5.78.50.231:8888
 4.16.68.158:443
 104.148.86.58:3129
-```
+```
```

### Comparing `pscrape-0.0.2/pscrape/scraper.py` & `pscrape-0.0.3/pscrape/scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,137 +22,139 @@
         'https',  # yes, no
         'last_checked',
     ],
 )
 
 
 class Proxies:
-    """Scrape and validate proxies from free-proxy-list.net.
+  """Scrape and validate proxies from free-proxy-list.net.
 
-    Args:
-        country (None | str, optional): Country ISO Code. Defaults to None.
-        anon (None | str, optional): Anonymity level. Defaults to None.
-            anonymous, elite, or transparent.
-        https (bool, optional): Https only. Defaults to False.
-        debug (bool, optional): Display scraped and validated proxies. Defaults to False.
-
-    """
-
-    def __init__(
-            self,
-            country: None | str = None,
-            anon: None | str = None,
-            https: bool = False,
-            debug: bool = False,
-    ):
-        self.country = country
-        self.anon = anon
-        self.https = https
-        self.debug = debug
-
-    def _fetch(self):
-        r = requests.get('https://free-proxy-list.net')
-        if r.status_code != 200:
-            print('Error scraping proxies: %d - %s' % r.status_code, r.reason)
-            return
-        soup = bs4.BeautifulSoup(r.content, 'html.parser')
-        body = soup.find('tbody')
-        rows = body.find_all('tr')
-        proxies = []
-        for row in rows:
-            proxy = Proxy(*[x.text.strip() for x in row.find_all('td')])
-            if (
-                (self.country and proxy.code != self.country) or
-                (self.anon and self.anon not in proxy.anonymity) or
-                (self.https and proxy.https == 'no')
-            ):
-                continue
-            proxies.append(proxy)
-        if self.debug:
-            print('+ Total scraped proxies:  %d' % len(proxies))
-        return proxies
-
-    @staticmethod
-    def _check_one(proxy: Proxy):
-        ip_port = f'{proxy.ip_address}:{proxy.port}'
-        r = requests.get(
-            'https://httpbin.org/ip',
-            proxies={'http': ip_port, 'https': ip_port},
-            timeout=2,
-        )
-        return (proxy, r.status_code)
-
-    def _check_all(self, proxies: list[str]):
-        working = []
-        with ThreadPoolExecutor() as executor:
-            futures = [
-                executor.submit(self._check_one, proxy)
-                for proxy in proxies
-            ]
-            for future in as_completed(futures):
-                try:
-                    proxy, status_code = future.result()
-                    if status_code == 200:
-                        if self.debug:
-                            type = 'https' if proxy.https == 'yes' else 'http'
-                            addr = f'{proxy.ip_address}:{proxy.port}'
-                            print(
-                                '> %-22s | %-3s | %-12s | %s' %
-                                (addr, proxy.code, proxy.anonymity, type),
-                            )
-                        working.append(f'{proxy.ip_address}:{proxy.port}')
-                except BaseException:
-                    continue
-        if self.debug:
-            print('+ Total validated proxies: %d' % len(working))
-        return working
-
-    def scrape(self):
-        proxies = self._fetch()
-        working = self._check_all(proxies)
-        return working
+  Args:
+      country (None | str, optional): Country ISO Code. Defaults to None.
+      anon (None | str, optional): Anonymity level. Defaults to None.
+          anonymous, elite, or transparent.
+      https (bool, optional): Https only. Defaults to False.
+      debug (bool, optional): Display scraped and validated proxies. Defaults to False.
+
+  """
+
+  def __init__(
+          self,
+          country: None | str = None,
+          anon: None | str = None,
+          https: bool = False,
+          debug: bool = False,
+  ):
+    self.country = country
+    self.anon = anon
+    self.https = https
+    self.debug = debug
+
+  def _fetch(self):
+    r = requests.get('https://free-proxy-list.net')
+    if r.status_code != 200:
+      print('Error scraping proxies: %d - %s' % r.status_code, r.reason)
+      return
+    soup = bs4.BeautifulSoup(r.content, 'html.parser')
+    body = soup.find('tbody')
+    rows = body.find_all('tr')
+    proxies = []
+    for row in rows:
+      proxy = Proxy(*[x.text.strip() for x in row.find_all('td')])
+      if (
+          self.country and proxy.code != self.country
+      ) or (
+          self.anon and self.anon not in proxy.anonymity
+      ) or (
+          self.https and proxy.https == 'no'
+      ):
+        continue
+      proxies.append(proxy)
+    if self.debug:
+      print('+ Total scraped proxies:  %d' % len(proxies))
+    return proxies
+
+  @staticmethod
+  def _check_one(proxy: Proxy):
+    ip_port = f'{proxy.ip_address}:{proxy.port}'
+    r = requests.get(
+        'https://httpbin.org/ip',
+        proxies={'http': ip_port, 'https': ip_port},
+        timeout=2,
+    )
+    return (proxy, r.status_code)
 
+  def _check_all(self, proxies: list[str]):
+    working = []
+    with ThreadPoolExecutor() as executor:
+      futures = [
+          executor.submit(self._check_one, proxy)
+          for proxy in proxies
+      ]
+      for future in as_completed(futures):
+        try:
+          proxy, status_code = future.result()
+          if status_code == 200:
+            if self.debug:
+              type = 'https' if proxy.https == 'yes' else 'http'
+              addr = f'{proxy.ip_address}:{proxy.port}'
+              print(
+                  '> %-22s | %-3s | %-12s | %s' %
+                  (addr, proxy.code, proxy.anonymity, type),
+              )
+            working.append(f'{proxy.ip_address}:{proxy.port}')
+        except BaseException:
+          continue
+    if self.debug:
+      print('+ Total validated proxies: %d' % len(working))
+    return working
+
+  def scrape(self):
+    proxies = self._fetch()
+    working = self._check_all(proxies)
+    return working
 
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        '-c',
-        '--country',
-        help='Country ISO Code',
-    )
-    parser.add_argument(
-        '-a',
-        '--anon',
-        choices=['anonymous', 'elite', 'transparent'],
-        help='Anonymity level',
-    )
-    parser.add_argument(
-        '--https',
-        action='store_true',
-        default=False,
-        help='Https only',
-    )
-    parser.add_argument(
-        '-o',
-        '--output_file',
-        type=lambda p: Path(p).absolute(),
-        help='Save list of proxies to file.',
-    )
 
-    if len(sys.argv) < 2:
-        parser.print_help(sys.stderr)
-        sys.exit(1)
-
-    args = parser.parse_args()
-
-    proxies = Proxies(
-        country=args.country,
-        anon=args.anon,
-        https=args.https,
-        debug=True,
-    ).scrape()
-
-    if args.output_file:
-        with open(args.output_file, 'w') as f:
-            for proxy in proxies:
-                f.write(proxy + '\n')
-        print('+ Saved proxy list to: %s' % args.output_file)
+def main():
+  parser = argparse.ArgumentParser()
+  parser.add_argument(
+      '-c',
+      '--country',
+      help='Country ISO Code',
+  )
+  parser.add_argument(
+      '-a',
+      '--anon',
+      choices=['anonymous', 'elite', 'transparent'],
+      help='Anonymity level',
+  )
+  parser.add_argument(
+      '--https',
+      action='store_true',
+      default=False,
+      help='Https only',
+  )
+  parser.add_argument(
+      '-o',
+      '--output_file',
+      type=lambda p: Path(p).absolute(),
+      help='Save list of proxies to file.',
+  )
+
+  if len(sys.argv) < 2:
+    parser.print_help(sys.stderr)
+    sys.exit(1)
+
+  args = parser.parse_args()
+
+  proxies = Proxies(
+      country=args.country,
+      anon=args.anon,
+      https=args.https,
+      debug=True,
+  ).scrape()
+
+  if args.output_file:
+    with open(args.output_file, 'w') as f:
+      for proxy in proxies:
+        f.write(proxy + '\n')
+    print('+ Saved proxy list to: %s' % args.output_file)
```

### Comparing `pscrape-0.0.2/pscrape.egg-info/PKG-INFO` & `pscrape-0.0.3/pscrape.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pscrape
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quickly generate a list of free and working proxies
 Home-page: https://github.com/lbirchler/pscrape
 Author: lbirchler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,16 +15,16 @@
 quickly generate a list of free and working proxies
 
 ---
 
 
 ## Installation
 
-```bash
-pip install pscrape 
+```
+python3 -m pip install pscrape 
 ```
 
 ---
 
 ## Usage
 
 ```
@@ -41,15 +41,15 @@
     anonymous, elite, or transparent.
 - **https** (bool, optional): Https only. Defaults to False.
 - **debug** (bool, optional): Display scraped and validated proxies. Defaults to False.
 
 
 ### CLI
 ```
-usage: pscraper [-h] [-c COUNTRY] [-a {anonymous,elite,transparent}] [--https]
+usage: pscrape [-h] [-c COUNTRY] [-a {anonymous,elite,transparent}] [--https]
                     [-o OUTPUT_FILE]
 
 optional arguments:
 -h, --help            show this help message and exit
 -c COUNTRY, --country COUNTRY
                     Country ISO Code
 -a {anonymous,elite,transparent}, --anon {anonymous,elite,transparent}
@@ -58,15 +58,15 @@
 -o OUTPUT_FILE, --output_file OUTPUT_FILE
                     Save list of proxies to file.
 ```
 
 Example:
 
 ```
-$ pscraper -c US --https -o /tmp/proxies.txt
+$ pscrape -c US --https -o /tmp/proxies.txt
 ```
 
 ```
 + Total scraped proxies:  12
 > 20.241.236.196:3128    | US  | anonymous    | https
 > 204.2.218.145:8080     | US  | elite proxy  | https
 > 104.223.135.178:10000  | US  | elite proxy  | https
```

### Comparing `pscrape-0.0.2/setup.cfg` & `pscrape-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pscrape
-version = 0.0.2
+version = 0.0.3
 author = lbirchler
 description = Quickly generate a list of free and working proxies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lbirchler/pscrape
 classifiers = 
 	Programming Language :: Python :: 3
```


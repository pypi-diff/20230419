# Comparing `tmp/dns-crawler-1.6.0.tar.gz` & `tmp/dns-crawler-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dns-crawler-1.6.0.tar", last modified: Thu Apr  6 14:45:42 2023, max compression
+gzip compressed data, was "dns-crawler-1.6.1.tar", last modified: Wed Apr 19 08:59:39 2023, max compression
```

## Comparing `dns-crawler-1.6.0.tar` & `dns-crawler-1.6.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:45:42.009989 dns-crawler-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-03-02 14:50:23.000000 dns-crawler-1.6.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    14552 2023-04-06 14:39:24.000000 dns-crawler-1.6.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      667 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    35061 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    20434 2023-04-06 14:45:42.005989 dns-crawler-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    19596 2023-03-02 14:50:23.000000 dns-crawler-1.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/config.docker.yml
--rw-rw-rw-   0 root         (0) root         (0)     4187 2023-03-02 14:15:34.000000 dns-crawler-1.6.0/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:45:42.005989 dns-crawler-1.6.0/dns_crawler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/dns_crawler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/certificate.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/config_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     6612 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/controller.py
--rw-rw-rw-   0 root         (0) root         (0)    11081 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/crawl.py
--rw-rw-rw-   0 root         (0) root         (0)    12402 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/dns_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/geoip_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/hsts_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/ip_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4421 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/mail_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/redis_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/single.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    16147 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/web_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/worker.py
--rw-rw-rw-   0 root         (0) root         (0)     5101 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/dns_crawler/workers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:45:42.005989 dns-crawler-1.6.0/dns_crawler.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20434 2023-04-06 14:45:41.000000 dns-crawler-1.6.0/dns_crawler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      885 2023-04-06 14:45:41.000000 dns-crawler-1.6.0/dns_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 14:45:41.000000 dns-crawler-1.6.0/dns_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-06 14:45:41.000000 dns-crawler-1.6.0/dns_crawler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-06 14:45:41.000000 dns-crawler-1.6.0/dns_crawler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-06 14:45:41.000000 dns-crawler-1.6.0/dns_crawler.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-06 14:33:34.000000 dns-crawler-1.6.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)   229038 2023-04-06 11:45:35.000000 dns-crawler-1.6.0/result-example.json
--rw-rw-rw-   0 root         (0) root         (0)    23932 2023-04-06 11:45:35.000000 dns-crawler-1.6.0/result-schema.json
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 14:45:42.009989 dns-crawler-1.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2733 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:45:42.005989 dns-crawler-1.6.0/test/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/test/config-nodns.yml
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-06 14:43:33.000000 dns-crawler-1.6.0/test/config-odvr.yml
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-06 13:56:53.000000 dns-crawler-1.6.0/test/nic.cz.test.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-02-23 15:46:15.000000 dns-crawler-1.6.0/update-docker-img.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:59:39.742687 dns-crawler-1.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-02-23 15:46:15.000000 dns-crawler-1.6.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2023-04-19 08:51:51.000000 dns-crawler-1.6.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    14651 2023-04-19 08:56:31.000000 dns-crawler-1.6.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      667 2023-02-23 15:46:15.000000 dns-crawler-1.6.1/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    35061 2023-02-23 15:46:15.000000 dns-crawler-1.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20434 2023-04-19 08:59:39.742687 dns-crawler-1.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    19596 2023-03-02 14:50:23.000000 dns-crawler-1.6.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-02-23 15:46:15.000000 dns-crawler-1.6.1/config.docker.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4187 2023-03-02 14:15:34.000000 dns-crawler-1.6.1/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:59:39.742687 dns-crawler-1.6.1/dns_crawler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 15:46:15.000000 dns-crawler-1.6.1/dns_crawler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/certificate.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/config_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6612 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    11081 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/crawl.py
+-rw-rw-rw-   0 root         (0) root         (0)    12402 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/dns_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-19 08:51:51.000000 dns-crawler-1.6.1/dns_crawler/geoip_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/hsts_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/ip_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4421 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/mail_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/redis_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/single.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16163 2023-04-11 06:19:54.000000 dns-crawler-1.6.1/dns_crawler/web_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5101 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/dns_crawler/workers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:59:39.742687 dns-crawler-1.6.1/dns_crawler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20434 2023-04-19 08:59:39.000000 dns-crawler-1.6.1/dns_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      887 2023-04-19 08:59:39.000000 dns-crawler-1.6.1/dns_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:59:39.000000 dns-crawler-1.6.1/dns_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-19 08:59:39.000000 dns-crawler-1.6.1/dns_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-19 08:59:39.000000 dns-crawler-1.6.1/dns_crawler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-19 08:59:39.000000 dns-crawler-1.6.1/dns_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-06 14:33:34.000000 dns-crawler-1.6.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)   229038 2023-04-06 11:45:35.000000 dns-crawler-1.6.1/result-example.json
+-rw-rw-rw-   0 root         (0) root         (0)    23932 2023-04-06 11:45:35.000000 dns-crawler-1.6.1/result-schema.json
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-19 08:51:51.000000 dns-crawler-1.6.1/ruff.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 08:59:39.742687 dns-crawler-1.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2733 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:59:39.742687 dns-crawler-1.6.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-02-23 15:46:15.000000 dns-crawler-1.6.1/test/config-nodns.yml
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-19 08:59:31.000000 dns-crawler-1.6.1/test/config-odvr.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-06 13:56:53.000000 dns-crawler-1.6.1/test/nic.cz.test.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-02-23 15:46:15.000000 dns-crawler-1.6.1/update-docker-img.sh
```

### Comparing `dns-crawler-1.6.0/.gitlab-ci.yml` & `dns-crawler-1.6.1/.gitlab-ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,17 @@
   - test
   - build
   - deploy
 
 lint:
   stage: lint
   before_script:
-    - pip install flake8 flake8-quotes
+    - pip install ruff
   script:
-    - flake8 --config=.flake8
+    - ruff --format=gitlab .
 
 validate_result_example:
   stage: lint
   before_script:
     - pip install -q check-jsonschema
   script: 
     - check-jsonschema --schemafile result-schema.json result-example.json
```

### Comparing `dns-crawler-1.6.0/CHANGELOG.md` & `dns-crawler-1.6.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 1.6.1
+
+- Replaced Flake8 with Ruff
+
+### WEB
+
+- Another fix for prematurely closing connections
+
 ## 1.6.0 (2023-04-06)
 
 - Minimal supported Python version is now 3.7
 - Updated `PyICU` dependency so it installs smoothly on distros with new sw versions (eg. Gentoo & Arch)
 - Updated `cryptography` and `pyOpenSSL` to make things work with new OpenSSL
 - Updated `RQ`, we are now using its `enqueue_many` feature instead of the old custom implementation (which was basically the same thing, but now it's upstream)
 - Updated most of other dependencies to latest stable versions
```

### Comparing `dns-crawler-1.6.0/Dockerfile` & `dns-crawler-1.6.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/LICENSE` & `dns-crawler-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/PKG-INFO` & `dns-crawler-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dns-crawler
-Version: 1.6.0
+Version: 1.6.1
 Summary: A crawler for getting info about DNS domains and services attached to them.
 Home-page: https://gitlab.nic.cz/adam/dns-crawler
 Author: Jiri Helebrant
 Author-email: jiri.helebrant@nic.cz
 License: UNKNOWN
 Project-URL: Operation in .CZ, https://www.csirt.cz/en/dns-crawler/
 Project-URL: CZ.NIC stats dashboard, https://stats.nic.cz/
```

### Comparing `dns-crawler-1.6.0/README.md` & `dns-crawler-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/config.yml` & `dns-crawler-1.6.1/config.yml`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/certificate.py` & `dns-crawler-1.6.1/dns_crawler/certificate.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/config_loader.py` & `dns-crawler-1.6.1/dns_crawler/config_loader.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/controller.py` & `dns-crawler-1.6.1/dns_crawler/controller.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/crawl.py` & `dns-crawler-1.6.1/dns_crawler/crawl.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/dns_utils.py` & `dns-crawler-1.6.1/dns_crawler/dns_utils.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/geoip_utils.py` & `dns-crawler-1.6.1/dns_crawler/geoip_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     if "isp" in config["geoip"]:
         try:
             db_path = path.join(pwd, config["geoip"]["isp"])
             geoip_isp = geoip2.database.Reader(db_path)
         except FileNotFoundError:
             stderr.write(f"GeoIP ISP DB cannot be found in '{db_path}'. Disabling.\n")
 
-    if "asn" in config["geoip"] and not ("isp" in config["geoip"]):
+    if "asn" in config["geoip"] and ("isp" not in config["geoip"]):
         try:
             db_path = path.join(pwd, config["geoip"]["asn"])
             geoip_asn = geoip2.database.Reader(db_path)
         except FileNotFoundError:
             stderr.write(f"GeoIP ASN DB cannot be found in '{db_path}'. Disabling.\n")
 
     return (geoip_country, geoip_isp, geoip_asn)
```

### Comparing `dns-crawler-1.6.0/dns_crawler/hsts_utils.py` & `dns-crawler-1.6.1/dns_crawler/hsts_utils.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/ip_utils.py` & `dns-crawler-1.6.1/dns_crawler/ip_utils.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/mail_utils.py` & `dns-crawler-1.6.1/dns_crawler/mail_utils.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/redis_utils.py` & `dns-crawler-1.6.1/dns_crawler/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/single.py` & `dns-crawler-1.6.1/dns_crawler/single.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/timestamp.py` & `dns-crawler-1.6.1/dns_crawler/timestamp.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/utils.py` & `dns-crawler-1.6.1/dns_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/web_utils.py` & `dns-crawler-1.6.1/dns_crawler/web_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
                     chunk_len += CHUNK_SIZE
                     content_bytes.append(chunk)
                     if chunk_len > content_size_limit or time() - start_time > config["timeouts"]["http_read"]:
                         h["r"].close()
             except (requests.exceptions.ConnectionError, requests.exceptions.ReadTimeout,
                     requests.exceptions.InvalidURL, requests.exceptions.InvalidSchema,
                     requests.exceptions.ContentDecodingError, requests.exceptions.ChunkedEncodingError,
-                    UnicodeError, ValueError) as e:
+                    UnicodeError, ValueError, AttributeError) as e:
                 h["e"] = emsg(e)
             except requests.exceptions.InvalidHeader as e:
                 h["e"] = f"Invalid Location header in previous step. '{url}' - {emsg(e)}"
             except urllib3.exceptions.LocationParseError as e:
                 h["e"] = emsg(e)
             history.append(h)
             redirect_count = redirect_count + 1
```

### Comparing `dns-crawler-1.6.0/dns_crawler/worker.py` & `dns-crawler-1.6.1/dns_crawler/worker.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler/workers.py` & `dns-crawler-1.6.1/dns_crawler/workers.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/dns_crawler.egg-info/PKG-INFO` & `dns-crawler-1.6.1/dns_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dns-crawler
-Version: 1.6.0
+Version: 1.6.1
 Summary: A crawler for getting info about DNS domains and services attached to them.
 Home-page: https://gitlab.nic.cz/adam/dns-crawler
 Author: Jiri Helebrant
 Author-email: jiri.helebrant@nic.cz
 License: UNKNOWN
 Project-URL: Operation in .CZ, https://www.csirt.cz/en/dns-crawler/
 Project-URL: CZ.NIC stats dashboard, https://stats.nic.cz/
```

### Comparing `dns-crawler-1.6.0/dns_crawler.egg-info/SOURCES.txt` & `dns-crawler-1.6.1/dns_crawler.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-.flake8
 .gitignore
 .gitlab-ci.yml
 CHANGELOG.md
 Dockerfile
 LICENSE
 README.md
 config.docker.yml
 config.yml
 requirements.txt
 result-example.json
 result-schema.json
+ruff.toml
 setup.py
 update-docker-img.sh
 dns_crawler/__init__.py
 dns_crawler/certificate.py
 dns_crawler/config_loader.py
 dns_crawler/controller.py
 dns_crawler/crawl.py
```

### Comparing `dns-crawler-1.6.0/result-example.json` & `dns-crawler-1.6.1/result-example.json`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/result-schema.json` & `dns-crawler-1.6.1/result-schema.json`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/setup.py` & `dns-crawler-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `dns-crawler-1.6.0/test/nic.cz.test.py` & `dns-crawler-1.6.1/test/nic.cz.test.py`

 * *Files identical despite different names*


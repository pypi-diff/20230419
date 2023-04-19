# Comparing `tmp/fedexapi_chnoma-1.2.tar.gz` & `tmp/fedexapi_chnoma-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedexapi_chnoma-1.2.tar", last modified: Mon Oct 17 16:19:04 2022, max compression
+gzip compressed data, was "fedexapi_chnoma-1.2.1.tar", last modified: Wed Apr 19 18:36:07 2023, max compression
```

## Comparing `fedexapi_chnoma-1.2.tar` & `fedexapi_chnoma-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 adrian    (1000) adrian    (1001)        0 2022-10-17 16:19:04.667581 fedexapi_chnoma-1.2/
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)     1079 2022-06-24 21:15:12.000000 fedexapi_chnoma-1.2/LICENSE
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)      951 2022-10-17 16:19:04.727786 fedexapi_chnoma-1.2/PKG-INFO
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)    11135 2022-10-17 16:02:48.000000 fedexapi_chnoma-1.2/fedex_api.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1001)        0 2022-10-17 16:19:04.721496 fedexapi_chnoma-1.2/fedexapi_chnoma.egg-info/
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)      951 2022-10-17 16:19:04.000000 fedexapi_chnoma-1.2/fedexapi_chnoma.egg-info/PKG-INFO
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)      229 2022-10-17 16:19:04.000000 fedexapi_chnoma-1.2/fedexapi_chnoma.egg-info/SOURCES.txt
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)        1 2022-10-17 16:19:04.000000 fedexapi_chnoma-1.2/fedexapi_chnoma.egg-info/dependency_links.txt
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)        9 2022-10-17 16:19:04.000000 fedexapi_chnoma-1.2/fedexapi_chnoma.egg-info/requires.txt
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)       10 2022-10-17 16:19:04.000000 fedexapi_chnoma-1.2/fedexapi_chnoma.egg-info/top_level.txt
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)      701 2022-10-17 16:09:13.000000 fedexapi_chnoma-1.2/pyproject.toml
--rwxr-xr-x   0 adrian    (1000) adrian    (1001)       38 2022-10-17 16:19:04.732786 fedexapi_chnoma-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 18:36:07.020719 fedexapi_chnoma-1.2.1/
+-rw-rw-rw-   0        0        0     1079 2023-03-09 14:41:47.000000 fedexapi_chnoma-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-04-19 18:36:07.018719 fedexapi_chnoma-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10964 2023-04-19 18:32:02.000000 fedexapi_chnoma-1.2.1/fedex_api.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:36:07.004484 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 18:36:06.000000 fedexapi_chnoma-1.2.1/fedexapi_chnoma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      703 2023-04-19 18:33:49.000000 fedexapi_chnoma-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 18:36:07.020719 fedexapi_chnoma-1.2.1/setup.cfg
```

### Comparing `fedexapi_chnoma-1.2/LICENSE` & `fedexapi_chnoma-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fedexapi_chnoma-1.2/fedex_api.py` & `fedexapi_chnoma-1.2.1/fedex_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -220,16 +220,14 @@
                                 data={"grant_type": "client_credentials",
                                       "client_id": self.API_KEY,
                                       "client_secret": self.SECRET_KEY})
         try:
             self.AUTH_KEY = request.json()['access_token']
         except IndexError:
             raise AuthenticationError("\nInvalid authentication request.")
-        print("Obtained authentication key: ", self.AUTH_KEY,
-              "\n_________________________________________________________________________________\n\n\n")
 
     def track_by_number(self, number: str) -> TrackingResult:
         payload = {"trackingInfo": [{"trackingNumberInfo": {"trackingNumber": str(number)}}],
                    "includeDetailedScans": "False"}
         headers = {"Content-type": "application/json",
                    "Authorization": f"Bearer {self.AUTH_KEY}"}
         response = requests.request("POST", self.TRACK_URL,
```

### Comparing `fedexapi_chnoma-1.2/pyproject.toml` & `fedexapi_chnoma-1.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fedexapi_chnoma"
-version = "1.2"
+version = "1.2.1"
 description = "A module I devloped to abstract the Fedex API for use in my programs."
 authors = [
   { name="Adrian J. Arnett", email="adrianarnett0@gmail.com" },
 ]
 readme = "readme.md"
 keywords = ["FedEx", "API"]
 requires-python = ">=3.7"
```


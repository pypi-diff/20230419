# Comparing `tmp/haki_crawler-0.5.tar.gz` & `tmp/haki_crawler-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haki_crawler-0.5.tar", last modified: Sun Apr 16 11:00:49 2023, max compression
+gzip compressed data, was "haki_crawler-0.6.tar", last modified: Wed Apr 19 07:05:09 2023, max compression
```

## Comparing `haki_crawler-0.5.tar` & `haki_crawler-0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 11:00:49.582330 haki_crawler-0.5/
--rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 11:00:49.582074 haki_crawler-0.5/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 11:00:49.579192 haki_crawler-0.5/haki_crawler/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-16 10:09:24.000000 haki_crawler-0.5/haki_crawler/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7737 2023-04-16 11:00:30.000000 haki_crawler-0.5/haki_crawler/sensortower.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 11:00:49.581553 haki_crawler-0.5/haki_crawler.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      240 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        9 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       13 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-16 11:00:49.582422 haki_crawler-0.5/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1221 2023-04-16 11:00:41.000000 haki_crawler-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:05:09.901063 haki_crawler-0.6/
+-rw-rw-rw-   0        0        0      634 2023-04-19 07:05:09.901063 haki_crawler-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 07:05:09.886063 haki_crawler-0.6/haki_crawler/
+-rw-rw-rw-   0        0        0        0 2023-04-17 04:16:01.000000 haki_crawler-0.6/haki_crawler/__init__.py
+-rw-rw-rw-   0        0        0     3711 2023-04-19 07:01:16.000000 haki_crawler-0.6/haki_crawler/appfigures.py
+-rw-rw-rw-   0        0        0     7966 2023-04-17 04:16:01.000000 haki_crawler-0.6/haki_crawler/sensortower.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:05:09.900062 haki_crawler-0.6/haki_crawler.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:05:09.902063 haki_crawler-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-04-19 07:03:06.000000 haki_crawler-0.6/setup.py
```

### Comparing `haki_crawler-0.5/PKG-INFO` & `haki_crawler-0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: haki_crawler
-Version: 0.5
-Summary: A short description of your package
-Home-page: https://example.com
-Author: namhn1495
-Author-email: namhn1495@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
-# haki
+Metadata-Version: 2.1
+Name: haki_crawler
+Version: 0.6
+Summary: A short description of your package
+Home-page: https://example.com
+Author: namhn1495
+Author-email: namhn1495@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# haki
```

### Comparing `haki_crawler-0.5/haki_crawler/sensortower.py` & `haki_crawler-0.6/haki_crawler/sensortower.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,228 @@
-from datetime import date, timedelta
-from datetime import date
-import requests
-import json
-
-
-def app_info(cookie, app_id='com.lemon.lvoverseas', country='US', auth_token='your_auth_token'):
-    """
-    This function retrieves data about a specified app from the Sensor Tower API.
-
-    Args:
-    - app_id (str): The ID of the app to retrieve data for.
-    - cookie (str): The value of the 'session' cookie needed to authenticate the request.
-    - country (str): The two-letter code for the country to retrieve data for. Defaults to 'US'.
-    - auth_token (str): The authentication token for the Sensor Tower API. Defaults to 'your_auth_token'.
-
-    Returns:
-    - response (requests.Response): A response object containing the data retrieved from the API.
-    """
-
-    session = cookie['session']
-    device_id = cookie['device_id']
-
-    # Create the headers needed for the request
-    headers = {
-        'Cookie': f'session={session}; device_id={device_id}'
-    }
-
-    # Set the parameters for the request
-    params = {
-        'country': country,
-        'auth_token': auth_token,
-        'app_ids': app_id
-    }
-
-    # Set the URL for the request
-    url = "https://api.sensortower.com/v1/android/apps"
-
-    # Send the request to the API and return the response
-    response = requests.request("GET", url, headers=headers, params=params)
-    return response.json()
-
-
-def app_info_minified(
-        cookie,
-        app_id='com.lemon.lvoverseas',
-        country='US',
-        auth_token='your_auth_token'
-):
-    """
-    This function retrieves data about a specified app from the Sensor Tower API but minified
-
-    Args:
-    - app_id (str): The ID of the app to retrieve data for.
-    - cookie (str): The value of the 'session' cookie needed to authenticate the request.
-    - country (str): The two-letter code for the country to retrieve data for. Defaults to 'US'.
-    - auth_token (str): The authentication token for the Sensor Tower API. Defaults to 'your_auth_token'.
-
-    Returns:
-    - response (requests.Response): A response object containing the data retrieved from the API.
-    """
-
-    session = cookie['session']
-    device_id = cookie['device_id']
-
-    # Create the headers needed for the request
-    headers = {
-        'Cookie': f'session={session}; device_id={device_id}'
-    }
-
-    # Set the parameters for the request
-    params = {
-        'country': country,
-        'auth_token': auth_token,
-        'app_ids': app_id
-    }
-
-    # Set the URL for the request
-    url = "https://app.sensortower.com/api/android/apps/{}".format(app_id)
-    # Send the request to the API and return the response
-    response = requests.request("GET", url, headers=headers, params=params)
-    return response.json()
-
-
-def retention(cookie, app_id='com.lemon.lvoverseas', country='US', auth_token='your_auth_token'):
-    """
-    This function retrieves retention data for a specified app from the Sensor Tower API.
-
-    Args:
-    - cookie (dict): A dictionary containing 'session' and 'device_id' values needed to authenticate the request.
-    - app_id (str): The ID of the app to retrieve retention data for. Defaults to 'com.lemon.lvoverseas'.
-    - country (str): The two-letter code for the country to retrieve data for. Defaults to 'US'.
-    - auth_token (str): The authentication token for the Sensor Tower API. Defaults to 'your_auth_token'.
-
-    Returns:
-    - response (requests.Response): A response object containing the data retrieved from the API.
-    """
-
-    session = cookie['session']
-    device_id = cookie['device_id']
-
-    # Create the headers needed for the request
-    headers = {
-        'Cookie': f'session={session}; device_id={device_id}'
-    }
-
-    # Set the parameters for the request
-    params = {
-        'country': country,
-        'auth_token': auth_token,
-        'app_ids': app_id,
-        'date_granularity': "all_time",
-        'start_date': date.today().strftime('%Y-%m-%d')
-    }
-
-    # Set the URL for the request
-    url = "https://api.sensortower.com/v1/android/usage/retention"
-
-    # Send the request to the API and return the response
-    response = requests.request("GET", url, headers=headers, params=params)
-    return response.json()
-
-
-def usages(
-    cookie,
-    app_id='com.lemon.lvoverseas',
-    usage_type='demographics',
-    time_range=90,
-    country='US',
-    auth_token='your_auth_token'
-):
-    """
-    This function retrieves usage data for a specified app from the Sensor Tower API.
-
-    Args:
-    - cookie (dict): A dictionary containing 'session' and 'device_id' values needed to authenticate the request.
-    - app_id (str): The ID of the app to retrieve usage data for.
-    - usage_type (str): The type of usage data to retrieve. Accepted values: 'session_count', 'session_duration', 'time_spent', 'demographics'.
-    - time_range (int): The number of days to retrieve data for. Defaults to 90.
-
-    Returns:
-    - response (requests.Response): A response object containing the data retrieved from the API.
-    """
-
-    today = date.today()
-    prior_date = today - timedelta(days=time_range)
-
-    session = cookie['session']
-    device_id = cookie['device_id']
-
-    # Create the headers needed for the request
-    headers = {
-        'Cookie': f'session={session}; device_id={device_id}'
-    }
-
-    # Set the parameters for the request
-    params = {
-        'country': country,
-        'auth_token': auth_token,
-        'app_ids': app_id,
-        'date_granularity': "all_time",
-        "start_date": today.strftime('%Y-%m-%d'),
-        "end_date": prior_date.strftime('%Y-%m-%d'),
-    }
-
-    # Set the URL for the request
-    url = f"https://api.sensortower.com/v1/android/usage/{usage_type}"
-
-    # Send the request to the API and return the response
-    response = requests.request("GET", url, headers=headers, params=params)
-    return response.json()
-
-
-def advanced_search(cookie, custom_filter_id, term, limit=250, country='US', auth_token='your_auth_token'):
-    """
-    This function performs an advanced search on the Sensor Tower website.
-
-    Args:
-    - cookie (str): The value of the 'session' cookie needed to authenticate the request.
-    - custom_filter_id (str): The ID of the custom filter to use for the search.
-    - term (str): The search term to use for the search.
-    - limit (int): The maximum number of results to return. Defaults to 250.
-
-    Returns:
-    - response (requests.Response): A response object containing the data retrieved from the search.
-    """
-
-    # Extract session and device_id from the cookie
-    session = cookie['session']
-    device_id = cookie['device_id']
-
-    # Set the URL and parameters for the request
-    url = "https://app.sensortower.com/advanced_search"
-    params = {
-        'country': country,
-        'auth_token': auth_token,
-        'device_type': 'android',
-        'entity_type': 'app',
-        'os': 'android',
-        'search_fields[]': ['name', 'short_description'],
-        'custom_fields_filter_id': custom_filter_id,
-        'term': term,
-        'limit': limit
-    }
-
-    # Set the headers for the request
-    headers = {
-        'Cookie': f'session={session}; device_id={device_id}'
-    }
-
-    # Send the request to the Sensor Tower website and return the response
-    response = requests.request("GET", url, headers=headers, params=params)
-    return response.json()
-
-
-if __name__ == "__main__":
-    # cookie = requests.get('http://localhost:3000/sensortower')
-    # cookie = cookie.json()
-
-    cookie = {
-        "session": "2e8e2b1cfd6d791d55b235e53066f7a3",
-        "device_id": "446def50-8494-487a-ab39-d8d965f014d2",
-    }
-
-    result = advanced_search(
-        cookie=cookie, custom_filter_id="643bd16ee1714cfff1654c97", term="voice changer")
-    print(json.dumps(result, indent=2))
+from datetime import date, timedelta
+from datetime import date
+import requests
+import json
+
+
+def app_info(cookie, app_id='com.lemon.lvoverseas', country='US', auth_token='your_auth_token'):
+    """
+    This function retrieves data about a specified app from the Sensor Tower API.
+
+    Args:
+    - app_id (str): The ID of the app to retrieve data for.
+    - cookie (str): The value of the 'session' cookie needed to authenticate the request.
+    - country (str): The two-letter code for the country to retrieve data for. Defaults to 'US'.
+    - auth_token (str): The authentication token for the Sensor Tower API. Defaults to 'your_auth_token'.
+
+    Returns:
+    - response (requests.Response): A response object containing the data retrieved from the API.
+    """
+
+    session = cookie['session']
+    device_id = cookie['device_id']
+
+    # Create the headers needed for the request
+    headers = {
+        'Cookie': f'session={session}; device_id={device_id}'
+    }
+
+    # Set the parameters for the request
+    params = {
+        'country': country,
+        'auth_token': auth_token,
+        'app_ids': app_id
+    }
+
+    # Set the URL for the request
+    url = "https://api.sensortower.com/v1/android/apps"
+
+    # Send the request to the API and return the response
+    response = requests.request("GET", url, headers=headers, params=params)
+    return response.json()
+
+
+def app_info_minified(
+        cookie,
+        app_id='com.lemon.lvoverseas',
+        country='US',
+        auth_token='your_auth_token'
+):
+    """
+    This function retrieves data about a specified app from the Sensor Tower API but minified
+
+    Args:
+    - app_id (str): The ID of the app to retrieve data for.
+    - cookie (str): The value of the 'session' cookie needed to authenticate the request.
+    - country (str): The two-letter code for the country to retrieve data for. Defaults to 'US'.
+    - auth_token (str): The authentication token for the Sensor Tower API. Defaults to 'your_auth_token'.
+
+    Returns:
+    - response (requests.Response): A response object containing the data retrieved from the API.
+    """
+
+    session = cookie['session']
+    device_id = cookie['device_id']
+
+    # Create the headers needed for the request
+    headers = {
+        'Cookie': f'session={session}; device_id={device_id}'
+    }
+
+    # Set the parameters for the request
+    params = {
+        'country': country,
+        'auth_token': auth_token,
+        'app_ids': app_id
+    }
+
+    # Set the URL for the request
+    url = "https://app.sensortower.com/api/android/apps/{}".format(app_id)
+    # Send the request to the API and return the response
+    response = requests.request("GET", url, headers=headers, params=params)
+    return response.json()
+
+
+def retention(cookie, app_id='com.lemon.lvoverseas', country='US', auth_token='your_auth_token'):
+    """
+    This function retrieves retention data for a specified app from the Sensor Tower API.
+
+    Args:
+    - cookie (dict): A dictionary containing 'session' and 'device_id' values needed to authenticate the request.
+    - app_id (str): The ID of the app to retrieve retention data for. Defaults to 'com.lemon.lvoverseas'.
+    - country (str): The two-letter code for the country to retrieve data for. Defaults to 'US'.
+    - auth_token (str): The authentication token for the Sensor Tower API. Defaults to 'your_auth_token'.
+
+    Returns:
+    - response (requests.Response): A response object containing the data retrieved from the API.
+    """
+
+    session = cookie['session']
+    device_id = cookie['device_id']
+
+    # Create the headers needed for the request
+    headers = {
+        'Cookie': f'session={session}; device_id={device_id}'
+    }
+
+    # Set the parameters for the request
+    params = {
+        'country': country,
+        'auth_token': auth_token,
+        'app_ids': app_id,
+        'date_granularity': "all_time",
+        'start_date': date.today().strftime('%Y-%m-%d')
+    }
+
+    # Set the URL for the request
+    url = "https://api.sensortower.com/v1/android/usage/retention"
+
+    # Send the request to the API and return the response
+    response = requests.request("GET", url, headers=headers, params=params)
+    return response.json()
+
+
+def usages(
+    cookie,
+    app_id='com.lemon.lvoverseas',
+    usage_type='demographics',
+    time_range=90,
+    country='US',
+    auth_token='your_auth_token'
+):
+    """
+    This function retrieves usage data for a specified app from the Sensor Tower API.
+
+    Args:
+    - cookie (dict): A dictionary containing 'session' and 'device_id' values needed to authenticate the request.
+    - app_id (str): The ID of the app to retrieve usage data for.
+    - usage_type (str): The type of usage data to retrieve. Accepted values: 'session_count', 'session_duration', 'time_spent', 'demographics'.
+    - time_range (int): The number of days to retrieve data for. Defaults to 90.
+
+    Returns:
+    - response (requests.Response): A response object containing the data retrieved from the API.
+    """
+
+    today = date.today()
+    prior_date = today - timedelta(days=time_range)
+
+    session = cookie['session']
+    device_id = cookie['device_id']
+
+    # Create the headers needed for the request
+    headers = {
+        'Cookie': f'session={session}; device_id={device_id}'
+    }
+
+    # Set the parameters for the request
+    params = {
+        'country': country,
+        'auth_token': auth_token,
+        'app_ids': app_id,
+        'date_granularity': "all_time",
+        "start_date": today.strftime('%Y-%m-%d'),
+        "end_date": prior_date.strftime('%Y-%m-%d'),
+    }
+
+    # Set the URL for the request
+    url = f"https://api.sensortower.com/v1/android/usage/{usage_type}"
+
+    # Send the request to the API and return the response
+    response = requests.request("GET", url, headers=headers, params=params)
+    return response.json()
+
+
+def advanced_search(cookie, custom_filter_id, term, limit=250, country='US', auth_token='your_auth_token'):
+    """
+    This function performs an advanced search on the Sensor Tower website.
+
+    Args:
+    - cookie (str): The value of the 'session' cookie needed to authenticate the request.
+    - custom_filter_id (str): The ID of the custom filter to use for the search.
+    - term (str): The search term to use for the search.
+    - limit (int): The maximum number of results to return. Defaults to 250.
+
+    Returns:
+    - response (requests.Response): A response object containing the data retrieved from the search.
+    """
+
+    # Extract session and device_id from the cookie
+    session = cookie['session']
+    device_id = cookie['device_id']
+
+    # Set the URL and parameters for the request
+    url = "https://app.sensortower.com/advanced_search"
+    params = {
+        'country': country,
+        'auth_token': auth_token,
+        'device_type': 'android',
+        'entity_type': 'app',
+        'os': 'android',
+        'search_fields[]': ['name', 'short_description'],
+        'custom_fields_filter_id': custom_filter_id,
+        'term': term,
+        'limit': limit
+    }
+
+    # Set the headers for the request
+    headers = {
+        'Cookie': f'session={session}; device_id={device_id}'
+    }
+
+    # Send the request to the Sensor Tower website and return the response
+    response = requests.request("GET", url, headers=headers, params=params)
+    return response.json()
+
+
+if __name__ == "__main__":
+    # cookie = requests.get('http://localhost:3000/sensortower')
+    # cookie = cookie.json()
+
+    cookie = {
+        "session": "2e8e2b1cfd6d791d55b235e53066f7a3",
+        "device_id": "446def50-8494-487a-ab39-d8d965f014d2",
+    }
+
+    result = advanced_search(
+        cookie=cookie, custom_filter_id="643bd16ee1714cfff1654c97", term="voice changer")
+    print(json.dumps(result, indent=2))
+
```

### Comparing `haki_crawler-0.5/haki_crawler.egg-info/PKG-INFO` & `haki_crawler-0.6/haki_crawler.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: haki-crawler
-Version: 0.5
-Summary: A short description of your package
-Home-page: https://example.com
-Author: namhn1495
-Author-email: namhn1495@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
-# haki
+Metadata-Version: 2.1
+Name: haki-crawler
+Version: 0.6
+Summary: A short description of your package
+Home-page: https://example.com
+Author: namhn1495
+Author-email: namhn1495@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# haki
```

### Comparing `haki_crawler-0.5/setup.py` & `haki_crawler-0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from setuptools import setup, find_packages
-import os
-import shutil
-
-
-
-LIB_NAME = "haki_crawler"
-
-
-thu_muc_can_xoa = ["build", "dist", "{}.egg-info".format(LIB_NAME)]
-
-for thu_muc in thu_muc_can_xoa:
-    if os.path.exists(thu_muc):
-        shutil.rmtree(thu_muc)
-        print(f"Đã xóa thư mục: {thu_muc}")
-    else:
-        print(f"Thư mục {thu_muc} không tồn tại")
-
-setup(
-    name=LIB_NAME,
-    version="0.5",
-    packages=find_packages(),
-    install_requires=[
-        # Danh sách các gói phụ thuộc của gói này
-        "requests",
-    ],
-    author="namhn1495",
-    author_email="namhn1495@gmail.com",
-    description="A short description of your package",
-    long_description=open("README.md").read(),
-    long_description_content_type="text/markdown",
-    url="https://example.com",
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-    ],
-)
+from setuptools import setup, find_packages
+import os
+import shutil
+
+
+
+LIB_NAME = "haki_crawler"
+
+
+thu_muc_can_xoa = ["build", "dist", "{}.egg-info".format(LIB_NAME)]
+
+for thu_muc in thu_muc_can_xoa:
+    if os.path.exists(thu_muc):
+        shutil.rmtree(thu_muc)
+        print(f"Đã xóa thư mục: {thu_muc}")
+    else:
+        print(f"Thư mục {thu_muc} không tồn tại")
+
+setup(
+    name=LIB_NAME,
+    version="0.6",
+    packages=find_packages(),
+    install_requires=[
+        # Danh sách các gói phụ thuộc của gói này
+        "requests",
+    ],
+    author="namhn1495",
+    author_email="namhn1495@gmail.com",
+    description="A short description of your package",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    url="https://example.com",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+    ],
+)
```


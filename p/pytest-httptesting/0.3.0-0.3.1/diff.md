# Comparing `tmp/pytest_httptesting-0.3.0.tar.gz` & `tmp/pytest_httptesting-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_httptesting-0.3.0.tar", max compression
+gzip compressed data, was "pytest_httptesting-0.3.1.tar", max compression
```

## Comparing `pytest_httptesting-0.3.0.tar` & `pytest_httptesting-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2022-11-13 16:42:42.780000 pytest_httptesting-0.3.0/LICENSE
--rw-r--r--   0        0        0     3419 2023-03-15 21:38:05.994262 pytest_httptesting-0.3.0/README.md
--rw-r--r--   0        0        0        0 2022-11-13 15:15:16.880000 pytest_httptesting-0.3.0/http_testing/__init__.py
--rw-r--r--   0        0        0        0 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.0/http_testing/assertion_elements/__init__.py
--rw-r--r--   0        0        0      567 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.0/http_testing/assertion_elements/assert_element_checker_base.py
--rw-r--r--   0        0        0     1354 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.0/http_testing/assertion_elements/assertion_attribute_base.py
--rw-r--r--   0        0        0     1587 2022-12-08 23:04:34.980000 pytest_httptesting-0.3.0/http_testing/assertion_elements/content_assertion.py
--rw-r--r--   0        0        0     2888 2023-03-15 21:51:49.084262 pytest_httptesting-0.3.0/http_testing/assertion_elements/cookies_assertion.py
--rw-r--r--   0        0        0     1601 2022-12-08 23:04:34.980000 pytest_httptesting-0.3.0/http_testing/assertion_elements/headers_assertion.py
--rw-r--r--   0        0        0      728 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.0/http_testing/assertion_elements/status_code_assertion.py
--rw-r--r--   0        0        0     1316 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.0/http_testing/assertions.py
--rw-r--r--   0        0        0       79 2023-03-15 21:50:59.084262 pytest_httptesting-0.3.0/http_testing/cookie.py
--rw-r--r--   0        0        0      259 2023-03-15 20:54:56.384262 pytest_httptesting-0.3.0/http_testing/http_client_configuration.py
--rw-r--r--   0        0        0     2747 2023-03-14 21:00:43.542822 pytest_httptesting-0.3.0/http_testing/page_checker.py
--rw-r--r--   0        0        0     1001 2023-03-15 20:57:32.694262 pytest_httptesting-0.3.0/http_testing/plugin.py
--rw-r--r--   0        0        0      682 2022-12-08 23:04:34.980000 pytest_httptesting-0.3.0/http_testing/validators.py
--rw-r--r--   0        0        0      705 2023-03-15 21:06:19.164262 pytest_httptesting-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 pytest_httptesting-0.3.0/setup.py
--rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 pytest_httptesting-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-11-13 16:42:42.780000 pytest_httptesting-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3419 2023-03-15 21:38:05.994262 pytest_httptesting-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2022-11-13 15:15:16.880000 pytest_httptesting-0.3.1/http_testing/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.1/http_testing/assertion_elements/__init__.py
+-rw-r--r--   0        0        0      567 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.1/http_testing/assertion_elements/assert_element_checker_base.py
+-rw-r--r--   0        0        0     1354 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.1/http_testing/assertion_elements/assertion_attribute_base.py
+-rw-r--r--   0        0        0     1587 2022-12-08 23:04:34.980000 pytest_httptesting-0.3.1/http_testing/assertion_elements/content_assertion.py
+-rw-r--r--   0        0        0     2888 2023-04-19 19:28:06.610000 pytest_httptesting-0.3.1/http_testing/assertion_elements/cookies_assertion.py
+-rw-r--r--   0        0        0     1601 2022-12-08 23:04:34.980000 pytest_httptesting-0.3.1/http_testing/assertion_elements/headers_assertion.py
+-rw-r--r--   0        0        0      728 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.1/http_testing/assertion_elements/status_code_assertion.py
+-rw-r--r--   0        0        0     1316 2022-11-13 15:15:16.890000 pytest_httptesting-0.3.1/http_testing/assertions.py
+-rw-r--r--   0        0        0       79 2023-03-15 21:50:59.084262 pytest_httptesting-0.3.1/http_testing/cookie.py
+-rw-r--r--   0        0        0      259 2023-03-15 20:54:56.384262 pytest_httptesting-0.3.1/http_testing/http_client_configuration.py
+-rw-r--r--   0        0        0     2747 2023-03-14 21:00:43.542822 pytest_httptesting-0.3.1/http_testing/page_checker.py
+-rw-r--r--   0        0        0     1217 2023-04-19 19:51:28.110000 pytest_httptesting-0.3.1/http_testing/plugin.py
+-rw-r--r--   0        0        0      682 2023-04-19 19:29:37.490000 pytest_httptesting-0.3.1/http_testing/validators.py
+-rw-r--r--   0        0        0      705 2023-04-19 19:48:48.690000 pytest_httptesting-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 pytest_httptesting-0.3.1/setup.py
+-rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 pytest_httptesting-0.3.1/PKG-INFO
```

### Comparing `pytest_httptesting-0.3.0/LICENSE` & `pytest_httptesting-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/README.md` & `pytest_httptesting-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/assertion_elements/assert_element_checker_base.py` & `pytest_httptesting-0.3.1/http_testing/assertion_elements/assert_element_checker_base.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/assertion_elements/assertion_attribute_base.py` & `pytest_httptesting-0.3.1/http_testing/assertion_elements/assertion_attribute_base.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/assertion_elements/content_assertion.py` & `pytest_httptesting-0.3.1/http_testing/assertion_elements/content_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/assertion_elements/cookies_assertion.py` & `pytest_httptesting-0.3.1/http_testing/assertion_elements/cookies_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/assertion_elements/headers_assertion.py` & `pytest_httptesting-0.3.1/http_testing/assertion_elements/headers_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/assertion_elements/status_code_assertion.py` & `pytest_httptesting-0.3.1/http_testing/assertion_elements/status_code_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/assertions.py` & `pytest_httptesting-0.3.1/http_testing/assertions.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/page_checker.py` & `pytest_httptesting-0.3.1/http_testing/page_checker.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/http_testing/validators.py` & `pytest_httptesting-0.3.1/http_testing/validators.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.3.0/pyproject.toml` & `pytest_httptesting-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pytest-httptesting"
-version = "0.3.0"
+version = "0.3.1"
 description = "http_testing framework on top of pytest"
 authors = ["HE Qile <mr.qile@gmail.com>"]
 readme = "README.md"
 packages = [{include = "http_testing"}]
 
 homepage = "https://github.com/heqile/http_testing"
 repository = "https://github.com/heqile/http_testing"
 
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest = "^7.2.0"
-httpx = "^0.23.0"
-attrs = "^22.1.0"
+httpx = "^0.24.0"
+attrs = "^23.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 mypy = "^1.1.1"
 black = "^23.1.0"
```

### Comparing `pytest_httptesting-0.3.0/setup.py` & `pytest_httptesting-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['http_testing', 'http_testing.assertion_elements']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['attrs>=22.1.0,<23.0.0', 'httpx>=0.23.0,<0.24.0', 'pytest>=7.2.0,<8.0.0']
+['attrs>=23.1.0,<24.0.0', 'httpx>=0.24.0,<0.25.0', 'pytest>=7.2.0,<8.0.0']
 
 entry_points = \
 {'pytest11': ['http_page_checker = http_testing.plugin']}
 
 setup_kwargs = {
     'name': 'pytest-httptesting',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'http_testing framework on top of pytest',
     'long_description': '# HTTP_TESTING\n\n## Description\nThis project aims to help to create e2e tests, by chaining http calls and verifications on target pages.\n\n## Concept\nThis project is built on pytest.\n\nEach .py file in test represents several tests scenario on one target site, we can provide the site\'s hostname\nas a local variable, the framework know how to construct http call from that.\n\nEach test function in the .py test file represent a scenario of test which is consisted by several steps. For example,\ntest user\'s account page, first, we authenticate the client by post user\'s name and password,\nthen access the account page to verify some values. Each step is described by calling the variable `check`\nwhich is a pytest fixture.\n\n## Tutorial\n### Install\n```bash\npip install pytest-httptesting\n```\n\n### Create test suite\n```python\n# test/test_example.py\nfrom http_testing.assertions import Assertions, NegativeAssertions\nfrom http_testing.cookie import Cookie\nfrom http_testing.page_checker import PageChecker\nfrom http_testing.validators import Regex\n\nhost = "www.google.com"  # mandatory: used in the `check` fixture\nscheme = "https"  # "https" by default\nport = None  # None by default\n\n\ndef test_scenario_one(check: PageChecker):\n    check(\n        title="Senario One",\n        path="/",\n        should_find=Assertions(\n            status_code=200,\n            content=["<title>Google</title>"],\n            headers={"Content-Type": "text/html; charset=ISO-8859-1"},\n            cookies=[Cookie(name="AEC", value=Regex(r".*"))],\n        ),\n        should_not_find=NegativeAssertions(\n            status_code=400,\n            content=["groot"],\n            headers={"nooooo": ""},\n            cookies=[Cookie(name="nop", value="a")],\n        ),\n        timeout=10,  # you can pass additional kwargs to httpx request\n    )\n\n    assert check.previous_response.status_code == 200  # inspect previous response\n```\n\n### Run test\n```bash\n$ pytest test --tb=no --no-header -v  # traceback is disabled because it is not very useful to anayse the functional error\n============= test session starts =============\ncollected 1 item\n\ntest/test_example.py::test_scenario_one PASSED\n\n============= 1 passed in 0.16s =============\n\n```\n\n### Debug\nIn case of error, a temporary file will be generated, as shown in the `short test summary info`. It is a json file concluding\nresponse content, status code, headers and cookies.\n```bash\n$ pytest test --tb=no --no-header -v\n============= test session starts =============\ncollected 1 item\n\ntest/test_example.py::test_scenario_one FAILED\n\n============= short test summary info =============\nFAILED test/test_example.py::test_scenario_one - AssertionError: Senario One - \'Content-Typessss\':\'text/html; charset=ISO-8859-1\' not found in headers on page \'https://www.google.com/\' - please check file \'/tmp/tmptaowd2u5\'\n============= 1 failed in 1.22s =============\n\n```\n\n### Advanced\n#### Customize the http client configuration\nIt is possible to create a fixture `http_client` to create your own http client.\n```python\n@pytest.fixture\ndef http_client():\n    with Client(verify=False, cookies={"cookie_1": "cookie_value_1"}) as client:\n        yield client\n```\n\n#### Customize the base url\nIt is possible to create a fixture `base_url` to override the default construction of base url.\n```python\nfrom httpx import URL\n@pytest.fixture\ndef base_url() -> URL:\n    return URL("https://www.google.com")\n```\n',
     'author': 'HE Qile',
     'author_email': 'mr.qile@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/heqile/http_testing',
```

### Comparing `pytest_httptesting-0.3.0/PKG-INFO` & `pytest_httptesting-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-httptesting
-Version: 0.3.0
+Version: 0.3.1
 Summary: http_testing framework on top of pytest
 Home-page: https://github.com/heqile/http_testing
 Author: HE Qile
 Author-email: mr.qile@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=22.1.0,<23.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Project-URL: Repository, https://github.com/heqile/http_testing
 Description-Content-Type: text/markdown
 
 # HTTP_TESTING
 
 ## Description
```


# Comparing `tmp/adata-0.0.2b0.tar.gz` & `tmp/adata-0.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-0.0.2b0.tar", last modified: Tue Apr 18 15:37:59 2023, max compression
+gzip compressed data, was "adata-0.0.3b0.tar", last modified: Wed Apr 19 16:00:43 2023, max compression
```

## Comparing `adata-0.0.2b0.tar` & `adata-0.0.3b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.206817 adata-0.0.2b0/
--rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.2b0/HISTORY.md
--rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.2b0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.2b0/MANIFEST.in
--rw-rw-rw-   0        0        0     6780 2023-04-18 15:37:59.135762 adata-0.0.2b0/PKG-INFO
--rw-rw-rw-   0        0        0     6141 2023-04-18 15:14:02.000000 adata-0.0.2b0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.088171 adata-0.0.2b0/adata/
--rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.2b0/adata/__init__.py
--rw-rw-rw-   0        0        0      756 2023-04-18 15:34:24.000000 adata-0.0.2b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.100173 adata-0.0.2b0/adata/bond/
--rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/bond/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.2b0/adata/bond/bond_market.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.101174 adata-0.0.2b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.2b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.107762 adata-0.0.2b0/adata/common/headers/
--rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.2b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.2b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.2b0/adata/common/headers/sina_headers.py
--rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.2b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.112762 adata-0.0.2b0/adata/common/utils/
--rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.2b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.2b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0      972 2023-04-05 09:48:28.000000 adata-0.0.2b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.116764 adata-0.0.2b0/adata/etf/
--rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/etf/__init__.py
--rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.2b0/adata/etf/etf_market.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.117793 adata-0.0.2b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.2b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.119763 adata-0.0.2b0/adata/stock/
--rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.120794 adata-0.0.2b0/adata/stock/index/
--rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/stock/index/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.125764 adata-0.0.2b0/adata/stock/info/
--rw-rw-rw-   0        0        0      322 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/info/__init__.py
--rw-rw-rw-   0        0        0     2459 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0     4145 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/info/stock_concept.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.132763 adata-0.0.2b0/adata/stock/market/
--rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/market/__init__.py
--rw-rw-rw-   0        0        0     2644 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/market/stock_dividend.py
--rw-rw-rw-   0        0        0     9479 2023-04-18 15:14:02.000000 adata-0.0.2b0/adata/stock/market/stock_market.py
--rw-rw-rw-   0        0        0     3631 2023-04-18 15:14:02.000000 adata-0.0.2b0/adata/stock/market/stock_market_concept.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.133763 adata-0.0.2b0/adata/stock/sentiment/
--rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/stock/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.096172 adata-0.0.2b0/adata.egg-info/
--rw-rw-rw-   0        0        0     6780 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-04-18 15:37:59.000000 adata-0.0.2b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       69 2023-04-06 11:14:06.000000 adata-0.0.2b0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 15:37:59.206817 adata-0.0.2b0/setup.cfg
--rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.931081 adata-0.0.3b0/
+-rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.3b0/HISTORY.md
+-rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.3b0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.3b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6780 2023-04-19 16:00:43.930106 adata-0.0.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6141 2023-04-18 15:14:02.000000 adata-0.0.3b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.776573 adata-0.0.3b0/adata/
+-rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.3b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-04-19 15:43:41.000000 adata-0.0.3b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.789563 adata-0.0.3b0/adata/bond/
+-rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/bond/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.3b0/adata/bond/bond_market.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.790563 adata-0.0.3b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.3b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.797563 adata-0.0.3b0/adata/common/headers/
+-rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.3b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.3b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.3b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.3b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.907106 adata-0.0.3b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.3b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.3b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0      972 2023-04-19 14:58:23.000000 adata-0.0.3b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.910106 adata-0.0.3b0/adata/etf/
+-rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/etf/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.3b0/adata/etf/etf_market.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.912106 adata-0.0.3b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.3b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.913106 adata-0.0.3b0/adata/stock/
+-rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.915106 adata-0.0.3b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/stock/index/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.919106 adata-0.0.3b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      322 2023-04-13 14:47:15.000000 adata-0.0.3b0/adata/stock/info/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-04-19 14:07:29.000000 adata-0.0.3b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0     4193 2023-04-19 14:07:29.000000 adata-0.0.3b0/adata/stock/info/stock_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.927139 adata-0.0.3b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.3b0/adata/stock/market/__init__.py
+-rw-rw-rw-   0        0        0     2710 2023-04-19 14:07:29.000000 adata-0.0.3b0/adata/stock/market/stock_dividend.py
+-rw-rw-rw-   0        0        0     9769 2023-04-19 15:40:50.000000 adata-0.0.3b0/adata/stock/market/stock_market.py
+-rw-rw-rw-   0        0        0     5740 2023-04-19 15:24:26.000000 adata-0.0.3b0/adata/stock/market/stock_market_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.928107 adata-0.0.3b0/adata/stock/sentiment/
+-rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.3b0/adata/stock/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:00:43.785563 adata-0.0.3b0/adata.egg-info/
+-rw-rw-rw-   0        0        0     6780 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 16:00:43.000000 adata-0.0.3b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2023-04-06 11:14:06.000000 adata-0.0.3b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:00:43.931081 adata-0.0.3b0/setup.cfg
+-rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.3b0/setup.py
```

### Comparing `adata-0.0.2b0/LICENSE` & `adata-0.0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/PKG-INFO` & `adata-0.0.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.2b0
+Version: 0.0.3b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `adata-0.0.2b0/README.md` & `adata-0.0.3b0/README.md`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/adata/__init__.py` & `adata-0.0.3b0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/adata/__version__.py` & `adata-0.0.3b0/adata/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (0, 0, 2)
+VERSION = (0, 0, 3)
 # PRERELEASE = None  # alpha, beta or rc
 PRERELEASE = 'beta'  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
```

### Comparing `adata-0.0.2b0/adata/common/headers/baidu_headers.py` & `adata-0.0.3b0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/adata/common/headers/sina_headers.py` & `adata-0.0.3b0/adata/common/headers/sina_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/adata/common/headers/ths_headers.py` & `adata-0.0.3b0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/adata/common/utils/snowflake.py` & `adata-0.0.3b0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/adata/common/utils/sunrequests.py` & `adata-0.0.3b0/adata/common/utils/sunrequests.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import requests
 
 
 class SunRequests(object):
     def __init__(self) -> None:
         super().__init__()
 
-    def request(self, method='get', url=None, times=3, sleep_time=1111, **kwargs):
+    def request(self, method='get', url=None, times=3, sleep_time=2222, **kwargs):
         """
         简单封装的请求，参考requests，增加循环次数和次数之间的等待时间
         :param method: 请求方法： get；post
         :param url: url
         :param times: 次数，int
         :param sleep_time: 循环的等待时间，毫秒
         :param kwargs: 其它 requests 参数，用法相同
```

### Comparing `adata-0.0.2b0/adata/stock/info/stock_code.py` & `adata-0.0.3b0/adata/stock/info/stock_code.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 @time: 2023/3/28
 @log: change log
 """
 import time
 
 import pandas as pd
 import requests
-
 from tqdm import tqdm
+
 from adata.common.headers import baidu_headers
 
 
 class StockCode(object):
     """
     股票代码
     """
 
     def __init__(self) -> None:
         super().__init__()
 
     def all_code(self):
         """
         获取所有股票的代码
-        :return: 所有股票的代码信息： ['code','name','exchange']
+        :return: 所有股票的代码信息： ['stock_code','short_name','exchange']
         """
         return self.__market_rank_baidu()
 
     def __market_rank_baidu(self):
         """
         获取百度当前涨幅排名的代码
         web： https://gushitong.baidu.com/top/ab-increase-%E6%B6%A8%E5%B9%85%E6%A6%9C
         url：https://finance.pae.baidu.com/selfselect/getmarketrank?sort_type=1&sort_key=14&from_mid=1&pn=0&rn=200&group=pclist&type=ab&finClientType=pc
         其中：pn 起始数 rn 翻页数，最大200
-        :return 代码列表：['code','short_name','exchange']
+        :return 代码列表：['stock_code','short_name','exchange']
         """
         # 1. 请求市场排名的 url
         api_url = f"https://finance.pae.baidu.com/selfselect/getmarketrank" \
                   f"?sort_type=1&sort_key=14&from_mid=1&group=pclist&type=ab&finClientType=pc"
         max_page_size = 200
         data = []
 
@@ -59,12 +59,13 @@
                 code_list = result[0]['DisplayData']['resultData']['tplData']['result']['rank']
                 data.extend(code_list)
             except Exception as e:
                 time.sleep(2)
                 print(e)
                 continue
         # 4. 封装数据
-        return pd.DataFrame(data=data)[['code', 'name', 'exchange']].rename(columns={'name': 'short_name'})
+        rename = {'name': 'short_name', 'code': 'stock_code'}
+        return pd.DataFrame(data=data)[['code', 'name', 'exchange']].rename(columns=rename)
 
 
 if __name__ == '__main__':
     print(StockCode().all_code())
```

### Comparing `adata-0.0.2b0/adata/stock/info/stock_concept.py` & `adata-0.0.3b0/adata/stock/info/stock_concept.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __init__(self) -> None:
         super().__init__()
 
     def all_concept_code_ths(self):
         """
         获取同花顺概念列表：代码和名称
-        :return: 概念[[code,name]]
+        :return: 概念[[concept_code,name]]
         """
         return pd.concat([self.concept_code_ths_pc(), self.concept_code_ths_app()]).reset_index(drop=True)
 
     def concept_code_ths_pc(self):
         """
         获取同花顺的所有概念和概念代码
         web: http://q.10jqka.com.cn/gn/
@@ -45,36 +45,36 @@
             data = []
             for a in soup.find_all('a'):
                 href = str(a['href'])
                 if href.startswith(api_url + 'detail/code/'):
                     data.append([href[-7: -1], a.string, href])
 
             # 4. 封装数据
-            data_df = pd.DataFrame(data=data, columns=['code', 'name', 'href'])[['code', 'name']]
+            data_df = pd.DataFrame(data=data, columns=['concept_code', 'name', 'href'])[['concept_code', 'name']]
             data_df['source'] = '同花顺PC'
             return data_df
 
     def concept_code_ths_app(self):
         """
         获取app的概率列表，通过问财询问得到结果
-        :return: app的概念列表： code，name
+        :return: app的概念列表： concept_code，name
         """
         data = []
         for i in range(1, 10):
             api_url = f"http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?perpage=100&page={i}&query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119"
             res = requests.request('get', url=api_url, headers=ths_headers.c_headers)
             res_json = res.json()
             if res_json['status_msg'] == 'ok':
                 data_list = res_json['answer']['components'][0]['data']['datas']
                 if len(data_list) < 1:
                     break
                 for d in data_list:
                     data.append([d['code'], d['指数简称']])
-        data_df = pd.DataFrame(data=data, columns=['code', 'name']).drop_duplicates(keep='first', inplace=False,
-                                                                                    ignore_index=False)
+        data_df = pd.DataFrame(data=data, columns=['concept_code', 'name']).drop_duplicates(keep='first', inplace=False,
+                                                                                            ignore_index=False)
         data_df['source'] = '同花顺APP'
         return data_df
 
 
 if __name__ == '__main__':
     print(StockConcept().all_concept_code_ths())
     print(StockConcept().concept_code_ths_pc())
```

### Comparing `adata-0.0.2b0/adata/stock/market/stock_dividend.py` & `adata-0.0.3b0/adata/stock/market/stock_dividend.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,33 +18,33 @@
     """
     股票分红
     """
 
     def __init__(self) -> None:
         super().__init__()
 
-    def get_dividend(self, code='000001'):
+    def get_dividend(self, stock_code='000001'):
         """
         获取当个股票的分红信息
-        :param code: 股票代码
+        :param stock_code: 股票代码
         :return: 股票分红信息
         """
-        return self.__dividend_baidu(code)
+        return self.__dividend_baidu(stock_code)
 
-    def __dividend_baidu(self, code):
+    def __dividend_baidu(self, stock_code):
         """
         获取百度的股票分红数据：公告日；分红方案；除权除息日
         web： https://gushitong.baidu.com/stock/ab-300033
         url： https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&client=app&query=300033&code=300033&word=300033&resource_id=5429&ma_ver=4&finClientType=pc
-        :param code: 6位股票代码
+        :param stock_code: 6位股票代码
         :return: 股票分红信息
         """
         # 1.请求接口 url
         api_url = f"https://gushitong.baidu.com/opendata?openapi=1&dspName=iphone&tn=tangram&client=app&" \
-                  f"query={code}&code={code}&word={code}&resource_id=5429&ma_ver=4&finClientType=pc"
+                  f"query={stock_code}&code={stock_code}&word={stock_code}&resource_id=5429&ma_ver=4&finClientType=pc"
         res = requests.request('get', api_url, headers=baidu_headers.text_headers)
 
         # 2. 判断结果是否正确
         if len(res.text) < 1 or res.status_code != 200:
             return pd.DataFrame()
         res_json = res.json()
         if res_json['ResultCode'] != '0':
@@ -60,14 +60,14 @@
             'newCompany']
         bonus_transfer = new_company['bonusTransfer']
         header = bonus_transfer['header']
         body = bonus_transfer['body']
 
         # 4. 封装数据
         result_df = pd.DataFrame(data=body, columns=header)[['公告日', '分红方案', '除权除息日']]
-        result_df['code'] = code
+        result_df['stock_code'] = stock_code
         rename_columns = {'公告日': 'report_date', '分红方案': 'dividend_plan', '除权除息日': 'ex_dividend_date'}
         return result_df.rename(columns=rename_columns)
 
 
 if __name__ == '__main__':
-    print(StockDividend().get_dividend(code='000001'))
+    print(StockDividend().get_dividend(stock_code='000001'))
```

### Comparing `adata-0.0.2b0/adata/stock/market/stock_market.py` & `adata-0.0.3b0/adata/stock/market/stock_market.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,63 +18,63 @@
     """
     股票行情
     """
 
     def __init__(self) -> None:
         super().__init__()
 
-    def get_market(self, code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
+    def get_market(self, stock_code: str = '000001', start_date='1990-01-01', k_type=1, adjust_type: int = 1):
         """
         获取单个股票的行情
-        :param code: 股票代码
+        :param stock_code: 股票代码
         :param start_date: 开始时间
         :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
         :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 （目前：只有前复权,作为股票交易已经可用）
         :return: k线行情数据
         """
-        return self.__market_baidu(code, start_date, k_type)
+        return self.__market_baidu(stock_code, start_date, k_type)
 
-    def get_market_min(self, code: str = '000001'):
+    def get_market_min(self, stock_code: str = '000001'):
         """
         获取单个股票的今日分时行情
-        :param code: 股票代码
+        :param stock_code: 股票代码
         :return: 当日分钟行情数据
         """
-        return self.__market_baidu_today_min(code)
+        return self.__market_baidu_today_min(stock_code)
 
     def list_market_current(self, code_list=None):
         """
         获取多个股票最新行情信息
         :param code_list: 股票代码
         :return: 当前最新的行情价格信息
         """
         if code_list is None:
             return pd.DataFrame()
         return self.__market_sina_current(code_list=code_list)
 
-    def __market_baidu(self, code, start_date, k_type=1):
+    def __market_baidu(self, stock_code, start_date, k_type=1):
         """
         获取百度的股票行情数据
         web： https://gushitong.baidu.com/stock/ab-002926
         url：quotation_fiveday_ab 5日分时，quotation_kline_ab K线， quotation_minute_ab 当日分钟
         k线
         https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_kline_ab&finClientType=pc&code=002926&start_time=2018-02-05 00:00:00&ktype=1
         分钟
         https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_minute_ab&finClientType=pc
         "ma5均价","ma5成交量","ma10均价","ma10成交量","ma20均价","ma20成交量"
-        :param code: 6位股票代码
+        :param stock_code: 6位股票代码
         :param start_date: 开始时间
         :param k_type: k线类型：1.日；2.周；3.月
         # :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权 TODO
         :return: k线行情数据:"时间戳", "时间","开盘","收盘","成交量","最高","最低","成交额","涨跌额","涨跌幅","换手率","昨收"
         """
         # 1. 请求接口 url
         api_url = f"https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&" \
                   f"isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_kline_ab&finClientType=pc&" \
-                  f"code={code}&start_time={start_date} 00:00:00&ktype={k_type}"
+                  f"code={stock_code}&start_time={start_date} 00:00:00&ktype={k_type}"
 
         res_json = None
         for i in range(3):
             res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
             # 2. 校验请求结果数据
             res_json = res.json()
             if res_json['ResultCode'] == '0':
@@ -96,31 +96,32 @@
 
         # 4. 封装数据
         field = ['time', 'open', 'close', 'volume', 'high', 'low', 'amount', 'range', 'ratio', 'turnoverratio',
                  'preClose']
         rename_columns = {'turnoverratio': 'turnover_ratio', 'preClose': 'pre_close', 'range': 'change',
                           'ratio': 'change_pct', 'time': 'trade_time'}
         result_df = pd.DataFrame(data=data, columns=keys)[field].rename(columns=rename_columns)
+        result_df['stock_code'] = stock_code
         result_df['trade_date'] = result_df['trade_time']
-        result_df['trade_time'] = pd.to_datetime(result_df['trade_time'])
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime('%Y-%m-%d %H:%M:%S')
         return result_df
 
-    def __market_baidu_today_min(self, code):
+    def __market_baidu_today_min(self, stock_code):
         """
         获取百度的股票行情数据
         web： https://gushitong.baidu.com/stock/ab-002926
         url: https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_minute_ab&finClientType=pc
         time, price, ratio, increase, volume, avgPrice, amount, timeKey, datetime, oriAmount
-        :param code: 6位股票代码
+        :param stock_code: 6位股票代码
         :return: k线行情数据:"时间","价格","涨跌率","涨幅","均价","成交量", "成交额"
         """
         # 1. 请求接口 url
         api_url = f"https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&isIndex=false&isBk=false&" \
                   f"isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_minute_ab&finClientType=pc&" \
-                  f"code={code}"
+                  f"code={stock_code}"
 
         res_json = None
         for i in range(3):
             res = requests.request('get', api_url, headers=baidu_headers.json_headers, proxies={})
             # 2. 校验请求结果数据
             res_json = res.json()
             if res_json['ResultCode'] == '0':
@@ -138,21 +139,22 @@
         # 4. 封装数据
         field = ['time', 'price', 'ratio', 'increase', 'volume', 'avgPrice', 'amount', 'timeKey', 'datetime',
                  'oriAmount']
         rename_columns = {'avgPrice': 'avg_price', 'oriAmount': 'ori_amount', 'ratio': 'change_pct',
                           'increase': 'change'}
         result_df = pd.DataFrame(data=market_data_list, columns=field).rename(columns=rename_columns)
         result_df['amount'] = result_df['ori_amount']
-        result_df['code'] = code
+        result_df['stock_code'] = stock_code
         # 这里是分钟均价，数据存在四舍五入的情况
         result_df['volume'] = result_df['volume'].astype(int) * 100
-        result_df['trade_time'] = pd.to_datetime(result_df['time'], unit='s').dt.tz_localize('UTC').dt.tz_convert(
+        result_df['trade_time'] = pd.to_datetime(result_df['time'], unit='s', utc=True).dt.tz_convert(
             'Asia/Shanghai')
-        result_df['trade_date'] = result_df['trade_time'].dt.date
-        return result_df[['code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']]
+        result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime("%Y-%m-%d %H:%M:%S")
+        result_df['trade_date'] = result_df['trade_time'].str[:10]
+        return result_df[['stock_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']]
 
     def __market_sina_current(self, code_list):
         """
         获取新浪的最新股票行情
         url : https://hq.sinajs.cn/list=s_sh600905,s_sz000725,s_sz000100,s_sh601919
         :param code_list:  代码列表
         :return: 最新行情数据：代码,简称,当前价格(元),涨跌额(元),涨跌幅(%),成交量(股),成交额(元)
@@ -184,20 +186,20 @@
             idx = data_str.index('=')
             code = [data_str[idx - 6:idx]]
             code.extend(data_str[idx + 2:-1].split(','))
             if len(code) == 7:
                 data.append(code)
 
         # 4. 封装数据
-        columns = ['code', 'short_name', 'price', 'change', 'change_pct', 'volume', 'amount']
+        columns = ['stock_code', 'short_name', 'price', 'change', 'change_pct', 'volume', 'amount']
         result_df = pd.DataFrame(data=data, columns=columns)
         # 北京的单位是股和万元
-        mask = result_df['code'].str.startswith(('0', '3', '6', '9'))
+        mask = result_df['stock_code'].str.startswith(('0', '3', '6', '9'))
         result_df.loc[mask, 'volume'] = result_df['volume'].astype(int) * 100
         result_df.loc[mask, 'amount'] = result_df['amount'].astype(float) * 10000
         return result_df
 
 
 if __name__ == '__main__':
-    print(StockMarket().get_market(code='000001', start_date='2021-01-01', k_type=1))
-    print(StockMarket().get_market_min(code='000001'))
+    print(StockMarket().get_market(stock_code='000001', start_date='2021-01-01', k_type=1))
+    print(StockMarket().get_market_min(stock_code='000001'))
     print(StockMarket().list_market_current(code_list=['000001', '600001', '000795', '872925']))
```

### Comparing `adata-0.0.2b0/adata.egg-info/PKG-INFO` & `adata-0.0.3b0/adata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.2b0
+Version: 0.0.3b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `adata-0.0.2b0/adata.egg-info/SOURCES.txt` & `adata-0.0.3b0/adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adata-0.0.2b0/setup.py` & `adata-0.0.3b0/setup.py`

 * *Files identical despite different names*


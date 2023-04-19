# Comparing `tmp/enular-0.2.3.tar.gz` & `tmp/enular-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enular-0.2.3.tar", last modified: Fri Sep  2 11:51:29 2022, max compression
+gzip compressed data, was "enular-1.0.0.tar", last modified: Wed Apr 19 14:35:00 2023, max compression
```

## Comparing `enular-0.2.3.tar` & `enular-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 adriancpwong   (501) staff       (20)        0 2022-09-02 11:51:29.854200 enular-0.2.3/
--rw-r--r--   0 adriancpwong   (501) staff       (20)     2688 2022-09-02 11:51:29.853826 enular-0.2.3/PKG-INFO
--rw-r--r--   0 adriancpwong   (501) staff       (20)     1641 2022-09-02 11:50:35.000000 enular-0.2.3/README.md
-drwxr-xr-x   0 adriancpwong   (501) staff       (20)        0 2022-09-02 11:51:29.850261 enular-0.2.3/enular/
--rwxr-xr-x   0 adriancpwong   (501) staff       (20)      231 2022-09-02 11:50:48.000000 enular-0.2.3/enular/__init__.py
--rw-r--r--   0 adriancpwong   (501) staff       (20)      736 2022-09-02 11:50:48.000000 enular-0.2.3/enular/_analyzers.py
--rwxr-xr-x   0 adriancpwong   (501) staff       (20)     4093 2022-07-29 15:11:20.000000 enular-0.2.3/enular/base.py
-drwxr-xr-x   0 adriancpwong   (501) staff       (20)        0 2022-09-02 11:51:29.853147 enular-0.2.3/enular.egg-info/
--rw-r--r--   0 adriancpwong   (501) staff       (20)     2688 2022-09-02 11:51:29.000000 enular-0.2.3/enular.egg-info/PKG-INFO
--rw-r--r--   0 adriancpwong   (501) staff       (20)      222 2022-09-02 11:51:29.000000 enular-0.2.3/enular.egg-info/SOURCES.txt
--rw-r--r--   0 adriancpwong   (501) staff       (20)        1 2022-09-02 11:51:29.000000 enular-0.2.3/enular.egg-info/dependency_links.txt
--rw-r--r--   0 adriancpwong   (501) staff       (20)       11 2022-09-02 11:51:29.000000 enular-0.2.3/enular.egg-info/requires.txt
--rw-r--r--   0 adriancpwong   (501) staff       (20)        7 2022-09-02 11:51:29.000000 enular-0.2.3/enular.egg-info/top_level.txt
--rw-r--r--   0 adriancpwong   (501) staff       (20)       38 2022-09-02 11:51:29.854332 enular-0.2.3/setup.cfg
--rwxr-xr-x   0 adriancpwong   (501) staff       (20)     1302 2022-09-02 11:51:13.000000 enular-0.2.3/setup.py
+drwxr-xr-x   0 adriancpwong   (501) staff       (20)        0 2023-04-19 14:35:00.744188 enular-1.0.0/
+-rw-r--r--   0 adriancpwong   (501) staff       (20)     2693 2023-04-19 14:35:00.743843 enular-1.0.0/PKG-INFO
+-rw-r--r--   0 adriancpwong   (501) staff       (20)     1646 2023-04-19 14:33:35.000000 enular-1.0.0/README.md
+drwxr-xr-x   0 adriancpwong   (501) staff       (20)        0 2023-04-19 14:35:00.741878 enular-1.0.0/enular/
+-rwxr-xr-x   0 adriancpwong   (501) staff       (20)      163 2023-02-09 02:56:29.000000 enular-1.0.0/enular/__init__.py
+-rw-r--r--   0 adriancpwong   (501) staff       (20)      739 2023-01-12 12:53:31.000000 enular-1.0.0/enular/_analyzers.py
+-rwxr-xr-x   0 adriancpwong   (501) staff       (20)     4063 2023-02-10 13:50:52.000000 enular-1.0.0/enular/base.py
+-rwxr-xr-x   0 adriancpwong   (501) staff       (20)     4161 2023-02-08 23:15:36.000000 enular-1.0.0/enular/fixes.py
+drwxr-xr-x   0 adriancpwong   (501) staff       (20)        0 2023-04-19 14:35:00.743396 enular-1.0.0/enular.egg-info/
+-rw-r--r--   0 adriancpwong   (501) staff       (20)     2693 2023-04-19 14:35:00.000000 enular-1.0.0/enular.egg-info/PKG-INFO
+-rw-r--r--   0 adriancpwong   (501) staff       (20)      238 2023-04-19 14:35:00.000000 enular-1.0.0/enular.egg-info/SOURCES.txt
+-rw-r--r--   0 adriancpwong   (501) staff       (20)        1 2023-04-19 14:35:00.000000 enular-1.0.0/enular.egg-info/dependency_links.txt
+-rw-r--r--   0 adriancpwong   (501) staff       (20)       11 2023-04-19 14:35:00.000000 enular-1.0.0/enular.egg-info/requires.txt
+-rw-r--r--   0 adriancpwong   (501) staff       (20)        7 2023-04-19 14:35:00.000000 enular-1.0.0/enular.egg-info/top_level.txt
+-rw-r--r--   0 adriancpwong   (501) staff       (20)       38 2023-04-19 14:35:00.744323 enular-1.0.0/setup.cfg
+-rwxr-xr-x   0 adriancpwong   (501) staff       (20)     1302 2023-04-19 14:32:50.000000 enular-1.0.0/setup.py
```

### Comparing `enular-0.2.3/PKG-INFO` & `enular-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: enular
-Version: 0.2.3
+Version: 1.0.0
 Summary: Enular Library
 Home-page: https://enular.com
 Author: Adrian Chun Pang Wong, Dylan Fitzsimmons, Enular Limited
 Author-email: adrian@enular.com
 License: MIT
 Description: # Enular Library
          
         pip install enular
         
-        NOTE: Pre-alpha version (v0.2.3) and development in progress. Expect beta release in late 2022.
+        NOTE: Alpha version (v1.0.0) and development in progress. Expect beta release in late 2023.
         
         The Enular Library contains tools for backtesting, evaluating and visualising algorithmic trading strategies. It allows the user to easily combine indicators with complex operations into strategies, similar to neural networks. It also provides indicators, data sources, and paper trading capabilities. Documentation coming soon. Enular.com
         
         Details:
-        - Uses Backtrader's Cerebro engine with fixes from Backtrader2
+        - Uses parts of Backtrader's Cerebro engine with fixes from Backtrader2
         - Data streaming from Yahoo Finance
         - Indicator and strategy collection
         - Improve accessiblity with simplified architecture
         - Highly scalable strategies: extend classes and redefine trade logic
         - Live trading capabilities
         
         Architecture:
```

### Comparing `enular-0.2.3/README.md` & `enular-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Enular Library
  
 pip install enular
 
-NOTE: Pre-alpha version (v0.2.3) and development in progress. Expect beta release in late 2022.
+NOTE: Alpha version (v1.0.0) and development in progress. Expect beta release in late 2023.
 
 The Enular Library contains tools for backtesting, evaluating and visualising algorithmic trading strategies. It allows the user to easily combine indicators with complex operations into strategies, similar to neural networks. It also provides indicators, data sources, and paper trading capabilities. Documentation coming soon. Enular.com
 
 Details:
-- Uses Backtrader's Cerebro engine with fixes from Backtrader2
+- Uses parts of Backtrader's Cerebro engine with fixes from Backtrader2
 - Data streaming from Yahoo Finance
 - Indicator and strategy collection
 - Improve accessiblity with simplified architecture
 - Highly scalable strategies: extend classes and redefine trade logic
 - Live trading capabilities
 
 Architecture:
```

### Comparing `enular-0.2.3/enular/_analyzers.py` & `enular-1.0.0/enular/_analyzers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import os
 import sys
 
 import backtrader as bt
-from enular.base import *
+from enularlib.base import *
 
 class Screener_SMA(Analyzer):
     params = (('period',20), ('devfactor',2),)
 
     def start(self):
         self.bband = {data: bt.indicators.BollingerBands(data,
                 period=self.params.period, devfactor=self.params.devfactor)
```

### Comparing `enular-0.2.3/enular/base.py` & `enular-1.0.0/enular/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,37 @@
 from __future__ import (absolute_import, division, print_function, unicode_literals)
+from backtrader import backtrader as bt
+#import backtrader as bt
 
-#!/usr/bin/env python
-import os
-import io
-import sys
-
-from datetime import date, datetime
-import matplotlib
-import yfinance as yf
-import numpy
-import scipy
-import sklearn
-import pandas
-import backtrader as bt
-import webbrowser
-import quantstats
 
 #Dependencies for Yahoo data streamer
 from backtrader.utils.py3 import (urlopen, urlquote, ProxyHandler, build_opener, install_opener)
-import collections
-import itertools
 from backtrader import feed
 from backtrader.utils import date2num
 
+from . import qslib
+
 if __name__ == '__main__':
     print ('Do not run this file.')
 
 #CORE
 
 class Cerebro(bt.Cerebro):  
     
-    def quantstats(self, results):
+    def quantstats(self, results, qsids):
             strat = results[0]
             portfolio_stats = strat.analyzers.getbyname('PyFolio')
             returns, positions, transactions, gross_lev = portfolio_stats.get_pf_items()
             returns.index = returns.index.tz_convert(None)
-            quantstats.reports.html(returns, output='stats.html', title='BTC Sentiment', download_filename='stats.html')
-            webbrowser.open('file://' + os.path.realpath('stats.html'))
+
+            qsids_output = qsids + 'stats.html'
+            qsids_download_filename = '/home/ubuntu/django/Enular/templates/stats/' + qsids + 'stats.html'
+
+            qslib.reports.html(returns, output=qsids_output, title='Results', download_filename=qsids_download_filename)
+            #webbrowser.open('file://' + os.path.realpath('stats.html'))
 
 class Dummy(bt.Indicator):    
     
     lines = ('dummy',)
 
     def next(self):
         self.lines.dummy[0] = 0.0
```

### Comparing `enular-0.2.3/enular.egg-info/PKG-INFO` & `enular-1.0.0/enular.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: enular
-Version: 0.2.3
+Version: 1.0.0
 Summary: Enular Library
 Home-page: https://enular.com
 Author: Adrian Chun Pang Wong, Dylan Fitzsimmons, Enular Limited
 Author-email: adrian@enular.com
 License: MIT
 Description: # Enular Library
          
         pip install enular
         
-        NOTE: Pre-alpha version (v0.2.3) and development in progress. Expect beta release in late 2022.
+        NOTE: Alpha version (v1.0.0) and development in progress. Expect beta release in late 2023.
         
         The Enular Library contains tools for backtesting, evaluating and visualising algorithmic trading strategies. It allows the user to easily combine indicators with complex operations into strategies, similar to neural networks. It also provides indicators, data sources, and paper trading capabilities. Documentation coming soon. Enular.com
         
         Details:
-        - Uses Backtrader's Cerebro engine with fixes from Backtrader2
+        - Uses parts of Backtrader's Cerebro engine with fixes from Backtrader2
         - Data streaming from Yahoo Finance
         - Indicator and strategy collection
         - Improve accessiblity with simplified architecture
         - Highly scalable strategies: extend classes and redefine trade logic
         - Live trading capabilities
         
         Architecture:
```

### Comparing `enular-0.2.3/setup.py` & `enular-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="enular",
-    version="0.2.3",
+    version="1.0.0",
     description="Enular Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://enular.com",
     author="Adrian Chun Pang Wong, Dylan Fitzsimmons, Enular Limited",
     author_email="adrian@enular.com",
     license="MIT",
```


# Comparing `tmp/pyBCV-1.0.2-py3-none-any.whl.zip` & `tmp/pyBCV-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4622 bytes, number of entries: 7
+Zip file size: 4579 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-02 04:16 pyBCV/__init__.py
--rw-rw-rw-  2.0 fat     4277 b- defN 23-Apr-04 01:33 pyBCV/pyBCV.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Apr-04 01:38 pyBCV-1.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4485 b- defN 23-Apr-04 01:38 pyBCV-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-04 01:38 pyBCV-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-04 01:38 pyBCV-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      518 b- defN 23-Apr-04 01:38 pyBCV-1.0.2.dist-info/RECORD
-7 files, 10497 bytes uncompressed, 3708 bytes compressed:  64.7%
+-rw-rw-rw-  2.0 fat     3527 b- defN 23-Apr-19 18:41 pyBCV/pyBCV.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4473 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      518 b- defN 23-Apr-19 18:50 pyBCV-1.0.3.dist-info/RECORD
+7 files, 9735 bytes uncompressed, 3665 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pyBCV/__init__.py
 Comment: 
 
 Filename: pyBCV/pyBCV.py
 Comment: 
 
-Filename: pyBCV-1.0.2.dist-info/LICENSE
+Filename: pyBCV-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyBCV-1.0.2.dist-info/METADATA
+Filename: pyBCV-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pyBCV-1.0.2.dist-info/WHEEL
+Filename: pyBCV-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyBCV-1.0.2.dist-info/top_level.txt
+Filename: pyBCV-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyBCV-1.0.2.dist-info/RECORD
+Filename: pyBCV-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyBCV/pyBCV.py

```diff
@@ -1,101 +1,85 @@
+from typing import Any
+
 import requests
 from bs4 import BeautifulSoup
 
 requests.packages.urllib3.disable_warnings()
 
 class Currency:
-    def get_rate(self, currency_code=None):
-        webSite = 'https://www.bcv.org.ve/'
-        webResult = requests.get(webSite, verify=False)
-
-        if webResult.status_code == 200: # OK!
-            dataWeb = BeautifulSoup(webResult.content, 'html.parser')
-
-            label_html = dataWeb.find_all('div', 'col-sm-12 col-xs-12')
-            label_html_date = dataWeb.find('div', 'pull-right dinpro center')
-            priceResult = []
-            dateValid = []
-
-            for i in label_html:
-                x = i.find('strong')
-                priceResult.append(x.text.strip().replace(',', '.'))
-            
-            for z in label_html_date:
-                dateValid.append(z.text.strip())
+    def get_rate(self, currency_code=None) -> dict[str, str] | str:
+        response = requests.get('https://www.bcv.org.ve/', verify=False)
+
+        if response.status_code == requests.codes.ok:
+            soup = BeautifulSoup(response.content, 'html.parser')
+
+            rates_of_cambie = []
+            date_valid = []
+
+            for i in soup.find_all('div', 'col-sm-12 col-xs-12'):
+                rates_of_cambie.append(i.find('strong').text.strip().replace(',', '.'))
+            for x in soup.find('div', 'pull-right dinpro center'):
+                date_valid.append(x.text.strip())
 
             rates = {
-                'EUR' : f'Bs. {round(float(priceResult[-5]), 2)}',
-                'CNY' : f'Bs. {round(float(priceResult[-4]), 2)}',
-                'TRY' : f'Bs. {round(float(priceResult[-3]), 2)}',
-                'RUB' : f'Bs. {round(float(priceResult[-2]), 2)}',
-                'USD' : f'Bs. {round(float(priceResult[-1]), 2)}',
-                'DATE' : f'{dateValid[0]} {dateValid[1]}'
+                'EUR': f'Bs. {rates_of_cambie[-5]}',
+                'CNY': f'Bs. {rates_of_cambie[-4]}',
+                'TRY': f'Bs. {rates_of_cambie[-3]}',
+                'RUB': f'Bs. {rates_of_cambie[-2]}',
+                'USD': f'Bs. {rates_of_cambie[-1]}',
+                date_valid[0].replace(':', ''): date_valid[1].replace('  ', ' ')
             }
 
             if not currency_code:
                 return rates
-
+            
             elif currency_code in rates:
                 return rates[currency_code]
-            
     
-    def get_by_bank(self, bank_code=None, rate_or_sale=None):
-        webSite = 'https://www.bcv.org.ve/tasas-informativas-sistema-bancario'
-        webResult = requests.get(webSite, verify=False)
-
-        if webResult.status_code == 200: #OK!
-            dataWeb = BeautifulSoup(webResult.content, 'html.parser')
-
-            label_html_date = dataWeb.find_all('td', 'views-field views-field-field-fecha-del-indicador')
-            label_html_bank = dataWeb.find_all('td', 'views-field views-field-views-conditional')
-            label_html_ratebuys = dataWeb.find_all('td', 'views-field views-field-field-tasa-compra')
-            label_html_ratesales = dataWeb.find_all('td', 'views-field views-field-field-tasa-venta')
-
-            dateIndicator = []
-            titleBank = []
-            rateBuys = []
-            rateSales = []
-
-            for w in label_html_date:
-                dateIndicator.append(w.text.strip())
-            for x in label_html_bank:
-                titleBank.append(x.text.strip())
-            for y in label_html_ratebuys:
-                rateBuys.append(y.text.strip().replace(',', '.'))
-            for z in label_html_ratesales:
-                rateSales.append(z.text.strip().replace(',', '.'))
-
-            titleBank[3] = titleBank[3].replace('é', 'e')
-
+class Bank:
+    def get_by_bank(self, bank_code=None, rate_or_sale=None) -> dict[Any, dict[str, str]] | str | dict[str, str]:
+        response = requests.get('https://www.bcv.org.ve/tasas-informativas-sistema-bancario', verify=False)
+
+        if response.status_code == requests.codes.ok:
+            soup = BeautifulSoup(response.content, 'html.parser')
+
+            date_indicator = []
+            title_bank = []
+            rate_buys = []
+            rate_sales = []
+
+            for i in soup.find_all('td', 'views-field views-field-field-fecha-del-indicador'):
+                date_indicator.append(i.text.strip())
+            for j in soup.find_all('td', 'views-field views-field-views-conditional'):
+                title_bank.append(j.text.strip())
+            for k in soup.find_all('td', 'views-field views-field-field-tasa-compra'):
+                rate_buys.append(k.text.strip().replace(',', '.'))
+            for e in soup.find_all('td', 'views-field views-field-field-tasa-venta'):
+                rate_sales.append(e.text.strip().replace(',', '.'))
+            
             bank = {
-                titleBank[0]: {
-                'Fecha' : f'{dateIndicator[0]}',
-                'Compra' : f'Bs. {round(float(rateBuys[0]), 2)}',
-                'Venta' : f'Bs. {round(float(rateSales[0]), 2)}'
-                },
-                titleBank[1]: {
-                'Fecha' : f'{dateIndicator[1]}',
-                'Compra' : f'Bs. {round(float(rateBuys[1]), 2)}',
-                'Venta' : f'Bs. {round(float(rateSales[1]), 2)}'
+                title_bank[0]: {
+                'Fecha': date_indicator[0],
+                'Compra': f'Bs. {rate_buys[0]}',
+                'Venta': f'Bs. {rate_sales[0]}'
                 },
-                titleBank[2]: {
-                'Fecha' : f'{dateIndicator[2]}',
-                'Compra' : f'Bs. {round(float(rateBuys[2]), 2)}',
-                'Venta' : f'Bs. {round(float(rateSales[2]), 2)}'
+                title_bank[1]: {
+                'Fecha': date_indicator[1],
+                'Compra': f'Bs. {rate_buys[1]}',
+                'Venta': f'Bs. {rate_sales[1]}'
                 },
-                titleBank[3]: {
-                'Fecha' : f'{dateIndicator[3]}',
-                'Compra' : f'Bs. {round(float(rateBuys[3]), 2)}',
-                'Venta' : f'Bs. {round(float(rateSales[3]), 2)}'
+                title_bank[2]: {
+                'Fecha': date_indicator[2],
+                'Compra': f'Bs. {rate_buys[2]}',
+                'Venta': f'Bs. {rate_sales[2]}'
                 },
-                titleBank[4]: {
-                'Fecha' : f'{dateIndicator[4]}',
-                'Compra' : f'Bs. {round(float(rateBuys[4]), 2)}',
-                'Venta' : f'Bs. {round(float(rateSales[4]), 2)}'
+                title_bank[3]: {
+                'Fecha': date_indicator[2],
+                'Compra': f'Bs. {rate_buys[2]}',
+                'Venta': f'Bs. {rate_sales[3]}'
                 },
             }
             
             if not bank_code:
                 return bank
 
             elif rate_or_sale in bank[bank_code]:
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `pyBCV-1.0.2.dist-info/LICENSE` & `pyBCV-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBCV-1.0.2.dist-info/METADATA` & `pyBCV-1.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBCV
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y las tasas informativas proporcionados por el Banco Central de Venezuela (BCV).
 Home-page: https://github.com/fcoagz/pyBCV
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pyBCV
 Project-URL: Bug Tracker, https://github.com/fcoagz/pyBCV/issues
@@ -33,75 +33,77 @@
 ```
 Si usas un Sistema Operativo como Linux o Mac:
 ```py
 pip3 install pyBCV
 ```
 
 ## Uso
-Para obtener información del BCV, creamos una instancia de la clase `Currency` y elegimos el módulo que deseamos utilizar para obtener la información. En pyBCV, los módulos disponibles son:
+Para obtener información del BCV, creamos una instancia de la clase `Currency` o `Bank` y elegimos el módulo que deseamos utilizar para obtener la información. En pyBCV, los módulos disponibles son:
 
-- get_rate(): Obtiene la tasa de cambio actual de una moneda específica.
-- get_by_bank(): Obtiene la fecha vigente y el sistema cambiario de compra y venta de moneda extranjera para un banco específico.
+- Currency().get_rate(): Obtiene la tasa de cambio actual de una moneda específica.
+- Bank().get_by_bank(): Obtiene la fecha vigente y el sistema cambiario de compra y venta de moneda extranjera para un banco específico.
 
 A continuación te digo como se utiliza estos módulos:
 ### Módulo **get_rate()**
 ___
 El módulo `get_rate()` acepta un código de moneda como argumento y devuelve la tasa de cambio actual de esa moneda.
 ```py
 import pyBCV
 
 bcv = pyBCV.Currency()
 
 tasa_usd = bcv.get_rate('USD')
 print(tasa_usd)
 
->> 'Bs. 24.53'
+>> 'Bs. 24.56330000'
 ```
 Para obtener una estructura tipo JSON de las monedas disponibles en pyBCV, utilizamos el módulo get_rate() sin argumentos, el cual devuelve un diccionario.
 ```py
 import pyBCV
 
 bcv = pyBCV.Currency()
 
 tasa_de_cambio = bcv.get_rate()
 print(tasa_de_cambio)
 
->> {'EUR': 'Bs. 26.65', 'CNY': 'Bs. 3.57', 'TRY': 'Bs. 1.28', 'RUB': 'Bs. 0.32', 'USD': 'Bs. 24.53'}
+>> {'EUR': 'Bs. 26.92555256', 'CNY': 'Bs. 3.57247989', 'TRY': 'Bs. 1.26605811', 'RUB': 'Bs. 0.30064870', 'USD': 'Bs. 24.56330000'}
 ```
 
 ### Módulo **get_by_bank()**
 ___
 El módulo `get_by_bank()` acepta el nombre de un banco como argumento y devuelve la fecha vigente y el sistema cambiario de compra y venta de moneda extranjera para ese banco.
 ```py
 import pyBCV
 
-bcv = pyBCV.Currency()
+bcv = pyBCV.Bank()
 
 banco = bcv.get_by_bank('Bancamiga')
 print(banco)
 
->> {'Fecha': '31-03-2023', 'Compra': 'Bs. 24.50', 'Venta': 'Bs. 24.55'}
+>> {'Fecha': '18-04-2023', 'Compra': 'Bs. 24.5275', 'Venta': 
+'Bs. 24.5991'}
 ``` 
 Para acceder a una sola propiedad. El módulo `get_by_bank()` acepta el nombre de un banco como primer argumento y el nombre de una propiedad como segundo argumento (por ejemplo: "Fecha") y devuelve el valor de esa propiedad para el banco especificado.
 ```py
 import pyBCV
 
-bcv = pyBCV.Currency()
+bcv = pyBCV.Bank()
 
 banco = bcv.get_by_bank('Bancamiga', 'Fecha')
 print(banco)
 
->> '31-03-2023'
+>> '18-04-2023'
 ``` 
 Si queremos obtener una estructura tipo JSON de los bancos disponibles en pyBCV, utilizamos el módulo `get_by_bank()` sin argumentos.
 ```py
 import pyBCV
 
-bcv = pyBCV.Currency()
+bcv = pyBCV.Bank()
 
 bancos = bcv.get_by_bank()
 print(bancos)
 
->> {'Bancamiga': {'Fecha': '31-03-2023', 'Compra': 'Bs. 24.5', 'Venta': 'Bs. 24.55'}, 'Banco Nacional de Crédito BNC': {'Fecha': '31-03-2023', 'Compra': 'Bs. 24.46', 'Venta': 'Bs. 24.64'}, 'BBVA Provincial': {'Fecha': '31-03-2023', 'Compra': 'Bs. 24.33', 'Venta': 'Bs. 24.45'}, 'Banesco': {'Fecha': '31-03-2023', 'Compra': 'Bs. 24.36', 'Venta': 'Bs. 24.54'}, 'Banco Mercantil': {'Fecha': '31-03-2023', 'Compra': 'Bs. 24.41', 'Venta': 'Bs. 24.5'}}
+>> {'Banco Nacional de Crédito BNC': {'Fecha': '18-04-2023', 'Compra': 'Bs. 24.3989', 'Venta': 'Bs. 24.4180'}, 'Bancamiga': {'Fecha': '18-04-2023', 'Compra': 'Bs. 24.5275', 'Venta': 
+'Bs. 24.5991'}, 'Banesco': {'Fecha': '18-04-2023', 'Compra': 'Bs. 24.5685', 'Venta': 'Bs. 24.6619'}, 'BBVA Provincial': {'Fecha': '18-04-2023', 'Compra': 'Bs. 24.5685', 'Venta': 'Bs. 24.6770'}}
 ``` 
 # Propósito de pyBCV
 El objetivo principal de PyBCV es proporcionar una forma fácil y rápida de acceder a los datos de tipos de cambio y tasas informativas del BCV en un formato que sea fácil de usar y manipular en Python.
```

## Comparing `pyBCV-1.0.2.dist-info/RECORD` & `pyBCV-1.0.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pyBCV/__init__.py,sha256=SZ6EoGVEUueFJA0MDTWGqgeobENhu1fFFDiZwIY8Mns,25
-pyBCV/pyBCV.py,sha256=vZUhRiuE6MBeqHu_QYOfonFnUPSomAUdNvAa9Y7pNSI,4277
-pyBCV-1.0.2.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
-pyBCV-1.0.2.dist-info/METADATA,sha256=9FuxnrWUnIk-w7HkoNRNoBeqzAao_QFj2TW2IiX1Leo,4485
-pyBCV-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyBCV-1.0.2.dist-info/top_level.txt,sha256=lmSpnf39p5nhU1AD7bYr8VERsutkAjoN25gojXaQh90,6
-pyBCV-1.0.2.dist-info/RECORD,,
+pyBCV/pyBCV.py,sha256=w02nubZVcI8MT9iPjlkhdrpxdhgzLJCjHORW6cXk4sw,3527
+pyBCV-1.0.3.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
+pyBCV-1.0.3.dist-info/METADATA,sha256=oQql2IuRJtNg9Mn5CnZ5TCZTIZd-8kJnBYJF85yThrc,4473
+pyBCV-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyBCV-1.0.3.dist-info/top_level.txt,sha256=lmSpnf39p5nhU1AD7bYr8VERsutkAjoN25gojXaQh90,6
+pyBCV-1.0.3.dist-info/RECORD,,
```


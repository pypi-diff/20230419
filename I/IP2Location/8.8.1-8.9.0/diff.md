# Comparing `tmp/IP2Location-8.8.1.tar.gz` & `tmp/IP2Location-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IP2Location-8.8.1.tar", last modified: Fri Aug 12 07:21:39 2022, max compression
+gzip compressed data, was "IP2Location-8.9.0.tar", last modified: Fri Oct 14 08:24:48 2022, max compression
```

## Comparing `IP2Location-8.8.1.tar` & `IP2Location-8.9.0.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-08-12 07:21:39.356396 IP2Location-8.8.1/
--rw-rw-rw-   0        0        0       40 2021-11-08 05:06:23.000000 IP2Location-8.8.1/AUTHORS
-drwxrwxrwx   0        0        0        0 2022-08-12 07:21:39.355184 IP2Location-8.8.1/IP2Location.egg-info/
--rw-rw-rw-   0        0        0    10207 2022-08-12 07:21:39.000000 IP2Location-8.8.1/IP2Location.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2022-08-12 07:21:39.000000 IP2Location-8.8.1/IP2Location.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-12 07:21:39.000000 IP2Location-8.8.1/IP2Location.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-08-12 07:21:39.000000 IP2Location-8.8.1/IP2Location.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    38533 2022-06-22 02:48:04.000000 IP2Location-8.8.1/IP2Location.py
--rw-rw-rw-   0        0        0     1093 2022-06-22 03:04:02.000000 IP2Location-8.8.1/LICENSE.TXT
--rw-rw-rw-   0        0        0    10207 2022-08-12 07:21:39.355184 IP2Location-8.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     8984 2022-08-12 07:15:56.000000 IP2Location-8.8.1/README.md
--rw-rw-rw-   0        0        0       42 2022-08-12 07:21:39.356396 IP2Location-8.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1363 2022-08-12 07:15:38.000000 IP2Location-8.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-14 08:24:48.167898 IP2Location-8.9.0/
+-rw-rw-rw-   0        0        0       40 2022-10-14 02:22:33.000000 IP2Location-8.9.0/AUTHORS
+drwxrwxrwx   0        0        0        0 2022-10-14 08:24:48.159292 IP2Location-8.9.0/IP2Location/
+-rw-rw-rw-   0        0        0      234 2022-10-14 03:17:50.000000 IP2Location-8.9.0/IP2Location/__init__.py
+-rw-rw-rw-   0        0        0     1787 2022-10-14 03:19:58.000000 IP2Location-8.9.0/IP2Location/country.py
+-rw-rw-rw-   0        0        0    32397 2022-10-14 03:17:59.000000 IP2Location-8.9.0/IP2Location/database.py
+-rw-rw-rw-   0        0        0     7649 2022-10-11 08:39:18.000000 IP2Location-8.9.0/IP2Location/iptools.py
+-rw-rw-rw-   0        0        0     1828 2022-10-14 03:20:01.000000 IP2Location-8.9.0/IP2Location/region.py
+-rw-rw-rw-   0        0        0     4669 2022-10-11 08:27:38.000000 IP2Location-8.9.0/IP2Location/webservice.py
+drwxrwxrwx   0        0        0        0 2022-10-14 08:24:48.165899 IP2Location-8.9.0/IP2Location.egg-info/
+-rw-rw-rw-   0        0        0    11892 2022-10-14 08:24:48.000000 IP2Location-8.9.0/IP2Location.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2022-10-14 08:24:48.000000 IP2Location-8.9.0/IP2Location.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-14 08:24:48.000000 IP2Location-8.9.0/IP2Location.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2022-10-14 08:24:48.000000 IP2Location-8.9.0/IP2Location.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2022-10-14 02:22:33.000000 IP2Location-8.9.0/LICENSE.TXT
+-rw-rw-rw-   0        0        0    11892 2022-10-14 08:24:48.166897 IP2Location-8.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10669 2022-10-14 08:15:08.000000 IP2Location-8.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2022-10-14 08:24:48.167898 IP2Location-8.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2022-10-14 08:07:39.000000 IP2Location-8.9.0/setup.py
```

### Comparing `IP2Location-8.8.1/IP2Location.egg-info/PKG-INFO` & `IP2Location-8.9.0/IP2Location.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IP2Location
-Version: 8.8.1
+Version: 8.9.0
 Summary: This is an IP geolocation library that enables the user to find the country, region, city, latitude and longitude, ZIP code, time zone, ISP, domain name, area code, weather info, mobile info, elevation, usage type, address type and IAB category from an IP address. It supports both IPv4 and IPv6 lookup.
 Home-page: https://github.com/chrislim2888/ip2location-python
 Author: IP2Location
 Author-email: support@ip2location.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 License-File: AUTHORS
 
-# IP2Location 8.8.1
+# IP2Location 8.9.0
 
 
 This is a IP2Location Python library that enables the user to find the country, region or state, city, latitude and longitude, ZIP code, time zone, Internet Service Provider (ISP) or company name, domain name, net speed, area code, weather station code, weather station name, mobile country code (MCC), mobile network code (MNC) and carrier brand, elevation, usage type, address type and IAB category by IP address or hostname originates from. The library reads the geo location information from **IP2Location BIN data** file.
 
 Supported IPv4 and IPv6 address.
 
 For more details, please visit:
@@ -108,15 +108,33 @@
 | ipv6_to_decimal | Translate IPv6 address from hexadecimal address to decimal format. |
 | decimal_to_ipv6 | Translate IPv6 address from decimal number into hexadecimal address. |
 | ipv4_to_cidr    | Convert IPv4 range into a list of IPv4 CIDR notation.        |
 | cidr_to_ipv4    | Convert IPv4 CIDR notation into a list of IPv4 addresses.    |
 | ipv6_to_cidr    | Convert IPv6 range into a list of IPv6 CIDR notation.        |
 | cidr_to_ipv6    | Convert IPv6 CIDR notation into a list of IPv6 addresses.    |
 | compressed_ipv6 | Compress a IPv6 to shorten the length.                       |
-| expand_ipv6     | Expand a shorten IPv6 to full length.                        |
+| expand_ipv6     | Expand a shorten IPv6 to full length.                       
+
+### Country Class
+
+Below is the description of the functions available in the **Country** class.
+
+| Function Name                          | Description                                                  |
+| -------------------------------------- | ------------------------------------------------------------ |
+| Constructor                            | Expect a IP2Location Country Information CSV file. This database is free for download at https://www.ip2location.com/free/country-information |
+| get_country_info | Provide a ISO 3166 country code to get the country information in array. Will return a full list of countries information if country code not provided. Below is the information returned: <ul><li>country_code</li><li>country_alpha3_code</li><li>country_numeric_code</li><li>capital</li><li>country_demonym</li><li>total_area</li><li>population</li><li>idd_code</li><li>currency_code</li><li>currency_name</li><li>currency_symbol</li><li>lang_code</li><li>lang_name</li><li>cctld</li></ul> |
+
+### Region Class
+
+Below is the description of the functions available in the **Region** class.
+
+| Function Name                                       | Description                                                  |
+| --------------------------------------------------- | ------------------------------------------------------------ |
+| Constructor                                         | Expect a IP2Location ISO 3166-2 Subdivision Code CSV file. This database is free for download at https://www.ip2location.com/free/iso3166-2 |
+| get_region_code | Provide a ISO 3166 country code and the region name to get ISO 3166-2 subdivision code for the region. | |
 
 # Testing
 
     python sample.py
     python test.py
     python lookup.py <ip_address>
```

### Comparing `IP2Location-8.8.1/IP2Location.py` & `IP2Location-8.9.0/IP2Location/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -671,167 +671,8 @@
 
                 if ipfrom <= ipno < ipto:
                     return self._read_record(mid, ipv)
                 else:
                     if ipno < ipfrom:
                         high = mid - 1
                     else:
-                        low = mid + 1
-
-class IP2LocationWebService(object):
-    ''' IP2Location web service '''
-    def __init__(self,apikey,package,usessl=True):
-        if ((re.match(r"^[0-9A-Z]{10}$", apikey) == None) and (apikey != 'demo')):
-            raise ValueError("Please provide a valid IP2Location web service API key.")
-        if (re.match(r"^WS[0-9]+$", package) == None):
-            package = 'WS1'
-        self.apikey = apikey
-        self.package = package
-        self.usessl = usessl
-    
-    def lookup(self,ip,addons=[],language='en'):
-        '''This function will look the given IP address up in IP2Location web service.'''
-        parameters = urlencode((("key", self.apikey), ("ip", ip), ("package", self.package), ("addon", ','.join(addons)), ("lang", language)))
-        response = httprequest(parameters, self.usessl)
-        if (response == None):
-            return False
-        # if ('response' in response):
-        if (('response' in response) and (response['response'] != 'OK')):
-            raise IP2LocationAPIError(response['response'])
-        return response
-
-    def getcredit(self):
-        '''Get the remaing credit in your IP2Location web service account.'''
-        parameters = urlencode((("key", self.apikey), ("check", True)))
-        response = httprequest(parameters, self.usessl)
-        if (response == None):
-            return 0
-        if ('response' in response is False):
-            return 0
-        return response['response']
-  
-class IP2LocationAPIError(Exception):
-    """Raise for IP2Location API Error Message"""
-
-class IP2LocationIPTools(object):
-
-    def is_ipv4(self, ip):
-        if '.' in ip:
-            ip_parts = ip.split('.')
-            if len(ip_parts) == 4:
-                for i in range(0,len(ip_parts)):
-                    if str(ip_parts[i]).isdigit():
-                        if int(ip_parts[i]) > 255:
-                            return False
-                    else:
-                        return False
-                pattern = r'^([0-9]{1,3}[.]){3}[0-9]{1,3}$'
-                if match(pattern, ip) is not None:
-                    return True
-            else:
-                return False
-        else:
-            return False
-        return False
-
-    def is_ipv6(self, ip):
-        try:
-            socket.inet_pton(socket.AF_INET6, ip)
-        except socket.error:  # not a valid address
-            return False
-        return True
-    
-    def ipv4_to_decimal(self, ip):
-        try:
-            ipnum = struct.unpack('!L', socket.inet_pton(socket.AF_INET, ip))[0]
-        except (socket.error, OSError, ValueError):
-            # ipnum = -1
-            return
-        return ipnum
-    
-    def decimal_to_ipv4(self, decimal):
-        if str(decimal).isdigit() is False:
-            return
-        if (int(decimal) > 4294967295):
-            return
-        else:
-            return (socket.inet_ntoa(struct.pack('!I', int(decimal))))
-    
-    def ipv6_to_decimal(self, ip):
-        if self.is_ipv6(ip) is False:
-            return
-        return(int(ipaddress.ip_address(u(ip))))
-    
-    def decimal_to_ipv6(self, decimal):
-        if str(decimal).isdigit() is False:
-            return
-        result = ipaddress.IPv6Address(int(decimal))
-        if (result.ipv4_mapped != None):
-            return('::ffff:' + str(result.ipv4_mapped))
-        else:
-            return str(result)
-    
-    def ipv4_to_cidr(self, from_ip, to_ip):
-        if self.is_ipv4(from_ip) is False:
-            return
-        if self.is_ipv4(to_ip) is False:
-            return
-        startip = ipaddress.IPv4Address(u(from_ip))
-        endip = ipaddress.IPv4Address(u(to_ip))
-        ar = [ipaddr for ipaddr in ipaddress.summarize_address_range(startip, endip)]
-        ar1 = []
-        for i in range(len(ar)):
-            ar1.append(str(ar[i]))
-        return (ar1)
-    
-    def ipv6_to_cidr(self, from_ip, to_ip):
-        if self.is_ipv6(from_ip) is False:
-            return
-        if self.is_ipv6(to_ip) is False:
-            return
-        startip = ipaddress.IPv6Address(u(from_ip))
-        endip = ipaddress.IPv6Address(u(to_ip))
-        ar = [ipaddr for ipaddr in ipaddress.summarize_address_range(startip, endip)]
-        ar1 = []
-        for i in range(len(ar)):
-            ar1.append(str(ar[i]))
-        return (ar1)
-    
-    def cidr_to_ipv4(self, cidr):
-        if '/' not in cidr:
-            return
-        net=ipaddress.ip_network(u(cidr))
-        return({"ip_start": str(net[0]), "ip_end": str(net[-1])})
-    
-    def cidr_to_ipv6(self, cidr):
-        if '/' not in cidr:
-            return
-        parts = cidr.split('/')
-        hexstartaddress = binascii.hexlify(socket.inet_pton(socket.AF_INET6, parts[0]))
-        if (len(hexstartaddress) < 16):
-            hexstartaddress = hexstartaddress.zfill(16-hexstartaddress.len())
-        bits = 128 - int(parts[1])
-        hexlastaddress = hexstartaddress
-        pos = 31
-        while (bits > 0):
-            int_value = int(hexlastaddress[pos:pos+1], 16)
-            # new = binascii.hexlify((int_value | (pow(2, min(4, bits)) - 1)).to_bytes(1, 'big'))
-            new = binascii.hexlify((int_value | (pow(2, min(4, bits)) - 1)).to_bytes(1, 'little'))[1:]
-            hexlastaddresslist = list(u(hexlastaddress))
-            hexlastaddresslist[pos] = u(new)
-            string_hexlastaddresslist = [str(int) for int in hexlastaddresslist] 
-            hexlastaddress = ''.join(string_hexlastaddresslist)
-            bits = bits - 4
-            pos = pos - 1
-        binlastaddress = binascii.unhexlify(b(hexlastaddress))
-        return({"ip_start": self.expand_ipv6(parts[0]), "ip_end": self.expand_ipv6(socket.inet_ntop(socket.AF_INET6, binlastaddress))})
-    
-    def compressed_ipv6(self, ip):
-        if self.is_ipv6(ip) is False:
-            return
-        return ((ipaddress.IPv6Address(u(ip)).compressed))
-    
-    def expand_ipv6(self, ip):
-        if self.is_ipv6(ip) is False:
-            return
-        return ((ipaddress.IPv6Address(u(ip)).exploded))
-
+                        low = mid + 1
```

### Comparing `IP2Location-8.8.1/LICENSE.TXT` & `IP2Location-8.9.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `IP2Location-8.8.1/PKG-INFO` & `IP2Location-8.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IP2Location
-Version: 8.8.1
+Version: 8.9.0
 Summary: This is an IP geolocation library that enables the user to find the country, region, city, latitude and longitude, ZIP code, time zone, ISP, domain name, area code, weather info, mobile info, elevation, usage type, address type and IAB category from an IP address. It supports both IPv4 and IPv6 lookup.
 Home-page: https://github.com/chrislim2888/ip2location-python
 Author: IP2Location
 Author-email: support@ip2location.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 License-File: AUTHORS
 
-# IP2Location 8.8.1
+# IP2Location 8.9.0
 
 
 This is a IP2Location Python library that enables the user to find the country, region or state, city, latitude and longitude, ZIP code, time zone, Internet Service Provider (ISP) or company name, domain name, net speed, area code, weather station code, weather station name, mobile country code (MCC), mobile network code (MNC) and carrier brand, elevation, usage type, address type and IAB category by IP address or hostname originates from. The library reads the geo location information from **IP2Location BIN data** file.
 
 Supported IPv4 and IPv6 address.
 
 For more details, please visit:
@@ -108,15 +108,33 @@
 | ipv6_to_decimal | Translate IPv6 address from hexadecimal address to decimal format. |
 | decimal_to_ipv6 | Translate IPv6 address from decimal number into hexadecimal address. |
 | ipv4_to_cidr    | Convert IPv4 range into a list of IPv4 CIDR notation.        |
 | cidr_to_ipv4    | Convert IPv4 CIDR notation into a list of IPv4 addresses.    |
 | ipv6_to_cidr    | Convert IPv6 range into a list of IPv6 CIDR notation.        |
 | cidr_to_ipv6    | Convert IPv6 CIDR notation into a list of IPv6 addresses.    |
 | compressed_ipv6 | Compress a IPv6 to shorten the length.                       |
-| expand_ipv6     | Expand a shorten IPv6 to full length.                        |
+| expand_ipv6     | Expand a shorten IPv6 to full length.                       
+
+### Country Class
+
+Below is the description of the functions available in the **Country** class.
+
+| Function Name                          | Description                                                  |
+| -------------------------------------- | ------------------------------------------------------------ |
+| Constructor                            | Expect a IP2Location Country Information CSV file. This database is free for download at https://www.ip2location.com/free/country-information |
+| get_country_info | Provide a ISO 3166 country code to get the country information in array. Will return a full list of countries information if country code not provided. Below is the information returned: <ul><li>country_code</li><li>country_alpha3_code</li><li>country_numeric_code</li><li>capital</li><li>country_demonym</li><li>total_area</li><li>population</li><li>idd_code</li><li>currency_code</li><li>currency_name</li><li>currency_symbol</li><li>lang_code</li><li>lang_name</li><li>cctld</li></ul> |
+
+### Region Class
+
+Below is the description of the functions available in the **Region** class.
+
+| Function Name                                       | Description                                                  |
+| --------------------------------------------------- | ------------------------------------------------------------ |
+| Constructor                                         | Expect a IP2Location ISO 3166-2 Subdivision Code CSV file. This database is free for download at https://www.ip2location.com/free/iso3166-2 |
+| get_region_code | Provide a ISO 3166 country code and the region name to get ISO 3166-2 subdivision code for the region. | |
 
 # Testing
 
     python sample.py
     python test.py
     python lookup.py <ip_address>
```

### Comparing `IP2Location-8.8.1/README.md` & `IP2Location-8.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# IP2Location 8.8.1
+# IP2Location 8.9.0
 
 
 This is a IP2Location Python library that enables the user to find the country, region or state, city, latitude and longitude, ZIP code, time zone, Internet Service Provider (ISP) or company name, domain name, net speed, area code, weather station code, weather station name, mobile country code (MCC), mobile network code (MNC) and carrier brand, elevation, usage type, address type and IAB category by IP address or hostname originates from. The library reads the geo location information from **IP2Location BIN data** file.
 
 Supported IPv4 and IPv6 address.
 
 For more details, please visit:
@@ -85,15 +85,33 @@
 | ipv6_to_decimal | Translate IPv6 address from hexadecimal address to decimal format. |
 | decimal_to_ipv6 | Translate IPv6 address from decimal number into hexadecimal address. |
 | ipv4_to_cidr    | Convert IPv4 range into a list of IPv4 CIDR notation.        |
 | cidr_to_ipv4    | Convert IPv4 CIDR notation into a list of IPv4 addresses.    |
 | ipv6_to_cidr    | Convert IPv6 range into a list of IPv6 CIDR notation.        |
 | cidr_to_ipv6    | Convert IPv6 CIDR notation into a list of IPv6 addresses.    |
 | compressed_ipv6 | Compress a IPv6 to shorten the length.                       |
-| expand_ipv6     | Expand a shorten IPv6 to full length.                        |
+| expand_ipv6     | Expand a shorten IPv6 to full length.                       
+
+### Country Class
+
+Below is the description of the functions available in the **Country** class.
+
+| Function Name                          | Description                                                  |
+| -------------------------------------- | ------------------------------------------------------------ |
+| Constructor                            | Expect a IP2Location Country Information CSV file. This database is free for download at https://www.ip2location.com/free/country-information |
+| get_country_info | Provide a ISO 3166 country code to get the country information in array. Will return a full list of countries information if country code not provided. Below is the information returned: <ul><li>country_code</li><li>country_alpha3_code</li><li>country_numeric_code</li><li>capital</li><li>country_demonym</li><li>total_area</li><li>population</li><li>idd_code</li><li>currency_code</li><li>currency_name</li><li>currency_symbol</li><li>lang_code</li><li>lang_name</li><li>cctld</li></ul> |
+
+### Region Class
+
+Below is the description of the functions available in the **Region** class.
+
+| Function Name                                       | Description                                                  |
+| --------------------------------------------------- | ------------------------------------------------------------ |
+| Constructor                                         | Expect a IP2Location ISO 3166-2 Subdivision Code CSV file. This database is free for download at https://www.ip2location.com/free/iso3166-2 |
+| get_region_code | Provide a ISO 3166 country code and the region name to get ISO 3166-2 subdivision code for the region. | |
 
 # Testing
 
     python sample.py
     python test.py
     python lookup.py <ip_address>
```

### Comparing `IP2Location-8.8.1/setup.py` & `IP2Location-8.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="IP2Location",
-	version="8.8.1", 
+	version="8.9.0", 
 	author="IP2Location",
 	author_email="support@ip2location.com",
 	description="This is an IP geolocation library that enables the user to find the country, region, city, latitude and longitude, ZIP code, time zone, ISP, domain name, area code, weather info, mobile info, elevation, usage type, address type and IAB category from an IP address. It supports both IPv4 and IPv6 lookup.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	py_modules=['IP2Location'],
 	url="https://github.com/chrislim2888/ip2location-python",
```


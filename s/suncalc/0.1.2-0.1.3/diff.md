# Comparing `tmp/suncalc-0.1.2.tar.gz` & `tmp/suncalc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suncalc-0.1.2.tar", last modified: Wed Dec  2 22:59:39 2020, max compression
+gzip compressed data, was "suncalc-0.1.3.tar", last modified: Wed Apr 19 00:02:50 2023, max compression
```

## Comparing `suncalc-0.1.2.tar` & `suncalc-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2020-12-02 22:59:39.000000 suncalc-0.1.2/
--rw-r--r--   0 kyle       (501) staff       (20)      247 2020-12-02 22:59:12.000000 suncalc-0.1.2/CHANGELOG.md
--rw-r--r--   0 kyle       (501) staff       (20)       21 2020-11-20 15:53:52.000000 suncalc-0.1.2/MANIFEST.in
--rw-r--r--   0 kyle       (501) staff       (20)    10629 2020-12-02 22:59:39.000000 suncalc-0.1.2/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)     7750 2020-11-20 17:47:10.000000 suncalc-0.1.2/README.md
--rw-r--r--   0 kyle       (501) staff       (20)      423 2020-12-02 22:59:39.000000 suncalc-0.1.2/setup.cfg
--rw-r--r--   0 kyle       (501) staff       (20)     1528 2020-12-02 22:59:18.000000 suncalc-0.1.2/setup.py
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2020-12-02 22:59:39.000000 suncalc-0.1.2/suncalc/
--rw-r--r--   0 kyle       (501) staff       (20)      135 2020-12-02 22:59:18.000000 suncalc-0.1.2/suncalc/__init__.py
--rw-r--r--   0 kyle       (501) staff       (20)    12125 2020-12-02 22:58:32.000000 suncalc-0.1.2/suncalc/suncalc.py
--rw-r--r--   0 kyle       (501) staff       (20)        0 2020-12-02 22:36:24.000000 suncalc-0.1.2/suncalc/test.py
-drwxr-xr-x   0 kyle       (501) staff       (20)        0 2020-12-02 22:59:39.000000 suncalc-0.1.2/suncalc.egg-info/
--rw-r--r--   0 kyle       (501) staff       (20)    10629 2020-12-02 22:59:39.000000 suncalc-0.1.2/suncalc.egg-info/PKG-INFO
--rw-r--r--   0 kyle       (501) staff       (20)      292 2020-12-02 22:59:39.000000 suncalc-0.1.2/suncalc.egg-info/SOURCES.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2020-12-02 22:59:39.000000 suncalc-0.1.2/suncalc.egg-info/dependency_links.txt
--rw-r--r--   0 kyle       (501) staff       (20)        1 2020-11-20 02:53:23.000000 suncalc-0.1.2/suncalc.egg-info/not-zip-safe
--rw-r--r--   0 kyle       (501) staff       (20)       46 2020-12-02 22:59:39.000000 suncalc-0.1.2/suncalc.egg-info/requires.txt
--rw-r--r--   0 kyle       (501) staff       (20)        8 2020-12-02 22:59:39.000000 suncalc-0.1.2/suncalc.egg-info/top_level.txt
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-04-19 00:02:50.833970 suncalc-0.1.3/
+-rw-r--r--   0 kyle       (501) staff       (20)      342 2023-04-19 00:02:27.000000 suncalc-0.1.3/CHANGELOG.md
+-rw-r--r--   0 kyle       (501) staff       (20)     1068 2023-04-19 00:02:27.000000 suncalc-0.1.3/LICENSE
+-rw-r--r--   0 kyle       (501) staff       (20)       21 2023-04-19 00:02:27.000000 suncalc-0.1.3/MANIFEST.in
+-rw-r--r--   0 kyle       (501) staff       (20)     9021 2023-04-19 00:02:50.834048 suncalc-0.1.3/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)     7762 2023-04-19 00:02:27.000000 suncalc-0.1.3/README.md
+-rw-r--r--   0 kyle       (501) staff       (20)      423 2023-04-19 00:02:50.834603 suncalc-0.1.3/setup.cfg
+-rw-r--r--   0 kyle       (501) staff       (20)     1628 2023-04-19 00:02:27.000000 suncalc-0.1.3/setup.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-04-19 00:02:50.833128 suncalc-0.1.3/suncalc/
+-rw-r--r--   0 kyle       (501) staff       (20)      135 2023-04-19 00:02:27.000000 suncalc-0.1.3/suncalc/__init__.py
+-rw-r--r--   0 kyle       (501) staff       (20)    12135 2023-04-19 00:02:27.000000 suncalc-0.1.3/suncalc/suncalc.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-04-19 00:02:50.833862 suncalc-0.1.3/suncalc.egg-info/
+-rw-r--r--   0 kyle       (501) staff       (20)     9021 2023-04-19 00:02:50.000000 suncalc-0.1.3/suncalc.egg-info/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      284 2023-04-19 00:02:50.000000 suncalc-0.1.3/suncalc.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-04-19 00:02:50.000000 suncalc-0.1.3/suncalc.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-04-19 00:02:50.000000 suncalc-0.1.3/suncalc.egg-info/not-zip-safe
+-rw-r--r--   0 kyle       (501) staff       (20)       46 2023-04-19 00:02:50.000000 suncalc-0.1.3/suncalc.egg-info/requires.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        8 2023-04-19 00:02:50.000000 suncalc-0.1.3/suncalc.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `suncalc-0.1.2/PKG-INFO` & `suncalc-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,250 +1,256 @@
 Metadata-Version: 2.1
 Name: suncalc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fast, vectorized Python port of suncalc.js
 Home-page: https://github.com/kylebarron/suncalc-py
 Author: Kyle Barron
 Author-email: kylebarron2@gmail.com
 License: MIT license
-Description: # suncalc-py
-        
-        <p>
-          <a href="https://github.com/kylebarron/suncalc-py/actions?query=workflow%3ACI" target="_blank">
-              <img src="https://github.com/kylebarron/suncalc-py/workflows/test/badge.svg" alt="Test">
-          </a>
-          <a href="https://pypi.org/project/suncalc" target="_blank">
-              <img src="https://img.shields.io/pypi/v/suncalc?color=%2334D058&label=pypi%20package" alt="Package version">
-          </a>
-          <a href="https://github.com/kylebarron/suncalc-py/blob/master/LICENSE" target="_blank">
-              <img src="https://img.shields.io/github/license/kylebarron/suncalc-py.svg" alt="Downloads">
-          </a>
-        </p>
-        
-        
-        A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
-        calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
-        etc.) for the given location and time.
-        
-        [suncalc-js]: https://github.com/mourner/suncalc
-        
-        While other similar libraries exist, I didn't originally encounter any that met
-        my requirements of being both openly-licensed and vectorized <sup>1</sup>
-        
-        ## Install
-        
-        ```
-        pip install suncalc
-        ```
-        
-        ## Using
-        
-        ### Example
-        
-        `suncalc` is designed to work both with single values and with arrays of values.
-        
-        First, import the module:
-        
-        ```py
-        from suncalc import get_position, get_times
-        from datetime import datetime
-        ```
-        
-        There are currently two methods: `get_position`, to get the sun azimuth and
-        altitude for a given date and position, and `get_times`, to get sunlight phases
-        for a given date and position.
-        
-        ```py
-        date = datetime.now()
-        lon = 20
-        lat = 45
-        get_position(date, lon, lat)
-        # {'azimuth': -0.8619668996997687, 'altitude': 0.5586446727994595}
-        
-        get_times(date, lon, lat)
-        # {'solar_noon': Timestamp('2020-11-20 08:47:08.410863770'),
-        #  'nadir': Timestamp('2020-11-19 20:47:08.410863770'),
-        #  'sunrise': Timestamp('2020-11-20 03:13:22.645455322'),
-        #  'sunset': Timestamp('2020-11-20 14:20:54.176272461'),
-        #  'sunrise_end': Timestamp('2020-11-20 03:15:48.318936035'),
-        #  'sunset_start': Timestamp('2020-11-20 14:18:28.502791748'),
-        #  'dawn': Timestamp('2020-11-20 02:50:00.045539551'),
-        #  'dusk': Timestamp('2020-11-20 14:44:16.776188232'),
-        #  'nautical_dawn': Timestamp('2020-11-20 02:23:10.019832520'),
-        #  'nautical_dusk': Timestamp('2020-11-20 15:11:06.801895264'),
-        #  'night_end': Timestamp('2020-11-20 01:56:36.144269287'),
-        #  'night': Timestamp('2020-11-20 15:37:40.677458252'),
-        #  'golden_hour_end': Timestamp('2020-11-20 03:44:46.795967773'),
-        #  'golden_hour': Timestamp('2020-11-20 13:49:30.025760010')}
-        ```
-        
-        These methods also work for _arrays_ of data, and since the implementation is
-        vectorized it's much faster than a for loop in Python.
-        
-        ```py
-        import pandas as pd
-        
-        df = pd.DataFrame({
-            'date': [date] * 10,
-            'lon': [lon] * 10,
-            'lat': [lat] * 10
-        })
-        pd.DataFrame(get_position(df['date'], df['lon'], df['lat']))
-        # azimuth	altitude
-        # 0	-1.485509	-1.048223
-        # 1	-1.485509	-1.048223
-        # ...
-        
-        pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))['solar_noon']
-        # 0   2020-11-20 08:47:08.410863872+00:00
-        # 1   2020-11-20 08:47:08.410863872+00:00
-        # ...
-        # Name: solar_noon, dtype: datetime64[ns, UTC]
-        ```
-        
-        If you want to join this data back to your `DataFrame`, you can use `pd.concat`:
-        
-        ```py
-        times = pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))
-        pd.concat([df, times], axis=1)
-        ```
-        
-        ### API
-        
-        #### `get_position`
-        
-        Calculate sun position (azimuth and altitude) for a given date and
-        latitude/longitude
-        
-        - `date` (`datetime` or a pandas series of datetimes): date and time to find sun position of. **Datetime must be in UTC**.
-        - `lng` (`float` or numpy array of `float`): longitude to find sun position of
-        - `lat` (`float` or numpy array of `float`): latitude to find sun position of
-        
-        Returns a `dict` with two keys: `azimuth` and `altitude`. If the input values
-        were singletons, the `dict`'s values will be floats. Otherwise they'll be numpy
-        arrays of floats.
-        
-        #### `get_times`
-        
-        - `date` (`datetime` or a pandas series of datetimes): date and time to find sunlight phases of. **Datetime must be in UTC**.
-        - `lng` (`float` or numpy array of `float`): longitude to find sunlight phases of
-        - `lat` (`float` or numpy array of `float`): latitude to find sunlight phases of
-        - `height` (`float` or numpy array of `float`, default `0`): observer height in meters
-        - `times` (`Iterable[Tuple[float, str, str]]`): an iterable defining the angle above the horizon and strings for custom sunlight phases. The default is:
-        
-            ```py
-            # (angle, morning name, evening name)
-            DEFAULT_TIMES = [
-                (-0.833, 'sunrise', 'sunset'),
-                (-0.3, 'sunrise_end', 'sunset_start'),
-                (-6, 'dawn', 'dusk'),
-                (-12, 'nautical_dawn', 'nautical_dusk'),
-                (-18, 'night_end', 'night'),
-                (6, 'golden_hour_end', 'golden_hour')
-            ]
-            ```
-        
-        Returns a `dict` where the keys are `solar_noon`, `nadir`, plus any keys passed
-        in the `times` argument. If the input values were singletons, the `dict`'s
-        values will be of type `datetime.datetime` (or `pd.Timestamp` if you have pandas
-        installed, which is a subclass of and therefore compatible with
-        `datetime.datetime`). Otherwise they'll be pandas `DateTime` series. **The
-        returned times will be in UTC.**
-        
-        ## Benchmark
-        
-        This benchmark is to show that the vectorized implementation is nearly 100x
-        faster than a for loop in Python.
-        
-        First set up a `DataFrame` with random data. Here I create 100,000 rows.
-        
-        ```py
-        from suncalc import get_position, get_times
-        import pandas as pd
-        
-        def random_dates(start, end, n=10):
-            """Create an array of random dates"""
-            start_u = start.value//10**9
-            end_u = end.value//10**9
-            return pd.to_datetime(np.random.randint(start_u, end_u, n), unit='s')
-        
-        start = pd.to_datetime('2015-01-01')
-        end = pd.to_datetime('2018-01-01')
-        dates = random_dates(start, end, n=100_000)
-        
-        lons = np.random.uniform(low=-179, high=179, size=(100_000,))
-        lats = np.random.uniform(low=-89, high=89, size=(100_000,))
-        
-        df = pd.DataFrame({'date': dates, 'lat': lats, 'lon': lons})
-        ```
-        
-        Then compute `SunCalc.get_position` two ways: the first using the vectorized
-        implementation and the second using `df.apply`, which is equivalent to a for
-        loop. The first is more than **100x faster** than the second.
-        
-        ```py
-        %timeit get_position(df['date'], df['lon'], df['lat'])
-        # 41.4 ms ± 437 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-        
-        %timeit df.apply(lambda row: get_position(row['date'], row['lon'], row['lat']), axis=1)
-        # 4.89 s ± 184 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-        ```
-        
-        Likewise, compute `SunCalc.get_times` the same two ways: first using the
-        vectorized implementation and the second using `df.apply`. The first is **2800x
-        faster** than the second! Some of the difference here is that under the hood the
-        non-vectorized approach uses `pd.to_datetime` while the vectorized
-        implementation uses `np.astype('datetime64[ns, UTC]')`. `pd.to_datetime` is
-        really slow!!
-        
-        ```py
-        %timeit get_times(df['date'], df['lon'], df['lat'])
-        # 55.3 ms ± 1.91 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-        
-        %time df.apply(lambda row: get_times(row['date'], row['lon'], row['lat']), axis=1)
-        # CPU times: user 2min 33s, sys: 288 ms, total: 2min 34s
-        # Wall time: 2min 34s
-        ```
-        
-        ---
-        
-        1: [`pyorbital`](https://github.com/pytroll/pyorbital) looks great but is
-        GPL3-licensed; [`pysolar`](https://github.com/pingswept/pysolar) is also
-        GPL3-licensed; [`pyEphem`](https://rhodesmill.org/pyephem/) is LGPL3-licensed.
-        [`suncalcPy`](https://github.com/Broham/suncalcPy) is another port of
-        `suncalc.js`, and is MIT-licensed, but doesn't use Numpy and thus isn't
-        vectorized. I recently discovered [`sunpy`](https://github.com/sunpy/sunpy) and
-        [`astropy`](https://github.com/astropy/astropy), both of which probably would've
-        worked but I didn't see them at first and they look quite complex for this
-        simple task...
-        
-        
-        # Changelog
-        
-        ## [0.1.2] - 2020-12-02
-        
-        - Try to catch NaN before passing to `datetime.utcfromtimestamp`
-        
-        ## [0.1.1] - 2020-11-20
-        
-        - Fix PyPI install by adding `MANIFEST.in`
-        - Update documentation
-        
-        ## [0.1.0] - 2020-11-19
-        
-        - Initial release on PyPI
-        
 Keywords: suncalc,sun
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: tests
+License-File: LICENSE
+
+# suncalc-py
+
+<p>
+  <a href="https://github.com/kylebarron/suncalc-py/actions?query=workflow%3ACI" target="_blank">
+      <img src="https://github.com/kylebarron/suncalc-py/workflows/test/badge.svg" alt="Test">
+  </a>
+  <a href="https://pypi.org/project/suncalc" target="_blank">
+      <img src="https://img.shields.io/pypi/v/suncalc?color=%2334D058&label=pypi%20package" alt="Package version">
+  </a>
+  <a href="https://github.com/kylebarron/suncalc-py/blob/master/LICENSE" target="_blank">
+      <img src="https://img.shields.io/github/license/kylebarron/suncalc-py.svg" alt="Downloads">
+  </a>
+</p>
+
+
+A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
+calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
+etc.) for the given location and time.
+
+[suncalc-js]: https://github.com/mourner/suncalc
+
+While other similar libraries exist, I didn't originally encounter any that met
+my requirements of being openly-licensed, vectorized, and simple to use <sup>1</sup>.
+
+## Install
+
+```
+pip install suncalc
+```
+
+## Using
+
+### Example
+
+`suncalc` is designed to work both with single values and with arrays of values.
+
+First, import the module:
+
+```py
+from suncalc import get_position, get_times
+from datetime import datetime
+```
+
+There are currently two methods: `get_position`, to get the sun azimuth and
+altitude for a given date and position, and `get_times`, to get sunlight phases
+for a given date and position.
+
+```py
+date = datetime.now()
+lon = 20
+lat = 45
+get_position(date, lon, lat)
+# {'azimuth': -0.8619668996997687, 'altitude': 0.5586446727994595}
+
+get_times(date, lon, lat)
+# {'solar_noon': Timestamp('2020-11-20 08:47:08.410863770'),
+#  'nadir': Timestamp('2020-11-19 20:47:08.410863770'),
+#  'sunrise': Timestamp('2020-11-20 03:13:22.645455322'),
+#  'sunset': Timestamp('2020-11-20 14:20:54.176272461'),
+#  'sunrise_end': Timestamp('2020-11-20 03:15:48.318936035'),
+#  'sunset_start': Timestamp('2020-11-20 14:18:28.502791748'),
+#  'dawn': Timestamp('2020-11-20 02:50:00.045539551'),
+#  'dusk': Timestamp('2020-11-20 14:44:16.776188232'),
+#  'nautical_dawn': Timestamp('2020-11-20 02:23:10.019832520'),
+#  'nautical_dusk': Timestamp('2020-11-20 15:11:06.801895264'),
+#  'night_end': Timestamp('2020-11-20 01:56:36.144269287'),
+#  'night': Timestamp('2020-11-20 15:37:40.677458252'),
+#  'golden_hour_end': Timestamp('2020-11-20 03:44:46.795967773'),
+#  'golden_hour': Timestamp('2020-11-20 13:49:30.025760010')}
+```
+
+These methods also work for _arrays_ of data, and since the implementation is
+vectorized it's much faster than a for loop in Python.
+
+```py
+import pandas as pd
+
+df = pd.DataFrame({
+    'date': [date] * 10,
+    'lon': [lon] * 10,
+    'lat': [lat] * 10
+})
+pd.DataFrame(get_position(df['date'], df['lon'], df['lat']))
+# azimuth	altitude
+# 0	-1.485509	-1.048223
+# 1	-1.485509	-1.048223
+# ...
+
+pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))['solar_noon']
+# 0   2020-11-20 08:47:08.410863872+00:00
+# 1   2020-11-20 08:47:08.410863872+00:00
+# ...
+# Name: solar_noon, dtype: datetime64[ns, UTC]
+```
+
+If you want to join this data back to your `DataFrame`, you can use `pd.concat`:
+
+```py
+times = pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))
+pd.concat([df, times], axis=1)
+```
+
+### API
+
+#### `get_position`
+
+Calculate sun position (azimuth and altitude) for a given date and
+latitude/longitude
+
+- `date` (`datetime` or a pandas series of datetimes): date and time to find sun position of. **Datetime must be in UTC**.
+- `lng` (`float` or numpy array of `float`): longitude to find sun position of
+- `lat` (`float` or numpy array of `float`): latitude to find sun position of
+
+Returns a `dict` with two keys: `azimuth` and `altitude`. If the input values
+were singletons, the `dict`'s values will be floats. Otherwise they'll be numpy
+arrays of floats.
+
+#### `get_times`
+
+- `date` (`datetime` or a pandas series of datetimes): date and time to find sunlight phases of. **Datetime must be in UTC**.
+- `lng` (`float` or numpy array of `float`): longitude to find sunlight phases of
+- `lat` (`float` or numpy array of `float`): latitude to find sunlight phases of
+- `height` (`float` or numpy array of `float`, default `0`): observer height in meters
+- `times` (`Iterable[Tuple[float, str, str]]`): an iterable defining the angle above the horizon and strings for custom sunlight phases. The default is:
+
+    ```py
+    # (angle, morning name, evening name)
+    DEFAULT_TIMES = [
+        (-0.833, 'sunrise', 'sunset'),
+        (-0.3, 'sunrise_end', 'sunset_start'),
+        (-6, 'dawn', 'dusk'),
+        (-12, 'nautical_dawn', 'nautical_dusk'),
+        (-18, 'night_end', 'night'),
+        (6, 'golden_hour_end', 'golden_hour')
+    ]
+    ```
+
+Returns a `dict` where the keys are `solar_noon`, `nadir`, plus any keys passed
+in the `times` argument. If the input values were singletons, the `dict`'s
+values will be of type `datetime.datetime` (or `pd.Timestamp` if you have pandas
+installed, which is a subclass of and therefore compatible with
+`datetime.datetime`). Otherwise they'll be pandas `DateTime` series. **The
+returned times will be in UTC.**
+
+## Benchmark
+
+This benchmark is to show that the vectorized implementation is nearly 100x
+faster than a for loop in Python.
+
+First set up a `DataFrame` with random data. Here I create 100,000 rows.
+
+```py
+from suncalc import get_position, get_times
+import pandas as pd
+
+def random_dates(start, end, n=10):
+    """Create an array of random dates"""
+    start_u = start.value//10**9
+    end_u = end.value//10**9
+    return pd.to_datetime(np.random.randint(start_u, end_u, n), unit='s')
+
+start = pd.to_datetime('2015-01-01')
+end = pd.to_datetime('2018-01-01')
+dates = random_dates(start, end, n=100_000)
+
+lons = np.random.uniform(low=-179, high=179, size=(100_000,))
+lats = np.random.uniform(low=-89, high=89, size=(100_000,))
+
+df = pd.DataFrame({'date': dates, 'lat': lats, 'lon': lons})
+```
+
+Then compute `SunCalc.get_position` two ways: the first using the vectorized
+implementation and the second using `df.apply`, which is equivalent to a for
+loop. The first is more than **100x faster** than the second.
+
+```py
+%timeit get_position(df['date'], df['lon'], df['lat'])
+# 41.4 ms ± 437 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+
+%timeit df.apply(lambda row: get_position(row['date'], row['lon'], row['lat']), axis=1)
+# 4.89 s ± 184 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+```
+
+Likewise, compute `SunCalc.get_times` the same two ways: first using the
+vectorized implementation and the second using `df.apply`. The first is **2800x
+faster** than the second! Some of the difference here is that under the hood the
+non-vectorized approach uses `pd.to_datetime` while the vectorized
+implementation uses `np.astype('datetime64[ns, UTC]')`. `pd.to_datetime` is
+really slow!!
+
+```py
+%timeit get_times(df['date'], df['lon'], df['lat'])
+# 55.3 ms ± 1.91 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
+
+%time df.apply(lambda row: get_times(row['date'], row['lon'], row['lat']), axis=1)
+# CPU times: user 2min 33s, sys: 288 ms, total: 2min 34s
+# Wall time: 2min 34s
+```
+
+---
+
+1: [`pyorbital`](https://github.com/pytroll/pyorbital) looks great but is
+GPL3-licensed; [`pysolar`](https://github.com/pingswept/pysolar) is also
+GPL3-licensed; [`pyEphem`](https://rhodesmill.org/pyephem/) is LGPL3-licensed.
+[`suncalcPy`](https://github.com/Broham/suncalcPy) is another port of
+`suncalc.js`, and is MIT-licensed, but doesn't use Numpy and thus isn't
+vectorized. I recently discovered [`sunpy`](https://github.com/sunpy/sunpy) and
+[`astropy`](https://github.com/astropy/astropy), both of which probably would've
+worked but I didn't see them at first and they look quite complex for this
+simple task...
+
+
+# Changelog
+
+## [0.1.3] - 2023-04-18
+
+- Ensure pandas 2.0 compatibility (fix integer casting of datetimes)
+
+## [0.1.2] - 2020-12-02
+
+- Try to catch NaN before passing to `datetime.utcfromtimestamp`
+
+## [0.1.1] - 2020-11-20
+
+- Fix PyPI install by adding `MANIFEST.in`
+- Update documentation
+
+## [0.1.0] - 2020-11-19
+
+- Initial release on PyPI
```

#### html2text {}

```diff
@@ -1,20 +1,29 @@
-Metadata-Version: 2.1 Name: suncalc Version: 0.1.2 Summary: A fast, vectorized
+Metadata-Version: 2.1 Name: suncalc Version: 0.1.3 Summary: A fast, vectorized
 Python port of suncalc.js Home-page: https://github.com/kylebarron/suncalc-py
 Author: Kyle Barron Author-email: kylebarron2@gmail.com License: MIT license
-Description: # suncalc-py
+Keywords: suncalc,sun Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.6 Description-Content-Type:
+text/markdown Provides-Extra: pandas Provides-Extra: tests License-File:
+LICENSE # suncalc-py
 [Test] [Package_version] [Downloads]
 A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
 calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
 etc.) for the given location and time. [suncalc-js]: https://github.com/
 mourner/suncalc While other similar libraries exist, I didn't originally
-encounter any that met my requirements of being both openly-licensed and
-vectorized 1 ## Install ``` pip install suncalc ``` ## Using ### Example
-`suncalc` is designed to work both with single values and with arrays of
-values. First, import the module: ```py from suncalc import get_position,
+encounter any that met my requirements of being openly-licensed, vectorized,
+and simple to use 1. ## Install ``` pip install suncalc ``` ## Using ###
+Example `suncalc` is designed to work both with single values and with arrays
+of values. First, import the module: ```py from suncalc import get_position,
 get_times from datetime import datetime ``` There are currently two methods:
 `get_position`, to get the sun azimuth and altitude for a given date and
 position, and `get_times`, to get sunlight phases for a given date and
 position. ```py date = datetime.now() lon = 20 lat = 45 get_position(date, lon,
 lat) # {'azimuth': -0.8619668996997687, 'altitude': 0.5586446727994595}
 get_times(date, lon, lat) # {'solar_noon': Timestamp('2020-11-20 08:47:
 08.410863770'), # 'nadir': Timestamp('2020-11-19 20:47:08.410863770'), #
@@ -91,19 +100,12 @@
 licensed; [`pysolar`](https://github.com/pingswept/pysolar) is also GPL3-
 licensed; [`pyEphem`](https://rhodesmill.org/pyephem/) is LGPL3-licensed.
 [`suncalcPy`](https://github.com/Broham/suncalcPy) is another port of
 `suncalc.js`, and is MIT-licensed, but doesn't use Numpy and thus isn't
 vectorized. I recently discovered [`sunpy`](https://github.com/sunpy/sunpy) and
 [`astropy`](https://github.com/astropy/astropy), both of which probably
 would've worked but I didn't see them at first and they look quite complex for
-this simple task... # Changelog ## [0.1.2] - 2020-12-02 - Try to catch NaN
-before passing to `datetime.utcfromtimestamp` ## [0.1.1] - 2020-11-20 - Fix
-PyPI install by adding `MANIFEST.in` - Update documentation ## [0.1.0] - 2020-
-11-19 - Initial release on PyPI Keywords: suncalc,sun Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.6
-Description-Content-Type: text/markdown Provides-Extra: pandas Provides-Extra:
-tests
+this simple task... # Changelog ## [0.1.3] - 2023-04-18 - Ensure pandas 2.0
+compatibility (fix integer casting of datetimes) ## [0.1.2] - 2020-12-02 - Try
+to catch NaN before passing to `datetime.utcfromtimestamp` ## [0.1.1] - 2020-
+11-20 - Fix PyPI install by adding `MANIFEST.in` - Update documentation ##
+[0.1.0] - 2020-11-19 - Initial release on PyPI
```

### Comparing `suncalc-0.1.2/README.md` & `suncalc-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
 calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
 etc.) for the given location and time.
 
 [suncalc-js]: https://github.com/mourner/suncalc
 
 While other similar libraries exist, I didn't originally encounter any that met
-my requirements of being both openly-licensed and vectorized <sup>1</sup>
+my requirements of being openly-licensed, vectorized, and simple to use <sup>1</sup>.
 
 ## Install
 
 ```
 pip install suncalc
 ```
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 # suncalc-py
 [Test] [Package_version] [Downloads]
 A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
 calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
 etc.) for the given location and time. [suncalc-js]: https://github.com/
 mourner/suncalc While other similar libraries exist, I didn't originally
-encounter any that met my requirements of being both openly-licensed and
-vectorized 1 ## Install ``` pip install suncalc ``` ## Using ### Example
-`suncalc` is designed to work both with single values and with arrays of
-values. First, import the module: ```py from suncalc import get_position,
+encounter any that met my requirements of being openly-licensed, vectorized,
+and simple to use 1. ## Install ``` pip install suncalc ``` ## Using ###
+Example `suncalc` is designed to work both with single values and with arrays
+of values. First, import the module: ```py from suncalc import get_position,
 get_times from datetime import datetime ``` There are currently two methods:
 `get_position`, to get the sun azimuth and altitude for a given date and
 position, and `get_times`, to get sunlight phases for a given date and
 position. ```py date = datetime.now() lon = 20 lat = 45 get_position(date, lon,
 lat) # {'azimuth': -0.8619668996997687, 'altitude': 0.5586446727994595}
 get_times(date, lon, lat) # {'solar_noon': Timestamp('2020-11-20 08:47:
 08.410863770'), # 'nadir': Timestamp('2020-11-19 20:47:08.410863770'), #
```

### Comparing `suncalc-0.1.2/setup.py` & `suncalc-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,24 +26,26 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description="A fast, vectorized Python port of suncalc.js",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     keywords=['suncalc', 'sun'],
     name='suncalc',
     packages=find_packages(include=['suncalc', 'suncalc.*']),
     setup_requires=setup_requirements,
     extras_require=extra_reqs,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/kylebarron/suncalc-py',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `suncalc-0.1.2/suncalc/suncalc.py` & `suncalc-0.1.3/suncalc/suncalc.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,27 +65,27 @@
     # datetime.datetime
     if isinstance(date, datetime):
         return date.timestamp() * 1000
 
     # Pandas series of Pandas datetime objects
     if pd and pd.api.types.is_datetime64_any_dtype(date):
         # A datetime-like series coerce to int is (always?) in nanoseconds
-        return date.astype(int) / 10 ** 6
+        return date.astype('int64') / 10 ** 6
 
     # Single pandas Timestamp
     if pd and isinstance(date, pd.Timestamp):
         date = date.to_numpy()
 
     # Numpy datetime64
     if np.issubdtype(date.dtype, np.datetime64):
-        return date.astype('datetime64[ms]').astype('int')
+        return date.astype('datetime64[ms]').astype('int64')
 
     # Last-ditch effort
     if pd:
-        return np.array(pd.to_datetime(date).astype(int) / 10 ** 6)
+        return np.array(pd.to_datetime(date).astype('int64') / 10 ** 6)
 
     raise ValueError(f'Unknown date type: {type(date)}')
 
 
 def to_julian(date):
     return to_milliseconds(date) / dayMs - 0.5 + J1970
```

### Comparing `suncalc-0.1.2/suncalc.egg-info/PKG-INFO` & `suncalc-0.1.3/suncalc.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,250 +1,256 @@
 Metadata-Version: 2.1
 Name: suncalc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fast, vectorized Python port of suncalc.js
 Home-page: https://github.com/kylebarron/suncalc-py
 Author: Kyle Barron
 Author-email: kylebarron2@gmail.com
 License: MIT license
-Description: # suncalc-py
-        
-        <p>
-          <a href="https://github.com/kylebarron/suncalc-py/actions?query=workflow%3ACI" target="_blank">
-              <img src="https://github.com/kylebarron/suncalc-py/workflows/test/badge.svg" alt="Test">
-          </a>
-          <a href="https://pypi.org/project/suncalc" target="_blank">
-              <img src="https://img.shields.io/pypi/v/suncalc?color=%2334D058&label=pypi%20package" alt="Package version">
-          </a>
-          <a href="https://github.com/kylebarron/suncalc-py/blob/master/LICENSE" target="_blank">
-              <img src="https://img.shields.io/github/license/kylebarron/suncalc-py.svg" alt="Downloads">
-          </a>
-        </p>
-        
-        
-        A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
-        calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
-        etc.) for the given location and time.
-        
-        [suncalc-js]: https://github.com/mourner/suncalc
-        
-        While other similar libraries exist, I didn't originally encounter any that met
-        my requirements of being both openly-licensed and vectorized <sup>1</sup>
-        
-        ## Install
-        
-        ```
-        pip install suncalc
-        ```
-        
-        ## Using
-        
-        ### Example
-        
-        `suncalc` is designed to work both with single values and with arrays of values.
-        
-        First, import the module:
-        
-        ```py
-        from suncalc import get_position, get_times
-        from datetime import datetime
-        ```
-        
-        There are currently two methods: `get_position`, to get the sun azimuth and
-        altitude for a given date and position, and `get_times`, to get sunlight phases
-        for a given date and position.
-        
-        ```py
-        date = datetime.now()
-        lon = 20
-        lat = 45
-        get_position(date, lon, lat)
-        # {'azimuth': -0.8619668996997687, 'altitude': 0.5586446727994595}
-        
-        get_times(date, lon, lat)
-        # {'solar_noon': Timestamp('2020-11-20 08:47:08.410863770'),
-        #  'nadir': Timestamp('2020-11-19 20:47:08.410863770'),
-        #  'sunrise': Timestamp('2020-11-20 03:13:22.645455322'),
-        #  'sunset': Timestamp('2020-11-20 14:20:54.176272461'),
-        #  'sunrise_end': Timestamp('2020-11-20 03:15:48.318936035'),
-        #  'sunset_start': Timestamp('2020-11-20 14:18:28.502791748'),
-        #  'dawn': Timestamp('2020-11-20 02:50:00.045539551'),
-        #  'dusk': Timestamp('2020-11-20 14:44:16.776188232'),
-        #  'nautical_dawn': Timestamp('2020-11-20 02:23:10.019832520'),
-        #  'nautical_dusk': Timestamp('2020-11-20 15:11:06.801895264'),
-        #  'night_end': Timestamp('2020-11-20 01:56:36.144269287'),
-        #  'night': Timestamp('2020-11-20 15:37:40.677458252'),
-        #  'golden_hour_end': Timestamp('2020-11-20 03:44:46.795967773'),
-        #  'golden_hour': Timestamp('2020-11-20 13:49:30.025760010')}
-        ```
-        
-        These methods also work for _arrays_ of data, and since the implementation is
-        vectorized it's much faster than a for loop in Python.
-        
-        ```py
-        import pandas as pd
-        
-        df = pd.DataFrame({
-            'date': [date] * 10,
-            'lon': [lon] * 10,
-            'lat': [lat] * 10
-        })
-        pd.DataFrame(get_position(df['date'], df['lon'], df['lat']))
-        # azimuth	altitude
-        # 0	-1.485509	-1.048223
-        # 1	-1.485509	-1.048223
-        # ...
-        
-        pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))['solar_noon']
-        # 0   2020-11-20 08:47:08.410863872+00:00
-        # 1   2020-11-20 08:47:08.410863872+00:00
-        # ...
-        # Name: solar_noon, dtype: datetime64[ns, UTC]
-        ```
-        
-        If you want to join this data back to your `DataFrame`, you can use `pd.concat`:
-        
-        ```py
-        times = pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))
-        pd.concat([df, times], axis=1)
-        ```
-        
-        ### API
-        
-        #### `get_position`
-        
-        Calculate sun position (azimuth and altitude) for a given date and
-        latitude/longitude
-        
-        - `date` (`datetime` or a pandas series of datetimes): date and time to find sun position of. **Datetime must be in UTC**.
-        - `lng` (`float` or numpy array of `float`): longitude to find sun position of
-        - `lat` (`float` or numpy array of `float`): latitude to find sun position of
-        
-        Returns a `dict` with two keys: `azimuth` and `altitude`. If the input values
-        were singletons, the `dict`'s values will be floats. Otherwise they'll be numpy
-        arrays of floats.
-        
-        #### `get_times`
-        
-        - `date` (`datetime` or a pandas series of datetimes): date and time to find sunlight phases of. **Datetime must be in UTC**.
-        - `lng` (`float` or numpy array of `float`): longitude to find sunlight phases of
-        - `lat` (`float` or numpy array of `float`): latitude to find sunlight phases of
-        - `height` (`float` or numpy array of `float`, default `0`): observer height in meters
-        - `times` (`Iterable[Tuple[float, str, str]]`): an iterable defining the angle above the horizon and strings for custom sunlight phases. The default is:
-        
-            ```py
-            # (angle, morning name, evening name)
-            DEFAULT_TIMES = [
-                (-0.833, 'sunrise', 'sunset'),
-                (-0.3, 'sunrise_end', 'sunset_start'),
-                (-6, 'dawn', 'dusk'),
-                (-12, 'nautical_dawn', 'nautical_dusk'),
-                (-18, 'night_end', 'night'),
-                (6, 'golden_hour_end', 'golden_hour')
-            ]
-            ```
-        
-        Returns a `dict` where the keys are `solar_noon`, `nadir`, plus any keys passed
-        in the `times` argument. If the input values were singletons, the `dict`'s
-        values will be of type `datetime.datetime` (or `pd.Timestamp` if you have pandas
-        installed, which is a subclass of and therefore compatible with
-        `datetime.datetime`). Otherwise they'll be pandas `DateTime` series. **The
-        returned times will be in UTC.**
-        
-        ## Benchmark
-        
-        This benchmark is to show that the vectorized implementation is nearly 100x
-        faster than a for loop in Python.
-        
-        First set up a `DataFrame` with random data. Here I create 100,000 rows.
-        
-        ```py
-        from suncalc import get_position, get_times
-        import pandas as pd
-        
-        def random_dates(start, end, n=10):
-            """Create an array of random dates"""
-            start_u = start.value//10**9
-            end_u = end.value//10**9
-            return pd.to_datetime(np.random.randint(start_u, end_u, n), unit='s')
-        
-        start = pd.to_datetime('2015-01-01')
-        end = pd.to_datetime('2018-01-01')
-        dates = random_dates(start, end, n=100_000)
-        
-        lons = np.random.uniform(low=-179, high=179, size=(100_000,))
-        lats = np.random.uniform(low=-89, high=89, size=(100_000,))
-        
-        df = pd.DataFrame({'date': dates, 'lat': lats, 'lon': lons})
-        ```
-        
-        Then compute `SunCalc.get_position` two ways: the first using the vectorized
-        implementation and the second using `df.apply`, which is equivalent to a for
-        loop. The first is more than **100x faster** than the second.
-        
-        ```py
-        %timeit get_position(df['date'], df['lon'], df['lat'])
-        # 41.4 ms ± 437 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
-        
-        %timeit df.apply(lambda row: get_position(row['date'], row['lon'], row['lat']), axis=1)
-        # 4.89 s ± 184 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
-        ```
-        
-        Likewise, compute `SunCalc.get_times` the same two ways: first using the
-        vectorized implementation and the second using `df.apply`. The first is **2800x
-        faster** than the second! Some of the difference here is that under the hood the
-        non-vectorized approach uses `pd.to_datetime` while the vectorized
-        implementation uses `np.astype('datetime64[ns, UTC]')`. `pd.to_datetime` is
-        really slow!!
-        
-        ```py
-        %timeit get_times(df['date'], df['lon'], df['lat'])
-        # 55.3 ms ± 1.91 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
-        
-        %time df.apply(lambda row: get_times(row['date'], row['lon'], row['lat']), axis=1)
-        # CPU times: user 2min 33s, sys: 288 ms, total: 2min 34s
-        # Wall time: 2min 34s
-        ```
-        
-        ---
-        
-        1: [`pyorbital`](https://github.com/pytroll/pyorbital) looks great but is
-        GPL3-licensed; [`pysolar`](https://github.com/pingswept/pysolar) is also
-        GPL3-licensed; [`pyEphem`](https://rhodesmill.org/pyephem/) is LGPL3-licensed.
-        [`suncalcPy`](https://github.com/Broham/suncalcPy) is another port of
-        `suncalc.js`, and is MIT-licensed, but doesn't use Numpy and thus isn't
-        vectorized. I recently discovered [`sunpy`](https://github.com/sunpy/sunpy) and
-        [`astropy`](https://github.com/astropy/astropy), both of which probably would've
-        worked but I didn't see them at first and they look quite complex for this
-        simple task...
-        
-        
-        # Changelog
-        
-        ## [0.1.2] - 2020-12-02
-        
-        - Try to catch NaN before passing to `datetime.utcfromtimestamp`
-        
-        ## [0.1.1] - 2020-11-20
-        
-        - Fix PyPI install by adding `MANIFEST.in`
-        - Update documentation
-        
-        ## [0.1.0] - 2020-11-19
-        
-        - Initial release on PyPI
-        
 Keywords: suncalc,sun
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: tests
+License-File: LICENSE
+
+# suncalc-py
+
+<p>
+  <a href="https://github.com/kylebarron/suncalc-py/actions?query=workflow%3ACI" target="_blank">
+      <img src="https://github.com/kylebarron/suncalc-py/workflows/test/badge.svg" alt="Test">
+  </a>
+  <a href="https://pypi.org/project/suncalc" target="_blank">
+      <img src="https://img.shields.io/pypi/v/suncalc?color=%2334D058&label=pypi%20package" alt="Package version">
+  </a>
+  <a href="https://github.com/kylebarron/suncalc-py/blob/master/LICENSE" target="_blank">
+      <img src="https://img.shields.io/github/license/kylebarron/suncalc-py.svg" alt="Downloads">
+  </a>
+</p>
+
+
+A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
+calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
+etc.) for the given location and time.
+
+[suncalc-js]: https://github.com/mourner/suncalc
+
+While other similar libraries exist, I didn't originally encounter any that met
+my requirements of being openly-licensed, vectorized, and simple to use <sup>1</sup>.
+
+## Install
+
+```
+pip install suncalc
+```
+
+## Using
+
+### Example
+
+`suncalc` is designed to work both with single values and with arrays of values.
+
+First, import the module:
+
+```py
+from suncalc import get_position, get_times
+from datetime import datetime
+```
+
+There are currently two methods: `get_position`, to get the sun azimuth and
+altitude for a given date and position, and `get_times`, to get sunlight phases
+for a given date and position.
+
+```py
+date = datetime.now()
+lon = 20
+lat = 45
+get_position(date, lon, lat)
+# {'azimuth': -0.8619668996997687, 'altitude': 0.5586446727994595}
+
+get_times(date, lon, lat)
+# {'solar_noon': Timestamp('2020-11-20 08:47:08.410863770'),
+#  'nadir': Timestamp('2020-11-19 20:47:08.410863770'),
+#  'sunrise': Timestamp('2020-11-20 03:13:22.645455322'),
+#  'sunset': Timestamp('2020-11-20 14:20:54.176272461'),
+#  'sunrise_end': Timestamp('2020-11-20 03:15:48.318936035'),
+#  'sunset_start': Timestamp('2020-11-20 14:18:28.502791748'),
+#  'dawn': Timestamp('2020-11-20 02:50:00.045539551'),
+#  'dusk': Timestamp('2020-11-20 14:44:16.776188232'),
+#  'nautical_dawn': Timestamp('2020-11-20 02:23:10.019832520'),
+#  'nautical_dusk': Timestamp('2020-11-20 15:11:06.801895264'),
+#  'night_end': Timestamp('2020-11-20 01:56:36.144269287'),
+#  'night': Timestamp('2020-11-20 15:37:40.677458252'),
+#  'golden_hour_end': Timestamp('2020-11-20 03:44:46.795967773'),
+#  'golden_hour': Timestamp('2020-11-20 13:49:30.025760010')}
+```
+
+These methods also work for _arrays_ of data, and since the implementation is
+vectorized it's much faster than a for loop in Python.
+
+```py
+import pandas as pd
+
+df = pd.DataFrame({
+    'date': [date] * 10,
+    'lon': [lon] * 10,
+    'lat': [lat] * 10
+})
+pd.DataFrame(get_position(df['date'], df['lon'], df['lat']))
+# azimuth	altitude
+# 0	-1.485509	-1.048223
+# 1	-1.485509	-1.048223
+# ...
+
+pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))['solar_noon']
+# 0   2020-11-20 08:47:08.410863872+00:00
+# 1   2020-11-20 08:47:08.410863872+00:00
+# ...
+# Name: solar_noon, dtype: datetime64[ns, UTC]
+```
+
+If you want to join this data back to your `DataFrame`, you can use `pd.concat`:
+
+```py
+times = pd.DataFrame(get_times(df['date'], df['lon'], df['lat']))
+pd.concat([df, times], axis=1)
+```
+
+### API
+
+#### `get_position`
+
+Calculate sun position (azimuth and altitude) for a given date and
+latitude/longitude
+
+- `date` (`datetime` or a pandas series of datetimes): date and time to find sun position of. **Datetime must be in UTC**.
+- `lng` (`float` or numpy array of `float`): longitude to find sun position of
+- `lat` (`float` or numpy array of `float`): latitude to find sun position of
+
+Returns a `dict` with two keys: `azimuth` and `altitude`. If the input values
+were singletons, the `dict`'s values will be floats. Otherwise they'll be numpy
+arrays of floats.
+
+#### `get_times`
+
+- `date` (`datetime` or a pandas series of datetimes): date and time to find sunlight phases of. **Datetime must be in UTC**.
+- `lng` (`float` or numpy array of `float`): longitude to find sunlight phases of
+- `lat` (`float` or numpy array of `float`): latitude to find sunlight phases of
+- `height` (`float` or numpy array of `float`, default `0`): observer height in meters
+- `times` (`Iterable[Tuple[float, str, str]]`): an iterable defining the angle above the horizon and strings for custom sunlight phases. The default is:
+
+    ```py
+    # (angle, morning name, evening name)
+    DEFAULT_TIMES = [
+        (-0.833, 'sunrise', 'sunset'),
+        (-0.3, 'sunrise_end', 'sunset_start'),
+        (-6, 'dawn', 'dusk'),
+        (-12, 'nautical_dawn', 'nautical_dusk'),
+        (-18, 'night_end', 'night'),
+        (6, 'golden_hour_end', 'golden_hour')
+    ]
+    ```
+
+Returns a `dict` where the keys are `solar_noon`, `nadir`, plus any keys passed
+in the `times` argument. If the input values were singletons, the `dict`'s
+values will be of type `datetime.datetime` (or `pd.Timestamp` if you have pandas
+installed, which is a subclass of and therefore compatible with
+`datetime.datetime`). Otherwise they'll be pandas `DateTime` series. **The
+returned times will be in UTC.**
+
+## Benchmark
+
+This benchmark is to show that the vectorized implementation is nearly 100x
+faster than a for loop in Python.
+
+First set up a `DataFrame` with random data. Here I create 100,000 rows.
+
+```py
+from suncalc import get_position, get_times
+import pandas as pd
+
+def random_dates(start, end, n=10):
+    """Create an array of random dates"""
+    start_u = start.value//10**9
+    end_u = end.value//10**9
+    return pd.to_datetime(np.random.randint(start_u, end_u, n), unit='s')
+
+start = pd.to_datetime('2015-01-01')
+end = pd.to_datetime('2018-01-01')
+dates = random_dates(start, end, n=100_000)
+
+lons = np.random.uniform(low=-179, high=179, size=(100_000,))
+lats = np.random.uniform(low=-89, high=89, size=(100_000,))
+
+df = pd.DataFrame({'date': dates, 'lat': lats, 'lon': lons})
+```
+
+Then compute `SunCalc.get_position` two ways: the first using the vectorized
+implementation and the second using `df.apply`, which is equivalent to a for
+loop. The first is more than **100x faster** than the second.
+
+```py
+%timeit get_position(df['date'], df['lon'], df['lat'])
+# 41.4 ms ± 437 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+
+%timeit df.apply(lambda row: get_position(row['date'], row['lon'], row['lat']), axis=1)
+# 4.89 s ± 184 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+```
+
+Likewise, compute `SunCalc.get_times` the same two ways: first using the
+vectorized implementation and the second using `df.apply`. The first is **2800x
+faster** than the second! Some of the difference here is that under the hood the
+non-vectorized approach uses `pd.to_datetime` while the vectorized
+implementation uses `np.astype('datetime64[ns, UTC]')`. `pd.to_datetime` is
+really slow!!
+
+```py
+%timeit get_times(df['date'], df['lon'], df['lat'])
+# 55.3 ms ± 1.91 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
+
+%time df.apply(lambda row: get_times(row['date'], row['lon'], row['lat']), axis=1)
+# CPU times: user 2min 33s, sys: 288 ms, total: 2min 34s
+# Wall time: 2min 34s
+```
+
+---
+
+1: [`pyorbital`](https://github.com/pytroll/pyorbital) looks great but is
+GPL3-licensed; [`pysolar`](https://github.com/pingswept/pysolar) is also
+GPL3-licensed; [`pyEphem`](https://rhodesmill.org/pyephem/) is LGPL3-licensed.
+[`suncalcPy`](https://github.com/Broham/suncalcPy) is another port of
+`suncalc.js`, and is MIT-licensed, but doesn't use Numpy and thus isn't
+vectorized. I recently discovered [`sunpy`](https://github.com/sunpy/sunpy) and
+[`astropy`](https://github.com/astropy/astropy), both of which probably would've
+worked but I didn't see them at first and they look quite complex for this
+simple task...
+
+
+# Changelog
+
+## [0.1.3] - 2023-04-18
+
+- Ensure pandas 2.0 compatibility (fix integer casting of datetimes)
+
+## [0.1.2] - 2020-12-02
+
+- Try to catch NaN before passing to `datetime.utcfromtimestamp`
+
+## [0.1.1] - 2020-11-20
+
+- Fix PyPI install by adding `MANIFEST.in`
+- Update documentation
+
+## [0.1.0] - 2020-11-19
+
+- Initial release on PyPI
```

#### html2text {}

```diff
@@ -1,20 +1,29 @@
-Metadata-Version: 2.1 Name: suncalc Version: 0.1.2 Summary: A fast, vectorized
+Metadata-Version: 2.1 Name: suncalc Version: 0.1.3 Summary: A fast, vectorized
 Python port of suncalc.js Home-page: https://github.com/kylebarron/suncalc-py
 Author: Kyle Barron Author-email: kylebarron2@gmail.com License: MIT license
-Description: # suncalc-py
+Keywords: suncalc,sun Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.6 Description-Content-Type:
+text/markdown Provides-Extra: pandas Provides-Extra: tests License-File:
+LICENSE # suncalc-py
 [Test] [Package_version] [Downloads]
 A fast, vectorized Python implementation of [`suncalc.js`][suncalc-js] for
 calculating sun position and sunlight phases (times for sunrise, sunset, dusk,
 etc.) for the given location and time. [suncalc-js]: https://github.com/
 mourner/suncalc While other similar libraries exist, I didn't originally
-encounter any that met my requirements of being both openly-licensed and
-vectorized 1 ## Install ``` pip install suncalc ``` ## Using ### Example
-`suncalc` is designed to work both with single values and with arrays of
-values. First, import the module: ```py from suncalc import get_position,
+encounter any that met my requirements of being openly-licensed, vectorized,
+and simple to use 1. ## Install ``` pip install suncalc ``` ## Using ###
+Example `suncalc` is designed to work both with single values and with arrays
+of values. First, import the module: ```py from suncalc import get_position,
 get_times from datetime import datetime ``` There are currently two methods:
 `get_position`, to get the sun azimuth and altitude for a given date and
 position, and `get_times`, to get sunlight phases for a given date and
 position. ```py date = datetime.now() lon = 20 lat = 45 get_position(date, lon,
 lat) # {'azimuth': -0.8619668996997687, 'altitude': 0.5586446727994595}
 get_times(date, lon, lat) # {'solar_noon': Timestamp('2020-11-20 08:47:
 08.410863770'), # 'nadir': Timestamp('2020-11-19 20:47:08.410863770'), #
@@ -91,19 +100,12 @@
 licensed; [`pysolar`](https://github.com/pingswept/pysolar) is also GPL3-
 licensed; [`pyEphem`](https://rhodesmill.org/pyephem/) is LGPL3-licensed.
 [`suncalcPy`](https://github.com/Broham/suncalcPy) is another port of
 `suncalc.js`, and is MIT-licensed, but doesn't use Numpy and thus isn't
 vectorized. I recently discovered [`sunpy`](https://github.com/sunpy/sunpy) and
 [`astropy`](https://github.com/astropy/astropy), both of which probably
 would've worked but I didn't see them at first and they look quite complex for
-this simple task... # Changelog ## [0.1.2] - 2020-12-02 - Try to catch NaN
-before passing to `datetime.utcfromtimestamp` ## [0.1.1] - 2020-11-20 - Fix
-PyPI install by adding `MANIFEST.in` - Update documentation ## [0.1.0] - 2020-
-11-19 - Initial release on PyPI Keywords: suncalc,sun Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.6
-Description-Content-Type: text/markdown Provides-Extra: pandas Provides-Extra:
-tests
+this simple task... # Changelog ## [0.1.3] - 2023-04-18 - Ensure pandas 2.0
+compatibility (fix integer casting of datetimes) ## [0.1.2] - 2020-12-02 - Try
+to catch NaN before passing to `datetime.utcfromtimestamp` ## [0.1.1] - 2020-
+11-20 - Fix PyPI install by adding `MANIFEST.in` - Update documentation ##
+[0.1.0] - 2020-11-19 - Initial release on PyPI
```


# Comparing `tmp/phm_feature-0.1.0.tar.gz` & `tmp/phm_feature-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phm_feature-0.1.0.tar", last modified: Mon Mar 20 07:43:26 2023, max compression
+gzip compressed data, was "phm_feature-0.1.1.tar", last modified: Wed Apr 19 08:43:30 2023, max compression
```

## Comparing `phm_feature-0.1.0.tar` & `phm_feature-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxr-x   0 qsy       (1000) qsy       (1000)        0 2023-03-20 07:43:26.926478 phm_feature-0.1.0/
--rw-rw-r--   0 qsy       (1000) qsy       (1000)     1074 2022-10-13 06:30:26.000000 phm_feature-0.1.0/LICENSE
--rw-rw-r--   0 qsy       (1000) qsy       (1000)     3142 2023-03-20 07:43:26.926478 phm_feature-0.1.0/PKG-INFO
--rw-rw-r--   0 qsy       (1000) qsy       (1000)     2095 2023-02-09 02:59:36.000000 phm_feature-0.1.0/README.md
-drwxrwxr-x   0 qsy       (1000) qsy       (1000)        0 2023-03-20 07:43:26.926478 phm_feature-0.1.0/phm_feature/
--rw-rw-r--   0 qsy       (1000) qsy       (1000)    10884 2023-03-20 07:16:24.000000 phm_feature-0.1.0/phm_feature/__init__.py
-drwxrwxr-x   0 qsy       (1000) qsy       (1000)        0 2023-03-20 07:43:26.926478 phm_feature-0.1.0/phm_feature.egg-info/
--rw-rw-r--   0 qsy       (1000) qsy       (1000)     3142 2023-03-20 07:43:26.000000 phm_feature-0.1.0/phm_feature.egg-info/PKG-INFO
--rw-rw-r--   0 qsy       (1000) qsy       (1000)      190 2023-03-20 07:43:26.000000 phm_feature-0.1.0/phm_feature.egg-info/SOURCES.txt
--rw-rw-r--   0 qsy       (1000) qsy       (1000)        1 2023-03-20 07:43:26.000000 phm_feature-0.1.0/phm_feature.egg-info/dependency_links.txt
--rw-rw-r--   0 qsy       (1000) qsy       (1000)       12 2023-03-20 07:43:26.000000 phm_feature-0.1.0/phm_feature.egg-info/top_level.txt
--rw-rw-r--   0 qsy       (1000) qsy       (1000)       38 2023-03-20 07:43:26.926478 phm_feature-0.1.0/setup.cfg
--rw-rw-r--   0 qsy       (1000) qsy       (1000)      550 2023-03-20 05:28:07.000000 phm_feature-0.1.0/setup.py
+drwxrwxr-x   0 qsy       (1000) qsy       (1000)        0 2023-04-19 08:43:30.243554 phm_feature-0.1.1/
+-rwx------   0 qsy       (1000) qsy       (1000)     1074 2022-10-13 06:30:26.000000 phm_feature-0.1.1/LICENSE
+-rw-rw-r--   0 qsy       (1000) qsy       (1000)     6917 2023-04-19 08:43:30.243554 phm_feature-0.1.1/PKG-INFO
+-rwx------   0 qsy       (1000) qsy       (1000)     5078 2023-03-21 06:25:19.000000 phm_feature-0.1.1/README.md
+drwxrwxr-x   0 qsy       (1000) qsy       (1000)        0 2023-04-19 08:43:30.243554 phm_feature-0.1.1/phm_feature/
+-rwx------   0 qsy       (1000) qsy       (1000)    12618 2023-04-19 08:41:03.000000 phm_feature-0.1.1/phm_feature/__init__.py
+drwxrwxr-x   0 qsy       (1000) qsy       (1000)        0 2023-04-19 08:43:30.243554 phm_feature-0.1.1/phm_feature/torchphm/
+-rwx------   0 qsy       (1000) qsy       (1000)       76 2023-04-19 08:41:03.000000 phm_feature-0.1.1/phm_feature/torchphm/__init__.py
+-rwx------   0 qsy       (1000) qsy       (1000)     5822 2023-04-19 08:41:03.000000 phm_feature-0.1.1/phm_feature/torchphm/beta_hpss.py
+-rwx------   0 qsy       (1000) qsy       (1000)    11652 2023-04-19 08:41:03.000000 phm_feature-0.1.1/phm_feature/torchphm/functional.py
+-rwx------   0 qsy       (1000) qsy       (1000)    16333 2023-04-19 08:41:03.000000 phm_feature-0.1.1/phm_feature/torchphm/layers.py
+drwxrwxr-x   0 qsy       (1000) qsy       (1000)        0 2023-04-19 08:43:30.243554 phm_feature-0.1.1/phm_feature.egg-info/
+-rwx------   0 qsy       (1000) qsy       (1000)     6917 2023-04-19 08:43:30.000000 phm_feature-0.1.1/phm_feature.egg-info/PKG-INFO
+-rwx------   0 qsy       (1000) qsy       (1000)      323 2023-04-19 08:43:30.000000 phm_feature-0.1.1/phm_feature.egg-info/SOURCES.txt
+-rwx------   0 qsy       (1000) qsy       (1000)        1 2023-04-19 08:43:30.000000 phm_feature-0.1.1/phm_feature.egg-info/dependency_links.txt
+-rwx------   0 qsy       (1000) qsy       (1000)       12 2023-04-19 08:43:30.000000 phm_feature-0.1.1/phm_feature.egg-info/top_level.txt
+-rw-rw-r--   0 qsy       (1000) qsy       (1000)       38 2023-04-19 08:43:30.243554 phm_feature-0.1.1/setup.cfg
+-rwx------   0 qsy       (1000) qsy       (1000)      550 2023-04-19 08:42:32.000000 phm_feature-0.1.1/setup.py
```

### Comparing `phm_feature-0.1.0/LICENSE` & `phm_feature-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phm_feature-0.1.0/phm_feature/__init__.py` & `phm_feature-0.1.1/phm_feature/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 from __future__ import absolute_import, unicode_literals
+import pdb
 import collections
-import scipy.fftpack
-import scipy.signal
-import scipy.stats
+import scipy
+#from scipy import fftpack, signal, stats
+#import scipy.fftpack
+#import scipy.signal
+#import scipy.stats
 import logging
 import sys
 import threading
 import numpy as np
 from functools import partial
 from multiprocessing import cpu_count
 from multiprocessing import Pool
 import os
+import json
+import torch
+from .torchphm.functional import (
+    stft,
+    phase_vocoder,
+    magphase,
+    amplitude_to_db,
+    db_to_amplitude,
+    complex_norm,
+    mu_law_encoding,
+    mu_law_decoding,
+    apply_filterbank,
+)
 
 """phm 设备故障与寿命分析
 提取振动信号中的基础，时频域特征，用于phm用途
 """
 
 __version__ = '0.1.0'
 __license__ = 'MIT'
@@ -71,24 +87,27 @@
                 ict["result"].append({"key":key, "value":dic[key], "description":"裕度因子"})
             elif key == "form_factor":
                 ict["result"].append({"key":key, "value":dic[key], "description":"波形因子"})
             elif key == "kurtosis":
                 ict["result"].append({"key":key, "value":dic[key], "description":"峭度"})
             elif key == "skewness":
                 ict["result"].append({"key":key, "value":dic[key], "description":"偏斜度"})
-        print(dict(ict))
-        return dict(ict)
+        #print(dict(ict))
+        return json.dumps(dict(ict))
 
     def __repr__(self):
         return 'Tokenizer of vibration-wave {}'.format(self.name)
 
     def feature_t(self, s):
         '''提取时间域特征
         '''
-        print("串行提取时域特征")
+        assert type(s) == str
+        s = np.array(json.loads(s))
+        #s = s.tolist()
+        #print("串行提取时域特征")
         dct = self.init_result()
 
         _mean = np.mean(s, axis=-1)
         dct["mean"] = _mean.tolist()
 
         _max = np.max(s, axis=-1)
         dct["max"] = _max.tolist()
@@ -134,16 +153,54 @@
         dct["skewness"] = _skewness.tolist()
 
         _form_factor = _rms/_arv
         dct["form_factor"] = _form_factor.tolist()
 
         return self.rebuild_time_result(dct)
 
-    def feature_f(self, array, fs):
-        raise Exception('oh friend, sorry, this functions is not finish yet')
+    def feature_f(self, s, fs, fft_length, hop_length, pad_mode):
+        '''
+        提取频域数据
+        默认选择hamming窗体
+        '''
+        try:
+
+            fs = float(fs)
+
+            assert type(s) == str
+            assert type(fs) == float
+
+            import pdb
+            #pdb.set_trace()
+    
+            waveform = np.array(json.loads(s)) # 2d array 所采集的振动数据
+            #print(waveform.shape[-1])
+            
+            Fs = self.fs2Fs(waveform.shape[-1], fs) # 频率分辨率的arraylist
+
+
+            pad = fft_length // 2
+            window = torch.hann_window(fft_length)
+            complex_spec = stft(
+                torch.Tensor(waveform),
+                fft_length=fft_length,
+                hop_length=hop_length,
+                window=window,
+                pad_mode=pad_mode,
+            )
+            mag_spec, phase_spec = magphase(complex_spec)
+            import pdb
+            magnitude = json.dumps(mag_spec.numpy().tolist())
+            phase = json.dumps(phase_spec.numpy().tolist())
+            fft_complex = json.dumps(complex_spec.numpy().tolist())
+            return {"magnitude":magnitude, "phase":phase, "fft_complex":fft_complex}
+
+        except AssertionError:
+    
+            raise Exception('assertion Error, pls double check \ntype(s) == str \ntype(fs) == float')
 
     def fft(self, array, num):
         return scipy.fftpack.fft(array, num)
 
     def power(self, array, num):
         return (np.abs(scipy.fftpack.fft(array, num))**2)/num
 
@@ -166,40 +223,43 @@
         mag = np.abs(xh3) * 2
         #fre = np.linspace(0, fs / 2, int(len(xe) / 2 + 1))
         return mag
 
     def yin(self, s, window_size):
         '''YIN方法找一倍频率'''
         yin_s = []
-        print(s.shape, window_size)
+        #print(s.shape, window_size)
         assert window_size < s.shape[-1]
         start_l, start_r = 0, window_size
         end_l, end_r = 0, window_size
         while(True):
             yin_s.append(np.subtract(s[:,end_l:end_r], s[:,start_l:start_r]))
             end_l+=1
             end_r+=1
             if end_r > s.shape[-1]:
                 break
         return np.array(yin_s)
 
     def fs2Fs(self, L, fs):
-        '''通过采样频率和采样时长，计算频谱刻度
-           sample-freq and sample-time calculate the list of Freqs mini units
+        ''' L 采样点数
+            fs 采样频率
+            :fre: 频率分辨率
+
+            除2是考虑到傅立叶变换的对称性
         '''
         fre = np.linspace(0, fs / 2, int(L / 2 + 1))
         return fre
 
     def window(self, array, window_type='hamming'):
         '''chunk size
         '''
         if window_type == "hamming":
             return np.multiply(np.hamming(array.shape[-1]), array)
         else:
-            raise Exception('Oh, my friend. u should specified the window name first')
+            raise Exception('you should specified the window name first, default can be hamming')
 
     def divide(self, array, window_size, hop_size):
         ''' chunk request hop_size is (0,0.5)*window_size
         '''
         results = []
         start,end,shape = 0,window_size,array.shape
         while(True):
@@ -258,21 +318,21 @@
 
 def _pyin(s, window_size):
     _s = [np.array(_).reshape(1,-1) for _ in s.tolist()]
     result = pool.map(partial(_yin, window_size=window_size), _s)
     return result
 
 def _pfeature_t(s):
-    print("并行提取时域特征")
+    #print("并行提取时域特征")
     _s = [np.array(_).reshape(1,-1) for _ in s.tolist()]
     result = pool.map(_feature_t, _s)
     return result
 
 def _pfeature_f(s, fs):
-    pass
+    raise NotImplementedError("频域特征的并行提取，暂时不支持多线程")
 
 def _pfft(s, num):
     _s = [np.array(_).reshape(1,-1) for _ in s.tolist()]
     result = pool.map(partial(_fft, num=num), _s)
     return result
 
 def _ppower(s, n):
```

### Comparing `phm_feature-0.1.0/setup.py` & `phm_feature-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="phm_feature",
-  version="0.1.0",
+  version="0.1.1",
   author="QinHaiNing",
   author_email="2364839934@qq.com",
   description="time-freq feature from signal for phm purpose",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="",
   packages=setuptools.find_packages(),
```


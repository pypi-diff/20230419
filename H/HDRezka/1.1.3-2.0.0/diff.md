# Comparing `tmp/HDRezka-1.1.3.tar.gz` & `tmp/HDRezka-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HDRezka-1.1.3.tar", last modified: Sat Apr  8 04:08:49 2023, max compression
+gzip compressed data, was "HDRezka-2.0.0.tar", last modified: Wed Apr 19 13:13:51 2023, max compression
```

## Comparing `HDRezka-1.1.3.tar` & `HDRezka-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 04:08:49.210662 HDRezka-1.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-08 04:08:49.163772 HDRezka-1.1.3/HDRezka.egg-info/
--rw-rw-rw-   0        0        0     3284 2023-04-08 04:08:48.000000 HDRezka-1.1.3/HDRezka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-04-08 04:08:48.000000 HDRezka-1.1.3/HDRezka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 04:08:48.000000 HDRezka-1.1.3/HDRezka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-08 04:08:48.000000 HDRezka-1.1.3/HDRezka.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-08 04:08:48.000000 HDRezka-1.1.3/HDRezka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3284 2023-04-08 04:08:49.210662 HDRezka-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-04-08 04:06:20.000000 HDRezka-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 04:08:49.195129 HDRezka-1.1.3/hdrezka/
--rw-rw-rw-   0        0        0      371 2023-04-08 04:06:33.000000 HDRezka-1.1.3/hdrezka/__init__.py
--rw-rw-rw-   0        0        0     1017 2023-04-06 11:53:59.000000 HDRezka-1.1.3/hdrezka/_antiobfuscation.py
--rw-rw-rw-   0        0        0      299 2023-04-08 03:54:33.000000 HDRezka-1.1.3/hdrezka/_bs4.py
-drwxrwxrwx   0        0        0        0 2023-04-08 04:08:49.195129 HDRezka-1.1.3/hdrezka/api/
--rw-rw-rw-   0        0        0       42 2023-04-06 11:57:13.000000 HDRezka-1.1.3/hdrezka/api/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-04-06 12:47:03.000000 HDRezka-1.1.3/hdrezka/api/ajax.py
--rw-rw-rw-   0        0        0      315 2023-04-06 11:55:17.000000 HDRezka-1.1.3/hdrezka/api/http.py
--rw-rw-rw-   0        0        0     1164 2023-04-06 11:53:59.000000 HDRezka-1.1.3/hdrezka/api/search.py
--rw-rw-rw-   0        0        0      365 2023-04-03 09:50:05.000000 HDRezka-1.1.3/hdrezka/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-08 04:08:49.210662 HDRezka-1.1.3/hdrezka/post/
--rw-rw-rw-   0        0        0       40 2023-04-06 11:11:48.000000 HDRezka-1.1.3/hdrezka/post/__init__.py
--rw-rw-rw-   0        0        0      110 2023-04-06 11:12:40.000000 HDRezka-1.1.3/hdrezka/post/_dataclass.py
-drwxrwxrwx   0        0        0        0 2023-04-08 04:08:49.210662 HDRezka-1.1.3/hdrezka/post/info/
--rw-rw-rw-   0        0        0       42 2023-04-02 10:26:20.000000 HDRezka-1.1.3/hdrezka/post/info/__init__.py
--rw-rw-rw-   0        0        0      582 2023-04-06 11:53:58.000000 HDRezka-1.1.3/hdrezka/post/info/fields.py
--rw-rw-rw-   0        0        0     5363 2023-04-06 12:13:34.000000 HDRezka-1.1.3/hdrezka/post/info/info.py
--rw-rw-rw-   0        0        0     3154 2023-04-06 12:24:02.000000 HDRezka-1.1.3/hdrezka/post/page.py
--rw-rw-rw-   0        0        0     2444 2023-04-06 11:57:13.000000 HDRezka-1.1.3/hdrezka/post/post.py
--rw-rw-rw-   0        0        0     3210 2023-04-08 04:03:01.000000 HDRezka-1.1.3/hdrezka/post/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-08 04:08:49.210662 HDRezka-1.1.3/hdrezka/stream/
--rw-rw-rw-   0        0        0       22 2023-04-03 14:41:41.000000 HDRezka-1.1.3/hdrezka/stream/__init__.py
--rw-rw-rw-   0        0        0     2548 2023-04-06 12:11:12.000000 HDRezka-1.1.3/hdrezka/stream/player.py
--rw-rw-rw-   0        0        0      387 2023-04-06 11:53:59.000000 HDRezka-1.1.3/hdrezka/translators.py
--rw-rw-rw-   0        0        0       42 2023-04-08 04:08:49.210662 HDRezka-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2007 2023-04-08 04:03:01.000000 HDRezka-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:13:51.768142 HDRezka-2.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-19 13:13:51.759143 HDRezka-2.0.0/HDRezka.egg-info/
+-rw-rw-rw-   0        0        0     4410 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4410 2023-04-19 13:13:51.767142 HDRezka-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-04-19 13:06:04.000000 HDRezka-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 13:13:51.765144 HDRezka-2.0.0/hdrezka/
+-rw-rw-rw-   0        0        0      901 2023-04-19 13:04:35.000000 HDRezka-2.0.0/hdrezka/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-04-19 10:05:55.000000 HDRezka-2.0.0/hdrezka/_antiobfuscation.py
+-rw-rw-rw-   0        0        0      299 2023-04-08 03:54:33.000000 HDRezka-2.0.0/hdrezka/_bs4.py
+-rw-rw-rw-   0        0        0      365 2023-04-19 12:27:06.000000 HDRezka-2.0.0/hdrezka/errors.py
+-rw-rw-rw-   0        0        0      387 2023-04-06 11:53:59.000000 HDRezka-2.0.0/hdrezka/translators.py
+-rw-rw-rw-   0        0        0       42 2023-04-19 13:13:51.768142 HDRezka-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1992 2023-04-19 13:06:04.000000 HDRezka-2.0.0/setup.py
```

### Comparing `HDRezka-1.1.3/LICENSE` & `HDRezka-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HDRezka-1.1.3/hdrezka/_antiobfuscation.py` & `HDRezka-2.0.0/hdrezka/_antiobfuscation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
-from base64 import b64decode
+from binascii import a2b_base64
 
 __all__ = ('clear_trash',)
 
 _sub_trash = re.compile(
     '#h|//_//|I0A=|I0Ah|I0Aj|I0Ak|I0BA|I0Be|I14=|I14h|I14j|I14k|I15A|I15e|ISE=|ISEh|ISEj|ISEk|ISFA|ISFe|ISM=|ISMh'
     '|ISMj|ISMk|ISNA|ISNe|ISQ=|ISQh|ISQj|ISQk|ISRA|ISRe|IUA=|IUAh|IUAj|IUAk|IUBA|IUBe|IV4=|IV4h|IV4j|IV4k|IV5A|IV5e'
     '|IyE=|IyEh|IyEj|IyEk|IyFA|IyFe|IyM=|IyMh|IyMj|IyMk|IyNA|IyNe|IyQ=|IyQh|IyQj|IyQk|IyRA|IyRe|JCE=|JCEh|JCEj|JCEk'
     '|JCFA|JCFe|JCM=|JCMh|JCMj|JCMk|JCNA|JCNe|JCQ=|JCQh|JCQj|JCQk|JCRA|JCRe|JEA=|JEAh|JEAj|JEAk|JEBA|JEBe|JF4=|JF4h'
     '|JF4j|JF4k|JF5A|JF5e|QCE=|QCEh|QCEj|QCEk|QCFA|QCFe|QCM=|QCMh|QCMj|QCMk|QCNA|QCNe|QCQ=|QCQh|QCQj|QCQk|QCRA|QCRe'
     '|QEA=|QEAh|QEAj|QEAk|QEBA|QEBe|QF4=|QF4h|QF4j|QF4k|QF5A|QF5e|XiE=|XiEh|XiEj|XiEk|XiFA|XiFe|XiM=|XiMh|XiMj|XiMk'
     '|XiNA|XiNe|XiQ=|XiQh|XiQj|XiQk|XiRA|XiRe|XkA=|XkAh|XkAj|XkAk|XkBA|XkBe|Xl4=|Xl4h|Xl4j|Xl4k|Xl5A|Xl5e').sub
 
 
 def clear_trash(trash_string: str) -> str:
-    return b64decode(_sub_trash('', trash_string) + '==').decode()
+    return a2b_base64(b'%b==' % _sub_trash('', trash_string).encode('ASCII')).decode('ASCII')
```

### Comparing `HDRezka-1.1.3/setup.py` & `HDRezka-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 with open('README.md', encoding='UTF-8') as f:
     long_description = f.read().strip()
 with open('CHANGELOG.md', encoding='UTF-8') as f:
     long_description += f'\n\n---\n\n{f.read().strip()}\n'
 
 setuptools.setup(
     name='HDRezka',
-    version='1.1.3',
+    version='2.0.0',
 
     author='Nikita (NIKDISSV)',
     author_email='nikdissv@proton.me',
 
     description='HDRezka (rezka.ag) Python API',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/NIKDISSV-Forever/HDRezka',
     project_urls={
         'GitHub': 'https://github.com/NIKDISSV-Forever/HDRezka',
         'Documentation': 'https://nikdissv-forever.github.io/HDRezka/hdrezka'
     },
-    packages=setuptools.find_packages(),
+    packages=['hdrezka'],
     install_requires=install_requires,
 
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: End Users/Desktop',
```


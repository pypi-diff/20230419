# Comparing `tmp/r2diaphora-0.1.9.3.tar.gz` & `tmp/r2diaphora-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2diaphora-0.1.9.3.tar", last modified: Wed Feb 23 16:52:14 2022, max compression
+gzip compressed data, was "r2diaphora-0.2.1.tar", last modified: Wed Apr 19 13:12:35 2023, max compression
```

## Comparing `r2diaphora-0.1.9.3.tar` & `r2diaphora-0.2.1.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.641075 r2diaphora-0.1.9.3/
--rw-r--r--   0 fdd        (501) staff       (20)    34523 2021-05-17 12:55:35.000000 r2diaphora-0.1.9.3/LICENSE
--rw-r--r--   0 fdd        (501) staff       (20)       82 2021-10-20 18:26:44.000000 r2diaphora-0.1.9.3/MANIFEST.in
--rw-r--r--   0 fdd        (501) staff       (20)      485 2022-02-23 16:52:14.641364 r2diaphora-0.1.9.3/PKG-INFO
--rw-r--r--   0 fdd        (501) staff       (20)     2425 2021-11-09 19:44:19.000000 r2diaphora-0.1.9.3/README.md
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.062986 r2diaphora-0.1.9.3/r2diaphora/
--rw-r--r--   0 fdd        (501) staff       (20)      404 2021-10-29 12:54:17.000000 r2diaphora-0.1.9.3/r2diaphora/__init__.py
--rwxr-xr-x   0 fdd        (501) staff       (20)    93630 2022-02-23 16:43:02.000000 r2diaphora-0.1.9.3/r2diaphora/diaphora.py
--rw-r--r--   0 fdd        (501) staff       (20)    57599 2021-10-07 10:12:37.000000 r2diaphora-0.1.9.3/r2diaphora/diaphora_heuristics.py
--rwxr-xr-x   0 fdd        (501) staff       (20)    41475 2021-10-29 11:08:18.000000 r2diaphora-0.1.9.3/r2diaphora/diaphora_r2.py
--rw-r--r--   0 fdd        (501) staff       (20)     4604 2021-10-11 09:22:38.000000 r2diaphora-0.1.9.3/r2diaphora/difflibparser.py
--rw-r--r--   0 fdd        (501) staff       (20)    13283 2021-10-13 14:49:44.000000 r2diaphora-0.1.9.3/r2diaphora/html_diff.py
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.075574 r2diaphora-0.1.9.3/r2diaphora/idaapi/
--rw-r--r--   0 fdd        (501) staff       (20)        0 2021-10-08 12:02:16.000000 r2diaphora-0.1.9.3/r2diaphora/idaapi/__init__.py
--rw-r--r--   0 fdd        (501) staff       (20)    22885 2021-10-29 12:43:14.000000 r2diaphora-0.1.9.3/r2diaphora/idaapi/idaapi_to_r2.py
--rw-r--r--   0 fdd        (501) staff       (20)    77880 2021-10-08 12:01:52.000000 r2diaphora-0.1.9.3/r2diaphora/idaapi/instructions.py
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.084468 r2diaphora-0.1.9.3/r2diaphora/jkutils/
--rw-r--r--   0 fdd        (501) staff       (20)        0 2021-10-07 11:42:52.000000 r2diaphora-0.1.9.3/r2diaphora/jkutils/__init__.py
--rw-r--r--   0 fdd        (501) staff       (20)     6336 2021-05-17 12:55:35.000000 r2diaphora-0.1.9.3/r2diaphora/jkutils/factor.py
--rw-r--r--   0 fdd        (501) staff       (20)     6107 2021-10-08 12:00:07.000000 r2diaphora-0.1.9.3/r2diaphora/jkutils/graph_hashes.py
--rw-r--r--   0 fdd        (501) staff       (20)    10023 2021-05-17 12:55:35.000000 r2diaphora-0.1.9.3/r2diaphora/jkutils/kfuzzy.py
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.087558 r2diaphora-0.1.9.3/r2diaphora/others/
--rw-r--r--   0 fdd        (501) staff       (20)        0 2021-05-17 12:55:35.000000 r2diaphora-0.1.9.3/r2diaphora/others/__init__.py
--rw-r--r--   0 fdd        (501) staff       (20)     2807 2021-09-30 08:22:55.000000 r2diaphora-0.1.9.3/r2diaphora/others/tarjan_sort.py
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.038145 r2diaphora-0.1.9.3/r2diaphora/pycparser/
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.533073 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.545543 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/X11/
--rw-r--r--   0 fdd        (501) staff       (20)      118 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/X11/Intrinsic.h
--rw-r--r--   0 fdd        (501) staff       (20)      118 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/X11/Xlib.h
--rw-r--r--   0 fdd        (501) staff       (20)      311 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_defines.h
--rw-r--r--   0 fdd        (501) staff       (20)     1111 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/_ansi.h
--rw-r--r--   0 fdd        (501) staff       (20)     5734 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/_fake_defines.h
--rw-r--r--   0 fdd        (501) staff       (20)     7022 2021-10-20 17:38:17.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/_syslist.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/aio.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/alloca.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/ar.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/argz.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.550004 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/arpa/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/arpa/inet.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.557402 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/asm-generic/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/asm-generic/int-ll64.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/assert.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/complex.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/cpio.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/ctype.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/dirent.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/dlfcn.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/emmintrin.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/endian.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/envz.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/errno.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/fastmath.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/fcntl.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/features.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/fenv.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/float.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/fmtmsg.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/fnmatch.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/ftw.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/getopt.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/glob.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/grp.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/iconv.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/ieeefp.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/immintrin.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/inttypes.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/iso646.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/langinfo.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/libgen.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/libintl.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/limits.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.563150 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/linux/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/linux/socket.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/linux/version.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/locale.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/malloc.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/math.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.565287 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/mir_toolkit/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/mir_toolkit/client_types.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/monetary.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/mqueue.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/ndbm.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.567137 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/net/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/net/if.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/netdb.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.569771 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/netinet/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/netinet/in.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/netinet/tcp.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/newlib.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/nl_types.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.576360 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/openssl/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/openssl/err.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/openssl/evp.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/openssl/hmac.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/openssl/ssl.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/openssl/x509v3.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/paths.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/poll.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/process.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/pthread.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/pwd.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/reent.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/regdef.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/regex.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sched.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/search.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/semaphore.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/setjmp.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/signal.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/smmintrin.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/spawn.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stdarg.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stdatomic.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stdbool.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stddef.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stdint.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stdio.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stdlib.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stdnoreturn.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/string.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/strings.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/stropts.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.606732 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/ioctl.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/ipc.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/mman.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/msg.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/poll.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/resource.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/select.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/sem.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/shm.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/socket.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/stat.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/statvfs.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/sysctl.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/time.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/times.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/types.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/uio.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/un.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/utsname.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/sys/wait.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/syslog.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/tar.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/termios.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/tgmath.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/threads.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/time.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/trace.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/ulimit.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/unctrl.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/unistd.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/utime.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/utmp.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/utmpx.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/wchar.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/wctype.h
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/wordexp.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.607947 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/xcb/
--rw-r--r--   0 fdd        (501) staff       (20)       55 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/xcb/xcb.h
--rw-r--r--   0 fdd        (501) staff       (20)      514 2021-09-26 19:04:51.000000 r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/zlib.h
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.045247 r2diaphora-0.1.9.3/r2diaphora/signatures/
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.626522 r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/
--rw-rw-r--   0 fdd        (501) staff       (20)    32585 2018-06-20 23:08:39.000000 r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_arm.sig
--rw-rw-r--   0 fdd        (501) staff       (20)    44648 2018-06-20 23:08:39.000000 r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_mips.sig
--rw-rw-r--   0 fdd        (501) staff       (20)    42356 2018-06-20 23:08:39.000000 r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_ppc.sig
--rw-rw-r--   0 fdd        (501) staff       (20)    32757 2018-06-20 23:08:39.000000 r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_sh4.sig
--rw-rw-r--   0 fdd        (501) staff       (20)    31653 2018-06-20 23:08:39.000000 r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_x86-64.sig
--rw-rw-r--   0 fdd        (501) staff       (20)    53445 2018-06-20 23:08:39.000000 r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_x86.sig
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.069586 r2diaphora-0.1.9.3/r2diaphora.egg-info/
--rw-r--r--   0 fdd        (501) staff       (20)      485 2022-02-23 16:52:13.000000 r2diaphora-0.1.9.3/r2diaphora.egg-info/PKG-INFO
--rw-r--r--   0 fdd        (501) staff       (20)     7329 2022-02-23 16:52:14.000000 r2diaphora-0.1.9.3/r2diaphora.egg-info/SOURCES.txt
--rw-r--r--   0 fdd        (501) staff       (20)        1 2022-02-23 16:52:13.000000 r2diaphora-0.1.9.3/r2diaphora.egg-info/dependency_links.txt
--rw-r--r--   0 fdd        (501) staff       (20)       60 2022-02-23 16:52:13.000000 r2diaphora-0.1.9.3/r2diaphora.egg-info/entry_points.txt
--rw-r--r--   0 fdd        (501) staff       (20)      128 2022-02-23 16:52:13.000000 r2diaphora-0.1.9.3/r2diaphora.egg-info/requires.txt
--rw-r--r--   0 fdd        (501) staff       (20)       11 2022-02-23 16:52:13.000000 r2diaphora-0.1.9.3/r2diaphora.egg-info/top_level.txt
-drwxr-xr-x   0 fdd        (501) staff       (20)        0 2022-02-23 16:52:14.636099 r2diaphora-0.1.9.3/scripts/
--rwxr--r--   0 fdd        (501) staff       (20)      802 2021-10-07 11:19:24.000000 r2diaphora-0.1.9.3/scripts/r2diaphora-bulk
--rw-r--r--   0 fdd        (501) staff       (20)     2231 2021-11-09 19:44:41.000000 r2diaphora-0.1.9.3/scripts/r2diaphora-db
--rw-r--r--   0 fdd        (501) staff       (20)       79 2022-02-23 16:52:14.645365 r2diaphora-0.1.9.3/setup.cfg
--rw-r--r--   0 fdd        (501) staff       (20)     2071 2022-02-23 16:33:30.000000 r2diaphora-0.1.9.3/setup.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.583198 r2diaphora-0.2.1/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/LICENSE
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/MANIFEST.in
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-04-19 13:12:35.583198 r2diaphora-0.2.1/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/README.md
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.563198 r2diaphora-0.2.1/r2diaphora/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/__init__.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94376 2023-04-19 13:10:17.000000 r2diaphora-0.2.1/r2diaphora/diaphora.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/diaphora_heuristics.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    41477 2023-04-12 10:01:32.000000 r2diaphora-0.2.1/r2diaphora/diaphora_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/difflibparser.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/html_diff.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.563198 r2diaphora-0.2.1/r2diaphora/idaapi/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/idaapi/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    22772 2023-03-23 12:48:30.000000 r2diaphora-0.2.1/r2diaphora/idaapi/idaapi_to_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/idaapi/instructions.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.563198 r2diaphora-0.2.1/r2diaphora/jkutils/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/jkutils/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/jkutils/factor.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-03-22 16:06:47.000000 r2diaphora-0.2.1/r2diaphora/jkutils/graph_hashes.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/jkutils/kfuzzy.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.563198 r2diaphora-0.2.1/r2diaphora/others/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/others/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/others/tarjan_sort.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.555198 r2diaphora-0.2.1/r2diaphora/pycparser/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.575198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.575198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/X11/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/X11/Intrinsic.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/X11/Xlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      311 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_defines.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     1111 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/_ansi.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     5734 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/_fake_defines.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     5040 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/_syslist.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/aio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/alloca.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/ar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/argz.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/arpa/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/arpa/inet.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/asm-generic/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/asm-generic/int-ll64.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/assert.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/complex.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/cpio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/ctype.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/dirent.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/dlfcn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/emmintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/endian.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/envz.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/errno.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/fastmath.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/fcntl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/features.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/fenv.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/float.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/fmtmsg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/fnmatch.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/ftw.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/getopt.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/glob.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/grp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/iconv.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/ieeefp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/immintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/inttypes.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/iso646.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/langinfo.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/libgen.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/libintl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/limits.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/linux/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/linux/socket.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/linux/version.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/locale.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/malloc.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/math.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/mir_toolkit/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/mir_toolkit/client_types.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/monetary.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/mqueue.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/ndbm.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/net/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/net/if.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/netdb.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/netinet/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/netinet/in.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/netinet/tcp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/newlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/nl_types.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/openssl/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/openssl/err.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/openssl/evp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/openssl/hmac.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/openssl/ssl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/openssl/x509v3.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/paths.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/poll.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/process.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/pthread.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/pwd.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/reent.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/regdef.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/regex.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sched.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/search.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/semaphore.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/setjmp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/signal.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/smmintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/spawn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stdarg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stdatomic.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stdbool.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stddef.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stdint.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stdio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stdlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stdnoreturn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/string.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/strings.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/stropts.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/ioctl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/ipc.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/mman.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/msg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/poll.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/resource.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/select.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/sem.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/shm.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/socket.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/stat.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/statvfs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/sysctl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/time.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/times.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/types.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/uio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/un.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/utsname.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/sys/wait.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/syslog.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/tar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/termios.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/tgmath.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/threads.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/time.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/trace.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/ulimit.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/unctrl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/unistd.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/utime.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/utmp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/utmpx.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/wchar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/wctype.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/wordexp.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.579198 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/xcb/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/xcb/xcb.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      514 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/zlib.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.559198 r2diaphora-0.2.1/r2diaphora/signatures/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.583198 r2diaphora-0.2.1/r2diaphora/signatures/flirt/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    32585 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_arm.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    44648 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_mips.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    42356 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_ppc.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    32757 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_sh4.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    31653 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_x86-64.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    53445 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_x86.sig
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.563198 r2diaphora-0.2.1/r2diaphora.egg-info/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-04-19 13:12:35.000000 r2diaphora-0.2.1/r2diaphora.egg-info/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     7329 2023-04-19 13:12:35.000000 r2diaphora-0.2.1/r2diaphora.egg-info/SOURCES.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-04-19 13:12:35.000000 r2diaphora-0.2.1/r2diaphora.egg-info/dependency_links.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       59 2023-04-19 13:12:35.000000 r2diaphora-0.2.1/r2diaphora.egg-info/entry_points.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      128 2023-04-19 13:12:35.000000 r2diaphora-0.2.1/r2diaphora.egg-info/requires.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-04-19 13:12:35.000000 r2diaphora-0.2.1/r2diaphora.egg-info/top_level.txt
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-19 13:12:35.583198 r2diaphora-0.2.1/scripts/
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/scripts/r2diaphora-bulk
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-01-25 09:51:26.000000 r2diaphora-0.2.1/scripts/r2diaphora-db
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-04-19 13:12:35.583198 r2diaphora-0.2.1/setup.cfg
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2069 2023-04-19 12:57:44.000000 r2diaphora-0.2.1/setup.py
```

### Comparing `r2diaphora-0.1.9.3/LICENSE` & `r2diaphora-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/README.md` & `r2diaphora-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/diaphora.py` & `r2diaphora-0.2.1/r2diaphora/diaphora.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,15 +433,15 @@
                                                 clean_assembly mediumtext,
                                                 clean_pseudo mediumtext,
                                                 mnemonics_spp text,
                                                 switches text,
                                                 function_hash varchar(100),
                                                 bytes_sum integer,
                                                 md_index double,
-                                                constants text,
+                                                constants mediumtext,
                                                 constants_count integer,
                                                 segment_rva integer,
                                                 assembly_addrs text,
                                                 kgh_hash text,
                                                 userdata text) """
         cur.execute(sql)
 
@@ -696,52 +696,65 @@
         if row is not None:
             rowid = row["id"]
         cur.close()
         return rowid
 
     def save_function(self, props):
         if props == False:
-            log.warning("WARNING: Trying to save a non resolved function?")
+            log.warning("Trying to save a non resolved function?")
             return
 
         # Phase 1: Fix data types and insert the function row.
         cur = self.db_cursor()
         new_props = []
 
         sql = f"""use `{self.db_name}`"""
         cur.execute(sql)
 
+        # Some numbers are very long
+        sys.set_int_max_str_digits(8000)
         # The last 4 fields are callers, callees, basic_blocks_data & bb_relations
         for prop in props[:len(props)-4]:
             # XXX: Fixme! This is a hack for 64 bit architectures kernels
             if type(prop) is int and (prop > 0xFFFFFFFF or prop < -0xFFFFFFFF):
-                prop = str(prop)
+                try:
+                    prop = str(prop)
+                except ValueError:
+                    log.warning("Could not convert prop %s to string", prop)
+                    prop = ""
+
             elif type(prop) is bytes:
                 prop = prop.encode("utf-8")
 
             if type(prop) is list or type(prop) is set:
                 new_props.append(json.dumps(list(prop), ensure_ascii=False, cls=bytes_encoder))
+
             else:
                 new_props.append(prop)
 
-        sql = """insert into functions (name, nodes, edges, indegree, outdegree, size,
-                                                                        instructions, mnemonics, names, prototype,
-                                                                        cyclomatic_complexity, primes_value, address,
-                                                                        comment, mangled_function, bytes_hash, pseudocode,
-                                                                        pseudocode_lines, pseudocode_hash1, pseudocode_primes,
-                                                                        function_flags, assembly, prototype2, pseudocode_hash2,
-                                                                        pseudocode_hash3, strongly_connected, loops, rva,
-                                                                        tarjan_topological_sort, strongly_connected_spp,
-                                                                        clean_assembly, clean_pseudo, mnemonics_spp, switches,
-                                                                        function_hash, bytes_sum, md_index, constants,
-                                                                        constants_count, segment_rva, assembly_addrs, kgh_hash,
-                                                                        userdata)
-                                                                values (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s,
-                                                                                %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s,
-                                                                                %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)"""
+        self.ensure_safe_props(new_props)
+        sql = """
+        insert into functions (name, nodes, edges, indegree, outdegree, size,
+                instructions, mnemonics, names, prototype,
+                cyclomatic_complexity, primes_value, address,
+                comment, mangled_function, bytes_hash, pseudocode,
+                pseudocode_lines, pseudocode_hash1, pseudocode_primes,
+                function_flags, assembly, prototype2, pseudocode_hash2,
+                pseudocode_hash3, strongly_connected, loops, rva,
+                tarjan_topological_sort, strongly_connected_spp,
+                clean_assembly, clean_pseudo, mnemonics_spp, switches,
+                function_hash, bytes_sum, md_index, constants,
+                constants_count, segment_rva, assembly_addrs, kgh_hash,
+                userdata)
+        values (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s,
+                %s, %s, %s, %s, %s, %s, %s, %s, %s, %s,
+                %s, %s, %s, %s, %s, %s, %s, %s, %s, %s,
+                %s, %s, %s, %s, %s, %s, %s, %s, %s, %s,
+                %s, %s, %s)
+        """
 
         try:
             cur.execute(sql, new_props)
         except:
             print("Props???", new_props)
             raise
 
@@ -771,32 +784,40 @@
                 cur.execute(sql, (func_id, constant))
 
         # Phase 4: Save the basic blocks relationships
         if not self.function_summaries_only:
             # The last 2 fields are basic_blocks_data & bb_relations
             bb_data, bb_relations = props[len(props)-2:]
             instructions_ids = {}
-            sql = """insert into instructions (address, mnemonic, disasm,
-                                                                                            comment1, comment2, name,
-                                                                                            type, pseudocomment,
-                                                                                            pseudoitp)
-                                                                values (%s, %s, %s, %s, %s, %s, %s, %s, %s)"""
+            sql = """
+            insert into instructions (address, mnemonic, disasm,
+                comment1, comment2, name,
+                type, pseudocomment,
+                pseudoitp)
+            values (%s, %s, %s, %s, %s, %s, %s, %s, %s)
+            """
             self_get_instruction_id = self.get_instruction_id
             cur_execute = cur.execute
             for key in bb_data:
                 for insn in bb_data[key]:
                     addr, mnem, disasm, cmt1, cmt2, name, mtype = insn
                     db_id = self_get_instruction_id(str(addr))
                     if db_id is None:
                         pseudocomment = None
                         pseudoitp = None
                         if addr in self.pseudo_comments:
                             pseudocomment, pseudoitp = self.pseudo_comments[addr]
 
-                        cur_execute(sql, (str(addr), mnem, disasm, cmt1, cmt2, name, mtype, pseudocomment, pseudoitp))
+                        cur_execute(
+                            sql,
+                            (
+                                str(addr), mnem, disasm, cmt1[0:1023], cmt2[0:1023],
+                                name, mtype, pseudocomment, pseudoitp
+                            )
+                        )
                         db_id = cur.lastrowid
                     instructions_ids[addr] = db_id
 
             num = 0
             bb_ids = {}
             sql1 = "insert into basic_blocks (num, address) values (%s, %s)"
             sql2 = "insert into bb_instructions (basic_block_id, instruction_id) values (%s, %s)"
@@ -836,14 +857,52 @@
             sql = "insert into function_bblocks (function_id, basic_block_id) values (%s, %s)"
             for key in bb_ids:
                 bb_id = bb_ids[key]
                 cur_execute(sql, (func_id, bb_id))
 
         cur.close()
 
+    def ensure_safe_props(self, props):
+        size_limits = [
+            ("name", 1024),
+            ("mangled_function", 1024),
+            ("prototype", 1024),
+            ("prototype2", 1024),
+        ]
+        for size_limit in size_limits:
+            idx = self.get_fn_prop_index(size_limit[0])
+            if idx == -1:
+                continue
+            props[idx] = props[idx][0:size_limit[1]]
+
+    def get_fn_prop_index(self, key):
+        keys = self.get_fn_prop_keys()
+        idx = -1
+        try:
+            idx = keys.index(key)
+        except ValueError:
+            pass
+        return idx
+
+    def get_fn_prop_keys(self):
+        return [
+            "name", "nodes", "edges", "indegree", "outdegree", "size",
+            "instructions", "mnemonics", "names", "prototype",
+            "cyclomatic_complexity", "primes_value", "address",
+            "comment", "mangled_function", "bytes_hash", "pseudocode",
+            "pseudocode_lines", "pseudocode_hash1", "pseudocode_primes",
+            "function_flags", "assembly", "prototype2", "pseudocode_hash2",
+            "pseudocode_hash3", "strongly_connected", "loops", "rva",
+            "tarjan_topological_sort", "strongly_connected_spp",
+            "clean_assembly", "clean_pseudo", "mnemonics_spp", "switches",
+            "function_hash", "bytes_sum", "md_index", "constants",
+            "constants_count", "segment_rva", "assembly_addrs", "kgh_hash",
+            "userdata"
+        ]
+
     def get_valid_definition(self, defs):
         """ Try to get a valid structure definition by removing (yes) the 
                 invalid characters typically found in IDA's generated structs."""
         ret = defs.replace("?", "_").replace("@", "_")
         ret = ret.replace("$", "_")
         return ret
 
@@ -1019,29 +1078,31 @@
             dones.add(ins_ea)
 
             try:
                 bb_blocks[bb_ea].append([ins_ea, mnem, dis])
             except KeyError:
                 bb_blocks[bb_ea] = [ [ins_ea, mnem, dis] ]
 
-        sql = """ select (select address
-                                            from %s.basic_blocks
-                             where id = bbr.parent_id) ea1,
-                                     (select address
-                                            from %s.basic_blocks
-                             where id = bbr.child_id) ea2
-                            from %s.bb_relations bbr,
-                                     %s.function_bblocks fbs,
-                                     %s.basic_blocks bbs,
-                                     %s.functions f
-                         where f.id = fbs.function_id
-                             and bbs.id = fbs.basic_block_id
-                             and fbs.basic_block_id = bbr.child_id
-                             and f.address = %s
-                         order by 1 asc, 2 asc""" % (db, db, db, db, db, db)
+        sql = """
+        select (select address
+            from %s.basic_blocks
+            where id = bbr.parent_id) ea1,
+                        (select address
+                            from %s.basic_blocks
+            where id = bbr.child_id) ea2
+            from %s.bb_relations bbr,
+                        %s.function_bblocks fbs,
+                        %s.basic_blocks bbs,
+                        %s.functions f
+            where f.id = fbs.function_id
+                and bbs.id = fbs.basic_block_id
+                and fbs.basic_block_id = bbr.child_id
+                and f.address = %s
+            order by 1 asc, 2 asc
+        """ % (db, db, db, db, db, db)
         cur.execute(sql, (str(ea1), ))
         rows = result_iter(cur)
 
         bb_relations = {}
         for row in rows:
             bb_ea1 = str(row["ea1"])
             bb_ea2 = str(row["ea2"])
@@ -1863,18 +1924,18 @@
             # Create a copy of all the functions
             cur.execute("""
                 create temporary table best_matches 
                             (
                                 id integer,
                                 id1 integer,
                                 ea1 varchar(255),
-                                name1 varchar(255),
+                                name1 varchar(1024),
                                 id2 integer,
                                 ea2 varchar(255),
-                                name2 varchar(255)
+                                name2 varchar(1024)
                             )
             """)
 
             # Insert each matched function into the temporary table
             i = 0
             for match in the_items:
                 ea1 = match[1]
```

### Comparing `r2diaphora-0.1.9.3/r2diaphora/diaphora_heuristics.py` & `r2diaphora-0.2.1/r2diaphora/diaphora_heuristics.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/diaphora_r2.py` & `r2diaphora-0.2.1/r2diaphora/diaphora_r2.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,140 +22,67 @@
 """
 
 import os
 import re
 import sys
 import time
 import json
+import signal
 import decimal
 import difflib
-import threading
 import logging
 from logging.handlers import RotatingFileHandler
 from hashlib import md5, sha256
 
-try:
-    import thread
-except ImportError:
-    import _thread as thread
-
 import r2diaphora
 from r2diaphora import diaphora
 from r2diaphora.others.tarjan_sort import strongly_connected_components, robust_topological_sort
 from r2diaphora.jkutils.factor import primesbelow as primes
-from r2diaphora.jkutils.graph_hashes import CKoretKaramitasHash
+from r2diaphora.jkutils.graph_hashes import *
 
 from r2diaphora.idaapi.idaapi_to_r2 import *
 
-LOG_FORMAT = "%(asctime)-15s [%(levelname)s] - %(message)s"
-log = logging.getLogger("diaphora.r2")
-log.setLevel(logging.DEBUG)
-
-console = logging.StreamHandler()
-console.setLevel(logging.INFO)
-formatter = logging.Formatter(LOG_FORMAT)
-console.setFormatter(formatter)
-log.addHandler(console)
-
-if os.getenv("MODE") == "DEBUG":
-    print("[*] Running in DEBUG mode")
-    fh = RotatingFileHandler("diaphora_debug.log", maxBytes=1073741824, backupCount=5)      # 1GB
-    fh.setLevel(logging.DEBUG)
-    formatter = logging.Formatter(LOG_FORMAT)
-    fh.setFormatter(formatter)
-    log.addHandler(fh)
-
-# Messages
-MSG_RELAXED_RATIO_ENABLED = """AUTOHIDE DATABASE\n<b>Relaxed ratio calculations</b> will be enabled. It will ignore many small
-modifications to functions and will match more functions with higher ratios. Enable this option if you're only interested in the
-new functionality. Disable it for patch diffing if you're interested in small modifications (like buffer sizes).
-<br><br>
-This is automatically done for diffing big databases (more than 20,000 functions in the database).<br><br>
-You can disable it by un-checking the 'Relaxed calculations of differences ratios' option."""
-
-MSG_FUNCTION_SUMMARIES_ONLY = """AUTOHIDE DATABASE\n<b>Do not export basic blocks or instructions</b> will be enabled.<br>
-It will not export the information relative to basic blocks or<br>
-instructions and 'Diff assembly in a graph' will not be available.
-<br><br>
-This is automatically done for exporting huge databases with<br>
-more than 100,000 functions.<br><br>
-You can disable it by un-checking the 'Do not export basic blocks<br>
-or instructions' option."""
-
-
-#-----------------------------------------------------------------------
-def cdquit(fn_name):
-    # print to stderr, unbuffered in Python 2.
-    print('[-] Timeout: {0} took too long'.format(fn_name), file=sys.stderr)
-    sys.stderr.flush() # Python 3 stderr is likely buffered.
-    thread.interrupt_main() # raises KeyboardInterrupt
-
-def timeout(s):
-    '''
-    use as decorator to exit process if 
-    function takes longer than s seconds
-    '''
-    def outer(fn):
-        def inner(*args, **kwargs):
-            timer = threading.Timer(s, cdquit, args=[fn.__name__])
-            timer.start()
-            try:
-                result = fn(*args, **kwargs)
-            finally:
-                timer.cancel()
-            return result
-        return inner
-    return outer
-
+def raise_timeout(signum, frame):
+    raise TimeoutError
 
 #-----------------------------------------------------------------------
 g_bindiff_opts = {
     "decompiler_command": "pdg",
-    "use_decompiler": True
+    "use_decompiler": True,
+    "rebuild_ast": False,
 }
 
 #-----------------------------------------------------------------------
 class CIDABinDiff(diaphora.CBinDiff):
     def __init__(self, db_name: str = ""):
         diaphora.CBinDiff.__init__(self, db_name)
         self.names = Names()
         self.min_ea = MinEA()
         self.max_ea = MaxEA()
 
-    def show_choosers(self, force=False):
-        if len(self.best_chooser.items) > 0:
-            self.best_chooser.show(force)
-
-        if len(self.partial_chooser.items) > 0:
-            self.partial_chooser.show(force)
-
-        if self.unreliable_chooser is not None and len(self.unreliable_chooser.items) > 0:
-            self.unreliable_chooser.show(force)
-        if self.unmatched_primary is not None and len(self.unmatched_primary.items) > 0:
-            self.unmatched_primary.show(force)
-        if self.unmatched_second is not None and len(self.unmatched_second.items) > 0:
-            self.unmatched_second.show(force)
-
     def do_export(self, function_filter = None, userdata = ""):
+        global cpu_ins_list
+
         callgraph_primes = 1
         callgraph_all_primes = {}
         func_list = Functions(function_filter)
         total_funcs = len(func_list)
         t = time.time()
 
+        cpu_ins_list = GetInstructionList()
+        cpu_ins_list.sort()
+
         self.db.commit()
         self.db.start_transaction()
 
-        log.debug("FUNC LISTING IS %s" % (func_list))
-        i = 0
-        for func in func_list:
-            log.debug("PROPS FOR FUNC cur %s" % (func))
-            props = self.read_function(func)
+        log.debug("FUNC LISTING IS %s", func_list)
+        for i, func in enumerate(func_list, start = 1):
+            log.debug("PROPS FOR FUNC cur %s", func)
+            props = self.read_function_with_timeout(func, timeout = 60)
             if not props:
-                i += 1
                 continue
 
             ret = props[11]
             name = props[0]
             callgraph_primes *= decimal.Decimal(ret)
             try:
                 callgraph_all_primes[ret] += 1
@@ -163,23 +90,23 @@
                 callgraph_all_primes[ret] = 1
 
             props = list(props)
             props[42] = userdata
             try:
                 self.save_function(props)
             except Exception:
-                log.exception(f"Failed to save function {func}")
-                i += 1
+                log.exception("Failed to save function %s", func)
                 continue
 
-            i += 1
-            line = "Exported %s fn (%d/%d). Elapsed %d s, remaining time ~%d s"
             elapsed = time.time() - t
             remaining = (elapsed / i) * (total_funcs - i)
-            log.info(line % (name, i, total_funcs, elapsed, remaining))
+            log.info(
+                "Exported %s fn (%d/%d). Elapsed %d s, remaining time ~%d s", 
+                name, i, total_funcs, elapsed, remaining
+            )
 
         # Try to fix bug #30 and, also, try to speed up operations as
         # doing a commit every 10 functions, as before, is overkill.
         if total_funcs > 1000 and i % (total_funcs/1000) == 0:
             self.db.commit()
             self.db.start_transaction()
 
@@ -194,16 +121,16 @@
         except Exception:
             log.exception("")
 
         self.db.commit()
         self.db_close()
 
     def reinit(self, main_db, diff_db, create_choosers=True):
-        log.debug("Main database '%s'." % main_db)
-        log.debug("Diff database '%s'." % diff_db)
+        log.debug("Main database %s", main_db)
+        log.debug("Diff database %s", diff_db)
 
         self.__init__(main_db)
         self.attach_database(diff_db)
 
         if create_choosers:
             self.create_choosers()
 
@@ -219,18 +146,17 @@
         self.import_definitions()
 
         # Import just the selected item
         ea1 = str(int(item[1], 16))
         ea2 = str(int(item[3], 16))
         self.do_import_one(ea1, ea2, True)
 
-        new_func = self.read_function(str(ea1))
+        new_func = self.read_function_with_timeout(str(ea1), timeout = 120)
         self.delete_function(ea1)
         self.save_function(new_func)
-
         self.db.commit()
 
     def import_instruction_level(self, ea1, ea2, cur):
         cur = self.db_cursor()
         try:
             # Check first if we have any importable items
             sql = """ select ins.address ea, ins.disasm dis, ins.comment1 cmt1, ins.comment2 cmt2, ins.name name, ins.type type
@@ -323,21 +249,24 @@
 
     def decompile_and_get(self, ea):
         sv = decompile(ea, decompiler_command=self.decompiler_command);
         if sv is None:
             # Failed to decompile
             return None
 
-        visitor = CAstVisitor()
-        visitor.apply_to(
-            f"""
-            {self.clean_pseudocode(sv)}
-            """
-        )
-        self.pseudo_hash[ea] = visitor.primes_hash
+        if self.rebuild_ast:
+            visitor = CAstVisitor()
+            visitor.apply_to(
+                f"""
+                {self.clean_pseudocode(sv)}
+                """
+            )
+            self.pseudo_hash[ea] = visitor.primes_hash
+        else:
+            self.pseudo_hash[ea] = 1
         self.pseudo[ea] = []
 
         first_line = None
         for line in sv.split("\n"):
             if line == "" or line.startswith("//"):
                 continue
 
@@ -389,35 +318,51 @@
         # make sure, its not a reference but really constant
         drefs = [d.get("to", -1) for d in DataRefsFrom(ea)]
         if value in drefs:
             return False
 
         return True
 
+    def read_function_with_timeout(self, f, timeout = 60):
+        # Register a function to raise a TimeoutError on the signal.
+        signal.signal(signal.SIGALRM, raise_timeout)
+        # Schedule the signal to be sent after ``time``.
+        signal.alarm(timeout)
+        ret = None
+
+        try:
+            ret = self.read_function(f)
+        except TimeoutError:
+            log.warning("Timeout while reading function at 0x%s", f)
+        except Exception:
+            log.exception("Exception while trying to read %s", f)
+        finally:
+            # Unregister the signal so it won't be triggered
+            # if the timeout is not reached.
+            signal.signal(signal.SIGALRM, signal.SIG_IGN)
+        return ret
+
     # Most important function
-    @timeout(300)
     def read_function(self, f, discard=False):
-        log.debug(f"READ F {f}")
-
-        name = ""
-        true_name = ""
+        log_exec_r2_cmd(f"s {f}")
+        kgh = CKoretKaramitasHash(get_r2())
+        name, true_name = "", ""
         try:
             name_info = log_exec_r2_cmdj(f"fd.j @ {f}")[0]
             name = name_info.get("name")
             true_name = name_info.get("realname")
-            log.debug(f"F NAME {name}")
             demangled_name = name #r2.cmdj(f"isj. @ {f}").get("name", "")
             #if demangled_name != "":
             #    name = demangled_name
             if name.startswith("section..") or name.startswith("sym.imp."):
                 log.info(f"Skipping uninteresting function {name}")
                 return False
 
         except Exception:
-            log.exception(f"Could not read function name for address {f}")
+            log.error(f"Could not read function name for address {f}")
 
         # WTF
         f = int(f)
 
         fninfo = get_func(f)
         flow = log_exec_r2_cmdj(f"afbj @ {f}")
         size = fninfo.get("size", 0)
@@ -431,15 +376,15 @@
             # Skip library and thunk functions
         #    flags = GetFunctionFlags(f)
         #    if flags & FUNC_LIB or flags & FUNC_THUNK or flags == -1:
         #        return False
 
         nodes = 0
         edges = 0
-        instructions = 0
+        instructions = fninfo["ninstrs"]
         mnems = []
         dones = {}
         names = set()
         bytes_hash = []
         bytes_sum = 0
         function_hash = []
         outdegree = 0
@@ -449,50 +394,46 @@
         bb_relations = {}
         bb_topo_num = {}
         bb_topological = {}
         switches = []
         bb_degree = {}
         bb_edges = []
         assembly_addrs = [] # TODO: Fill info
-        kgh_hash = ""
+        kgh_hash = 1
         callers = [c.get("from") for c in log_exec_r2_cmdj(f"axtj @ {f}")]
         fn_refs = log_exec_r2_cmdj(f"axffj @ {f}")
         callees = [c.get("at") for c in fn_refs if c.get("type") == "CALL"]
 
         # Intialize to string constants, inmediate constants will be added later
         constants = [
             GetString(r.get("ref"), -1, -1) for r in fn_refs 
                         if r.get("type") == "DATA" and r.get("name", "").startswith("str.")
         ]
 
         mnemonics_spp = 1
-        cpu_ins_list = GetInstructionList()
-        cpu_ins_list.sort()
-
         image_base = self.get_base_address()
-        flags = log_exec_r2_cmdj("fj")
         s = time.time()
         log.debug(f"Fn {name} - Starting block iteration")
         for block in flow:
             nodes += 1
-            block_startEA = +block["addr"];
-            block_endEA = +block["addr"] + +block["size"];
-            block.update({"startEA": block_startEA})
-            block.update({"endEA": block_endEA})
+            block.update({"start": block["addr"], "end": block["addr"] + block["size"] })
             instructions_data = []
 
-            block_ea = block_startEA - image_base
+            block_ea = block["start"] - image_base
             idx = len(bb_topological)
             bb_topological[idx] = []
             bb_topo_num[block_ea] = idx
 
-            for x in Heads(block["addr"], block["ninstr"]):
-                mnem = GetMnem(x)
-                disasm = GetDisasm(x)
-                instructions += 1
+            for x in block["instrs"]:
+                _, ins = diaphora_decode(x)
+                mnem   = ins["mnemonic"]
+                disasm = ins["disasm"]
+
+                if "call" in ins.get("type"):
+                    kgh_hash *= FEATURE_CALL
 
                 if mnem in cpu_ins_list:
                     mnemonics_spp *= self.primes[cpu_ins_list.index(mnem)]
 
                 try:
                     assembly[block_ea].append(disasm)
                 except KeyError:
@@ -500,65 +441,76 @@
                         assembly[block_ea] = [disasm]
                     else:
                         try:
                             assembly[block_ea] = ["loc_%x:" % x, disasm]
                         except Exception:
                             assembly[block_ea] = ["loc_%s:" % x, disasm]
 
-                decoded_size, ins = diaphora_decode(x)
-                if len(ins) < 1:
-                    continue
-                ins = ins[0]
-
                 for oper in ins.get("opex", {}).get("operands", []):
                     if oper["type"] == "imm":
                         if self.is_constant(oper, x) and self.constant_filter(oper["value"]):
                             constants.append(oper["value"])
 
-                mnem_bytes = ins["bytes"][0:ins["mask"].rfind("f") + 1]
+                mnem_bytes = ""
+                for i, mask_char in enumerate(ins["mask"]):
+                    if mask_char == "f":
+                        mnem_bytes += ins["bytes"][i]
                 curr_bytes = bytes.fromhex(mnem_bytes)
 
                 bytes_hash.append(curr_bytes)
                 bytes_sum += sum(curr_bytes)
 
                 function_hash.append(bytes.fromhex(ins["bytes"]))
                 outdegree += len(CodeRefsFrom(x, 0))
                 mnems.append(mnem)
-                op_value = GetOperandValue(x, 1)
+                op_value = self.get_operand_value(ins, 1)
                 if op_value == -1:
-                    op_value = GetOperandValue(x, 0)
+                    op_value = self.get_operand_value(ins, 0)
 
                 tmp_name = None
                 if op_value != BADADDR and op_value in self.names:
                     tmp_name = self.names[op_value]
                     if not tmp_name.startswith("fcn."):
                         names.add(tmp_name)
 
-                l = list(CodeRefsFrom(x, 0))
-                if len(l) == 0:
-                    l = DataRefsFrom(x)
+                drefs = DataRefsFrom(x)
+                refs = coderefs = list(CodeRefsFrom(x, 0))
+                if len(coderefs) == 0:
+                    refs = drefs
+                if len(drefs) > 0:
+                    kgh_hash *= FEATURE_DATA_REFS
+                for xref in coderefs:
+                    if not is_func(xref) or get_flag_at_addr(xref).get("name") != name:
+                        kgh_hash *= FEATURE_CALL_REF
 
                 tmp_type = None
-                for ref in l:
+                for ref in refs:
                     if ref in self.names:
                         tmp_name = self.names[ref]
                         tmp_type = GetType(ref)
 
                 ins_cmt1 = GetCommentEx(x, 0)
                 ins_cmt2 = GetCommentEx(x, 1)
-                instructions_data.append([x - image_base, mnem, disasm, ins_cmt1, ins_cmt2, tmp_name, tmp_type])
+                instructions_data.append(
+                    [x - image_base, mnem, disasm, ins_cmt1, ins_cmt2, tmp_name, tmp_type]
+                )
+            # End for x in block["instr"]
 
             basic_blocks_data[block_ea] = instructions_data
             bb_relations[block_ea] = []
             if block_ea not in bb_degree:
                 # bb in degree, out degree
                 bb_degree[block_ea] = [0, 0]
 
-            succs = block_succs(block_startEA)
-            preds = block_preds(block_startEA)
+            succs = block_succs(block["start"])
+            preds = block_preds(block["start"])
+
+            kgh_hash *= kgh.get_node_value(len(succs), len(preds))
+            kgh_hash *= kgh.get_edges_value(block, succs, preds)
+
             for succ_block in succs:
                 succ_base = succ_block - image_base #.startEA - image_base
                 bb_relations[block_ea].append(succ_base)
                 bb_degree[block_ea][1] += 1
                 bb_edges.append((block_ea, succ_base))
                 if succ_base not in bb_degree:
                     bb_degree[succ_base] = [0, 0]
@@ -567,38 +519,28 @@
                 edges += 1
                 indegree += 1
                 if succ_block not in dones:
                     dones[succ_block] = 1
 
             for pred_block in preds:
                 try:
-                    bb_relations[pred_block - image_base].append(block["startEA"] - image_base)
+                    bb_relations[pred_block - image_base].append(block["start"] - image_base)
                 except KeyError:
-                    bb_relations[pred_block - image_base] = [block["startEA"] - image_base]
+                    bb_relations[pred_block - image_base] = [block["start"] - image_base]
 
                 edges += 1
                 outdegree += 1
                 #if not dones.has_key(succ_block):
                 #    dones[succ_block] = 1
                 if pred_block not in dones:
                     dones[pred_block] = 1
 
         log.debug(f"Fn {name} - Block iteration: {time.time() - s}s")
 
-        sws = [f for f in flags if f["name"].startswith("switch.")]
-        for sw in sws:
-            # Flags have an offset value, but this value is not the same for 
-            # switch flags and their cases
-            sw_ref = sw["name"].split(".")[1].lstrip("0x").lstrip("0")
-            if not test_addr_within_function(f, sw["offset"]):
-                continue
-
-            cases = [f for f in flags if f["name"].startswith(f"case.0x{sw_ref}.")]
-            cases_values = [case["name"].split(".")[-1] for case in cases]
-            switches.append([len(cases), cases_values])
+        switches = self.get_switches_info_for_fn(f)
 
         for block in flow:
             block_ea = block["addr"] - image_base
             for succ_block in block_succs(block["addr"]):
                 succ_base = succ_block - image_base
                 try:
                     bb_topological[bb_topo_num[block_ea]].append(bb_topo_num[succ_base])
@@ -606,76 +548,51 @@
                     # tailcall functions will generate a KeyError as jump'ed BB is not
                     # on function topology, but that's perfectly fine
                     pass
 
         s = time.time()
         strongly_connected_spp = 0
         try:
-            strongly_connected = strongly_connected_components(bb_relations)
+            strongly_connected, strongly_connected_spp = self.calc_strongly_connected(bb_relations)
             bb_topological_sorted = robust_topological_sort(bb_topological)
             bb_topological = json.dumps(bb_topological_sorted)
-            strongly_connected_spp = 1
-            for item in strongly_connected:
-                val = len(item)
-                if val > 1:
-                    strongly_connected_spp *= self.primes[val]
         except Exception:
-            # XXX: FIXME: The original implementation that we're using is
-            # recursive and can fail. We really need to create our own non
-            # recursive version.
             strongly_connected = []
             bb_topological = None
 
         loops = 0
         for sc in strongly_connected:
             if len(sc) > 1:
                 loops += 1
+                kgh_hash *= FEATURE_LOOP
             else:
                 if sc[0] in bb_relations and sc[0] in bb_relations[sc[0]]:
                     loops += 1
+                    kgh_hash *= FEATURE_LOOP
 
-        asm = []
-        keys = list(assembly.keys())
-        keys.sort()
-
-        # After sorting our the addresses of basic blocks, be sure that the
-        # very first address is always the entry point, no matter at what
-        # address it is.
-        try:
-            keys.remove(f - image_base)
-        except Exception:
-            pass
-        keys.insert(0, f - image_base)
-        for key in keys:
-            try:
-                asm.extend(assembly[key])
-            except Exception:
-                log.exception("")
-                pass
-        asm = "\n".join(asm)
+        kgh_hash *= (FEATURE_STRONGLY_CONNECTED ** len(strongly_connected))
         log.debug(f"Fn {name} - Topological analysis: {time.time() - s}s")
 
+        asm = self.build_asm_corpus(assembly, f, image_base)
+
         cc = edges - nodes + 2
         proto = self.guess_type(f)
         proto2 = GetType(f)
         try:
             prime = str(self.primes[cc])
         except Exception:
-            log.error("Cyclomatic complexity too big: 0x%x -> %d" % (f, cc))
+            log.error("Cyclomatic complexity too big: 0x%x -> %d", f, cc)
             prime = 0
 
         comment = GetFunctionCmt(f, 1)
         bytes_hash = md5(b"".join(bytes_hash)).hexdigest()
         function_hash = md5(b"".join(function_hash)).hexdigest()
 
         function_flags = GetFunctionFlags(f)
-        pseudo = None
-        pseudo_hash1 = None
-        pseudo_hash2 = None
-        pseudo_hash3 = None
+        pseudo, pseudo_hash1, pseudo_hash2, pseudo_hash3 = None, None, None, None
         pseudo_lines = 0
         pseudocode_primes = None
         if f in self.pseudo:
             pseudo = "\n".join(self.pseudo[f])
             pseudo_lines = len(self.pseudo[f])
             pseudo_hash1, pseudo_hash2, pseudo_hash3 = self.kfh.hash_bytes(pseudo).split(";")
             if pseudo_hash1 == "":
@@ -686,15 +603,15 @@
                 pseudo_hash3 = None
             pseudocode_primes = str(self.pseudo_hash[f])
 
         try:
             clean_assembly = self.get_cmp_asm_lines(asm)
         except Exception:
             clean_assembly = ""
-            log.error("Error getting assembly for 0x%x" % f)
+            log.error("Error getting assembly for 0x%x", f)
 
         clean_pseudo = self.get_cmp_pseudo_lines(pseudo)
 
         md_index = 0
         if bb_topological:
             bb_topo_order = {}
             for i, scc in enumerate(bb_topological_sorted):
@@ -710,32 +627,93 @@
                         bb_degree[dst][1],))
             rt2, rt3, rt5, rt7 = (decimal.Decimal(p).sqrt() for p in (2, 3, 5, 7))
             emb_tuples = (sum((z0, z1 * rt2, z2 * rt3, z3 * rt5, z4 * rt7))
                             for z0, z1, z2, z3, z4 in tuples)
             md_index = sum((1 / emb_t.sqrt() for emb_t in emb_tuples))
             md_index = str(md_index)
 
-        x = f
-        seg_rva = x - SegStart(x)
+        seg_rva = f - SegStart(f)
         rva = f - self.get_base_address()
-        log.debug(f"Fn {name} - Decompiler: {time.time() - s}s")
 
-        kgh = CKoretKaramitasHash(get_r2())
-        kgh_hash = kgh.calculate(f)
+        if name in no_ret_functions():
+            kgh_hash *= FEATURE_FUNC_NO_RET
+        if name.startswith("flirt."):
+            kgh_hash *= FEATURE_FUNC_LIB
 
         return (name, nodes, edges, indegree, outdegree, size, instructions, mnems, names,
                          proto, cc, prime, f, comment, true_name, bytes_hash, pseudo, pseudo_lines,
                          pseudo_hash1, pseudocode_primes, function_flags, asm, proto2,
                          pseudo_hash2, pseudo_hash3, len(strongly_connected), loops, rva, bb_topological,
                          strongly_connected_spp, clean_assembly, clean_pseudo, mnemonics_spp, switches,
                          function_hash, bytes_sum, md_index, constants, len(constants), seg_rva,
-                         assembly_addrs, kgh_hash, None,
+                         assembly_addrs, str(kgh_hash), None,
                          callers, callees,
                          basic_blocks_data, bb_relations)
 
+    def build_asm_corpus(self, assembly, f, image_base):
+        asm = []
+        keys = list(assembly.keys())
+        keys.sort()
+
+        # After sorting our the addresses of basic blocks, be sure that the
+        # very first address is always the entry point, no matter at what
+        # address it is.
+        try:
+            keys.remove(f - image_base)
+        except Exception:
+            pass
+        keys.insert(0, f - image_base)
+        for key in keys:
+            try:
+                asm.extend(assembly[key])
+            except Exception:
+                log.exception("Failed to build assembly corpus for function %s", f)
+
+        return "\n".join(asm)
+
+    def get_switches_info_for_fn(self, function_ea):
+        switches = []
+        flags = log_exec_r2_cmdj("fj")
+        sws = [f for f in flags if f["name"].startswith("switch.")]
+        for sw in sws:
+            # Flags have an offset value, but this value is not the same for 
+            # switch flags and their cases
+            sw_ref = sw["name"].split(".")[1].lstrip("0x").lstrip("0")
+            if not test_addr_within_function(function_ea, sw["offset"]):
+                continue
+
+            cases = [f for f in flags if f["name"].startswith(f"case.0x{sw_ref}.")]
+            cases_values = [case["name"].split(".")[-1] for case in cases]
+            switches.append([len(cases), cases_values])
+        return switches
+
+    def calc_strongly_connected(self, bb_relations):
+        strongly_connected = strongly_connected_components(bb_relations)
+        strongly_connected_spp = 1
+        for item in strongly_connected:
+            sc_len = len(item)
+            if sc_len > 1:
+                strongly_connected_spp *= self.primes[sc_len]
+        return strongly_connected, strongly_connected_spp
+
+    def get_operand_value(self, ins, n):
+        try:
+            op = ins["opex"]["operands"][n]
+        except (KeyError, IndexError):
+            return -1
+
+        if op["type"] == "imm":
+            return op["value"]
+        elif op["type"] == "reg":
+            return -1
+        elif op["type"] == "mem":
+            return op["disp"]
+        else:
+            return -1
+
     def create_function_dictionary(self, l):
         (name, nodes, edges, indegree, outdegree, size, instructions, mnems, names,
         proto, cc, prime, f, comment, true_name, bytes_hash, pseudo, pseudo_lines,
         pseudo_hash1, pseudocode_primes, function_flags, asm, proto2,
         pseudo_hash2, pseudo_hash3, strongly_connected_size, loops, rva, bb_topological,
         strongly_connected_spp, clean_assembly, clean_pseudo, mnemonics_spp, switches,
         function_hash, bytes_sum, md_index, constants, constants_size, seg_rva,
@@ -897,14 +875,15 @@
         opts.file_out = dbname
     bd = None
 
     try:
         bd = CIDABinDiff(opts.file_out)
         bd.use_decompiler_always = (get_arch() != "sh") and g_bindiff_opts.get("use_decompiler", True)
         bd.decompiler_command = g_bindiff_opts.get("decompiler_command", "pdg")
+        bd.rebuild_ast = g_bindiff_opts.get("rebuild_ast", False)
         bd.exclude_library_thunk = opts.exclude_library_thunk
         bd.unreliable = opts.unreliable
         bd.slow_heuristics = opts.slow
         bd.relaxed_ratio = opts.relax
         bd.experimental = opts.experimental
         bd.min_ea = opts.min_ea
         bd.max_ea = opts.max_ea
@@ -931,16 +910,14 @@
         self.file_in = kwargs.get('file_in', '')
         self.file_out = kwargs.get('file_out', '')
         self.use_decompiler = kwargs.get('use_decompiler', True)
         self.exclude_library_thunk = kwargs.get('exclude_library_thunk', True)
         # Enable, by default, relaxed calculations on difference ratios for
         # 'big' databases (>20k functions)
         self.relax = kwargs.get('relax', total_functions > 20000)
-        if self.relax:
-            log.debug(MSG_RELAXED_RATIO_ENABLED)
         self.unreliable = kwargs.get('unreliable', False)
         self.slow = kwargs.get('slow', False)
         self.experimental = kwargs.get('experimental', False)
         self.min_ea = 0 # kwargs.get('min_ea', MinEA())
         self.max_ea = -1 #kwargs.get('max_ea', MaxEA())
         self.ida_subs = kwargs.get('ida_subs', True)
         self.ignore_sub_names = kwargs.get('ignore_sub_names', True)
@@ -1004,14 +981,32 @@
     bd.open_db()
     bd.diff(db2name)
     return bd.get_results()
 
 def main():
     import argparse
 
+    LOG_FORMAT = "%(asctime)-15s [%(levelname)s] - %(message)s"
+    log = logging.getLogger("diaphora.r2")
+    log.setLevel(logging.INFO)
+
+    console = logging.StreamHandler()
+    console.setLevel(logging.INFO)
+    formatter = logging.Formatter(LOG_FORMAT)
+    console.setFormatter(formatter)
+    log.addHandler(console)
+
+    if os.getenv("MODE") == "DEBUG":
+        print("[*] Running in DEBUG mode")
+        fh = RotatingFileHandler("diaphora_debug.log", maxBytes=1073741824, backupCount=5)      # 1GB
+        fh.setLevel(logging.DEBUG)
+        formatter = logging.Formatter(LOG_FORMAT)
+        fh.setFormatter(formatter)
+        log.addHandler(fh)
+
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "file1",
         nargs=1,
         help='File to analyze'
     )
     parser.add_argument(
@@ -1059,23 +1054,30 @@
     parser.add_argument(
         "-a",
         dest='analyze_all',
         action='store_true',
         help="Analyze ALL functions (by default library functions are skipped)"
     )
 
+    parser.add_argument(
+        "--ast",
+        action='store_true',
+        help="Attempt to rebuild AST from the decompiler output for additional function traits"
+    )
+
     args = parser.parse_args()
     args.file1 = args.file1[0]
     decompiler_commands = {
         "ghidra": "pdg",
         "pdc": "pdc"
     }
 
     g_bindiff_opts["decompiler_command"] = decompiler_commands.get(args.decompiler)
     g_bindiff_opts["use_decompiler"] = not args.no_decompiler
+    g_bindiff_opts["rebuild_ast"] = args.ast
 
     db1name = dbname_for_file(args.file1)
     bd = diaphora.CBinDiff(db1name)
 
     fn_filter = lambda fn: (
         not fn["name"].startswith("flirt.") and fn["nbbs"] >= args.nbbs
     )
```

### Comparing `r2diaphora-0.1.9.3/r2diaphora/difflibparser.py` & `r2diaphora-0.2.1/r2diaphora/difflibparser.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/html_diff.py` & `r2diaphora-0.2.1/r2diaphora/html_diff.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/idaapi/idaapi_to_r2.py` & `r2diaphora-0.2.1/r2diaphora/idaapi/idaapi_to_r2.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,27 +294,26 @@
     if _no_ret_fns:
         return _no_ret_fns
 
     _no_ret_fns = log_exec_r2_cmd("tn").split("\n")
     return _no_ret_fns
 
 _all_fns = None
-def get_all_fns(exclude_libs = False):
+def get_all_fns(exclude_libs = False, function_filter = None):
     global _all_fns
-    if _all_fns:
-        if exclude_libs:
-            return [fn for fn in _all_fns if not fn["name"].startswith("flirt.")]
-        else:
-            return _all_fns
+    if not _all_fns:
+        _all_fns = log_exec_r2_cmdj("aflj")
 
-    _all_fns = log_exec_r2_cmdj("aflj")
+    fns = _all_fns
     if exclude_libs:
-        return [fn for fn in _all_fns if not fn["name"].startswith("flirt.")]
-    else:
-        return _all_fns
+        fns = [fn for fn in _all_fns if not fn["name"].startswith("flirt.")]
+    if function_filter:
+        fns = [fn for fn in fns if function_filter(fn)]
+
+    return fns
 
 def scan_libs():
     sigs_dir = os.path.join(os.path.expanduser("~"), ".r2diaphora", "signatures", "flirt")
     if os.path.isdir(sigs_dir):
         log_exec_r2_cmd(f"zfs {sigs_dir}/*.sig")
 
 def get_function_name(ea):
@@ -464,15 +463,19 @@
         return op["disp"]
     else:
         return -1
 
 #-----------------------------------------------------------------------
 def r2_get_imagebase():
     #ep = ((int(r2.cmd("ieq"), 16) >> 24) << 24)
-    ep = int(log_exec_r2_cmd("ia~baddr[1]"), 16)
+    ep = None
+    try:
+        ep = int(log_exec_r2_cmd("ia~baddr[1]"), 16)
+    except:
+        pass
     return ep
 
 #-----------------------------------------------------------------------
 def r2_get_idp_name():
     # idaapi.get_idp_name() returns the current processor (CPU arch)
     # of the opened binary.
     return log_exec_r2_cmd('ij~{core.arch}')
@@ -504,38 +507,31 @@
 #-----------------------------------------------------------------------
 def GetInstructionList():
     arch = log_exec_r2_cmdj("ij").get("bin", {}).get("arch", "")
     return CPU_INSTRUCTIONS.get(arch, [])
 
 #-----------------------------------------------------------------------
 def Heads(ea, size):
-    # res = log_exec_r2_cmd(f"pid {size} @ {ea}~[0]").strip()
-    # addrs = filter(None, [int16(x) for x in res.split("\n")])
-    # # Remove duplicates
-    # return list(dict.fromkeys(addrs))
-    ops = log_exec_r2_cmdj(f"aoj {size} @ {ea}")
-    return [op["addr"] for op in ops]
+    res = log_exec_r2_cmd(f"pid {size} @ {ea}~[0]").strip()
+    addrs = [int(x, 16) for x in res.split("\n") if x]
+    # Remove duplicates
+    return list(dict.fromkeys(addrs))
+    # ops = log_exec_r2_cmdj(f"aoj {size} @ {ea}")
+    # return [op["addr"] for op in ops]
 
 def GetCommentEx(x, type):
     return log_exec_r2_cmd("CC.@ %s"%(x))
 
 def diaphora_decode(x):
     #decoded_size = int(r2.cmd("ao~size[1]"))
     if x == 0:
         return 0, []
 
-    ins = log_exec_r2_cmdj(f"aoj 1 @ {x}")
-    if len(ins) == 0:
-        return 0, []
-
-    decoded_size = 0
-    for op in ins:
-        decoded_size += op["size"]
-
-    return decoded_size, ins
+    ins = log_exec_r2_cmdj(f"aoj 1 @ {x}")[0]
+    return ins["size"], ins
 
 #-----------------------------------------------------------------------
 def SegStart(ea):
     # Just return the segment's start address
     try:
         return int(log_exec_r2_cmd("iS.~1[3]"), 16)
     except Exception:
@@ -656,15 +652,15 @@
 
     # perform analysis
     r2.cmd("e asm.flags=false")
     r2.cmd("e asm.bytes=false")
     r2.cmd("e scr.color=false")
     r2.cmd("e io.cache=true")
     #r2.cmd("aeim")
-    r2.cmd("e anal.hasnext=true")
+    #r2.cmd("e anal.hasnext=true")
 
     dll_extensions = {
         "Darwin": "dylib",
         "Linux": "so",
         "Windows": "dll"
     }
```

### Comparing `r2diaphora-0.1.9.3/r2diaphora/idaapi/instructions.py` & `r2diaphora-0.2.1/r2diaphora/idaapi/instructions.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/jkutils/factor.py` & `r2diaphora-0.2.1/r2diaphora/jkutils/factor.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/jkutils/graph_hashes.py` & `r2diaphora-0.2.1/r2diaphora/jkutils/graph_hashes.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,15 @@
     for _ in preds:
       ret *= EDGE_IN_CONDITIONAL
 
     return ret
 
   def is_call_insn(self, ea):
     _, inss = diaphora_decode(ea)
-    if len(inss) < 1:
-      return False
-    return "call" in inss[0].get("type")
+    return "call" in inss.get("type")
 
   def calculate(self, f):
     fname = get_function_name(f).get("name")
     if not fname:
       return "NO-FUNCTION"
 
     flow = self.log_exec_r2_cmdj(f"afbj @ {f}")
@@ -135,15 +133,15 @@
       succs = block_succs(block_ea)
       preds = block_preds(block_ea)
 
       hash *= self.get_node_value(len(succs), len(preds))
       hash *= self.get_edges_value(block, succs, preds)
 
       # ...and each instruction on each basic block
-      for ea in Heads(block["start_ea"], block["ninstr"]):
+      for ea in block["instrs"]:
 
         if self.is_call_insn(ea):
           hash *= FEATURE_CALL
 
         l = list(DataRefsFrom(ea))
         if len(l) > 0:
           hash *= FEATURE_DATA_REFS
```

### Comparing `r2diaphora-0.1.9.3/r2diaphora/jkutils/kfuzzy.py` & `r2diaphora-0.2.1/r2diaphora/jkutils/kfuzzy.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/others/tarjan_sort.py` & `r2diaphora-0.2.1/r2diaphora/others/tarjan_sort.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h` & `r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/_fake_defines.h` & `r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/_fake_defines.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/pycparser/fake_libc_include/zlib.h` & `r2diaphora-0.2.1/r2diaphora/pycparser/fake_libc_include/zlib.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_arm.sig` & `r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_arm.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_mips.sig` & `r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_mips.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_ppc.sig` & `r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_ppc.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_sh4.sig` & `r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_sh4.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_x86-64.sig` & `r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_x86-64.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora/signatures/flirt/uclibc_x86.sig` & `r2diaphora-0.2.1/r2diaphora/signatures/flirt/uclibc_x86.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/r2diaphora.egg-info/SOURCES.txt` & `r2diaphora-0.2.1/r2diaphora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/scripts/r2diaphora-bulk` & `r2diaphora-0.2.1/scripts/r2diaphora-bulk`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/scripts/r2diaphora-db` & `r2diaphora-0.2.1/scripts/r2diaphora-db`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.1.9.3/setup.py` & `r2diaphora-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             shutil.copy2(
                 f,
                 os.path.join(os.path.expanduser("~"), ".r2diaphora", "signatures", "flirt")
             )
 
 setup(
     name="r2diaphora",
-    version="0.1.9.3",
+    version="0.2.1",
     description="radare2 port of diaphora",
     url="https://github.com/FernandoDoming/r2diaphora",
     author="Fernando Domínguez",
     author_email="fernando.dom.del@gmail.com",
     license="GNU GPL v3",
     packages=[
         "r2diaphora",
@@ -50,15 +50,15 @@
     install_requires=[
         "chardet>=4.0.0",
         "r2pipe>=1.6.3",
         "colorama>=0.4.4",
         "yattag>=1.14.0",
         "mysql-connector-python>=8.0.26",
         "python_magic>=0.4.24",
-        "pycparser>=2.20"
+        "pycparser>=2.21"
     ],
 
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8"
```


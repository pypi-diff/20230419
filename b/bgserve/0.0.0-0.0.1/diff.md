# Comparing `tmp/bgserve-0.0.0.tar.gz` & `tmp/bgserve-0.0.1.tar.gz`

## Comparing `bgserve-0.0.0.tar` & `bgserve-0.0.1.tar`

### file list

```diff
@@ -1,970 +1,972 @@
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bgserve-0.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180416 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    43242 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_bisect.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_bisect.meta.json
--rw-r--r--   0        0        0    52448 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18275 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171979 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113977 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0    91381 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    19751 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23909 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_tracemalloc.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_tracemalloc.meta.json
--rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27357 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50477 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23384 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   149882 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60724 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137668 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/atexit.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/atexit.meta.json
--rw-r--r--   0        0        0    50507 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bdb.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bdb.meta.json
--rw-r--r--   0        0        0    11249 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bisect.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bisect.meta.json
--rw-r--r--   0        0        0  1130460 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/cmd.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/cmd.meta.json
--rw-r--r--   0        0        0   123365 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   124178 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109252 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    37815 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    57793 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   141576 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58339 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62954 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    69882 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/doctest.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/doctest.meta.json
--rw-r--r--   0        0        0    90171 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    19592 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/fnmatch.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/fnmatch.meta.json
--rw-r--r--   0        0        0    88825 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   130403 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    16008 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/gc.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/gc.meta.json
--rw-r--r--   0        0        0    22436 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46238 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0    31977 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0   322723 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85385 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   138260 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ipaddress.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ipaddress.meta.json
--rw-r--r--   0        0        0   266357 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52559 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/mimetypes.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/mimetypes.meta.json
--rw-r--r--   0        0        0    26845 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    79030 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49246 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87512 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    92105 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pdb.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pdb.meta.json
--rw-r--r--   0        0        0    44441 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    31539 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pkgutil.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pkgutil.meta.json
--rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75245 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pprint.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pprint.meta.json
--rw-r--r--   0        0        0    30436 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    40085 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167593 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16469 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0    55591 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    16331 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71160 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    31744 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0    81557 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0    14421 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28528 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49789 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   191058 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27796 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15347 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   162212 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   142500 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14513 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   140373 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49143 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19601 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64763 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    42857 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14961 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49318 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0    48946 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tracemalloc.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tracemalloc.meta.json
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239680 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432450 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57914 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    42008 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unicodedata.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unicodedata.meta.json
--rw-r--r--   0        0        0    33634 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23837 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142976 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    27827 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/zipimport.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/zipimport.meta.json
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/__init__.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/__init__.meta.json
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_version.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_version.meta.json
--rw-r--r--   0        0        0    43286 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
--rw-r--r--   0        0        0   160442 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/capture.data.json
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/capture.meta.json
--rw-r--r--   0        0        0    25818 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/compat.data.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/compat.meta.json
--rw-r--r--   0        0        0    31615 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/debugging.data.json
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/debugging.meta.json
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/deprecated.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/deprecated.meta.json
--rw-r--r--   0        0        0    51446 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/doctest.data.json
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/doctest.meta.json
--rw-r--r--   0        0        0   151526 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/fixtures.data.json
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/fixtures.meta.json
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/freeze_support.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/helpconfig.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json
--rw-r--r--   0        0        0    58484 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/hookspec.data.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/hookspec.meta.json
--rw-r--r--   0        0        0    62366 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/legacypath.data.json
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/legacypath.meta.json
--rw-r--r--   0        0        0    75886 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/logging.data.json
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/logging.meta.json
--rw-r--r--   0        0        0    46893 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/main.data.json
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/main.meta.json
--rw-r--r--   0        0        0    25669 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
--rw-r--r--   0        0        0    57587 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/nodes.data.json
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/nodes.meta.json
--rw-r--r--   0        0        0    29796 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/outcomes.data.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/outcomes.meta.json
--rw-r--r--   0        0        0    35182 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/pathlib.data.json
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/pathlib.meta.json
--rw-r--r--   0        0        0   131478 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester.data.json
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester.meta.json
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
--rw-r--r--   0        0        0   116131 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/python.data.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/python.meta.json
--rw-r--r--   0        0        0    51114 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/python_api.data.json
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/python_api.meta.json
--rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/recwarn.data.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/recwarn.meta.json
--rw-r--r--   0        0        0    51055 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/reports.data.json
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/reports.meta.json
--rw-r--r--   0        0        0    40671 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/runner.data.json
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/runner.meta.json
--rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/scope.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/scope.meta.json
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/stash.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/stash.meta.json
--rw-r--r--   0        0        0    93198 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/terminal.data.json
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/terminal.meta.json
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/timing.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/timing.meta.json
--rw-r--r--   0        0        0    23323 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/tmpdir.data.json
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json
--rw-r--r--   0        0        0    26869 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/warning_types.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/warning_types.meta.json
--rw-r--r--   0        0        0    12931 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/warnings.data.json
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/warnings.meta.json
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
--rw-r--r--   0        0        0   163870 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/code.data.json
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/code.meta.json
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/source.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/source.meta.json
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
--rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
--rw-r--r--   0        0        0    61417 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
--rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
--rw-r--r--   0        0        0    23082 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/util.data.json
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json
--rw-r--r--   0        0        0   100262 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/__init__.data.json
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json
--rw-r--r--   0        0        0    39829 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/compat.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/compat.meta.json
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
--rw-r--r--   0        0        0    23726 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
--rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/expression.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json
--rw-r--r--   0        0        0   110718 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/structures.data.json
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json
--rw-r--r--   0        0        0    89102 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/__init__.data.json
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/__init__.meta.json
--rw-r--r--   0        0        0    68563 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/from_thread.data.json
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/from_thread.meta.json
--rw-r--r--   0        0        0    30859 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/lowlevel.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/lowlevel.meta.json
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/to_thread.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/to_thread.meta.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/__init__.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/__init__.meta.json
--rw-r--r--   0        0        0    48631 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_compat.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_compat.meta.json
--rw-r--r--   0        0        0    13112 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_eventloop.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json
--rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_exceptions.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json
--rw-r--r--   0        0        0   121048 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_fileio.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_fileio.meta.json
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_resources.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_resources.meta.json
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_signals.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_signals.meta.json
--rw-r--r--   0        0        0    33893 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_sockets.data.json
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_sockets.meta.json
--rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_streams.data.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_streams.meta.json
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json
--rw-r--r--   0        0        0    79843 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_synchronization.data.json
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json
--rw-r--r--   0        0        0    22065 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_tasks.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_tasks.meta.json
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_testing.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_testing.meta.json
--rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_typedattr.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/__init__.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/__init__.meta.json
--rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_resources.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_resources.meta.json
--rw-r--r--   0        0        0    31380 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_sockets.data.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_sockets.meta.json
--rw-r--r--   0        0        0    39177 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_streams.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_streams.meta.json
--rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json
--rw-r--r--   0        0        0    18299 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_tasks.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_tasks.meta.json
--rw-r--r--   0        0        0    17695 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_testing.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_testing.meta.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/__init__.meta.json
--rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/memory.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/memory.meta.json
--rw-r--r--   0        0        0    39484 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/stapled.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/stapled.meta.json
--rw-r--r--   0        0        0    38874 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/tls.data.json
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/tls.meta.json
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   104140 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   201010 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    36846 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    38461 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    17307 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    23143 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36118 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24192 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   101566 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    27534 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59061 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/__init__.data.json
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/__init__.meta.json
--rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_background_server.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_background_server.meta.json
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_protocols.data.json
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_protocols.meta.json
--rw-r--r--   0        0        0    10673 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_provide.data.json
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_provide.meta.json
--rw-r--r--   0        0        0    18600 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_resources.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_resources.meta.json
--rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_tilesets.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_tilesets.meta.json
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_util.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/bgserve/_util.meta.json
--rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47526 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182377 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56536 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    28032 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29285 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34364 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24155 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81835 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32843 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   408036 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/__init__.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/__init__.meta.json
--rw-r--r--   0        0        0    20149 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/ansi.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/ansi.meta.json
--rw-r--r--   0        0        0    22997 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/ansitowin32.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/ansitowin32.meta.json
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/initialise.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/colorama/initialise.meta.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    72753 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    61056 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    22007 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   129031 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12248 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25121 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79318 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30905 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    22407 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/utils.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/email/utils.meta.json
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/__init__.meta.json
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_abnf.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_abnf.meta.json
--rw-r--r--   0        0        0    34213 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_connection.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_connection.meta.json
--rw-r--r--   0        0        0    37510 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_events.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_events.meta.json
--rw-r--r--   0        0        0    19994 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_headers.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_headers.meta.json
--rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_readers.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_readers.meta.json
--rw-r--r--   0        0        0    11166 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_receivebuffer.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_receivebuffer.meta.json
--rw-r--r--   0        0        0    23721 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_state.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_state.meta.json
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_util.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_util.meta.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_version.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_version.meta.json
--rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_writers.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/h11/_writers.meta.json
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0    23435 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/__init__.meta.json
--rw-r--r--   0        0        0    66322 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/client.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/client.meta.json
--rw-r--r--   0        0        0    57975 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/cookiejar.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/cookiejar.meta.json
--rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/cookies.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/http/cookies.meta.json
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/__init__.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/__init__.meta.json
--rw-r--r--   0        0        0    17750 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/core.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/core.meta.json
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/idnadata.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/idnadata.meta.json
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/intranges.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/intranges.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/package_data.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/package_data.meta.json
--rw-r--r--   0        0        0    94496 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/uts46data.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/idna/uts46data.meta.json
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70627 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64619 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    91167 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11983 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    44727 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/iniconfig/__init__.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/iniconfig/__init__.meta.json
--rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/iniconfig/_parse.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/iniconfig/_parse.meta.json
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/iniconfig/exceptions.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14552 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   144318 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0    14242 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/logging/config.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/logging/config.meta.json
--rw-r--r--   0        0        0    31448 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30689 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95641 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   148169 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    51457 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17734 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28929 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29491 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67425 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   322669 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    27352 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    44467 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_parser.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_parser.meta.json
--rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    18090 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_tokenizer.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/markers.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/markers.meta.json
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/requirements.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/requirements.meta.json
--rw-r--r--   0        0        0    56613 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    28602 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    10299 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65915 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0   165321 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pkg_resources/__init__.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pkg_resources/__init__.meta.json
--rw-r--r--   0        0        0    13974 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/__init__.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/__init__.meta.json
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatter.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatter.meta.json
--rw-r--r--   0        0        0    41445 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/lexer.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/lexer.meta.json
--rw-r--r--   0        0        0    11229 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/token.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/token.meta.json
--rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/util.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/util.meta.json
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/__init__.data.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/__init__.meta.json
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/bbcode.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/bbcode.meta.json
--rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/html.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/html.meta.json
--rw-r--r--   0        0        0    25392 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/img.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/img.meta.json
--rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/irc.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/irc.meta.json
--rw-r--r--   0        0        0    13751 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/latex.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/latex.meta.json
--rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/other.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/other.meta.json
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/pangomarkup.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/pangomarkup.meta.json
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/rtf.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/rtf.meta.json
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/svg.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/svg.meta.json
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal.meta.json
--rw-r--r--   0        0        0    14984 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal256.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal256.meta.json
--rw-r--r--   0        0        0    11178 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pytest/__init__.data.json
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/pytest/__init__.meta.json
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/__init__.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/__init__.meta.json
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/__version__.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/__version__.meta.json
--rw-r--r--   0        0        0    16984 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/adapters.data.json
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/adapters.meta.json
--rw-r--r--   0        0        0    24825 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/api.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/api.meta.json
--rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/auth.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/auth.meta.json
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/compat.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/compat.meta.json
--rw-r--r--   0        0        0    21472 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/cookies.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/cookies.meta.json
--rw-r--r--   0        0        0    24618 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/exceptions.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/exceptions.meta.json
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/hooks.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/hooks.meta.json
--rw-r--r--   0        0        0    65510 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/models.data.json
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/models.meta.json
--rw-r--r--   0        0        0    73292 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/sessions.data.json
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/sessions.meta.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/status_codes.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/status_codes.meta.json
--rw-r--r--   0        0        0    24010 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/structures.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/structures.meta.json
--rw-r--r--   0        0        0    29287 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/utils.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/requests/utils.meta.json
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sniffio/__init__.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sniffio/__init__.meta.json
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sniffio/_impl.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sniffio/_impl.meta.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sniffio/_version.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/sniffio/_version.meta.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/__init__.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/__init__.meta.json
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/_compat.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/_compat.meta.json
--rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/_utils.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/_utils.meta.json
--rw-r--r--   0        0        0    29457 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/applications.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/applications.meta.json
--rw-r--r--   0        0        0    13802 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/background.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/background.meta.json
--rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/concurrency.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/concurrency.meta.json
--rw-r--r--   0        0        0    19014 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/convertors.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/convertors.meta.json
--rw-r--r--   0        0        0   123372 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/datastructures.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/datastructures.meta.json
--rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/exceptions.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/exceptions.meta.json
--rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/formparsers.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/formparsers.meta.json
--rw-r--r--   0        0        0    46450 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/requests.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/requests.meta.json
--rw-r--r--   0        0        0    35239 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/responses.data.json
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/responses.meta.json
--rw-r--r--   0        0        0    95308 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/routing.data.json
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/routing.meta.json
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/types.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/types.meta.json
--rw-r--r--   0        0        0    25857 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/websockets.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/websockets.meta.json
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/__init__.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/__init__.meta.json
--rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/base.data.json
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/base.meta.json
--rw-r--r--   0        0        0    16053 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/cors.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/cors.meta.json
--rw-r--r--   0        0        0    14901 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/errors.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/errors.meta.json
--rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/exceptions.data.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/__init__.data.json
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/__init__.meta.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_bgserve.data.json
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_bgserve.meta.json
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_provider.data.json
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_provider.meta.json
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_tilesets.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_tilesets.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_util.data.json
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/tests/test_util.meta.json
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24116 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   210202 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0    20626 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/error.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/error.meta.json
--rw-r--r--   0        0        0   182192 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0   154490 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/request.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/request.meta.json
--rw-r--r--   0        0        0    28538 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/response.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib/response.meta.json
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/__init__.data.json
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/__init__.meta.json
--rw-r--r--   0        0        0    24751 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/_collections.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/_collections.meta.json
--rw-r--r--   0        0        0    20369 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/connection.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/connection.meta.json
--rw-r--r--   0        0        0    32553 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/connectionpool.data.json
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/connectionpool.meta.json
--rw-r--r--   0        0        0    44997 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/exceptions.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/exceptions.meta.json
--rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/fields.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/fields.meta.json
--rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/filepost.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/filepost.meta.json
--rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/poolmanager.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/poolmanager.meta.json
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/request.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/request.meta.json
--rw-r--r--   0        0        0    40051 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/response.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/response.meta.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/__init__.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/__init__.meta.json
--rw-r--r--   0        0        0    12991 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/socks.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/socks.meta.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/__init__.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/__init__.meta.json
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.meta.json
--rw-r--r--   0        0        0    12574 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/__init__.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/__init__.meta.json
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/connection.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/connection.meta.json
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/queue.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/queue.meta.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/request.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/request.meta.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/response.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/response.meta.json
--rw-r--r--   0        0        0    44173 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/retry.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/retry.meta.json
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/ssl_.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/ssl_.meta.json
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/timeout.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/timeout.meta.json
--rw-r--r--   0        0        0    41867 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/url.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/url.meta.json
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/__init__.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/__init__.meta.json
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_subprocess.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_subprocess.meta.json
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_types.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_types.meta.json
--rw-r--r--   0        0        0    45576 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/config.data.json
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/config.meta.json
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/importer.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/importer.meta.json
--rw-r--r--   0        0        0    11816 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/logging.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/logging.meta.json
--rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/main.data.json
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/main.meta.json
--rw-r--r--   0        0        0    19321 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/server.data.json
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/server.meta.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/__init__.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/__init__.meta.json
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/asgi2.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/asgi2.meta.json
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/message_logger.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/message_logger.meta.json
--rw-r--r--   0        0        0     9631 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.meta.json
--rw-r--r--   0        0        0    20952 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/wsgi.data.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/wsgi.meta.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/__init__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/__init__.meta.json
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/utils.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/utils.meta.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/__init__.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/__init__.meta.json
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.meta.json
--rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.data.json
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.meta.json
--rw-r--r--   0        0        0    50905 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.data.json
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.meta.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.meta.json
--rw-r--r--   0        0        0    35750 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.data.json
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.meta.json
--rw-r--r--   0        0        0    34366 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.data.json
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.meta.json
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/__init__.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/__init__.meta.json
--rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/basereload.data.json
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/basereload.meta.json
--rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.data.json
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.meta.json
--rw-r--r--   0        0        0   111200 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/__init__.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/__init__.meta.json
--rw-r--r--   0        0        0    22499 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/_yaml.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/_yaml.meta.json
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/composer.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/composer.meta.json
--rw-r--r--   0        0        0    45569 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/constructor.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/constructor.meta.json
--rw-r--r--   0        0        0    19663 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/cyaml.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/cyaml.meta.json
--rw-r--r--   0        0        0    12855 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/dumper.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/dumper.meta.json
--rw-r--r--   0        0        0    37012 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/emitter.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/emitter.meta.json
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/error.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/error.meta.json
--rw-r--r--   0        0        0    27321 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/events.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/events.meta.json
--rw-r--r--   0        0        0    11994 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/loader.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/loader.meta.json
--rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/nodes.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/nodes.meta.json
--rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/parser.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/parser.meta.json
--rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/reader.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/reader.meta.json
--rw-r--r--   0        0        0    41647 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/representer.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/representer.meta.json
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/resolver.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/resolver.meta.json
--rw-r--r--   0        0        0    30414 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/scanner.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/scanner.meta.json
--rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/serializer.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/serializer.meta.json
--rw-r--r--   0        0        0    34788 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/tokens.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.0/.mypy_cache/3.11/yaml/tokens.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bgserve-0.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bgserve-0.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bgserve-0.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 bgserve-0.0.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bgserve-0.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/1cc2ca72ff6035b8
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/1ef54225dcc3c36f
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/2334d79e804ba4e4
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/239ef16b196660c8
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/27d94ce6f0564130
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/2b2c0a3d165a7577
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/2cd9215a48dd2de0
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/422bdd2b6bcf8932
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/42e5b5937c05c80e
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/53376c2dcdeb1ea2
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/5430df22f4ca7ced
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/5d467db0605f09ac
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/760f933107068ab
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/8e95d11fc2ac7464
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/8f4ab9b9cd5eb279
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/92a1f6d74d28ef66
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/d7547a60a4e80178
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/d939822cf2406b43
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/dab9d62161f0c772
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/e547c2336af5e3bf
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/e7485985c8f2c40a
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bgserve-0.0.0/.ruff_cache/content/f44104ea9c12ecfb
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bgserve-0.0.0/src/bgserve/__init__.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 bgserve-0.0.0/src/bgserve/_background_server.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 bgserve-0.0.0/src/bgserve/_protocols.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 bgserve-0.0.0/src/bgserve/_provide.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 bgserve-0.0.0/src/bgserve/_resources.py
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 bgserve-0.0.0/src/bgserve/_tilesets.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 bgserve-0.0.0/src/bgserve/_util.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bgserve-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bgserve-0.0.0/tests/test_bgserve.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 bgserve-0.0.0/tests/test_provider.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 bgserve-0.0.0/tests/test_tilesets.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 bgserve-0.0.0/tests/test_util.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bgserve-0.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bgserve-0.0.0/LICENSE
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 bgserve-0.0.0/README.md
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 bgserve-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 bgserve-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bgserve-0.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180416 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    43242 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_bisect.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_bisect.meta.json
+-rw-r--r--   0        0        0    52448 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18275 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171979 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113977 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0    91381 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    19751 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23909 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_tracemalloc.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_tracemalloc.meta.json
+-rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27357 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50477 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23384 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   149882 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60724 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137668 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/atexit.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/atexit.meta.json
+-rw-r--r--   0        0        0    50507 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bdb.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bdb.meta.json
+-rw-r--r--   0        0        0    11249 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bisect.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bisect.meta.json
+-rw-r--r--   0        0        0  1130460 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/cmd.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/cmd.meta.json
+-rw-r--r--   0        0        0   123365 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   124178 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109252 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    37815 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    57793 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   141576 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58339 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62954 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    69882 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/doctest.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/doctest.meta.json
+-rw-r--r--   0        0        0    90171 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    19592 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/fnmatch.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/fnmatch.meta.json
+-rw-r--r--   0        0        0    88825 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   130403 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    16008 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/gc.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/gc.meta.json
+-rw-r--r--   0        0        0    22436 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46238 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0    31977 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0   322723 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85385 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   138260 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ipaddress.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ipaddress.meta.json
+-rw-r--r--   0        0        0   266357 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52559 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/mimetypes.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/mimetypes.meta.json
+-rw-r--r--   0        0        0    26845 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    79030 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49246 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87512 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    92105 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pdb.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pdb.meta.json
+-rw-r--r--   0        0        0    44441 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    31539 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pkgutil.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pkgutil.meta.json
+-rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75245 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pprint.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pprint.meta.json
+-rw-r--r--   0        0        0    30436 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    40085 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167593 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16469 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0    55591 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    16331 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71160 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    31744 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0    81557 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0    14421 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28528 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49789 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   191058 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27796 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15347 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   162212 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   142500 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14513 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   140373 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49143 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19601 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64763 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    42857 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14961 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49318 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0    48946 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tracemalloc.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tracemalloc.meta.json
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239680 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432450 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57914 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    42008 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unicodedata.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unicodedata.meta.json
+-rw-r--r--   0        0        0    33634 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23837 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142976 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    27827 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/zipimport.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/zipimport.meta.json
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/__init__.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/__init__.meta.json
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_argcomplete.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_version.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_version.meta.json
+-rw-r--r--   0        0        0    43286 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/cacheprovider.data.json
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
+-rw-r--r--   0        0        0   160442 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/capture.data.json
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/capture.meta.json
+-rw-r--r--   0        0        0    25818 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/compat.data.json
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/compat.meta.json
+-rw-r--r--   0        0        0    31615 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/debugging.data.json
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/debugging.meta.json
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/deprecated.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/deprecated.meta.json
+-rw-r--r--   0        0        0    51446 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/doctest.data.json
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/doctest.meta.json
+-rw-r--r--   0        0        0   151526 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/fixtures.data.json
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/fixtures.meta.json
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/freeze_support.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/freeze_support.meta.json
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/helpconfig.data.json
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/helpconfig.meta.json
+-rw-r--r--   0        0        0    58484 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/hookspec.data.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/hookspec.meta.json
+-rw-r--r--   0        0        0    62366 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/legacypath.data.json
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/legacypath.meta.json
+-rw-r--r--   0        0        0    75886 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/logging.data.json
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/logging.meta.json
+-rw-r--r--   0        0        0    46893 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/main.data.json
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/main.meta.json
+-rw-r--r--   0        0        0    25669 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/monkeypatch.data.json
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
+-rw-r--r--   0        0        0    57587 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/nodes.data.json
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/nodes.meta.json
+-rw-r--r--   0        0        0    29796 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/outcomes.data.json
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/outcomes.meta.json
+-rw-r--r--   0        0        0    35182 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/pathlib.data.json
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/pathlib.meta.json
+-rw-r--r--   0        0        0   131478 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester.data.json
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester.meta.json
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
+-rw-r--r--   0        0        0   116131 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/python.data.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/python.meta.json
+-rw-r--r--   0        0        0    51114 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/python_api.data.json
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/python_api.meta.json
+-rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/recwarn.data.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/recwarn.meta.json
+-rw-r--r--   0        0        0    51055 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/reports.data.json
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/reports.meta.json
+-rw-r--r--   0        0        0    40671 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/runner.data.json
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/runner.meta.json
+-rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/scope.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/scope.meta.json
+-rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/stash.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/stash.meta.json
+-rw-r--r--   0        0        0    93198 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/terminal.data.json
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/terminal.meta.json
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/timing.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/timing.meta.json
+-rw-r--r--   0        0        0    23323 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/tmpdir.data.json
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/tmpdir.meta.json
+-rw-r--r--   0        0        0    26869 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/warning_types.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/warning_types.meta.json
+-rw-r--r--   0        0        0    12931 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/warnings.data.json
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/warnings.meta.json
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/__init__.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
+-rw-r--r--   0        0        0   163870 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/code.data.json
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/code.meta.json
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/source.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/source.meta.json
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/__init__.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
+-rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
+-rw-r--r--   0        0        0    61417 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
+-rw-r--r--   0        0        0    23082 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/util.data.json
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/util.meta.json
+-rw-r--r--   0        0        0   100262 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/__init__.data.json
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/__init__.meta.json
+-rw-r--r--   0        0        0    39829 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/argparsing.data.json
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/compat.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/compat.meta.json
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/exceptions.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/findpaths.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
+-rw-r--r--   0        0        0    23726 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/__init__.data.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
+-rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/expression.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/expression.meta.json
+-rw-r--r--   0        0        0   110718 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/structures.data.json
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/structures.meta.json
+-rw-r--r--   0        0        0    89102 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/__init__.data.json
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/__init__.meta.json
+-rw-r--r--   0        0        0    68563 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/from_thread.data.json
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/from_thread.meta.json
+-rw-r--r--   0        0        0    30859 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/lowlevel.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/lowlevel.meta.json
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/to_thread.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/to_thread.meta.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/__init__.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/__init__.meta.json
+-rw-r--r--   0        0        0    48631 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_compat.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_compat.meta.json
+-rw-r--r--   0        0        0    13112 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_eventloop.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json
+-rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_exceptions.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json
+-rw-r--r--   0        0        0   121048 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_fileio.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_fileio.meta.json
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_resources.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_resources.meta.json
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_signals.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_signals.meta.json
+-rw-r--r--   0        0        0    33893 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_sockets.data.json
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_sockets.meta.json
+-rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_streams.data.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_streams.meta.json
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json
+-rw-r--r--   0        0        0    79843 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_synchronization.data.json
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json
+-rw-r--r--   0        0        0    22065 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_tasks.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_tasks.meta.json
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_testing.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_testing.meta.json
+-rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_typedattr.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/__init__.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/__init__.meta.json
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_resources.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_resources.meta.json
+-rw-r--r--   0        0        0    31380 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_sockets.data.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_sockets.meta.json
+-rw-r--r--   0        0        0    39177 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_streams.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_streams.meta.json
+-rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json
+-rw-r--r--   0        0        0    18299 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_tasks.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_tasks.meta.json
+-rw-r--r--   0        0        0    17695 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_testing.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_testing.meta.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/__init__.meta.json
+-rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/memory.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/memory.meta.json
+-rw-r--r--   0        0        0    39484 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/stapled.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/stapled.meta.json
+-rw-r--r--   0        0        0    38874 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/tls.data.json
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/tls.meta.json
+-rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   104140 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   201010 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    36846 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    38461 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    17307 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    23143 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36118 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24192 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   101566 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    27534 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59061 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/__init__.data.json
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/__init__.meta.json
+-rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_background_server.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_background_server.meta.json
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_protocols.data.json
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_protocols.meta.json
+-rw-r--r--   0        0        0    10673 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_provide.data.json
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_provide.meta.json
+-rw-r--r--   0        0        0    18600 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_resources.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_resources.meta.json
+-rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_tilesets.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_tilesets.meta.json
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_util.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/bgserve/_util.meta.json
+-rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47526 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182377 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56536 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    28032 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29285 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34364 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24155 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81835 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32843 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   408036 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/__init__.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/__init__.meta.json
+-rw-r--r--   0        0        0    20149 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/ansi.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/ansi.meta.json
+-rw-r--r--   0        0        0    22997 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/ansitowin32.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/ansitowin32.meta.json
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/initialise.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/colorama/initialise.meta.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    72753 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    61056 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    22007 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   129031 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12248 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25121 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79318 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30905 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    22407 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/utils.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/email/utils.meta.json
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/__init__.meta.json
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_abnf.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_abnf.meta.json
+-rw-r--r--   0        0        0    34213 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_connection.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_connection.meta.json
+-rw-r--r--   0        0        0    37510 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_events.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_events.meta.json
+-rw-r--r--   0        0        0    19994 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_headers.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_headers.meta.json
+-rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_readers.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_readers.meta.json
+-rw-r--r--   0        0        0    11166 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_receivebuffer.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_receivebuffer.meta.json
+-rw-r--r--   0        0        0    23721 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_state.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_state.meta.json
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_util.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_util.meta.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_version.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_version.meta.json
+-rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_writers.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/h11/_writers.meta.json
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0    23435 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/__init__.meta.json
+-rw-r--r--   0        0        0    66322 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/client.data.json
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/client.meta.json
+-rw-r--r--   0        0        0    57975 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/cookiejar.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/cookiejar.meta.json
+-rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/cookies.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/http/cookies.meta.json
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/__init__.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/__init__.meta.json
+-rw-r--r--   0        0        0    17750 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/core.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/core.meta.json
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/idnadata.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/idnadata.meta.json
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/intranges.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/intranges.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/package_data.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/package_data.meta.json
+-rw-r--r--   0        0        0    94496 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/uts46data.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/idna/uts46data.meta.json
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70627 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64619 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    91167 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11983 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    44727 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/iniconfig/__init__.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/iniconfig/__init__.meta.json
+-rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/iniconfig/_parse.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/iniconfig/_parse.meta.json
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/iniconfig/exceptions.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/iniconfig/exceptions.meta.json
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14552 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   144318 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0    14242 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/logging/config.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/logging/config.meta.json
+-rw-r--r--   0        0        0    31448 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30689 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95641 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   148169 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    51457 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17734 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28929 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29491 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67425 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   322669 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    27352 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    44467 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_parser.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_parser.meta.json
+-rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    18090 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_tokenizer.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/_tokenizer.meta.json
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/markers.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/markers.meta.json
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/requirements.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/requirements.meta.json
+-rw-r--r--   0        0        0    56613 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    28602 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    10299 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65915 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0   165321 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pkg_resources/__init__.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pkg_resources/__init__.meta.json
+-rw-r--r--   0        0        0    13974 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/__init__.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/__init__.meta.json
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatter.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatter.meta.json
+-rw-r--r--   0        0        0    41445 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/lexer.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/lexer.meta.json
+-rw-r--r--   0        0        0    11229 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/token.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/token.meta.json
+-rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/util.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/util.meta.json
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/__init__.data.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/__init__.meta.json
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/bbcode.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/bbcode.meta.json
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/html.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/html.meta.json
+-rw-r--r--   0        0        0    25392 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/img.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/img.meta.json
+-rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/irc.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/irc.meta.json
+-rw-r--r--   0        0        0    13751 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/latex.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/latex.meta.json
+-rw-r--r--   0        0        0    12594 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/other.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/other.meta.json
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/pangomarkup.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/pangomarkup.meta.json
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/rtf.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/rtf.meta.json
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/svg.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/svg.meta.json
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal.meta.json
+-rw-r--r--   0        0        0    14984 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal256.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal256.meta.json
+-rw-r--r--   0        0        0    11178 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pytest/__init__.data.json
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/pytest/__init__.meta.json
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/__init__.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/__init__.meta.json
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/__version__.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/__version__.meta.json
+-rw-r--r--   0        0        0    16984 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/adapters.data.json
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/adapters.meta.json
+-rw-r--r--   0        0        0    24825 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/api.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/api.meta.json
+-rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/auth.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/auth.meta.json
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/compat.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/compat.meta.json
+-rw-r--r--   0        0        0    21472 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/cookies.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/cookies.meta.json
+-rw-r--r--   0        0        0    24618 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/exceptions.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/exceptions.meta.json
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/hooks.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/hooks.meta.json
+-rw-r--r--   0        0        0    65510 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/models.data.json
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/models.meta.json
+-rw-r--r--   0        0        0    73292 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/sessions.data.json
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/sessions.meta.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/status_codes.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/status_codes.meta.json
+-rw-r--r--   0        0        0    24010 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/structures.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/structures.meta.json
+-rw-r--r--   0        0        0    29287 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/utils.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/requests/utils.meta.json
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sniffio/__init__.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sniffio/__init__.meta.json
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sniffio/_impl.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sniffio/_impl.meta.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sniffio/_version.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/sniffio/_version.meta.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/__init__.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/__init__.meta.json
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/_compat.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/_compat.meta.json
+-rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/_utils.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/_utils.meta.json
+-rw-r--r--   0        0        0    29457 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/applications.data.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/applications.meta.json
+-rw-r--r--   0        0        0    13802 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/background.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/background.meta.json
+-rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/concurrency.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/concurrency.meta.json
+-rw-r--r--   0        0        0    19014 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/convertors.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/convertors.meta.json
+-rw-r--r--   0        0        0   123372 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/datastructures.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/datastructures.meta.json
+-rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/exceptions.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/exceptions.meta.json
+-rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/formparsers.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/formparsers.meta.json
+-rw-r--r--   0        0        0    46450 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/requests.data.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/requests.meta.json
+-rw-r--r--   0        0        0    35239 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/responses.data.json
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/responses.meta.json
+-rw-r--r--   0        0        0    95308 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/routing.data.json
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/routing.meta.json
+-rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/types.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/types.meta.json
+-rw-r--r--   0        0        0    25857 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/websockets.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/websockets.meta.json
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/__init__.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/__init__.meta.json
+-rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/base.data.json
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/base.meta.json
+-rw-r--r--   0        0        0    16053 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/cors.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/cors.meta.json
+-rw-r--r--   0        0        0    14901 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/errors.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/errors.meta.json
+-rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/exceptions.data.json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/__init__.data.json
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/__init__.meta.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_bgserve.data.json
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_bgserve.meta.json
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_provider.data.json
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_provider.meta.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_tilesets.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_tilesets.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_util.data.json
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/tests/test_util.meta.json
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24116 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   210202 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0    20626 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/error.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/error.meta.json
+-rw-r--r--   0        0        0   182192 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0   154490 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/request.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/request.meta.json
+-rw-r--r--   0        0        0    28538 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/response.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib/response.meta.json
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/__init__.data.json
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/__init__.meta.json
+-rw-r--r--   0        0        0    24751 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/_collections.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/_collections.meta.json
+-rw-r--r--   0        0        0    20369 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/connection.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/connection.meta.json
+-rw-r--r--   0        0        0    32553 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/connectionpool.data.json
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/connectionpool.meta.json
+-rw-r--r--   0        0        0    44997 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/exceptions.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/exceptions.meta.json
+-rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/fields.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/fields.meta.json
+-rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/filepost.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/filepost.meta.json
+-rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/poolmanager.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/poolmanager.meta.json
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/request.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/request.meta.json
+-rw-r--r--   0        0        0    40051 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/response.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/response.meta.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/__init__.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/__init__.meta.json
+-rw-r--r--   0        0        0    12991 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/socks.data.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/socks.meta.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/__init__.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/__init__.meta.json
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.meta.json
+-rw-r--r--   0        0        0    12574 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/__init__.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/__init__.meta.json
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/connection.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/connection.meta.json
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/queue.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/queue.meta.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/request.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/request.meta.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/response.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/response.meta.json
+-rw-r--r--   0        0        0    44173 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/retry.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/retry.meta.json
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/ssl_.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/ssl_.meta.json
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/timeout.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/timeout.meta.json
+-rw-r--r--   0        0        0    41867 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/url.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/url.meta.json
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/__init__.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/__init__.meta.json
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_subprocess.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_subprocess.meta.json
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_types.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_types.meta.json
+-rw-r--r--   0        0        0    45576 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/config.data.json
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/config.meta.json
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/importer.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/importer.meta.json
+-rw-r--r--   0        0        0    11816 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/logging.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/logging.meta.json
+-rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/main.data.json
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/main.meta.json
+-rw-r--r--   0        0        0    19321 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/server.data.json
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/server.meta.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/__init__.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/__init__.meta.json
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/asgi2.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/asgi2.meta.json
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/message_logger.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/message_logger.meta.json
+-rw-r--r--   0        0        0     9631 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.meta.json
+-rw-r--r--   0        0        0    20952 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/wsgi.data.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/wsgi.meta.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/__init__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/__init__.meta.json
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/utils.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/utils.meta.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/__init__.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/__init__.meta.json
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.meta.json
+-rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.data.json
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.meta.json
+-rw-r--r--   0        0        0    50905 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.data.json
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.meta.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.meta.json
+-rw-r--r--   0        0        0    35750 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.data.json
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.meta.json
+-rw-r--r--   0        0        0    34366 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.data.json
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.meta.json
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/__init__.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/__init__.meta.json
+-rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/basereload.data.json
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/basereload.meta.json
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.data.json
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.meta.json
+-rw-r--r--   0        0        0   111200 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/__init__.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/__init__.meta.json
+-rw-r--r--   0        0        0    22499 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/_yaml.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/_yaml.meta.json
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/composer.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/composer.meta.json
+-rw-r--r--   0        0        0    45569 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/constructor.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/constructor.meta.json
+-rw-r--r--   0        0        0    19663 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/cyaml.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/cyaml.meta.json
+-rw-r--r--   0        0        0    12855 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/dumper.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/dumper.meta.json
+-rw-r--r--   0        0        0    37012 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/emitter.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/emitter.meta.json
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/error.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/error.meta.json
+-rw-r--r--   0        0        0    27321 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/events.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/events.meta.json
+-rw-r--r--   0        0        0    11994 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/loader.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/loader.meta.json
+-rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/nodes.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/nodes.meta.json
+-rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/parser.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/parser.meta.json
+-rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/reader.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/reader.meta.json
+-rw-r--r--   0        0        0    41647 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/representer.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/representer.meta.json
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/resolver.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/resolver.meta.json
+-rw-r--r--   0        0        0    30414 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/scanner.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/scanner.meta.json
+-rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/serializer.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/serializer.meta.json
+-rw-r--r--   0        0        0    34788 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/tokens.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bgserve-0.0.1/.mypy_cache/3.11/yaml/tokens.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bgserve-0.0.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bgserve-0.0.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bgserve-0.0.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bgserve-0.0.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 bgserve-0.0.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bgserve-0.0.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/1cc2ca72ff6035b8
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/1ef54225dcc3c36f
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/2334d79e804ba4e4
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/239ef16b196660c8
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/27d94ce6f0564130
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/2b2c0a3d165a7577
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/2cd9215a48dd2de0
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/422bdd2b6bcf8932
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/42e5b5937c05c80e
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/53376c2dcdeb1ea2
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/5430df22f4ca7ced
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/5d467db0605f09ac
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/760f933107068ab
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/8e95d11fc2ac7464
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/8f4ab9b9cd5eb279
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/92a1f6d74d28ef66
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/cddb8de0e45222c6
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/d7547a60a4e80178
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/d939822cf2406b43
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/dab9d62161f0c772
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/e547c2336af5e3bf
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/e7485985c8f2c40a
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bgserve-0.0.1/.ruff_cache/content/f44104ea9c12ecfb
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bgserve-0.0.1/src/bgserve/__init__.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 bgserve-0.0.1/src/bgserve/_background_server.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 bgserve-0.0.1/src/bgserve/_protocols.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 bgserve-0.0.1/src/bgserve/_provide.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 bgserve-0.0.1/src/bgserve/_resources.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 bgserve-0.0.1/src/bgserve/_tilesets.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 bgserve-0.0.1/src/bgserve/_util.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bgserve-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bgserve-0.0.1/tests/test_bgserve.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 bgserve-0.0.1/tests/test_provider.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 bgserve-0.0.1/tests/test_tilesets.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 bgserve-0.0.1/tests/test_util.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bgserve-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bgserve-0.0.1/LICENSE
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 bgserve-0.0.1/README.md
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 bgserve-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 bgserve-0.0.1/PKG-INFO
```

### Comparing `bgserve-0.0.0/.github/workflows/ci.yml` & `bgserve-0.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/__future__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/__future__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_ast.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_ast.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_bisect.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_bisect.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_bisect.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_bisect.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_codecs.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_codecs.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_collections_abc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_collections_abc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_ctypes.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_ctypes.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_decimal.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_decimal.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_operator.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_operator.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_random.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_random.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_socket.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_socket.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_stat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_stat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_thread.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_thread.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_tracemalloc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_tracemalloc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_warnings.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_warnings.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_weakref.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_weakref.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_weakrefset.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_weakrefset.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/abc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/abc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/argparse.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/argparse.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/array.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/array.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ast.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ast.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/atexit.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/atexit.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/atexit.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/atexit.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bdb.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bdb.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bdb.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bdb.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bisect.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bisect.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bisect.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bisect.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/builtins.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/builtins.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/cmd.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/cmd.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/cmd.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/cmd.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/codecs.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/codecs.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/configparser.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/configparser.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/contextlib.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/contextlib.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/contextvars.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/contextvars.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/copy.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/copy.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/copyreg.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/copyreg.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/dataclasses.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/dataclasses.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/datetime.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/datetime.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/decimal.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/decimal.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/difflib.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/difflib.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/dis.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/dis.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/doctest.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/doctest.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/doctest.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/enum.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/enum.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/errno.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/errno.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/fnmatch.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/fnmatch.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/fnmatch.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/fnmatch.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/fractions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/fractions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/functools.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/functools.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/gc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/gc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/gc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/gc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/genericpath.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/genericpath.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/getpass.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/getpass.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/gettext.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/gettext.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/glob.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/glob.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/hashlib.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/hashlib.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/inspect.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/inspect.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/io.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/io.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ipaddress.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/ipaddress.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ipaddress.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/ipaddress.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/itertools.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/itertools.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/marshal.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/marshal.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/math.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/math.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/mimetypes.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/mimetypes.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/mimetypes.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/mimetypes.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/mmap.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/mmap.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/msvcrt.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/msvcrt.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/numbers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/numbers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/opcode.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/opcode.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/operator.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/operator.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pathlib.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pathlib.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pdb.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pdb.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pdb.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pdb.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pickle.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pickle.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pkgutil.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pkgutil.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pkgutil.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pkgutil.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/platform.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/platform.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/posixpath.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/posixpath.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pprint.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pprint.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pprint.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pprint.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/queue.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/queue.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/random.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/random.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/re.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/re.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/reprlib.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/reprlib.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/selectors.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/selectors.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/shlex.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/shlex.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/shutil.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/shutil.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/signal.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/signal.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/socket.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/socket.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sre_compile.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sre_compile.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sre_constants.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sre_constants.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sre_parse.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sre_parse.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ssl.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ssl.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/stat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/stat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/string.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/string.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/struct.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/struct.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/subprocess.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/subprocess.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sys.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sys.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sysconfig.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sysconfig.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tempfile.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tempfile.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/termios.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/termios.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/textwrap.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/textwrap.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/threading.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/threading.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/time.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/time.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/token.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/token.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tokenize.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tokenize.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tomllib.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tomllib.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/traceback.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/traceback.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tracemalloc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tracemalloc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tty.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tty.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/types.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/types.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/typing.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/typing.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/typing_extensions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/typing_extensions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unicodedata.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unicodedata.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unicodedata.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unicodedata.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uuid.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uuid.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/warnings.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/warnings.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/weakref.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/weakref.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/webbrowser.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/webbrowser.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/zipimport.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/zipimport.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/zipimport.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/zipimport.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_argcomplete.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_argcomplete.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_version.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_version.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_version.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_version.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/cacheprovider.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/cacheprovider.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/capture.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/capture.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/capture.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/capture.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/compat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/compat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/compat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/compat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/debugging.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/debugging.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/debugging.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/debugging.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/deprecated.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/deprecated.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/deprecated.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/deprecated.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/doctest.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/doctest.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/doctest.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/fixtures.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/fixtures.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/fixtures.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/fixtures.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/freeze_support.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/freeze_support.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/freeze_support.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/helpconfig.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/helpconfig.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/helpconfig.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/hookspec.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/hookspec.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/hookspec.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/hookspec.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/legacypath.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/legacypath.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/legacypath.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/legacypath.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/logging.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/logging.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/logging.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/logging.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/main.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/main.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/main.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/main.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/monkeypatch.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/monkeypatch.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/nodes.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/nodes.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/nodes.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/outcomes.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/outcomes.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/outcomes.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/outcomes.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/pathlib.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/pathlib.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester_assertions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/python.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/python.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/python.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/python.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/python_api.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/python_api.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/python_api.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/python_api.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/recwarn.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/recwarn.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/recwarn.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/recwarn.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/reports.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/reports.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/reports.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/reports.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/runner.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/runner.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/runner.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/scope.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/scope.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/scope.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/scope.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/stash.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/stash.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/stash.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/stash.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/terminal.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/terminal.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/terminal.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/terminal.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/timing.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/timing.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/timing.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/timing.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/tmpdir.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/tmpdir.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/tmpdir.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/warning_types.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/warning_types.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/warning_types.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/warning_types.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/warnings.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/warnings.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/warnings.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/code.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/code.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/code.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/code.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/source.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/source.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_code/source.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_code/source.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/saferepr.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/truncate.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/util.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/util.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/assertion/util.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/argparsing.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/argparsing.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/compat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/compat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/compat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/compat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/findpaths.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/config/findpaths.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/expression.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/expression.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/expression.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/structures.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/structures.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_pytest/mark/structures.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_typeshed/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/from_thread.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/from_thread.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/from_thread.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/from_thread.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/lowlevel.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/lowlevel.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/lowlevel.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/lowlevel.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/to_thread.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/to_thread.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/to_thread.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/to_thread.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_compat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_compat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_compat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_eventloop.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_eventloop.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_fileio.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_fileio.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_fileio.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_fileio.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_resources.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_resources.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_resources.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_resources.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_signals.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_signals.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_signals.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_signals.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_sockets.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_sockets.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_sockets.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_sockets.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_streams.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_streams.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_streams.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_streams.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_synchronization.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_synchronization.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_tasks.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_tasks.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_tasks.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_tasks.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_testing.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_testing.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_testing.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_testing.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_typedattr.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_typedattr.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_resources.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_resources.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_resources.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_resources.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_sockets.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_sockets.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_sockets.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_sockets.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_streams.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_streams.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_streams.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_streams.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_tasks.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_tasks.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_tasks.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_tasks.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_testing.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_testing.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/abc/_testing.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/abc/_testing.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/memory.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/memory.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/memory.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/memory.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/stapled.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/stapled.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/stapled.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/stapled.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/tls.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/tls.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/anyio/streams/tls.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/anyio/streams/tls.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/base_events.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/base_events.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/coroutines.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/events.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/events.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/futures.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/futures.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/locks.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/locks.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/mixins.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/mixins.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/protocols.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/protocols.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/queues.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/queues.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/runners.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/runners.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/selector_events.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/streams.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/streams.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/subprocess.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/tasks.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/tasks.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/threads.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/threads.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/timeouts.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/transports.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/transports.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/unix_events.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_background_server.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_background_server.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_background_server.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_background_server.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_protocols.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_protocols.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_protocols.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_protocols.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_provide.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_provide.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_provide.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_provide.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_resources.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_resources.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_resources.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_resources.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_tilesets.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_tilesets.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_tilesets.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_tilesets.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_util.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_util.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/bgserve/_util.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/bgserve/_util.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/_compat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/_compat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/_termui_impl.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/_termui_impl.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/_textwrap.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/_textwrap.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/core.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/core.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/decorators.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/decorators.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/formatting.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/formatting.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/globals.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/globals.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/parser.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/parser.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/shell_completion.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/shell_completion.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/termui.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/termui.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/types.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/types.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/utils.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/click/utils.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/collections/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/collections/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/collections/abc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/collections/abc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/ansi.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/ansi.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/ansi.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/ansitowin32.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/ansitowin32.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/ansitowin32.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/ansitowin32.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/initialise.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/initialise.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/colorama/initialise.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/colorama/initialise.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/process.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ctypes/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/ctypes/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/charset.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/charset.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/contentmanager.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/contentmanager.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/errors.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/errors.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/header.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/header.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/message.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/message.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/policy.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/policy.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/utils.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/utils.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/email/utils.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/email/utils.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_abnf.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_abnf.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_abnf.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_abnf.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_connection.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_connection.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_connection.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_connection.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_events.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_events.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_events.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_events.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_headers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_headers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_headers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_headers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_readers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_readers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_readers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_readers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_receivebuffer.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_receivebuffer.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_receivebuffer.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_receivebuffer.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_state.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_state.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_state.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_state.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_util.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_util.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_util.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_util.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_version.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_version.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_version.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_version.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_writers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_writers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/h11/_writers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/h11/_writers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/html/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/html/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/client.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/client.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/client.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/client.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/cookiejar.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/cookiejar.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/cookiejar.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/cookiejar.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/cookies.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/cookies.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/http/cookies.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/http/cookies.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/core.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/core.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/core.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/core.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/idnadata.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/idnadata.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/idnadata.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/idnadata.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/intranges.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/intranges.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/intranges.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/intranges.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/package_data.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/package_data.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/package_data.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/package_data.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/uts46data.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/uts46data.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/idna/uts46data.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/idna/uts46data.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/abc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/abc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/machinery.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/machinery.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/util.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/util.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/iniconfig/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/iniconfig/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/iniconfig/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/iniconfig/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/iniconfig/_parse.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/iniconfig/_parse.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/iniconfig/_parse.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/iniconfig/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/iniconfig/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/iniconfig/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/iniconfig/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/json/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/json/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/json/decoder.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/json/decoder.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/json/encoder.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/json/encoder.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/logging/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/logging/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/logging/config.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/logging/config.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/logging/config.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/logging/config.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/connection.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/context.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/context.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/managers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/pool.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/process.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/process.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/queues.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/util.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/multiprocessing/util.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/os/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/os/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/os/path.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/os/path.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_elffile.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_elffile.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_manylinux.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_musllinux.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_parser.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_parser.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_parser.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_structures.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_structures.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_tokenizer.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_tokenizer.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/_tokenizer.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/markers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/markers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/markers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/markers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/requirements.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/requirements.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/requirements.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/requirements.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/specifiers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/specifiers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/tags.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/tags.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/utils.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/utils.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/version.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/packaging/version.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pkg_resources/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pkg_resources/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pkg_resources/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pkg_resources/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatter.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatter.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatter.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatter.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/lexer.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/lexer.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/lexer.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/lexer.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/token.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/token.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/token.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/token.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/util.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/util.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/util.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/util.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/bbcode.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/bbcode.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/bbcode.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/bbcode.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/html.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/html.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/html.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/html.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/img.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/img.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/img.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/img.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/irc.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/irc.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/irc.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/irc.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/latex.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/latex.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/latex.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/latex.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/other.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/other.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/other.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/other.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/pangomarkup.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/pangomarkup.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/pangomarkup.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/pangomarkup.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/rtf.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/rtf.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/rtf.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/rtf.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/svg.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/svg.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/svg.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/svg.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal256.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal256.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pygments/formatters/terminal256.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pygments/formatters/terminal256.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pytest/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/pytest/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/__version__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/__version__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/__version__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/__version__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/adapters.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/adapters.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/adapters.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/adapters.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/api.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/api.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/api.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/api.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/auth.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/auth.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/auth.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/auth.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/compat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/compat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/compat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/compat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/cookies.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/cookies.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/cookies.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/cookies.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/hooks.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/hooks.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/hooks.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/hooks.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/models.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/models.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/models.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/models.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/sessions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/sessions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/sessions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/sessions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/status_codes.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/status_codes.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/status_codes.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/status_codes.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/structures.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/structures.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/structures.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/structures.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/utils.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/utils.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/requests/utils.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/requests/utils.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sniffio/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sniffio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sniffio/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sniffio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sniffio/_impl.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sniffio/_impl.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sniffio/_impl.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sniffio/_impl.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sniffio/_version.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/sniffio/_version.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/sniffio/_version.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/sniffio/_version.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/_compat.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/_compat.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/_compat.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/_utils.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/_utils.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/_utils.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/applications.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/applications.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/applications.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/applications.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/background.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/background.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/background.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/background.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/concurrency.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/concurrency.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/convertors.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/convertors.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/convertors.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/convertors.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/datastructures.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/datastructures.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/datastructures.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/datastructures.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/formparsers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/formparsers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/formparsers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/formparsers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/requests.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/requests.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/requests.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/requests.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/responses.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/responses.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/responses.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/responses.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/routing.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/routing.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/routing.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/routing.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/types.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/types.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/types.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/types.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/websockets.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/websockets.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/websockets.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/websockets.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/base.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/base.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/base.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/base.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/cors.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/cors.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/cors.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/cors.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/errors.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/errors.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/errors.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/errors.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_bgserve.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_bgserve.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_bgserve.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_bgserve.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_provider.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_provider.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_provider.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_provider.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_tilesets.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_tilesets.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_tilesets.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_tilesets.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_util.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_util.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/tests/test_util.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/tests/test_util.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/_log.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/_log.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/async_case.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/async_case.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/case.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/case.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/loader.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/loader.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/main.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/main.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/result.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/result.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/runner.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/runner.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/signals.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/signals.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/suite.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/unittest/suite.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/error.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/error.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/error.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/error.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/parse.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/parse.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/request.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/request.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/request.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/request.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/response.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/response.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib/response.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib/response.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/_collections.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/_collections.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/_collections.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/connection.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/connection.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/connection.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/connection.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/connectionpool.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/connectionpool.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/connectionpool.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/connectionpool.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/exceptions.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/exceptions.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/fields.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/fields.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/fields.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/fields.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/filepost.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/filepost.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/filepost.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/filepost.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/poolmanager.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/poolmanager.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/poolmanager.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/poolmanager.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/request.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/request.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/request.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/request.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/response.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/response.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/response.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/response.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/socks.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/socks.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/contrib/socks.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/contrib/socks.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/packages/ssl_match_hostname/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/connection.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/connection.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/connection.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/connection.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/queue.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/queue.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/queue.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/queue.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/request.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/request.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/request.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/request.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/response.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/response.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/response.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/response.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/retry.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/retry.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/retry.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/retry.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/ssl_.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/ssl_.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/ssl_.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/ssl_.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/timeout.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/timeout.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/timeout.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/timeout.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/url.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/url.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/urllib3/util/url.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/urllib3/util/url.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_subprocess.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_subprocess.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_subprocess.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_types.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_types.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/_types.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/_types.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/config.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/config.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/config.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/config.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/importer.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/importer.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/importer.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/importer.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/logging.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/logging.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/logging.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/logging.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/main.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/main.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/main.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/main.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/server.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/server.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/server.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/server.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/asgi2.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/asgi2.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/asgi2.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/asgi2.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/message_logger.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/message_logger.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/message_logger.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/message_logger.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/proxy_headers.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/wsgi.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/wsgi.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/middleware/wsgi.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/middleware/wsgi.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/utils.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/utils.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/utils.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/utils.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/flow_control.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/h11_impl.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/http/httptools_impl.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/websockets_impl.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/protocols/websockets/wsproto_impl.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/basereload.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/basereload.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/basereload.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/basereload.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/uvicorn/supervisors/multiprocess.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/__init__.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/__init__.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/__init__.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/_yaml.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/_yaml.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/_yaml.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/_yaml.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/composer.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/composer.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/composer.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/composer.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/constructor.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/constructor.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/constructor.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/constructor.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/cyaml.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/cyaml.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/cyaml.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/cyaml.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/dumper.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/dumper.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/dumper.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/dumper.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/emitter.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/emitter.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/emitter.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/emitter.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/error.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/error.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/error.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/error.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/events.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/events.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/events.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/events.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/loader.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/loader.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/loader.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/loader.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/nodes.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/nodes.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/nodes.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/parser.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/parser.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/parser.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/parser.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/reader.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/reader.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/reader.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/reader.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/representer.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/representer.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/representer.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/representer.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/resolver.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/resolver.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/resolver.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/resolver.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/scanner.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/scanner.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/scanner.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/scanner.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/serializer.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/serializer.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/serializer.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/serializer.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/tokens.data.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/tokens.data.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.mypy_cache/3.11/yaml/tokens.meta.json` & `bgserve-0.0.1/.mypy_cache/3.11/yaml/tokens.meta.json`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.pytest_cache/v/cache/nodeids` & `bgserve-0.0.1/.pytest_cache/v/cache/nodeids`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {'insert': "[(7, 'tests/test_provider.py::test_tileset_resource')]"}*

```diff
@@ -2,14 +2,15 @@
     "tests/test_bgserve.py::test_has_version",
     "tests/test_provider.py::test_content",
     "tests/test_provider.py::test_content_explicit_extension",
     "tests/test_provider.py::test_directory_resource",
     "tests/test_provider.py::test_file_content_type_csv",
     "tests/test_provider.py::test_file_content_type_json",
     "tests/test_provider.py::test_files",
+    "tests/test_provider.py::test_tileset_resource",
     "tests/test_tilesets.py::test_get_list[d=1&e=2&d=3-d-expected1]",
     "tests/test_tilesets.py::test_get_list[d=id1&d=id2&d=id3-d-expected0]",
     "tests/test_util.py::test_content_range[bytes=0-499-expected0]",
     "tests/test_util.py::test_content_range[bytes=1-,-expected3]",
     "tests/test_util.py::test_content_range[bytes=500--expected1]",
     "tests/test_util.py::test_content_range[bytes=500-999,-expected2]",
     "tests/test_util.py::test_create_file_response[None-FileResponse]",
```

### Comparing `bgserve-0.0.0/.ruff_cache/content/1ef54225dcc3c36f` & `bgserve-0.0.1/.ruff_cache/content/1ef54225dcc3c36f`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.ruff_cache/content/2334d79e804ba4e4` & `bgserve-0.0.1/.ruff_cache/content/2334d79e804ba4e4`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.ruff_cache/content/422bdd2b6bcf8932` & `bgserve-0.0.1/.ruff_cache/content/422bdd2b6bcf8932`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.ruff_cache/content/42e5b5937c05c80e` & `bgserve-0.0.1/.ruff_cache/content/42e5b5937c05c80e`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.ruff_cache/content/5430df22f4ca7ced` & `bgserve-0.0.1/.ruff_cache/content/5430df22f4ca7ced`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.ruff_cache/content/5d467db0605f09ac` & `bgserve-0.0.1/.ruff_cache/content/5d467db0605f09ac`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.ruff_cache/content/92a1f6d74d28ef66` & `bgserve-0.0.1/.ruff_cache/content/92a1f6d74d28ef66`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/.ruff_cache/content/e7485985c8f2c40a` & `bgserve-0.0.1/.ruff_cache/content/e7485985c8f2c40a`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/src/bgserve/_background_server.py` & `bgserve-0.0.1/src/bgserve/_background_server.py`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/src/bgserve/_protocols.py` & `bgserve-0.0.1/src/bgserve/_protocols.py`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/src/bgserve/_provide.py` & `bgserve-0.0.1/src/bgserve/_provide.py`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/src/bgserve/_resources.py` & `bgserve-0.0.1/src/bgserve/_resources.py`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/src/bgserve/_tilesets.py` & `bgserve-0.0.1/src/bgserve/_tilesets.py`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/src/bgserve/_util.py` & `bgserve-0.0.1/src/bgserve/_util.py`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/tests/test_provider.py` & `bgserve-0.0.1/tests/test_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pathlib
 import typing
 
 import pytest
 import requests
 
 from bgserve._provide import Provider
+from bgserve._tilesets import TilesetResource
 
 
 @pytest.fixture(scope="module")
 def provider() -> typing.Iterator[Provider]:
     provider = Provider()
     yield provider
     provider.stop()
@@ -82,7 +83,27 @@
     print(server_resource.url)
 
     response = requests.get(server_resource.url + "/hello.txt")
     assert response.text == "hello, world"
 
     response = requests.get(server_resource.url + "/nested_dir/foo.txt")
     assert response.text == "foo"
+
+
+def test_tileset_resource(provider: Provider) -> None:
+    class Tileset:
+        def tiles(self, tile_ids: typing.Sequence[str]) -> list[typing.Any]:
+            return [(tid, None) for tid in tile_ids]
+
+        def info(self) -> typing.Any:
+            return "tile_info"
+
+    tileset = Tileset()
+    resource = provider.create(tileset)
+    assert isinstance(resource, TilesetResource)
+
+    resource_url = f"{resource.server}tileset_info/?d={resource.uid}"
+    info = requests.get(resource_url).json()
+    assert info[resource.uid] == "tile_info"
+    tile_url = resource_url.replace("tileset_info", "tiles") + ".0.0"
+    tiles = requests.get(tile_url).json()
+    assert f"{resource.uid}.0.0" in tiles
```

### Comparing `bgserve-0.0.0/tests/test_util.py` & `bgserve-0.0.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/LICENSE` & `bgserve-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/README.md` & `bgserve-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bgserve-0.0.0/pyproject.toml` & `bgserve-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "portpicker>=1.5.2",
+    "portpicker",
     "uvicorn>=0.21.1",
     "starlette>=0.26.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/bgserve#readme"
 Issues = "https://github.com/unknown/bgserve/issues"
```

### Comparing `bgserve-0.0.0/PKG-INFO` & `bgserve-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgserve
-Version: 0.0.0
+Version: 0.0.1
 Summary: an extensible async background server
 Project-URL: Documentation, https://github.com/unknown/bgserve#readme
 Project-URL: Issues, https://github.com/unknown/bgserve/issues
 Project-URL: Source, https://github.com/unknown/bgserve
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: portpicker>=1.5.2
+Requires-Dist: portpicker
 Requires-Dist: starlette>=0.26.1
 Requires-Dist: uvicorn>=0.21.1
 Description-Content-Type: text/markdown
 
 # bgserve
 
 an extensible async background server for python
```


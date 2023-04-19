# Comparing `tmp/hspylib-hqt-0.9.1.tar.gz` & `tmp/hspylib-hqt-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-hqt-0.9.1.tar", last modified: Tue Apr 18 22:40:35 2023, max compression
+gzip compressed data, was "hspylib-hqt-0.9.2.tar", last modified: Wed Apr 19 19:05:04 2023, max compression
```

## Comparing `hspylib-hqt-0.9.1.tar` & `hspylib-hqt-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-18 22:40:35.911505 hspylib-hqt-0.9.1/
--rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.1/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     8761 2023-04-18 22:40:35.910420 hspylib-hqt-0.9.1/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)     7749 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-18 22:40:35.869077 hspylib-hqt-0.9.1/hqt/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hqt/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hqt/__init__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-18 22:40:35.894054 hspylib-hqt-0.9.1/hqt/promotions/
--rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hqt/promotions/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      849 2022-12-23 00:36:28.000000 hspylib-hqt-0.9.1/hqt/promotions/hcombobox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7692 2023-04-05 21:45:48.000000 hspylib-hqt-0.9.1/hqt/promotions/hconsole.py
--rw-r--r--   0 hjunior    (504) staff       (20)      678 2022-12-23 00:36:28.000000 hspylib-hqt-0.9.1/hqt/promotions/hframe.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2582 2023-04-05 21:45:47.000000 hspylib-hqt-0.9.1/hqt/promotions/hlabel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6575 2023-04-05 21:45:48.000000 hspylib-hqt-0.9.1/hqt/promotions/hlistwidget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4407 2023-04-05 21:45:47.000000 hspylib-hqt-0.9.1/hqt/promotions/hstacked_widget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6240 2023-04-05 21:45:47.000000 hspylib-hqt-0.9.1/hqt/promotions/htablemodel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5460 2023-04-05 21:45:48.000000 hspylib-hqt-0.9.1/hqt/promotions/htableview.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6295 2023-04-05 21:45:47.000000 hspylib-hqt-0.9.1/hqt/promotions/htoolbox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2604 2023-04-05 21:45:48.000000 hspylib-hqt-0.9.1/hqt/qt_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3867 2023-04-05 21:45:48.000000 hspylib-hqt-0.9.1/hqt/stream_capturer.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-18 22:40:35.901161 hspylib-hqt-0.9.1/hqt/views/
--rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hqt/views/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      875 2023-04-18 22:32:33.000000 hspylib-hqt-0.9.1/hqt/views/main_view.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2325 2023-04-05 21:45:48.000000 hspylib-hqt-0.9.1/hqt/views/qt_view.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-18 22:40:35.909578 hspylib-hqt-0.9.1/hspylib_hqt.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     8761 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hspylib_hqt.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hspylib_hqt.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hspylib_hqt.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hspylib_hqt.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-04-18 22:40:35.000000 hspylib-hqt-0.9.1/hspylib_hqt.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-18 22:40:35.911609 hspylib-hqt-0.9.1/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2072 2023-04-18 22:30:29.000000 hspylib-hqt-0.9.1/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.432510 hspylib-hqt-0.9.2/
+-rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.2/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)    11519 2023-04-19 19:05:04.431751 hspylib-hqt-0.9.2/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)    10507 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.396460 hspylib-hqt-0.9.2/hqt/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.413448 hspylib-hqt-0.9.2/hqt/promotions/
+-rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/promotions/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      834 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hcombobox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7677 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hconsole.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      663 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hframe.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2567 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hlabel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6559 2023-04-18 23:04:16.000000 hspylib-hqt-0.9.2/hqt/promotions/hlistwidget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4392 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/hstacked_widget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6224 2023-04-18 23:04:17.000000 hspylib-hqt-0.9.2/hqt/promotions/htablemodel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5444 2023-04-18 23:04:16.000000 hspylib-hqt-0.9.2/hqt/promotions/htableview.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6280 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/promotions/htoolbox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2588 2023-04-18 23:04:17.000000 hspylib-hqt-0.9.2/hqt/qt_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3851 2023-04-18 23:04:16.000000 hspylib-hqt-0.9.2/hqt/stream_capturer.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.421809 hspylib-hqt-0.9.2/hqt/views/
+-rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-04-19 19:05:03.000000 hspylib-hqt-0.9.2/hqt/views/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      860 2023-04-18 23:01:36.000000 hspylib-hqt-0.9.2/hqt/views/main_view.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2309 2023-04-18 23:04:17.000000 hspylib-hqt-0.9.2/hqt/views/qt_view.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:04.430888 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)    11519 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-04-19 19:05:04.000000 hspylib-hqt-0.9.2/hspylib_hqt.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-19 19:05:04.432645 hspylib-hqt-0.9.2/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2072 2023-04-18 22:30:29.000000 hspylib-hqt-0.9.2/setup.py
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/hcombobox.py` & `hspylib-hqt-0.9.2/hqt/promotions/hcombobox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: hcombobox.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/hconsole.py` & `hspylib-hqt-0.9.2/hqt/promotions/hconsole.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: hconsole.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/hframe.py` & `hspylib-hqt-0.9.2/hqt/promotions/hframe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: hframe.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/hlabel.py` & `hspylib-hqt-0.9.2/hqt/promotions/hlabel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: hlabel.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/hlistwidget.py` & `hspylib-hqt-0.9.2/hqt/promotions/hlistwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: hlistwidget.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 from typing import List, Optional, Union
 
+from hspylib.core.preconditions import check_argument, check_not_none, check_state
 from PyQt5.QtCore import pyqtSignal, QModelIndex, Qt
 from PyQt5.QtGui import QCursor, QKeyEvent
 from PyQt5.QtWidgets import QListWidget, QListWidgetItem, QMenu, QWidget
 
-from hspylib.core.preconditions import check_argument, check_not_none, check_state
-
 
 class HListWidget(QListWidget):
     """TODO"""
 
     keyPressed = pyqtSignal(int)
 
     @staticmethod
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/hstacked_widget.py` & `hspylib-hqt-0.9.2/hqt/promotions/hstacked_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: hspylib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: hstacked_widget.py
    @created: Wed, 8 Jun 2022
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/htablemodel.py` & `hspylib-hqt-0.9.2/hqt/promotions/htablemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: htablemodel.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 
 import collections
 from typing import List, Tuple, Type, TypeVar, Union
 
+from hspylib.core.collection_filter import CollectionFilter, FilterCondition
+from hspylib.core.tools.commons import class_attribute_names, class_attribute_values
 from PyQt5.QtCore import QAbstractTableModel, QModelIndex, Qt, QVariant
 from PyQt5.QtGui import QPalette
 from PyQt5.QtWidgets import QTableView
 
-from hspylib.core.collection_filter import CollectionFilter, FilterCondition
-from hspylib.core.tools.commons import class_attribute_names, class_attribute_values
-
 T = TypeVar("T")
 
 
 class HTableModel(QAbstractTableModel):
     """TODO"""
 
     def __init__(
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/htableview.py` & `hspylib-hqt-0.9.2/hqt/promotions/htableview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: htableview.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 import os
 from typing import Callable, Optional
 
 import pyperclip as clipboard
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QCursor, QPainter, QPaintEvent
-from PyQt5.QtWidgets import QAbstractScrollArea, QHeaderView, QMenu, QTableView, QWidget
-
 from hspylib.core.collection_filter import CollectionFilter
 from hspylib.core.preconditions import check_argument, check_not_none, check_state
 from hspylib.core.tools.text_tools import strip_linebreaks
+from PyQt5.QtCore import Qt
+from PyQt5.QtGui import QCursor, QPainter, QPaintEvent
+from PyQt5.QtWidgets import QAbstractScrollArea, QHeaderView, QMenu, QTableView, QWidget
 
 CB_ACTION = Callable[[], None]
 
 
 class HTableView(QTableView):
     """Promoted QTableView widget."""
```

### Comparing `hspylib-hqt-0.9.1/hqt/promotions/htoolbox.py` & `hspylib-hqt-0.9.2/hqt/promotions/htoolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: hspylib
-   @package: hspylib.modules.qt.promotions
+   @package: hqt.promotions
       @file: htoolbox.py
    @created: Fri, 29 Jul 2022
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
```

### Comparing `hspylib-hqt-0.9.1/hqt/qt_application.py` & `hspylib-hqt-0.9.2/hqt/qt_application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt
+   @package: hqt
       @file: qt_application.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 import sys
 from pathlib import Path
 from typing import TypeVar
 
-from PyQt5.QtGui import QFont, QFontDatabase, QIcon
-from PyQt5.QtWidgets import QApplication
-
 from hspylib.core.preconditions import check_argument, check_state
 from hspylib.core.tools.text_tools import titlecase
 from hspylib.modules.application.application import Application
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
+from PyQt5.QtGui import QFont, QFontDatabase, QIcon
+from PyQt5.QtWidgets import QApplication
 
 V = TypeVar("V", bound="QWidget")
 
 
 class QtApplication(Application):
     def __init__(
         self,
```

### Comparing `hspylib-hqt-0.9.1/hqt/stream_capturer.py` & `hspylib-hqt-0.9.2/hqt/stream_capturer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt
+   @package: hqt
       @file: stream_capturer.py
    @created: Wed, 30 Jun 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 
 import io
 import logging as log
 from contextlib import redirect_stderr, redirect_stdout
 from time import sleep
 
-from PyQt5.QtCore import pyqtSignal, QThread
-
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.commons import is_debugging, syserr
+from PyQt5.QtCore import pyqtSignal, QThread
 
 
 class StreamCapturer(QThread):
     """QThread to captures stdout and/or stderr messages and send them via PyQt Signal"""
 
     stdoutCaptured = pyqtSignal(str)
     stderrCaptured = pyqtSignal(str)
```

### Comparing `hspylib-hqt-0.9.1/hqt/views/main_view.py` & `hspylib-hqt-0.9.2/hqt/views/main_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.views
+   @package: hqt.views
       @file: main_view.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
```

### Comparing `hspylib-hqt-0.9.1/hqt/views/qt_view.py` & `hspylib-hqt-0.9.2/hqt/views/qt_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HSPyLib
-   @package: hspylib.modules.qt.views
+   @package: hqt.views
       @file: qt_view.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 import os
 from abc import ABC
 from typing import Optional, Tuple, Type
 
+from hspylib.core.preconditions import check_argument, check_state
+from hspylib.core.tools.commons import run_dir
 from PyQt5 import uic
 from PyQt5.QtGui import QFont
 from PyQt5.QtWidgets import QWidget
 
-from hspylib.core.preconditions import check_argument, check_state
-from hspylib.core.tools.commons import run_dir
-
 
 class QtView(ABC):
     """TODO"""
 
     MAIN_QT_VIEW_UI = "main_qt_view.ui"
 
     @staticmethod
```

### Comparing `hspylib-hqt-0.9.1/hspylib_hqt.egg-info/SOURCES.txt` & `hspylib-hqt-0.9.2/hspylib_hqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.1/setup.py` & `hspylib-hqt-0.9.2/setup.py`

 * *Files identical despite different names*


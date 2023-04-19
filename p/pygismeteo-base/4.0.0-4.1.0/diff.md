# Comparing `tmp/pygismeteo_base-4.0.0.tar.gz` & `tmp/pygismeteo_base-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygismeteo_base-4.0.0.tar", max compression
+gzip compressed data, was "pygismeteo_base-4.1.0.tar", max compression
```

## Comparing `pygismeteo_base-4.0.0.tar` & `pygismeteo_base-4.1.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1065 2023-01-01 14:14:23.946534 pygismeteo_base-4.0.0/LICENSE
--rw-r--r--   0        0        0      613 2023-01-01 14:14:23.946534 pygismeteo_base-4.0.0/README.md
--rw-r--r--   0        0        0       86 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/__init__.py
--rw-r--r--   0        0        0       78 2022-12-29 16:27:51.342735 pygismeteo_base-4.0.0/pygismeteo_base/constants.py
--rw-r--r--   0        0        0      826 2023-01-01 14:19:42.001570 pygismeteo_base-4.0.0/pygismeteo_base/current.py
--rw-r--r--   0        0        0      392 2022-12-25 17:09:52.159129 pygismeteo_base-4.0.0/pygismeteo_base/endpoint.py
--rw-r--r--   0        0        0      862 2022-12-25 17:26:27.405091 pygismeteo_base-4.0.0/pygismeteo_base/http.py
--rw-r--r--   0        0        0      309 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/__init__.py
--rw-r--r--   0        0        0     2027 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/current.py
--rw-r--r--   0        0        0      829 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/search_by_coordinates.py
--rw-r--r--   0        0        0      743 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/search_by_ip.py
--rw-r--r--   0        0        0      813 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/search_by_query.py
--rw-r--r--   0        0        0     3163 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/step24.py
--rw-r--r--   0        0        0     1946 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/step3.py
--rw-r--r--   0        0        0     1978 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/models/step6.py
--rw-r--r--   0        0        0        0 2022-12-24 09:49:57.579029 pygismeteo_base-4.0.0/pygismeteo_base/py.typed
--rw-r--r--   0        0        0      978 2023-01-01 13:55:46.756697 pygismeteo_base-4.0.0/pygismeteo_base/search.py
--rw-r--r--   0        0        0        0 2022-12-25 15:56:49.021653 pygismeteo_base-4.0.0/pygismeteo_base/step_n/__init__.py
--rw-r--r--   0        0        0     1320 2023-01-01 14:10:30.635288 pygismeteo_base-4.0.0/pygismeteo_base/step_n/abc.py
--rw-r--r--   0        0        0     1604 2023-01-01 14:09:01.343252 pygismeteo_base-4.0.0/pygismeteo_base/step_n/mixins.py
--rw-r--r--   0        0        0     1421 2023-01-01 14:44:02.352475 pygismeteo_base-4.0.0/pygismeteo_base/types.py
--rw-r--r--   0        0        0     1047 2022-12-24 09:49:57.580029 pygismeteo_base-4.0.0/pygismeteo_base/validators.py
--rw-r--r--   0        0        0     2730 2023-01-01 14:35:55.367050 pygismeteo_base-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 pygismeteo_base-4.0.0/setup.py
--rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 pygismeteo_base-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/LICENSE
+-rw-r--r--   0        0        0      553 2023-04-19 13:39:46.260706 pygismeteo_base-4.1.0/README.md
+-rw-r--r--   0        0        0       86 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/constants.py
+-rw-r--r--   0        0        0      755 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/current.py
+-rw-r--r--   0        0        0      392 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/endpoint.py
+-rw-r--r--   0        0        0      812 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/http.py
+-rw-r--r--   0        0        0      309 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/__init__.py
+-rw-r--r--   0        0        0     1812 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/current.py
+-rw-r--r--   0        0        0      759 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_coordinates.py
+-rw-r--r--   0        0        0      673 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_ip.py
+-rw-r--r--   0        0        0      783 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_query.py
+-rw-r--r--   0        0        0     2908 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/step24.py
+-rw-r--r--   0        0        0     1786 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/step3.py
+-rw-r--r--   0        0        0     1803 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/step6.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/py.typed
+-rw-r--r--   0        0        0      955 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/search.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/step_n/__init__.py
+-rw-r--r--   0        0        0     1246 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/step_n/abc.py
+-rw-r--r--   0        0        0     1604 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/step_n/mixins.py
+-rw-r--r--   0        0        0     1453 2023-04-16 14:30:28.989419 pygismeteo_base-4.1.0/pygismeteo_base/types.py
+-rw-r--r--   0        0        0     1017 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/validators.py
+-rw-r--r--   0        0        0     2706 2023-04-19 13:23:14.550693 pygismeteo_base-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.1.0/PKG-INFO
```

### Comparing `pygismeteo_base-4.0.0/LICENSE` & `pygismeteo_base-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.0.0/README.md` & `pygismeteo_base-4.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pygismeteo-base
 
-[![CI](https://github.com/monosans/pygismeteo-base/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pygismeteo-base/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pygismeteo-base/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pygismeteo-base/main)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/pygismeteo-base?logo=pypi)](https://pypi.org/project/pygismeteo-base/)
 
 База для [pygismeteo](https://github.com/monosans/pygismeteo) и [aiopygismeteo](https://github.com/monosans/aiopygismeteo).
 
 ## License / Лицензия
 
 [MIT](https://github.com/monosans/pygismeteo-base/blob/main/LICENSE)
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/current.py` & `pygismeteo_base-4.1.0/pygismeteo_base/current.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,11 @@
 
     def _get_params_by_coordinates(
         self, latitude: float, longitude: float
     ) -> Tuple[str, types.Params]:
         coords = validators.Coordinates(latitude=latitude, longitude=longitude)
         return self._endpoint, coords.dict()
 
-    def _get_params_by_id(
-        self,
-        # pylint: disable-next=invalid-name,redefined-builtin
-        id: int,
-    ) -> Tuple[str, types.Params]:
+    def _get_params_by_id(self, id: int) -> Tuple[str, types.Params]:  # noqa: A002
         locality_id = validators.LocalityID.parse_obj(id)
         url = f"{self._endpoint}/{locality_id.__root__}"
         return url, None
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/http.py` & `pygismeteo_base-4.1.0/pygismeteo_base/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,21 @@
 
 T = TypeVar("T")
 
 
 class BaseHttpClient(Generic[T]):
     __slots__ = ("session", "settings")
 
-    def __init__(
-        self, session: Optional[T], settings: validators.Settings
-    ) -> None:
+    def __init__(self, session: Optional[T], settings: validators.Settings) -> None:
         self.session = session
         self.settings = settings
 
     def _get_params_and_headers(
         self, params: types.Params
     ) -> Tuple[types.Params, types.Headers]:
         lang_dict = {"lang": self.settings.lang} if self.settings.lang else {}
         params_dict = params or {}
         token = self.settings.token or constants.DEFAULT_TOKEN
         return {**lang_dict, **params_dict}, {"X-Gismeteo-Token": token}
 
 
-# pylint: disable-next=invalid-name
 THttpClient = TypeVar("THttpClient", bound=BaseHttpClient[Any])
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/models/current.py` & `pygismeteo_base-4.1.0/pygismeteo_base/models/current.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 
 class Precipitation(BaseModel):
-    type_ext: Optional[int] = Field(default=None)
+    type_ext: Optional[int] = None
     intensity: int
-    correction: Optional[bool] = Field(default=None)
-    amount: Optional[float] = Field(default=None)
+    correction: Optional[bool] = None
+    amount: Optional[float] = None
     duration: int
     type: int
 
 
 class Pressure(BaseModel):
-    h_pa: Optional[int] = Field(default=None)
-    mm_hg_atm: Optional[int] = Field(default=None)
-    in_hg: Optional[float] = Field(default=None)
+    h_pa: Optional[int] = None
+    mm_hg_atm: Optional[int] = None
+    in_hg: Optional[float] = None
 
 
 class Humidity(BaseModel):
-    percent: Optional[int] = Field(default=None)
+    percent: Optional[int] = None
 
 
 class Direction(BaseModel):
-    degree: Optional[int] = Field(default=None)
-    scale_8: Optional[int] = Field(default=None)
+    degree: Optional[int] = None
+    scale_8: Optional[int] = None
 
 
 class Speed(BaseModel):
     km_h: int
     m_s: int
     mi_h: int
 
@@ -42,39 +42,39 @@
 
 class Cloudiness(BaseModel):
     type: int
     percent: int
 
 
 class Date(BaseModel):
-    utc: str = Field(..., alias="UTC")
+    utc: str = Field(alias="UTC")
     local: str
     time_zone_offset: int
-    hr_to_forecast: Optional[int] = Field(default=None)
+    hr_to_forecast: Optional[int] = None
     unix: int
 
 
 class Radiation(BaseModel):
-    uvb_index: Optional[int] = Field(default=None)
+    uvb_index: Optional[int] = None
     uvb: Optional[int] = Field(default=None, alias="UVB")
 
 
 class Comfort(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Water(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Air(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Temperature(BaseModel):
     comfort: Comfort
     water: Water
     air: Air
 
@@ -88,14 +88,14 @@
     pressure: Pressure
     humidity: Humidity
     icon: str
     gm: int
     wind: Wind
     cloudiness: Cloudiness
     date: Date
-    phenomenon: Optional[int] = Field(default=None)
+    phenomenon: Optional[int] = None
     radiation: Radiation
     city: int
     kind: str
     storm: bool
     temperature: Temperature
     description: Description
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/models/search_by_coordinates.py` & `pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
 
 class District(BaseModel):
     name: str
-    name_p: str = Field(..., alias="nameP")
+    name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
-class SubDistrict(BaseModel):
+class Country(BaseModel):
     name: str
-    name_p: str = Field(..., alias="nameP")
+    code: str
+    name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
-class Country(BaseModel):
-    name: Optional[str] = Field(default=None)
-    code: str
+class SubDistrict(BaseModel):
+    name: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
 class ModelItem(BaseModel):
-    district: Optional[District] = Field(default=None)
+    district: Optional[District] = None
     id: int
-    sub_district: Optional[SubDistrict] = Field(default=None)
+    sub_district: Optional[SubDistrict] = None
     url: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
-    name: Optional[str] = Field(default=None)
-    distance: float
+    name: str
+    rate: int
+    weight: int
     kind: str
     country: Country
 
 
 class Model(BaseModel):
     __root__: List[ModelItem]
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/models/search_by_ip.py` & `pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_ip.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 
 class District(BaseModel):
     name: str
-    name_p: str = Field(..., alias="nameP")
+    name_p: str = Field(alias="nameP")
 
 
 class SubDistrict(BaseModel):
     name: str
-    name_p: str = Field(..., alias="nameP")
+    name_p: str = Field(alias="nameP")
 
 
 class Country(BaseModel):
-    name: Optional[str] = Field(default=None)
+    name: Optional[str] = None
     code: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
 class Model(BaseModel):
-    district: Optional[District] = Field(default=None)
+    district: Optional[District] = None
     id: int
-    sub_district: Optional[SubDistrict] = Field(default=None)
+    sub_district: Optional[SubDistrict] = None
     url: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
-    name: Optional[str] = Field(default=None)
+    name: Optional[str] = None
     kind: str
     country: Country
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/models/step24.py` & `pygismeteo_base-4.1.0/pygismeteo_base/models/step24.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
 
 class Precipitation(BaseModel):
-    type_ext: Optional[int] = Field(default=None)
+    type_ext: Optional[int] = None
     intensity: int
     amount: float
     type: int
 
 
 class HPa(BaseModel):
     max: int
@@ -49,68 +49,68 @@
 
 class Cloudiness(BaseModel):
     type: int
     percent: int
 
 
 class Date(BaseModel):
-    utc: str = Field(..., alias="UTC")
+    utc: str = Field(alias="UTC")
     local: str
     time_zone_offset: int
     unix: int
 
 
 class Radiation(BaseModel):
     max: int
     max_index: int
 
 
 class Max(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Min(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Comfort(BaseModel):
     max: Max
     min: Min
 
 
 class Max1(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Min1(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Water(BaseModel):
     max: Max1
     min: Min1
 
 
 class Max2(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Min2(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Avg(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Air(BaseModel):
     max: Max2
     min: Min2
     avg: Avg
 
@@ -130,38 +130,38 @@
 class Min3(BaseModel):
     km_h: int
     m_s: int
     mi_h: int
 
 
 class Avg1(BaseModel):
-    km_h: Optional[int] = Field(default=None)
-    m_s: Optional[int] = Field(default=None)
-    mi_h: Optional[int] = Field(default=None)
+    km_h: Optional[int] = None
+    m_s: Optional[int] = None
+    mi_h: Optional[int] = None
 
 
 class Speed(BaseModel):
     max: Max3
     min: Min3
     avg: Avg1
 
 
 class Max4(BaseModel):
-    degree: Optional[int] = Field(default=None)
-    scale_8: Optional[int] = Field(default=None)
+    degree: Optional[int] = None
+    scale_8: Optional[int] = None
 
 
 class Min4(BaseModel):
-    degree: Optional[int] = Field(default=None)
-    scale_8: Optional[int] = Field(default=None)
+    degree: Optional[int] = None
+    scale_8: Optional[int] = None
 
 
 class Avg2(BaseModel):
-    degree: Optional[int] = Field(default=None)
-    scale_8: Optional[int] = Field(default=None)
+    degree: Optional[int] = None
+    scale_8: Optional[int] = None
 
 
 class Direction(BaseModel):
     max: Max4
     min: Min4
     avg: Avg2
 
@@ -175,18 +175,18 @@
     precipitation: Precipitation
     pressure: Pressure
     humidity: Humidity
     gm: int
     description: Description
     cloudiness: Cloudiness
     date: Date
-    phenomenon: Optional[int] = Field(default=None)
+    phenomenon: Optional[int] = None
     radiation: Radiation
     city: int
-    kind: Optional[str] = Field(default=None)
+    kind: Optional[str] = None
     storm: bool
     temperature: Temperature
     wind: Wind
     icon: str
 
 
 class Model(BaseModel):
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/models/step3.py` & `pygismeteo_base-4.1.0/pygismeteo_base/models/step6.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
 
 class Precipitation(BaseModel):
-    type_ext: Optional[int] = Field(default=None)
+    type_ext: Optional[int] = None
     intensity: int
-    correction: Optional[bool] = Field(default=None)
-    amount: Optional[float] = Field(default=None)
+    correction: Optional[bool] = None
+    amount: float
     duration: int
     type: int
 
 
 class Pressure(BaseModel):
-    h_pa: int
-    mm_hg_atm: int
-    in_hg: float
+    h_pa: Optional[int] = None
+    mm_hg_atm: Optional[int] = None
+    in_hg: Optional[float] = None
 
 
 class Humidity(BaseModel):
-    percent: Optional[int] = Field(default=None)
+    percent: int
 
 
 class Direction(BaseModel):
-    degree: Optional[int] = Field(default=None)
-    scale_8: Optional[int] = Field(default=None)
+    degree: Optional[int] = None
+    scale_8: Optional[int] = None
 
 
 class Speed(BaseModel):
     km_h: int
     m_s: int
     mi_h: int
 
@@ -42,39 +42,39 @@
 
 class Cloudiness(BaseModel):
     type: int
     percent: int
 
 
 class Date(BaseModel):
-    utc: str = Field(..., alias="UTC")
+    utc: str = Field(alias="UTC")
     time_zone_offset: int
     local: str
-    hr_to_forecast: Optional[int] = Field(default=None)
+    hr_to_forecast: Optional[int] = None
     unix: int
 
 
 class Radiation(BaseModel):
     uvb_index: int
-    uvb: int = Field(..., alias="UVB")
+    uvb: int = Field(alias="UVB")
 
 
 class Comfort(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Water(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Air(BaseModel):
-    c: float = Field(..., alias="C")
-    f: float = Field(..., alias="F")
+    c: float = Field(alias="C")
+    f: float = Field(alias="F")
 
 
 class Temperature(BaseModel):
     comfort: Comfort
     water: Water
     air: Air
 
@@ -88,15 +88,15 @@
     pressure: Pressure
     humidity: Humidity
     icon: str
     gm: int
     wind: Wind
     cloudiness: Cloudiness
     date: Date
-    phenomenon: Optional[int] = Field(default=None)
+    phenomenon: Optional[int] = None
     radiation: Radiation
     city: int
     kind: str
     storm: bool
     temperature: Temperature
     description: Description
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/search.py` & `pygismeteo_base-4.1.0/pygismeteo_base/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,18 @@
     def _endpoint(self) -> str:
         return "search/cities"
 
     @staticmethod
     def _get_params_by_coordinates(
         latitude: float, longitude: float, *, limit: types.SearchLimit
     ) -> types.Params:
-        coordinates = validators.Coordinates(
-            latitude=latitude, longitude=longitude
-        )
+        coordinates = validators.Coordinates(latitude=latitude, longitude=longitude)
         params = coordinates.dict()
         lim = validators.SearchLimit.parse_obj(limit).__root__
-        return {**params, "limit": lim}
+        return dict(params, limit=lim)
 
     @staticmethod
     def _get_params_by_ip(ip: str) -> types.Params:
         ip = str(validators.IPAddress.parse_obj(ip).__root__)
         return {"ip": ip}
 
     @staticmethod
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/step_n/abc.py` & `pygismeteo_base-4.1.0/pygismeteo_base/step_n/abc.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,22 +23,18 @@
         pass
 
     def _get_params_by_coordinates(
         self, latitude: float, longitude: float, *, days: Union[str, int]
     ) -> Tuple[str, types.Params]:
         coords = validators.Coordinates(latitude=latitude, longitude=longitude)
         days_model = self._days_validator.parse_obj(days)
-        params = {"days": days_model.__root__, **coords.dict()}
+        params = dict(coords.dict(), days=days_model.__root__)
         return self._endpoint, params
 
     def _get_params_by_id(
-        self,
-        # pylint: disable-next=invalid-name,redefined-builtin
-        id: int,
-        *,
-        days: Union[str, int],
+        self, id: int, *, days: Union[str, int]  # noqa: A002
     ) -> Tuple[str, types.Params]:
         id_model = validators.LocalityID.parse_obj(id)
         url = f"{self._endpoint}/{id_model.__root__}"
         days_model = self._days_validator.parse_obj(days)
         params = {"days": days_model.__root__}
         return url, params
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/step_n/mixins.py` & `pygismeteo_base-4.1.0/pygismeteo_base/step_n/mixins.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/types.py` & `pygismeteo_base-4.1.0/pygismeteo_base/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,16 +58,17 @@
     35,
     36,
 ]
 
 StepNModel: TypeAlias = Type[
     Union[models.step3.Model, models.step6.Model, models.step24.Model]
 ]
-# pylint: disable-next=invalid-name
 TDays = TypeVar("TDays", Step3Days, Step6or24Days)
-# pylint: disable-next=invalid-name
+TStepNModel = TypeVar(
+    "TStepNModel", models.step3.Model, models.step6.Model, models.step24.Model
+)
 TStepNModelItem = TypeVar(
     "TStepNModelItem",
     models.step3.ModelItem,
     models.step6.ModelItem,
     models.step24.ModelItem,
 )
```

### Comparing `pygismeteo_base-4.0.0/pygismeteo_base/validators.py` & `pygismeteo_base-4.1.0/pygismeteo_base/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 class ImmutableModel(BaseModel):
     class Config:
         allow_mutation = False
         anystr_strip_whitespace = True
 
 
 class Coordinates(ImmutableModel):
-    latitude: float = Field(..., ge=-90, le=90)
-    longitude: float = Field(..., ge=-180, le=180)
+    latitude: float = Field(ge=-90, le=90)
+    longitude: float = Field(ge=-180, le=180)
 
 
 class SearchLimit(ImmutableModel):
-    __root__: int = Field(..., ge=1, le=36)
+    __root__: int = Field(ge=1, le=36)
 
 
 class IPAddress(ImmutableModel):
     __root__: IPv4Address
 
 
 class Query(ImmutableModel):
     __root__: str
 
 
 class LocalityID(ImmutableModel):
-    __root__: int = Field(..., ge=1)
+    __root__: int = Field(ge=1)
 
 
 class Step3Days(ImmutableModel):
-    __root__: int = Field(..., ge=1, le=10)
+    __root__: int = Field(ge=1, le=10)
 
 
 class Step6or24Days(ImmutableModel):
-    __root__: int = Field(..., ge=3, le=10)
+    __root__: int = Field(ge=3, le=10)
```


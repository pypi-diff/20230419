# Comparing `tmp/qdrant_client-1.1.4.tar.gz` & `tmp/qdrant_client-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.1.4.tar", max compression
+gzip compressed data, was "qdrant_client-1.1.5.tar", max compression
```

## Comparing `qdrant_client-1.1.4.tar` & `qdrant_client-1.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    11357 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/LICENSE
--rw-r--r--   0        0        0     5639 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/README.md
--rw-r--r--   0        0        0     1277 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       56 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/qdrant_client/__init__.py
--rw-r--r--   0        0        0    25845 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/qdrant_client/client_base.py
--rw-r--r--   0        0        0     1104 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3231 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    62445 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    28633 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     1794 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    13456 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    44493 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2502 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    23694 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    30407 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    30820 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    18850 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    60032 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    21902 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     5866 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2922 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     2237 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    18939 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0       40 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    10979 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1168 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1936 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    14566 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2196 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/py.typed
--rw-r--r--   0        0        0    54281 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    88692 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2865 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2537 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 qdrant_client-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-19 14:31:07.696748 qdrant_client-1.1.5/LICENSE
+-rw-r--r--   0        0        0     5690 2023-04-19 14:31:07.696748 qdrant_client-1.1.5/README.md
+-rw-r--r--   0        0        0     1277 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/__init__.py
+-rw-r--r--   0        0        0    25845 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     4459 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3231 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    62445 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    28633 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     1794 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    13456 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    44493 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2502 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    23694 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      505 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10437 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    30407 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    30820 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9499 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    18850 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    60032 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2962 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    21902 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     5888 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     2237 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    18939 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0       40 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    10979 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1168 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    14566 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2196 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/py.typed
+-rw-r--r--   0        0        0    54281 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    88752 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2865 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2537 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3200 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 qdrant_client-1.1.5/PKG-INFO
```

### Comparing `qdrant_client-1.1.4/LICENSE` & `qdrant_client-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/README.md` & `qdrant_client-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 - REST and gRPC support
 - Minimal dependencies
 
 ## Local mode
 
 <p align="center">
   <!--- https://github.com/qdrant/qdrant-client/raw/master -->
-  <img max-height="180" src="docs/images/try-develop-deploy.png" alt="Qdrant">
+  <img max-height="180" src="https://github.com/qdrant/qdrant-client/raw/master/docs/images/try-develop-deploy.png" alt="Qdrant">
 </p>
 
 Python client allows you to run same code in local mode without running Qdrant server.
 
 Simply initialize client like this:
 
 ```python
```

### Comparing `qdrant_client-1.1.4/pyproject.toml` & `qdrant_client-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.1.4"
+version = "1.1.5"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 readme = "README.md"
```

### Comparing `qdrant_client-1.1.4/qdrant_client/client_base.py` & `qdrant_client-1.1.5/qdrant_client/client_base.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/conversions/common_types.py` & `qdrant_client-1.1.5/qdrant_client/conversions/common_types.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/conversions/conversion.py` & `qdrant_client-1.1.5/qdrant_client/conversions/conversion.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.1.5/qdrant_client/grpc/collections_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.1.5/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.1.5/qdrant_client/grpc/points_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.1.5/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.1.5/qdrant_client/http/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/api/points_api.py` & `qdrant_client-1.1.5/qdrant_client/http/api/points_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/api/service_api.py` & `qdrant_client-1.1.5/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.1.5/qdrant_client/http/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/api_client.py` & `qdrant_client-1.1.5/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/exceptions.py` & `qdrant_client-1.1.5/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/http/models/models.py` & `qdrant_client-1.1.5/qdrant_client/http/models/models.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/local/distances.py` & `qdrant_client-1.1.5/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/local/geo.py` & `qdrant_client-1.1.5/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/local/local_collection.py` & `qdrant_client-1.1.5/qdrant_client/local/local_collection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/local/payload_filters.py` & `qdrant_client-1.1.5/qdrant_client/local/payload_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     return True
 
 
 def check_match(condition: models.Match, value: Any) -> bool:
     if isinstance(condition, models.MatchValue):
         return value == condition.value
     if isinstance(condition, models.MatchText):
-        return condition.text in value
+        return value is not None and condition.text in value
     if isinstance(condition, models.MatchAny):
         return value in condition.any
     raise ValueError(f"Unknown match condition: {condition}")
 
 
 def check_condition(
     condition: models.Condition, payload: dict, point_id: models.ExtendedPointId
```

### Comparing `qdrant_client-1.1.4/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.1.5/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/local/persistence.py` & `qdrant_client-1.1.5/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.1.5/qdrant_client/local/qdrant_local.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/parallel_processor.py` & `qdrant_client-1.1.5/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/proto/collections.proto` & `qdrant_client-1.1.5/qdrant_client/proto/collections.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.1.5/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.1.5/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/proto/points.proto` & `qdrant_client-1.1.5/qdrant_client/proto/points.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/proto/points_service.proto` & `qdrant_client-1.1.5/qdrant_client/proto/points_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.1.5/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/qdrant_client.py` & `qdrant_client-1.1.5/qdrant_client/qdrant_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/qdrant_remote.py` & `qdrant_client-1.1.5/qdrant_client/qdrant_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,19 @@
                 f"`host` param is not expected to contain protocol (http:// or https://). "
                 f"Try to use `url` parameter instead."
             )
 
         elif url:
             parsed_url: Url = parse_url(url)
             self._host, self._port = parsed_url.host, parsed_url.port
-            self._scheme = parsed_url.scheme if parsed_url.scheme else self._scheme
+
+            if parsed_url.scheme:
+                self._https = parsed_url.scheme == "https"
+                self._scheme = parsed_url.scheme
+
             self._port = self._port if self._port else port
 
             if self._prefix and parsed_url.path:
                 raise ValueError(
                     "Prefix can be set either in `url` or in `prefix`. "
                     f"url is {url}, prefix is {parsed_url.path}"
                 )
```

### Comparing `qdrant_client-1.1.4/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.1.5/qdrant_client/uploader/grpc_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.1.5/qdrant_client/uploader/rest_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/qdrant_client/uploader/uploader.py` & `qdrant_client-1.1.5/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.4/PKG-INFO` & `qdrant_client-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
@@ -67,15 +67,15 @@
 - REST and gRPC support
 - Minimal dependencies
 
 ## Local mode
 
 <p align="center">
   <!--- https://github.com/qdrant/qdrant-client/raw/master -->
-  <img max-height="180" src="docs/images/try-develop-deploy.png" alt="Qdrant">
+  <img max-height="180" src="https://github.com/qdrant/qdrant-client/raw/master/docs/images/try-develop-deploy.png" alt="Qdrant">
 </p>
 
 Python client allows you to run same code in local mode without running Qdrant server.
 
 Simply initialize client like this:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.4 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.5 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client Keywords: vector,search,neural,matching,client Author:
 Andrey Vasnetsov Author-email: andrey@qdrant.tech Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/mistapi-0.37.3.tar.gz` & `tmp/mistapi-0.37.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tmunzer/4_dev/Mist/python_package/dist/.tmp-ne5n6dpk/mistapi-0.37.3.tar", last modified: Thu Apr  6 09:34:53 2023, max compression
+gzip compressed data, was "mistapi-0.37.4.tar", last modified: Wed Apr 19 13:36:51 2023, max compression
```

## Comparing `mistapi-0.37.3.tar` & `mistapi-0.37.4.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.819336 mistapi-0.37.3/
--rw-r--r--   0 tmunzer    (501) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.37.3/LICENSE
--rw-r--r--   0 tmunzer    (501) staff       (20)    11332 2023-04-06 09:34:53.819666 mistapi-0.37.3/PKG-INFO
--rw-r--r--   0 tmunzer    (501) staff       (20)    10556 2023-02-22 14:11:31.000000 mistapi-0.37.3/README.md
--rw-r--r--   0 tmunzer    (501) staff       (20)      952 2023-04-06 09:34:42.000000 mistapi-0.37.3/pyproject.toml
--rw-r--r--   0 tmunzer    (501) staff       (20)      125 2023-04-06 09:34:53.822457 mistapi-0.37.3/setup.cfg
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:52.619871 mistapi-0.37.3/src/
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:52.746095 mistapi-0.37.3/src/mistapi/
--rw-r--r--   0 tmunzer    (501) staff       (20)     7162 2023-04-06 09:34:39.000000 mistapi-0.37.3/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.37.3/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    19300 2023-02-09 10:15:49.000000 mistapi-0.37.3/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (501) staff       (20)      635 2023-04-06 09:34:42.000000 mistapi-0.37.3/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.37.3/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:52.776664 mistapi-0.37.3/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (501) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.37.3/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1514 2023-02-21 08:35:01.000000 mistapi-0.37.3/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.37.3/src/mistapi/__pagination.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:52.778780 mistapi-0.37.3/src/mistapi/api/
--rw-r--r--   0 tmunzer    (501) staff       (20)      446 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:52.781256 mistapi-0.37.3/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (501) staff       (20)      869 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:52.910575 mistapi-0.37.3/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (501) staff       (20)     1133 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1041 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1193 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1042 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1035 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1052 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/call_events.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1058 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1032 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1383 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1058 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1036 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1068 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1034 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1058 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1036 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1036 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.123249 mistapi-0.37.3/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (501) staff       (20)      505 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.221131 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (501) staff       (20)      798 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1157 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1167 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     6094 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1158 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1148 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1145 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5383 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.236190 mistapi-0.37.3/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (501) staff       (20)      471 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1149 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.271488 mistapi-0.37.3/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (501) staff       (20)      460 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1080 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.325350 mistapi-0.37.3/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (501) staff       (20)      584 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)      986 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (501) staff       (20)      995 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2478 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1005 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.332810 mistapi-0.37.3/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (501) staff       (20)      460 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)      965 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.342257 mistapi-0.37.3/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (501) staff       (20)      460 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1107 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.498102 mistapi-0.37.3/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (501) staff       (20)     1060 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3005 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1100 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1724 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1186 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2386 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1730 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1678 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2235 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2700 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3649 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4239 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1641 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2981 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4884 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1921 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2175 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.701928 mistapi-0.37.3/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (501) staff       (20)     3119 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2373 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5766 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5621 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3649 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3697 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3725 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4927 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2325 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1690 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1100 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    11362 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1086 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1696 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5470 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    17436 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3766 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3817 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5593 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2959 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4491 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2386 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4454 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2353 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3474 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1290 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3713 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    12357 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3649 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3625 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3601 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3625 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3819 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1388 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2694 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4286 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1133 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3673 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     6530 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3697 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1166 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5610 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3691 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3688 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3776 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3625 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    11476 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3673 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     7535 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3747 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3625 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5954 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3734 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    27680 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1728 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4293 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5485 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1739 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3533 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3625 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3521 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     6493 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4219 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4874 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3649 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.708353 mistapi-0.37.3/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (501) staff       (20)      505 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1008 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1091 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.714296 mistapi-0.37.3/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (501) staff       (20)      508 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1011 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1084 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.728030 mistapi-0.37.3/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (501) staff       (20)      707 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2120 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1476 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1865 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1959 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1047 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1687 2023-04-06 09:34:43.000000 mistapi-0.37.3/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1606 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.812235 mistapi-0.37.3/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (501) staff       (20)     2273 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     7852 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2636 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1111 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3753 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4969 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3635 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2337 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    17038 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2308 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    52504 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5018 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3796 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5866 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     6547 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1138 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     8258 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    12510 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4273 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1165 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1735 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4184 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5910 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5471 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5702 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3659 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3679 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5435 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2254 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3862 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    20490 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1820 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (501) staff       (20)    53181 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1688 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1755 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4352 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3655 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     2220 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4272 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3820 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     5871 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4255 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     4916 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3679 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     3583 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:53.818292 mistapi-0.37.3/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (501) staff       (20)      511 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1053 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     1034 2023-04-06 09:34:44.000000 mistapi-0.37.3/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (501) staff       (20)     8483 2023-02-09 10:30:57.000000 mistapi-0.37.3/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (501) staff       (20)        0 2023-04-06 09:34:52.762369 mistapi-0.37.3/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (501) staff       (20)    11332 2023-04-06 09:34:52.000000 mistapi-0.37.3/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (501) staff       (20)     7303 2023-04-06 09:34:52.000000 mistapi-0.37.3/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (501) staff       (20)        1 2023-04-06 09:34:52.000000 mistapi-0.37.3/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (501) staff       (20)       48 2023-04-06 09:34:52.000000 mistapi-0.37.3/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (501) staff       (20)        8 2023-04-06 09:34:52.000000 mistapi-0.37.3/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.089301 mistapi-0.37.4/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.37.4/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-19 13:36:51.089395 mistapi-0.37.4/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10556 2023-02-22 14:11:31.000000 mistapi-0.37.4/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      952 2023-04-19 13:22:50.000000 mistapi-0.37.4/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-04-19 13:36:51.089806 mistapi-0.37.4/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.008642 mistapi-0.37.4/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.016897 mistapi-0.37.4/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7162 2023-04-06 09:34:39.000000 mistapi-0.37.4/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.37.4/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    19300 2023-02-09 10:15:49.000000 mistapi-0.37.4/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.37.4/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.019083 mistapi-0.37.4/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.37.4/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1514 2023-02-21 08:35:01.000000 mistapi-0.37.4/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.37.4/src/mistapi/__pagination.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.019489 mistapi-0.37.4/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.019813 mistapi-0.37.4/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.024902 mistapi-0.37.4/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1133 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1041 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1193 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1042 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1035 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1052 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/call_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1032 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1383 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1036 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1068 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1034 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1036 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1036 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.025241 mistapi-0.37.4/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.028205 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6483 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1148 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5928 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.028902 mistapi-0.37.4/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1149 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.029435 mistapi-0.37.4/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1080 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.031188 mistapi-0.37.4/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1117 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1126 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2609 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.031829 mistapi-0.37.4/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      965 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.032395 mistapi-0.37.4/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1238 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.038356 mistapi-0.37.4/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1060 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3136 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1231 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1724 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1186 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2648 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1809 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2235 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4501 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1641 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3243 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5146 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1921 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2175 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.064808 mistapi-0.37.4/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3119 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2504 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6421 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6014 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3987 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5316 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2325 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1690 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1231 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11362 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1217 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1827 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5994 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17829 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4028 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4079 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5724 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5015 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2648 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4585 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2484 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3474 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1442 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3975 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    13405 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3863 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4081 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1388 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2956 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4548 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1133 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3935 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7181 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1297 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6134 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3953 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3950 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4038 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    12655 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3935 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7662 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4009 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6216 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3996 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    27680 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1728 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4686 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5874 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1739 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3795 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3521 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6882 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4481 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5136 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.065807 mistapi-0.37.4/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1139 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1091 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.066833 mistapi-0.37.4/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1142 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1084 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.069559 mistapi-0.37.4/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2251 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1476 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1996 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2090 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1047 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1818 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.088054 mistapi-0.37.4/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2273 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8638 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2636 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1111 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4015 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5358 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3897 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17300 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    56692 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5018 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5997 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6547 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1138 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8520 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    13727 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4535 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1165 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1735 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4446 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6430 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5733 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5702 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3790 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3941 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2385 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20752 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1951 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    53181 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1688 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1886 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4614 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3917 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2220 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4534 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3820 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6260 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4517 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5178 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3941 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3845 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.089026 mistapi-0.37.4/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1053 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1165 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8483 2023-02-09 10:30:57.000000 mistapi-0.37.4/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.018532 mistapi-0.37.4/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7303 2023-04-19 13:36:51.000000 mistapi-0.37.4/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       48 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.37.3/LICENSE` & `mistapi-0.37.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/PKG-INFO` & `mistapi-0.37.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.37.3
+Version: 0.37.4
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.37.3/README.md` & `mistapi-0.37.4/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/pyproject.toml` & `mistapi-0.37.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.37.3"
+version = "0.37.4"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.37.3/src/mistapi/__api_request.py` & `mistapi-0.37.4/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/__api_response.py` & `mistapi-0.37.4/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/__api_session.py` & `mistapi-0.37.4/src/mistapi/__api_session.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/__init__.py` & `mistapi-0.37.4/src/mistapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 '''
 
 from mistapi.__api_session import APISession
 from mistapi import api
 from mistapi import cli
 from mistapi.__pagination import get_next, get_all
 
-__version__ = "0.37.3"
+__version__ = "0.37.4"
 __author__ = "Thomas Munzer <tmunzer@juniper.net>"
```

### Comparing `mistapi-0.37.3/src/mistapi/__logger.py` & `mistapi-0.37.4/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/__models/privilege.py` & `mistapi-0.37.4/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/__pagination.py` & `mistapi-0.37.4/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/ap_channels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/applications.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/applications.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/call_events.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/call_events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/client_events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/countries.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/countries.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/device_events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/device_models.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/languages.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/languages.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.37.4/src/mistapi/api/v1/const/traffic_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,184 +9,187 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerListOfRenctlyClaimedDevices
+    API doc: https://doc.mist-lab.fr/#operation/getOrgAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices"
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def claimInstallerDevices(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgAlarmTemplate(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/claimInstallerDevices
+    API doc: https://doc.mist-lab.fr/#operation/createOrgAlarmTemplate
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices"
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def unassignInstallerRecentlyClaimedDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
+def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unassignInstallerRecentlyClaimedDevice
+    API doc: https://doc.mist-lab.fr/#operation/getOrgSuppressedAlarms
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}"
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/suppress"
     query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def provisionInstallerDevices(mist_session:_APISession, org_id:str, device_mac:str, body:object) -> _APIResponse:
+def unsuppressOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/provisionInstallerDevices
+    API doc: https://doc.mist-lab.fr/#operation/unsuppressOrgSuppressedAlarms
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/suppress"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def startInstallerLocateDevice(mist_session:_APISession, org_id:str, device_mac:str, body:object) -> _APIResponse:
+def suppressOrgAlarm(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/startInstallerLocateDevice
+    API doc: https://doc.mist-lab.fr/#operation/suppressOrgAlarm
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str org_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/locate"
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/suppress"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def stopInstallerLocateDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
+def getOrgAlarmTemplate(mist_session:_APISession, org_id:str, alarmtemplate_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/stopInstallerLocateDevice
+    API doc: https://doc.mist-lab.fr/#operation/getOrgAlarmTemplate
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str device_mac        
+    :param str alarmtemplate_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/unlocate"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/{alarmtemplate_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteInstallerDeviceImage(mist_session:_APISession, org_id:str, image_name:str, device_mac:str) -> _APIResponse:
+def deleteOrgAlarmTemplate(mist_session:_APISession, org_id:str, alarmtemplate_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteInstallerDeviceImage
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgAlarmTemplate
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str image_name
-    :param str device_mac        
+    :param str alarmtemplate_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/{image_name}"
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/{alarmtemplate_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def addInstallerDeviceImageFile(mist_session:_APISession, org_id:str, image_name:str, device_mac:str, file_path:str) -> _APIResponse:
+def updateOrgAlarmTemplate(mist_session:_APISession, org_id:str, alarmtemplate_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/addInstallerDeviceImage
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgAlarmTemplate
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str image_name
-    :param str device_mac        
+    :param str alarmtemplate_id        
     
-    FILE PARAMS
+    BODY PARAMS
     -----------
-    :param str file_path - path to the file to upload
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/{image_name}"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/{alarmtemplate_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
+    return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str site_name        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -73,41 +77,45 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def importInstallerMapFile(mist_session:_APISession, org_id:str, site_name:str, file_path:str) -> _APIResponse:
+def importInstallerMapFile(mist_session:_APISession, org_id:str, site_name:str, file_path:str, body:dict={}) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importInstallerMap
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str site_name        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     FILE PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps/import"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
+        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
         return resp
-    
+
 def deleteInstallerMap(mist_session:_APISession, org_id:str, site_name:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/deleteInstallerMap
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -137,14 +145,18 @@
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str site_name
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps/{map_id}"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -159,14 +171,18 @@
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str site_name
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps/{map_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.37.4/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.37.4/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/login/login.py` & `mistapi-0.37.4/src/mistapi/api/v1/login/login.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     """
     API doc: https://doc.mist-lab.fr/#operation/login
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/login"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.37.4/src/mistapi/api/v1/login/lookup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     """
     API doc: https://doc.mist-lab.fr/#operation/lookup
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/login/lookup"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.37.4/src/mistapi/api/v1/login/oauth.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str provider        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/login/oauth/{provider}"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.37.4/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def twoFactor(mist_session:_APISession, body:object) -> _APIResponse:
+def testSiteWlanTwilioSetup(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/twoFactor
+    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTwilioSetup
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/login/two_factor"
+    uri = f"/api/v1/utils/test_twilio"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.37.4/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.37.4/src/mistapi/api/v1/mobile/verify.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str secret        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/mobile/verify/{secret}"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/orgs.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,93 +9,93 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def createOrg(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspAdmins
+    API doc: https://doc.mist-lab.fr/#operation/createOrg
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str msp_id        
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/admins"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getMspAdmin(mist_session:_APISession, msp_id:str, admin_id:str) -> _APIResponse:
+def getOrgInfo(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspAdmin
+    API doc: https://doc.mist-lab.fr/#operation/getOrgInfo
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id
-    :param str admin_id        
+    :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/admins/{admin_id}"
+    uri = f"/api/v1/orgs/{org_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def revokeMspAdmin(mist_session:_APISession, msp_id:str, admin_id:str) -> _APIResponse:
+def deleteOrg(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/revokeMspAdmin
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrg
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id
-    :param str admin_id        
+    :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/admins/{admin_id}"
+    uri = f"/api/v1/orgs/{org_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateMspAdmin(mist_session:_APISession, msp_id:str, admin_id:str, body:object) -> _APIResponse:
+def updateOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateMspAdmin
+    API doc: https://doc.mist-lab.fr/#operation/updateOrg
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id
-    :param str admin_id        
+    :param str org_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/admins/{admin_id}"
+    uri = f"/api/v1/orgs/{org_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/claim.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/claim"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/self.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,70 +9,61 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def inviteMspAdmin(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+def getSelf(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/inviteMspAdmin
+    API doc: https://doc.mist-lab.fr/#operation/getSelf
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str msp_id        
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/invites"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/self"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def uninviteMspAdmin(mist_session:_APISession, msp_id:str, invite_id:str) -> _APIResponse:
+def deleteSelf(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/uninviteMspAdmin
+    API doc: https://doc.mist-lab.fr/#operation/deleteSelf
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str msp_id
-    :param str invite_id        
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/invites/{invite_id}"
+    uri = f"/api/v1/self"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateMspAdminInvite(mist_session:_APISession, msp_id:str, invite_id:str, body:object) -> _APIResponse:
+def updateSelf(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateMspAdminInvite
+    API doc: https://doc.mist-lab.fr/#operation/updateSelf
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str msp_id
-    :param str invite_id        
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/invites/{invite_id}"
+    uri = f"/api/v1/self"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/licenses"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/logo.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/logo"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/logs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/oauth.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,85 +9,57 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def createMsp(mist_session:_APISession, body:object) -> _APIResponse:
+def getOAuth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createMsp
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/msps"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
-    
-def getMspDetails(mist_session:_APISession, msp_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getMspDetails
+    API doc: https://doc.mist-lab.fr/#operation/getOAuth2UrlForLinking
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str provider        
+    
+    QUERY PARAMS
+    ------------
+    :param str forward        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}"
-    query_params={}
+    uri = f"/api/v1/self/oauth/{provider}"
+    query_params={}
+    if forward: query_params["forward"]=forward
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteMsp(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def linkOAuth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteMsp
+    API doc: https://doc.mist-lab.fr/#operation/linkOAuth2MistAccount
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str provider        
     
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/msps/{msp_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def updateMsp(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/updateMsp
-    
-    PARAMS
+    BODY PARAMS
     -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str msp_id        
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/self/oauth/{provider}"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/orggroups"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id
     :param str orggroup_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/orggroups/{orggroup_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,126 +9,140 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspOrgs
+    API doc: https://doc.mist-lab.fr/#operation/getOrgJsiDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str org_id        
+    
+    QUERY PARAMS
+    ------------
+    :param int limit
+    :param int page
+    :param str model
+    :param str serial
+    :param str mac        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/orgs"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/jsi/devices"
+    query_params={}
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
+    if model: query_params["model"]=model
+    if serial: query_params["serial"]=serial
+    if mac: query_params["mac"]=mac
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createMspOrg(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+def adoptOrgJsiDevice(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createMspOrg
+    API doc: https://doc.mist-lab.fr/#operation/adoptOrgJsiDevice
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/orgs"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/jsi/devices/outbound_ssh_cmd"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def manageMspOrgs(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+def createOrgJsiDeviceShellSession(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/manageMspOrgs
+    API doc: https://doc.mist-lab.fr/#operation/createOrgJsiDeviceShellSession
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str org_id
+    :param str device_mac        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/orgs"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/shell"
+    resp = mist_session.mist_post(uri=uri)
     return resp
     
-def searchMspOrgs(mist_session:_APISession, msp_id:str, name:str=None, org_id:str=None, sub_insufficient:bool=None, trial_enabled:bool=None, usage_types:list=None, limit:int=100) -> _APIResponse:
+def upgradeOrgJsiDevice(mist_session:_APISession, org_id:str, device_mac:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchMspOrgs
+    API doc: https://doc.mist-lab.fr/#operation/upgradeOrgJsiDevice
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str org_id
+    :param str device_mac        
     
-    QUERY PARAMS
-    ------------
-    :param str name
-    :param str org_id - org id
-    :param bool sub_insufficient - if this org has sufficient subscription
-    :param bool trial_enabled - if this org is under trial period
-    :param list usage_types - a list of types that enabled by usage
-    :param int limit        
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/orgs/search"
-    query_params={}
-    if name: query_params["name"]=name
-    if org_id: query_params["org_id"]=org_id
-    if sub_insufficient: query_params["sub_insufficient"]=sub_insufficient
-    if trial_enabled: query_params["trial_enabled"]=trial_enabled
-    if usage_types: query_params["usage_types"]=usage_types
-    if limit: query_params["limit"]=limit
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getMspOrg(mist_session:_APISession, msp_id:str, org_id:str) -> _APIResponse:
+def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspOrg
+    API doc: https://doc.mist-lab.fr/#operation/getOrgJsiPastPurchases
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id
     :param str org_id        
     
+    QUERY PARAMS
+    ------------
+    :param int limit
+    :param int page
+    :param str model
+    :param str serial        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/orgs/{org_id}"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/jsi/inventory"
+    query_params={}
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
+    if model: query_params["model"]=model
+    if serial: query_params["serial"]=serial
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/search.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/msps.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,91 +9,93 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def createMsp(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspSsoRoles
+    API doc: https://doc.mist-lab.fr/#operation/createMsp
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str msp_id        
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/ssoroles"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/msps"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def createMspSsoRole(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+def getMspDetails(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createMspSsoRole
+    API doc: https://doc.mist-lab.fr/#operation/getMspDetails
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/ssoroles"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/msps/{msp_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteMspSsoRole(mist_session:_APISession, msp_id:str, ssorole_id:str) -> _APIResponse:
+def deleteMsp(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteMspSsoRole
+    API doc: https://doc.mist-lab.fr/#operation/deleteMsp
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id
-    :param str ssorole_id        
+    :param str msp_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/ssoroles/{ssorole_id}"
+    uri = f"/api/v1/msps/{msp_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateMspSsoRole(mist_session:_APISession, msp_id:str, ssorole_id:str, body:object) -> _APIResponse:
+def updateMsp(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateMspSsoRole
+    API doc: https://doc.mist-lab.fr/#operation/updateMsp
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id
-    :param str ssorole_id        
+    :param str msp_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/ssoroles/{ssorole_id}"
+    uri = f"/api/v1/msps/{msp_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/ssos.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -85,14 +89,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str msp_id
     :param str sso_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/stats.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/tickets.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/admins.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,14 +65,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str admin_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/admins/{admin_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/alarms.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarms/ack"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -41,14 +45,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarms/ack_all"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -133,14 +141,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarms/unack"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -153,14 +165,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarms/unack_all"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -174,14 +190,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str alarm_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarms/{alarm_id}/ack"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,175 +9,164 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAlarmTemplates
+    API doc: https://doc.mist-lab.fr/#operation/getOrgWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
+    uri = f"/api/v1/orgs/{org_id}/wxtags"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgAlarmTemplate(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgWxTag(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgAlarmTemplate
+    API doc: https://doc.mist-lab.fr/#operation/createOrgWxTag
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
+    uri = f"/api/v1/orgs/{org_id}/wxtags"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgApplicationList(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSuppressedAlarms
+    API doc: https://doc.mist-lab.fr/#operation/getOrgApplicationList
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/suppress"
+    uri = f"/api/v1/orgs/{org_id}/wxtags/apps"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def unsuppressOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgWxTag(mist_session:_APISession, org_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unsuppressOrgSuppressedAlarms
+    API doc: https://doc.mist-lab.fr/#operation/getOrgWxTag
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str org_id
+    :param str wxtag_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/suppress"
+    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}"
     query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def suppressOrgAlarm(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/suppressOrgAlarm
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str org_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/suppress"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgAlarmTemplate(mist_session:_APISession, org_id:str, alarmtemplate_id:str) -> _APIResponse:
+def deleteOrgWxTag(mist_session:_APISession, org_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAlarmTemplate
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWxTag
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str alarmtemplate_id        
+    :param str wxtag_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/{alarmtemplate_id}"
+    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def deleteOrgAlarmTemplate(mist_session:_APISession, org_id:str, alarmtemplate_id:str) -> _APIResponse:
+def updateOrgWxTag(mist_session:_APISession, org_id:str, wxtag_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgAlarmTemplate
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgWxTag
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str alarmtemplate_id        
+    :param str wxtag_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/{alarmtemplate_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def updateOrgAlarmTemplate(mist_session:_APISession, org_id:str, alarmtemplate_id:str, body:object) -> _APIResponse:
+def getOrgCurrentMatchingClientsOfAWxTag(mist_session:_APISession, org_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgAlarmTemplate
+    API doc: https://doc.mist-lab.fr/#operation/getOrgCurrentMatchingClientsOfAWxTag
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str alarmtemplate_id        
+    :param str wxtag_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/alarmtemplates/{alarmtemplate_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}/clients"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/apitokens"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str apitoken_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/apitokens/{apitoken_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/aptemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str aptemplate_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/aptemplates/{aptemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assetfilters"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str assetfilter_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assetfilters/{assetfilter_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/assets.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assets"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -75,27 +79,31 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assets/import"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def importOrgAssets(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assets/import"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -153,14 +161,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str asset_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assets/{asset_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.37.4/src/mistapi/api/v1/register/verify.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def claimOrgLicense(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def verifyRegistration(mist_session:_APISession, token:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/claimOrgLicense
+    API doc: https://doc.mist-lab.fr/#operation/verifyRegistration
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str token        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/claim"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/register/verify/{token}"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/claim.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def cloneOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def claimOrgLicense(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/cloneOrg
+    API doc: https://doc.mist-lab.fr/#operation/claimOrgLicense
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/clone"
+    uri = f"/api/v1/orgs/{org_id}/claim"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/crl.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/crl/truncate"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/deviceprofiles"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -116,14 +120,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str deviceprofile_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/deviceprofiles/{deviceprofile_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -137,14 +145,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str deviceprofile_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/deviceprofiles/{deviceprofile_id}/assign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -158,14 +170,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str deviceprofile_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/deviceprofiles/{deviceprofile_id}/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -382,14 +382,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -425,14 +429,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/{device_id}/clear_tunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -446,14 +454,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/{device_id}/provision_tunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/evpn_topologies"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str evpn_topology_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/evpn_topologies/{evpn_topology_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/gatewaytemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str gatewaytemplate_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/gatewaytemplates/{gatewaytemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/guests.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str guest_mac        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/guests/{guest_mac}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/beacons.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,131 +9,121 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgInventory(mist_session:_APISession, org_id:str, serial:str=None, model:str=None, type:str=None, mac:str=None, site_id:str=None, vc_mac:str=None, vc:str=None, unassigned:bool=None, limit:int=100, page:int=1) -> _APIResponse:
+def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgInventory
+    API doc: https://doc.mist-lab.fr/#operation/getSiteBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
-    
-    QUERY PARAMS
-    ------------
-    :param str serial - device serial
-    :param str model - device model
-    :param str type(ap, switch, gateway)
-    :param str mac - MAC address
-    :param str site_id - site id if assigned, null if not assigned
-    :param str vc_mac
-    :param str vc
-    :param bool unassigned
-    :param int limit
-    :param int page        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory"
-    query_params={}
-    if serial: query_params["serial"]=serial
-    if model: query_params["model"]=model
-    if type: query_params["type"]=type
-    if mac: query_params["mac"]=mac
-    if site_id: query_params["site_id"]=site_id
-    if vc_mac: query_params["vc_mac"]=vc_mac
-    if vc: query_params["vc"]=vc
-    if unassigned: query_params["unassigned"]=unassigned
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    uri = f"/api/v1/sites/{site_id}/beacons"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def addOrgInventory(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createSiteBeacon(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/addOrgInventory
+    API doc: https://doc.mist-lab.fr/#operation/createSiteBeacon
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory"
+    uri = f"/api/v1/sites/{site_id}/beacons"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def updateOrgInventoryAssignment(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def getSiteBeacon(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgInventoryAssignment
+    API doc: https://doc.mist-lab.fr/#operation/getSiteBeacon
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id
+    :param str beacon_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def reevaluateOrgAutoAssignment(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def deleteSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/reevaluateOrgAutoAssignment
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id
+    :param str beacon_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory/reevaluate_auto_assignment"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def replaceOrgDevices(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def updateSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/replaceOrgDevices
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str site_id
+    :param str beacon_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory/replace"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/licenses.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,70 +9,73 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def inviteOrgAdmin(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def getOrgLicencesSummary(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/inviteOrgAdmin
+    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesSummary
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/invites"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/licenses"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def uninviteOrgAdmin(mist_session:_APISession, org_id:str, invite_id:str) -> _APIResponse:
+def moveOrDeleteOrgLicenseToAnotherOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/uninviteOrgAdmin
+    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteOrgLicenseToAnotherOrg
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str invite_id        
+    :param str org_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/invites/{invite_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/licenses"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def updateOrgAdminInvite(mist_session:_APISession, org_id:str, invite_id:str, body:object) -> _APIResponse:
+def getOrgLicencesBySite(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgAdminInvite
+    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesBySite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str invite_id        
+    :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/invites/{invite_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/licenses/usages"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/orgs.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,136 +9,134 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
+def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgJsiDevices
+    API doc: https://doc.mist-lab.fr/#operation/getMspOrgs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
-    
-    QUERY PARAMS
-    ------------
-    :param int limit
-    :param int page
-    :param str model
-    :param str serial
-    :param str mac        
+    :param str msp_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/jsi/devices"
-    query_params={}
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
-    if model: query_params["model"]=model
-    if serial: query_params["serial"]=serial
-    if mac: query_params["mac"]=mac
+    uri = f"/api/v1/msps/{msp_id}/orgs"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def adoptOrgJsiDevice(mist_session:_APISession, org_id:str) -> _APIResponse:
+def createMspOrg(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/adoptOrgJsiDevice
+    API doc: https://doc.mist-lab.fr/#operation/createMspOrg
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str msp_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/jsi/devices/outbound_ssh_cmd"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/msps/{msp_id}/orgs"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def createOrgJsiDeviceShellSession(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
+def manageMspOrgs(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgJsiDeviceShellSession
+    API doc: https://doc.mist-lab.fr/#operation/manageMspOrgs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str msp_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/shell"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/msps/{msp_id}/orgs"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def upgradeOrgJsiDevice(mist_session:_APISession, org_id:str, device_mac:str, body:object) -> _APIResponse:
+def searchMspOrgs(mist_session:_APISession, msp_id:str, name:str=None, org_id:str=None, sub_insufficient:bool=None, trial_enabled:bool=None, usage_types:list=None, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/upgradeOrgJsiDevice
+    API doc: https://doc.mist-lab.fr/#operation/searchMspOrgs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str device_mac        
+    :param str msp_id        
+    
+    QUERY PARAMS
+    ------------
+    :param str name
+    :param str org_id - org id
+    :param bool sub_insufficient - if this org has sufficient subscription
+    :param bool trial_enabled - if this org is under trial period
+    :param list usage_types - a list of types that enabled by usage
+    :param int limit        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/msps/{msp_id}/orgs/search"
+    query_params={}
+    if name: query_params["name"]=name
+    if org_id: query_params["org_id"]=org_id
+    if sub_insufficient: query_params["sub_insufficient"]=sub_insufficient
+    if trial_enabled: query_params["trial_enabled"]=trial_enabled
+    if usage_types: query_params["usage_types"]=usage_types
+    if limit: query_params["limit"]=limit
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
+def getMspOrg(mist_session:_APISession, msp_id:str, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgJsiPastPurchases
+    API doc: https://doc.mist-lab.fr/#operation/getMspOrg
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
+    :param str msp_id
     :param str org_id        
     
-    QUERY PARAMS
-    ------------
-    :param int limit
-    :param int page
-    :param str model
-    :param str serial        
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/jsi/inventory"
-    query_params={}
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
-    if model: query_params["model"]=model
-    if serial: query_params["serial"]=serial
+    uri = f"/api/v1/msps/{msp_id}/orgs/{org_id}"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,69 +9,48 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgLicencesSummary(mist_session:_APISession, org_id:str) -> _APIResponse:
+def unsubscribeOrgAlarmsReports(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesSummary
+    API doc: https://doc.mist-lab.fr/#operation/unsubscribeOrgAlarmsReports
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/licenses"
+    uri = f"/api/v1/orgs/{org_id}/subscriptions"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def moveOrDeleteOrgLicenseToAnotherOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def subscribeOrgAlarmsReports(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteOrgLicenseToAnotherOrg
+    API doc: https://doc.mist-lab.fr/#operation/subscribeOrgAlarmsReports
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/licenses"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
-def getOrgLicencesBySite(mist_session:_APISession, org_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesBySite
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str org_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/licenses/usages"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/subscriptions"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/logs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.37.4/src/mistapi/api/v1/recover/verify.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,33 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def importOrgMapsFile(mist_session:_APISession, org_id:str, file_path:str) -> _APIResponse:
+def verifyRecoverPasssword(mist_session:_APISession, token:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/importOrgMaps
+    API doc: https://doc.mist-lab.fr/#operation/verifyRecoverPasssword
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
-    
-    FILE PARAMS
-    -----------
-    :param str file_path - path to the file to upload
+    :param str token        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/maps/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    uri = f"/api/v1/recover/verify/{token}"
+    resp = mist_session.mist_post(uri=uri)
+    return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxclusters"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str mxcluster_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxclusters/{mxcluster_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -71,14 +75,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/assign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -91,14 +99,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/claim"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -111,14 +123,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -152,14 +168,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -265,14 +285,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str mxedge_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -307,14 +331,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str mxedge_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}/services/tunterm/bounce_port"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -393,14 +421,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str mxedge_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxtunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str mxtunnel_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxtunnels/{mxtunnel_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nacrules"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str nacrule_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nacrules/{nacrule_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nactags"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str nactag_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nactags/{nactag_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/networks"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str network_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/networks/{network_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/networktemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str networktemplate_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/networktemplates/{networktemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,85 +9,99 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def createOrg(mist_session:_APISession, body:object) -> _APIResponse:
+def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrg
+    API doc: https://doc.mist-lab.fr/#operation/getMspSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str msp_id        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/msps/{msp_id}/ssoroles"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgInfo(mist_session:_APISession, org_id:str) -> _APIResponse:
+def createMspSsoRole(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgInfo
+    API doc: https://doc.mist-lab.fr/#operation/createMspSsoRole
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str msp_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/msps/{msp_id}/ssoroles"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def deleteOrg(mist_session:_APISession, org_id:str) -> _APIResponse:
+def deleteMspSsoRole(mist_session:_APISession, msp_id:str, ssorole_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrg
+    API doc: https://doc.mist-lab.fr/#operation/deleteMspSsoRole
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str msp_id
+    :param str ssorole_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}"
+    uri = f"/api/v1/msps/{msp_id}/ssoroles/{ssorole_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def updateMspSsoRole(mist_session:_APISession, msp_id:str, ssorole_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrg
+    API doc: https://doc.mist-lab.fr/#operation/updateMspSsoRole
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str msp_id
+    :param str ssorole_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}"
+    uri = f"/api/v1/msps/{msp_id}/ssoroles/{ssorole_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,14 +59,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/otherdevices"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -124,14 +128,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str device_mac        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/otherdevices/{device_mac}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/pma.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,113 +9,121 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgPskPortals
+    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals"
+    uri = f"/api/v1/orgs/{org_id}/webhooks"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgPskPortal(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgWebhook(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/createOrgWebhook
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals"
+    uri = f"/api/v1/orgs/{org_id}/webhooks"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str) -> _APIResponse:
+def getOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhook
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str pskportal_id        
+    :param str webhook_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str) -> _APIResponse:
+def deleteOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWebhook
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str pskportal_id        
+    :param str webhook_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str, body:object) -> _APIResponse:
+def updateOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgWebhook
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str pskportal_id        
+    :param str webhook_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/psks.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -75,14 +79,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -108,27 +116,31 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks/import"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def importOrgPsks(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgPsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks/import"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -186,14 +198,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str psk_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks/{psk_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -207,14 +223,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str psk_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks/{psk_id}/delete_old_passphrase"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/rftemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str rftemplate_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/rftemplates/{rftemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/licenses.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def updateSdkClient(mist_session:_APISession, org_id:str, sdkclient_id:str, body:object) -> _APIResponse:
+def getSiteLicenseUsage(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSdkClient
+    API doc: https://doc.mist-lab.fr/#operation/getSiteLicenseUsage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str sdkclient_id        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/sdkclients/{sdkclient_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/licenses/usages"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sdkinvites"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str sdkinvite_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sdkinvites/{sdkinvite_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -128,14 +136,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str sdkinvite_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sdkinvites/{sdkinvite_id}/email"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -171,14 +183,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str sdkinvite_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sdkinvites/{sdkinvite_id}/sms"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sdktemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str sdktemplate_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sdktemplates/{sdktemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/secpolicies"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str secpolicy_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/secpolicies/{secpolicy_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/servicepolicies"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str servicepolicy_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/servicepolicies/{servicepolicy_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/services"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str service_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/services/{service_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/setting.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -83,14 +87,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/blacklist"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -103,14 +111,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/cradlepoint/setup"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -123,14 +135,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/cradlepoint/setup"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -163,14 +179,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/juniper/link_accounts"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -204,14 +224,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/pcap_bucket/setup"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -224,14 +248,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/pcap_bucket/verify"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -286,14 +314,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/zscaler/setup"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -306,14 +338,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/zscaler/setup"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sitegroups"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str sitegroup_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sitegroups/{sitegroup_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/sites.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sites"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -183,8 +187,7 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sites/{site_name}/maps/import"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sitetemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str sitetemplate_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sitetemplates/{sitetemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssoroles"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str ssorole_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssoroles/{ssorole_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str sso_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -84,14 +88,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str upgrade_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssr/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/stats.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/update.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,48 +9,48 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def unsubscribeOrgAlarmsReports(mist_session:_APISession, org_id:str) -> _APIResponse:
+def updateSelfEmail(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unsubscribeOrgAlarmsReports
+    API doc: https://doc.mist-lab.fr/#operation/updateSelfEmail
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str org_id        
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/subscriptions"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/self/update"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def subscribeOrgAlarmsReports(mist_session:_APISession, org_id:str) -> _APIResponse:
+def verifySelfEmail(mist_session:_APISession, token:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/subscribeOrgAlarmsReports
+    API doc: https://doc.mist-lab.fr/#operation/verifySelfEmail
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str token        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/subscriptions"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/self/update/verify/{token}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/templates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str template_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/templates/{template_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -128,14 +136,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str template_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/templates/{template_id}/clone"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/tickets"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -120,14 +124,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str ticket_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/tickets/{ticket_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -154,28 +162,32 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/tickets/{ticket_id}/comments"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def addOrgTicketComment(mist_session:_APISession, org_id:str, ticket_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/addOrgTicketComment
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str ticket_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/tickets/{ticket_id}/comments"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/vpns"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str vpn_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,113 +9,121 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/getOrgPskPortals
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/orgs/{org_id}/pskportals"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgWebhook(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgPskPortal(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/createOrgPskPortal
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/orgs/{org_id}/pskportals"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
+def getOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/getOrgPskPortal
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str webhook_id        
+    :param str pskportal_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
+def deleteOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgPskPortal
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str webhook_id        
+    :param str pskportal_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str, body:object) -> _APIResponse:
+def updateOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgPskPortal
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
-    :param str webhook_id        
+    :param str pskportal_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -133,14 +137,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str wlan_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -189,28 +197,32 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_image"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def updateOrgWlanPortalTemplate(mist_session:_APISession, org_id:str, wlan_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/updateOrgWlanPortalTemplate
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str wlan_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_template"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wxrules"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -128,14 +132,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str wxrules_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wxrules/{wxrules_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/inventory.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,156 +9,147 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgInventory(mist_session:_APISession, org_id:str, serial:str=None, model:str=None, type:str=None, mac:str=None, site_id:str=None, vc_mac:str=None, vc:str=None, unassigned:bool=None, limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWxTags
+    API doc: https://doc.mist-lab.fr/#operation/getOrgInventory
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    QUERY PARAMS
+    ------------
+    :param str serial - device serial
+    :param str model - device model
+    :param str type(ap, switch, gateway)
+    :param str mac - MAC address
+    :param str site_id - site id if assigned, null if not assigned
+    :param str vc_mac
+    :param str vc
+    :param bool unassigned
+    :param int limit
+    :param int page        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wxtags"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/inventory"
+    query_params={}
+    if serial: query_params["serial"]=serial
+    if model: query_params["model"]=model
+    if type: query_params["type"]=type
+    if mac: query_params["mac"]=mac
+    if site_id: query_params["site_id"]=site_id
+    if vc_mac: query_params["vc_mac"]=vc_mac
+    if vc: query_params["vc"]=vc
+    if unassigned: query_params["unassigned"]=unassigned
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgWxTag(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def addOrgInventory(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgWxTag
+    API doc: https://doc.mist-lab.fr/#operation/addOrgInventory
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wxtags"
+    uri = f"/api/v1/orgs/{org_id}/inventory"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgApplicationList(mist_session:_APISession, org_id:str) -> _APIResponse:
+def updateOrgInventoryAssignment(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgApplicationList
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgInventoryAssignment
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/wxtags/apps"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def getOrgWxTag(mist_session:_APISession, org_id:str, wxtag_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWxTag
-    
-    PARAMS
+    BODY PARAMS
     -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str org_id
-    :param str wxtag_id        
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/inventory"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def deleteOrgWxTag(mist_session:_APISession, org_id:str, wxtag_id:str) -> _APIResponse:
+def reevaluateOrgAutoAssignment(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWxTag
+    API doc: https://doc.mist-lab.fr/#operation/reevaluateOrgAutoAssignment
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str wxtag_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def updateOrgWxTag(mist_session:_APISession, org_id:str, wxtag_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgWxTag
+    :param str org_id        
     
-    PARAMS
+    BODY PARAMS
     -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str org_id
-    :param str wxtag_id        
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/inventory/reevaluate_auto_assignment"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgCurrentMatchingClientsOfAWxTag(mist_session:_APISession, org_id:str, wxtag_id:str) -> _APIResponse:
+def replaceOrgDevices(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgCurrentMatchingClientsOfAWxTag
+    API doc: https://doc.mist-lab.fr/#operation/replaceOrgDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id
-    :param str wxtag_id        
+    :param str org_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wxtags/{wxtag_id}/clients"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/inventory/replace"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wxtunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str wxtunnel_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wxtunnels/{wxtunnel_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def recoverPassword(mist_session:_APISession, body:object) -> _APIResponse:
+def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/recoverPassword
+    API doc: https://doc.mist-lab.fr/#operation/getAlarmSubscriptions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/recover"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/self/subscriptions"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,27 +9,48 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def verifyRecoverPasssword(mist_session:_APISession, token:str) -> _APIResponse:
+def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifyRecoverPasssword
+    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str token        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/recover/verify/{token}"
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
     resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/register/register.py` & `mistapi-0.37.4/src/mistapi/api/v1/register/register.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     """
     API doc: https://doc.mist-lab.fr/#operation/registerNewAdmin
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/register"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/register/verify.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,27 +9,32 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def verifyRegistration(mist_session:_APISession, token:str) -> _APIResponse:
+def updateSdkClient(mist_session:_APISession, org_id:str, sdkclient_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifyRegistration
+    API doc: https://doc.mist-lab.fr/#operation/updateSdkClient
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str token        
+    :param str org_id
+    :param str sdkclient_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/register/verify/{token}"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/orgs/{org_id}/sdkclients/{sdkclient_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/apitokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     """
     API doc: https://doc.mist-lab.fr/#operation/createApiToken
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/self/apitokens"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/logs.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/logs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.37.4/src/mistapi/api/v1/login/two_factor.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,53 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOAuth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
+def twoFactor(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOAuth2UrlForLinking
+    API doc: https://doc.mist-lab.fr/#operation/twoFactor
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str provider        
-    
-    QUERY PARAMS
-    ------------
-    :param str forward        
-    
-    RETURN
+    BODY PARAMS
     -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/self/oauth/{provider}"
-    query_params={}
-    if forward: query_params["forward"]=forward
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def linkOAuth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/linkOAuth2MistAccount
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str provider        
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/oauth/{provider}"
+    uri = f"/api/v1/login/two_factor"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/self.py` & `mistapi-0.37.4/src/mistapi/api/v1/msps/invites.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,57 +9,78 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSelf(mist_session:_APISession) -> _APIResponse:
+def inviteMspAdmin(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSelf
+    API doc: https://doc.mist-lab.fr/#operation/inviteMspAdmin
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str msp_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/msps/{msp_id}/invites"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def deleteSelf(mist_session:_APISession) -> _APIResponse:
+def uninviteMspAdmin(mist_session:_APISession, msp_id:str, invite_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSelf
+    API doc: https://doc.mist-lab.fr/#operation/uninviteMspAdmin
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str msp_id
+    :param str invite_id        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self"
+    uri = f"/api/v1/msps/{msp_id}/invites/{invite_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSelf(mist_session:_APISession, body:object) -> _APIResponse:
+def updateMspAdminInvite(mist_session:_APISession, msp_id:str, invite_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSelf
+    API doc: https://doc.mist-lab.fr/#operation/updateMspAdminInvite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str msp_id
+    :param str invite_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self"
+    uri = f"/api/v1/msps/{msp_id}/invites/{invite_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/clone.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,24 +9,31 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
+def cloneOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getAlarmSubscriptions
+    API doc: https://doc.mist-lab.fr/#operation/cloneOrg
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/subscriptions"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/clone"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/apps.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,45 +9,28 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
+def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
+    API doc: https://doc.mist-lab.fr/#operation/getSiteApps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    QUERY PARAMS
-    ------------
-    :param str by(qrcode)        
+    PATH PARAMS
+    -----------
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/two_factor/token"
-    query_params={}
-    if by: query_params["by"]=by
+    uri = f"/api/v1/sites/{site_id}/apps"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
-    
-def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/self/two_factor/verify"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/self/update.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/sites.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,44 +9,73 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def updateSelfEmail(mist_session:_APISession, body:object) -> _APIResponse:
+def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSelfEmail
+    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/update"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def verifySelfEmail(mist_session:_APISession, token:str) -> _APIResponse:
+def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifySelfEmail
+    API doc: https://doc.mist-lab.fr/#operation/deleteSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str token        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/update/verify/{token}"
+    uri = f"/api/v1/sites/{site_id}"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/alarms.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/alarms/ack"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -41,14 +45,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/alarms/ack_all"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -149,14 +157,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/alarms/unack"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -169,14 +181,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/alarms/unack_all"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -190,14 +206,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str alarm_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/alarms/{alarm_id}/ack"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -211,14 +231,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str alarm_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/alarms/{alarm_id}/unack"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,45 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/getSiteOtherDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    QUERY PARAMS
+    ------------
+    :param str vendor
+    :param str mac
+    :param str serial
+    :param str model
+    :param str name
+    :param int page
+    :param int limit        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/otherdevices"
+    query_params={}
+    if vendor: query_params["vendor"]=vendor
+    if mac: query_params["mac"]=mac
+    if serial: query_params["serial"]=serial
+    if model: query_params["model"]=model
+    if name: query_params["name"]=name
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assetfilters"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str assetfilter_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assetfilters/{assetfilter_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/assets.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assets"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -75,27 +79,31 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assets/import"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def importSiteAssets(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSiteAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assets/import"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -153,14 +161,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str asset_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assets/{asset_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,113 +9,121 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/getSiteVBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons"
+    uri = f"/api/v1/sites/{site_id}/vbeacons"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteBeacon(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteVBeacon(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteBeacon
+    API doc: https://doc.mist-lab.fr/#operation/createSiteVBeacon
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons"
+    uri = f"/api/v1/sites/{site_id}/vbeacons"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteBeacon(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
+def getSiteVBeacon(mist_session:_APISession, site_id:str, vbeacon_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteBeacon
+    API doc: https://doc.mist-lab.fr/#operation/getSiteVBeacon
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str beacon_id        
+    :param str vbeacon_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    uri = f"/api/v1/sites/{site_id}/vbeacons/{vbeacon_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
+def deleteSiteVBeacon(mist_session:_APISession, site_id:str, vbeacon_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteVBeacon
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str beacon_id        
+    :param str vbeacon_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    uri = f"/api/v1/sites/{site_id}/vbeacons/{vbeacon_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str, body:object) -> _APIResponse:
+def updateSiteVBeacon(mist_session:_APISession, site_id:str, vbeacon_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteVBeacon
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str beacon_id        
+    :param str vbeacon_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    uri = f"/api/v1/sites/{site_id}/vbeacons/{vbeacon_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/call.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/clients/disconnect"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -345,14 +349,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/clients/unauthorize"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/count.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/devices.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -338,14 +342,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/import"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -454,14 +462,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/reset_radio_config"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -474,14 +486,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/restart"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -592,14 +608,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -681,14 +701,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/zerioze"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -746,14 +770,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -767,14 +795,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/arp"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -788,14 +820,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/bounce_port"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -809,14 +845,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/cable_test"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -830,14 +870,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/check_radius_server"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -851,14 +895,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/clear_arp"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -872,14 +920,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/clear_bgp"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -893,14 +945,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/clear_bpdu_error"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -914,14 +970,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/clear_macs"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -984,14 +1044,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/ha"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1042,15 +1106,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/image{image_number}"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def getSiteDeviceIotPort(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceIotPort
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -1078,14 +1142,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/iot"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -1121,14 +1189,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/local_port_config"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -1163,14 +1235,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/ping"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1205,14 +1281,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/release_dhcp"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1268,14 +1348,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/restart"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1289,14 +1373,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/service_ping"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1310,14 +1398,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/show_route"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1331,14 +1423,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/show_service_path"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1352,14 +1448,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/show_session"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1394,14 +1494,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/support"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1415,14 +1519,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/synthetic_test"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1436,14 +1544,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/traceroute"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1478,14 +1590,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1543,14 +1659,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/vc"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -1564,14 +1684,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/vc"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -1585,14 +1709,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/vc/vc_port"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/events.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/evpn_topologies"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str evpn_topology_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/evpn_topologies/{evpn_topology_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/guests.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,14 +166,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str guest_mac        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/guests/{guest_mac}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,52 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteLicenseUsage(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteLicenseUsage
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/licenses/usages"
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
+    
+def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/location.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/location/ml/device/{device_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -172,14 +176,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/location/ml/map/{map_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/maps.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,48 +42,56 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def importSiteMapsFile(mist_session:_APISession, site_id:str, file_path:str) -> _APIResponse:
+def importSiteMapsFile(mist_session:_APISession, site_id:str, file_path:str, body:dict={}) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSiteMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     FILE PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/import"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
+        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
         return resp
-    
+
 def getSiteMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteMap
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -133,14 +141,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -241,14 +253,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_placement"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -262,14 +278,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/clear_auto_orient"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -283,14 +303,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/clear_autoplacement"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -339,55 +363,63 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/image"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
-def replaceSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file_path:str) -> _APIResponse:
+
+def replaceSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file_path:str, body:dict={}) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/replaceSiteMapImage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     FILE PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/replace"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
+        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
         return resp
-    
+
 def bulkAssignSiteApsToMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/bulkAssignSiteApsToMap
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/set_map"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -401,14 +433,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/wayfinding/import"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,134 +9,142 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteMxEdges
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/mxedges"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteMxEdge(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteMxEdge
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/mxedges"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteMxEdge(mist_session:_APISession, site_id:str, mxedge_id:str) -> _APIResponse:
+def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteMxEdge
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id
-    :param str mxedge_id        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}"
+    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteMxEdge(mist_session:_APISession, site_id:str, mxedge_id:str) -> _APIResponse:
+def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteMxEdge
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str mxedge_id        
+    :param str wxrules_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}"
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
     query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def updateSiteMxEdge(mist_session:_APISession, site_id:str, mxedge_id:str, body:object) -> _APIResponse:
+def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteMxEdge
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str mxedge_id        
+    :param str wxrules_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def uploadSiteMxEdgeSupportFiles(mist_session:_APISession, site_id:str, mxedge_id:str) -> _APIResponse:
+def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/uploadSiteMxEdgeSupportFiles
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str mxedge_id        
+    :param str wxrules_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}/support"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/visits.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,45 +9,50 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def searchSiteZoneSessions(mist_session:_APISession, site_id:str, zone_type:str, user_type:str="client", user:str=None, scope_id:str=None, scope:str="site", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteOtherDevices
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteZoneSessions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id        
+    :param str site_id
+    :param str zone_type(zones, rssizones)        
     
     QUERY PARAMS
     ------------
-    :param str vendor
-    :param str mac
-    :param str serial
-    :param str model
-    :param str name
+    :param str user_type(client, sdkclient, asset) - user type, client (default) / sdkclient / asset
+    :param str user - client MAC / Asset MAC / SDK UUID
+    :param str scope_id - if `scope`==`map`/`zone`/`rssizone`, the scope id
+    :param str scope(site, map, zone, rssizone) - scope
     :param int page
-    :param int limit        
+    :param int limit
+    :param int start
+    :param int end
+    :param str duration        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/otherdevices"
+    uri = f"/api/v1/sites/{site_id}/{zone_type}/visits/search"
     query_params={}
-    if vendor: query_params["vendor"]=vendor
-    if mac: query_params["mac"]=mac
-    if serial: query_params["serial"]=serial
-    if model: query_params["model"]=model
-    if name: query_params["name"]=name
+    if user_type: query_params["user_type"]=user_type
+    if user: query_params["user"]=user
+    if scope_id: query_params["scope_id"]=scope_id
+    if scope: query_params["scope"]=scope
     if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,14 +99,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/pcaps/capture"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -120,14 +124,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str pcap_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/pcaps/{pcap_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/psks.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/psks"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -75,14 +79,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/psks"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -108,27 +116,31 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/psks/import"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def importSitePsks(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSitePsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/psks/import"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -186,14 +198,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str psk_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/psks/{psk_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rfdiags"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -120,14 +124,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str rfdiag_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rfdiags/{rfdiag_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/rogues.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/rrm.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rrm/optimize"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rssizones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str rssizone_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rssizones/{rssizone_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/setting.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -83,14 +87,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting/blacklist"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -124,14 +132,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting/watched_station"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -165,14 +177,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/setting/whitelist"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.37.4/src/mistapi/api/v1/self/two_factor.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,69 +9,49 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
+def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str site_id        
+    QUERY PARAMS
+    ------------
+    :param str by(qrcode)        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    query_params={}
+    uri = f"/api/v1/self/two_factor/token"
+    query_params={}
+    if by: query_params["by"]=by
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSite
+    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
-    
-    PARAMS
+    BODY PARAMS
     -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/self/two_factor/verify"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/sle.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,14 +503,18 @@
     :param str site_id
     :param str scope
     :param str scope_id - * site_id if `scope`==`site`
 * device_id if `scope`==`ap`, `scope`==`switch` or `scope`==`gateway`
 * mac if `scope`==`client`
     :param str metric - values from /api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metrics        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/threshold"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -528,14 +532,18 @@
     :param str site_id
     :param str scope
     :param str scope_id - * site_id if `scope`==`site`
 * device_id if `scope`==`ap`, `scope`==`switch` or `scope`==`gateway`
 * mac if `scope`==`client`
     :param str metric - values from /api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metrics        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/threshold"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/ssr.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/ssr/{device_id}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/stats.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.37.4/src/mistapi/api/v1/orgs/maps.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,48 +9,36 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def importOrgMapsFile(mist_session:_APISession, org_id:str, file_path:str, body:dict={}) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
+    API doc: https://doc.mist-lab.fr/#operation/importOrgMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id        
+    :param str org_id        
     
-    RETURN
+    BODY PARAMS
     -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
-    PARAMS
+    FILE PARAMS
     -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
+    :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    resp = mist_session.mist_post(uri=uri)
-    return resp
-    
+    uri = f"/api/v1/orgs/{org_id}/maps/import"
+    with open(file_path, "rb") as f:    
+        files = {"file": f.read()}
+        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
+        return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/zones.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,48 +9,121 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
+    API doc: https://doc.mist-lab.fr/#operation/getSiteZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
+    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    uri = f"/api/v1/sites/{site_id}/zones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
+    
+def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str zone_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str zone_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str zone_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
+    return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/uisettings.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/uisettings"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -128,14 +132,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str uisetting_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/uisettings/{uisetting_id}"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,113 +9,121 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteVBeacons
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vbeacons"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteVBeacon(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWxTunnel(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteVBeacon
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vbeacons"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteVBeacon(mist_session:_APISession, site_id:str, vbeacon_id:str) -> _APIResponse:
+def getSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteVBeacon
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str vbeacon_id        
+    :param str wxtunnel_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vbeacons/{vbeacon_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteVBeacon(mist_session:_APISession, site_id:str, vbeacon_id:str) -> _APIResponse:
+def deleteSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteVBeacon
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str vbeacon_id        
+    :param str wxtunnel_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vbeacons/{vbeacon_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteVBeacon(mist_session:_APISession, site_id:str, vbeacon_id:str, body:object) -> _APIResponse:
+def updateSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteVBeacon
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str vbeacon_id        
+    :param str wxtunnel_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vbeacons/{vbeacon_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/webhooks"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -107,14 +111,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str webhook_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/wlans.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -133,14 +137,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str wlan_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans/{wlan_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
@@ -167,28 +175,32 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans/{wlan_id}/portal_image"
     with open(file_path, "rb") as f:    
         files = {"file": f.read()}
         resp = mist_session.mist_post_file(uri=uri, files=files)
         return resp
-    
+
 def updateSiteWlanPortalTemplate(mist_session:_APISession, site_id:str, wlan_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/updateSiteWlanPortalTemplate
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str wlan_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans/{wlan_id}/portal_template"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,134 +9,142 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRules
+    API doc: https://doc.mist-lab.fr/#operation/getSiteMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/mxedges"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteMxEdge(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/createSiteMxEdge
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/mxedges"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteMxEdge(mist_session:_APISession, site_id:str, mxedge_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
+    API doc: https://doc.mist-lab.fr/#operation/getSiteMxEdge
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id        
+    :param str site_id
+    :param str mxedge_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
+    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+def deleteSiteMxEdge(mist_session:_APISession, site_id:str, mxedge_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteMxEdge
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str mxedge_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+def updateSiteMxEdge(mist_session:_APISession, site_id:str, mxedge_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteMxEdge
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str mxedge_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
+def uploadSiteMxEdgeSupportFiles(mist_session:_APISession, site_id:str, mxedge_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/uploadSiteMxEdgeSupportFiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str mxedge_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/mxedges/{mxedge_id}/support"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.37.4/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wxtags"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
@@ -128,14 +132,18 @@
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str wxtag_id        
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.37.4/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.37.4/src/mistapi/api/v1/recover/recover.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def testSiteWlanTwilioSetup(mist_session:_APISession, body:object) -> _APIResponse:
+def recoverPassword(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTwilioSetup
+    API doc: https://doc.mist-lab.fr/#operation/recoverPassword
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/utils/test_twilio"
+    uri = f"/api/v1/recover"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.3/src/mistapi/cli.py` & `mistapi-0.37.4/src/mistapi/cli.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.3/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.37.4/src/mistapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.37.3
+Version: 0.37.4
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.37.3/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.37.4/src/mistapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


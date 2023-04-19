# Comparing `tmp/automationkit-0.5.0.tar.gz` & `tmp/automationkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automationkit-0.5.0.tar", max compression
+gzip compressed data, was "automationkit-0.5.1.tar", max compression
```

## Comparing `automationkit-0.5.0.tar` & `automationkit-0.5.1.tar`

### file list

```diff
@@ -1,549 +1,549 @@
--rw-r--r--   0        0        0     1083 2023-01-10 08:18:42.453518 automationkit-0.5.0/LICENSE.txt
--rwxr-xr-x   0        0        0     8289 2022-12-08 18:47:43.650692 automationkit-0.5.0/README.md
--rw-r--r--   0        0        0     1532 2023-03-24 04:52:15.283551 automationkit-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0      501 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/activation/__init__.py
--rwxr-xr-x   0        0        0    10785 2023-03-17 17:44:00.403493 automationkit-0.5.0/source/packages/akit/activation/base.py
--rw-r--r--   0        0        0     3158 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/activation/console.py
--rw-r--r--   0        0        0     2352 2023-02-20 16:38:34.617539 automationkit-0.5.0/source/packages/akit/activation/service.py
--rw-r--r--   0        0        0     1246 2023-02-20 16:40:19.955545 automationkit-0.5.0/source/packages/akit/activation/testrun.py
--rwxr-xr-x   0        0        0     7749 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/aspects.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/__init__.py
--rwxr-xr-x   0        0        0     2006 2023-02-20 17:00:06.783979 automationkit-0.5.0/source/packages/akit/cli/akitcommand.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      606 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/databases/__init__.py
--rw-r--r--   0        0        0     1635 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/databases/automation.py
--rw-r--r--   0        0        0      624 2023-01-15 20:20:46.496491 automationkit-0.5.0/source/packages/akit/cli/cmdtree/generators/__init__.py
--rw-r--r--   0        0        0     3417 2023-01-25 17:04:25.895810 automationkit-0.5.0/source/packages/akit/cli/cmdtree/generators/upnp.py
--rw-r--r--   0        0        0     4750 2023-01-23 05:04:42.854487 automationkit-0.5.0/source/packages/akit/cli/cmdtree/landscape.py
--rw-r--r--   0        0        0      575 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/network/__init__.py
--rw-r--r--   0        0        0      730 2023-03-16 03:38:01.488359 automationkit-0.5.0/source/packages/akit/cli/cmdtree/network/mdns.py
--rw-r--r--   0        0        0     1987 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/network/upnp.py
--rw-r--r--   0        0        0      572 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/servers/__init__.py
--rw-r--r--   0        0        0     1468 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/servers/results_server.py
--rw-r--r--   0        0        0      792 2023-01-15 20:15:04.705991 automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/__init__.py
--rw-r--r--   0        0        0     2654 2023-02-20 16:59:46.891655 automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/constants.py
--rw-r--r--   0        0        0     5729 2023-01-15 20:15:49.622323 automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/jobs.py
--rw-r--r--   0        0        0     3730 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/query.py
--rw-r--r--   0        0        0    12682 2023-02-20 18:25:00.841768 automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/run.py
--rw-r--r--   0        0        0     2096 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/cli/cmdtree/utilities.py
--rw-r--r--   0        0        0     3020 2023-01-15 20:12:48.600978 automationkit-0.5.0/source/packages/akit/cli/cmdtree/workflow.py
--rw-r--r--   0        0        0     1707 2023-02-20 16:56:04.216007 automationkit-0.5.0/source/packages/akit/comparisons.py
--rwxr-xr-x   0        0        0     2985 2023-02-05 22:33:03.153293 automationkit-0.5.0/source/packages/akit/compat.py
--rw-r--r--   0        0        0     1187 2023-02-20 16:56:10.372109 automationkit-0.5.0/source/packages/akit/conversions.py
--rw-r--r--   0        0        0      511 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/coupling/__init__.py
--rw-r--r--   0        0        0      713 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/coupling/basecoupling.py
--rw-r--r--   0        0        0     1562 2023-03-21 19:50:22.860805 automationkit-0.5.0/source/packages/akit/coupling/coordinatorcoupling.py
--rw-r--r--   0        0        0     6560 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/coupling/coordinators/sshpoolcoordinatorintegration.py
--rw-r--r--   0        0        0     7671 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/coupling/coordinators/upnpcoordinatorintegration.py
--rw-r--r--   0        0        0     5468 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/coupling/coordinators/wirelesscoordinatorintegration.py
--rwxr-xr-x   0        0        0     8306 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/coupling/integrationcoupling.py
--rw-r--r--   0        0        0     6560 2023-03-21 19:50:22.860805 automationkit-0.5.0/source/packages/akit/coupling/sshpoolcoordinatorintegration.py
--rw-r--r--   0        0        0     7465 2023-03-21 19:56:06.186465 automationkit-0.5.0/source/packages/akit/coupling/upnpcoordinatorintegration.py
--rw-r--r--   0        0        0     5468 2023-03-21 19:50:22.860805 automationkit-0.5.0/source/packages/akit/coupling/wirelesscoordinatorintegration.py
--rwxr-xr-x   0        0        0      492 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/datum/__init__.py
--rw-r--r--   0        0        0     5286 2023-02-20 16:42:09.077603 automationkit-0.5.0/source/packages/akit/datum/dbconnection.py
--rw-r--r--   0        0        0     3235 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/datum/dbio.py
--rwxr-xr-x   0        0        0    11727 2023-03-04 03:52:34.313141 automationkit-0.5.0/source/packages/akit/datum/orm.py
--rwxr-xr-x   0        0        0      515 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/environment/__init__.py
--rwxr-xr-x   0        0        0     2994 2023-02-12 21:48:30.070383 automationkit-0.5.0/source/packages/akit/environment/configuration.py
--rwxr-xr-x   0        0        0    12692 2023-02-05 22:33:31.781412 automationkit-0.5.0/source/packages/akit/environment/context.py
--rw-r--r--   0        0        0     2358 2023-03-17 06:55:49.471603 automationkit-0.5.0/source/packages/akit/environment/contextpaths.py
--rw-r--r--   0        0        0    14042 2023-02-20 18:40:35.027117 automationkit-0.5.0/source/packages/akit/environment/optionoverrides.py
--rw-r--r--   0        0        0      367 2023-02-20 16:42:47.342310 automationkit-0.5.0/source/packages/akit/environment/system.py
--rwxr-xr-x   0        0        0    10133 2023-03-10 16:22:08.505091 automationkit-0.5.0/source/packages/akit/environment/variables.py
--rwxr-xr-x   0        0        0    22570 2023-03-21 03:23:41.039830 automationkit-0.5.0/source/packages/akit/exceptions.py
--rw-r--r--   0        0        0     5106 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/extensible.py
--rw-r--r--   0        0        0     3039 2023-02-20 16:56:19.052251 automationkit-0.5.0/source/packages/akit/extensionpoints.py
--rw-r--r--   0        0        0     2954 2023-02-20 16:56:23.092318 automationkit-0.5.0/source/packages/akit/friendlyidentifier.py
--rw-r--r--   0        0        0     2257 2023-03-03 14:34:20.424087 automationkit-0.5.0/source/packages/akit/interfaces/icommandrunner.py
--rw-r--r--   0        0        0     1295 2023-03-03 14:39:50.955261 automationkit-0.5.0/source/packages/akit/interfaces/iexcludefilter.py
--rw-r--r--   0        0        0     1288 2023-03-18 14:59:30.880461 automationkit-0.5.0/source/packages/akit/interfaces/iincludefilter.py
--rwxr-xr-x   0        0        0      555 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/__init__.py
--rwxr-xr-x   0        0        0      552 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/agents/__init__.py
--rw-r--r--   0        0        0     1574 2023-02-20 16:43:24.374987 automationkit-0.5.0/source/packages/akit/interop/agents/dnsagent.py
--rw-r--r--   0        0        0      890 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/agents/poweragents.py
--rw-r--r--   0        0        0     8264 2023-02-20 16:43:32.623138 automationkit-0.5.0/source/packages/akit/interop/agents/serialagents.py
--rwxr-xr-x   0        0        0    70773 2023-02-20 00:30:02.564939 automationkit-0.5.0/source/packages/akit/interop/agents/sshagent.py
--rw-r--r--   0        0        0   117907 2023-02-20 16:43:50.383460 automationkit-0.5.0/source/packages/akit/interop/agents/wirelessapagent.py
--rw-r--r--   0        0        0      608 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/clients/__init__.py
--rw-r--r--   0        0        0     3683 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/clients/linuxclientintegration.py
--rw-r--r--   0        0        0     3639 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/clients/windowsclientintegration.py
--rw-r--r--   0        0        0      577 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/cluster/__init__.py
--rw-r--r--   0        0        0     3609 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/cluster/clusterintegration.py
--rw-r--r--   0        0        0     9144 2023-02-20 16:44:10.971831 automationkit-0.5.0/source/packages/akit/interop/concurrency/evolution.py
--rw-r--r--   0        0        0      964 2023-02-20 16:44:15.315909 automationkit-0.5.0/source/packages/akit/interop/concurrency/procedurecontext.py
--rw-r--r--   0        0        0      559 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/coordinators/__init__.py
--rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/coordinators/coordinatorbase.py
--rw-r--r--   0        0        0     3193 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/coordinators/powercoordinator.py
--rw-r--r--   0        0        0     2591 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/coordinators/serialcoordinator.py
--rw-r--r--   0        0        0    10379 2023-02-13 00:36:36.362837 automationkit-0.5.0/source/packages/akit/interop/coordinators/sshpoolcoordinator.py
--rw-r--r--   0        0        0    55913 2023-03-16 03:58:50.510765 automationkit-0.5.0/source/packages/akit/interop/coordinators/upnpcoordinator.py
--rw-r--r--   0        0        0     2812 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/coordinators/wirelessapcoordinator.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/credentials/__init__.py
--rw-r--r--   0        0        0     1503 2023-02-25 04:10:12.127659 automationkit-0.5.0/source/packages/akit/interop/credentials/basecredential.py
--rw-r--r--   0        0        0     2836 2023-02-25 04:19:08.322028 automationkit-0.5.0/source/packages/akit/interop/credentials/basiccredential.py
--rw-r--r--   0        0        0     7520 2023-02-25 04:14:08.582552 automationkit-0.5.0/source/packages/akit/interop/credentials/credentialmanager.py
--rw-r--r--   0        0        0     4832 2023-02-25 04:18:50.853830 automationkit-0.5.0/source/packages/akit/interop/credentials/sshcredential.py
--rw-r--r--   0        0        0     2974 2023-02-25 04:18:59.901933 automationkit-0.5.0/source/packages/akit/interop/credentials/wifichoicecredential.py
--rw-r--r--   0        0        0      519 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/__init__.py
--rw-r--r--   0        0        0     2252 2023-03-16 15:58:21.513616 automationkit-0.5.0/source/packages/akit/interop/dns/dnsaddress.py
--rw-r--r--   0        0        0      763 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/dnsapi.py
--rw-r--r--   0        0        0    12410 2023-03-16 18:10:53.479049 automationkit-0.5.0/source/packages/akit/interop/dns/dnsconst.py
--rw-r--r--   0        0        0     1030 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/dnserrors.py
--rw-r--r--   0        0        0     2101 2023-03-16 15:58:21.513616 automationkit-0.5.0/source/packages/akit/interop/dns/dnshostinfo.py
--rw-r--r--   0        0        0     9118 2023-03-16 16:22:49.474030 automationkit-0.5.0/source/packages/akit/interop/dns/dnsinboundmessage.py
--rw-r--r--   0        0        0    15544 2023-03-16 17:00:25.492789 automationkit-0.5.0/source/packages/akit/interop/dns/dnsoutboundmessage.py
--rw-r--r--   0        0        0     1842 2023-03-16 15:58:21.513616 automationkit-0.5.0/source/packages/akit/interop/dns/dnspointer.py
--rw-r--r--   0        0        0     2266 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/dnsquestion.py
--rw-r--r--   0        0        0      832 2023-03-16 05:21:20.896073 automationkit-0.5.0/source/packages/akit/interop/dns/dnsquestionresults.py
--rw-r--r--   0        0        0     6896 2023-03-16 15:58:21.513616 automationkit-0.5.0/source/packages/akit/interop/dns/dnsrecord.py
--rw-r--r--   0        0        0     3576 2023-03-16 15:58:35.037773 automationkit-0.5.0/source/packages/akit/interop/dns/dnsserver.py
--rw-r--r--   0        0        0     2699 2023-03-16 15:58:21.513616 automationkit-0.5.0/source/packages/akit/interop/dns/dnsservice.py
--rw-r--r--   0        0        0     1984 2023-03-16 15:58:21.513616 automationkit-0.5.0/source/packages/akit/interop/dns/dnstext.py
--rw-r--r--   0        0        0     3713 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/dnsutil.py
--rw-r--r--   0        0        0     2784 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/dnsvalidation.py
--rw-r--r--   0        0        0     2756 2023-03-16 15:58:35.037773 automationkit-0.5.0/source/packages/akit/interop/dns/mdnscataloger.py
--rw-r--r--   0        0        0     6263 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/mdnsservicecatalog.py
--rw-r--r--   0        0        0     2505 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/dns/mdnsserviceinfo.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/eventsinking/__init__.py
--rw-r--r--   0        0        0      787 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/eventsinking/enumerations.py
--rw-r--r--   0        0        0    11897 2023-01-26 08:19:19.824084 automationkit-0.5.0/source/packages/akit/interop/eventsinking/eventedvariable.py
--rw-r--r--   0        0        0     8080 2023-01-26 08:28:56.960950 automationkit-0.5.0/source/packages/akit/interop/eventsinking/eventedvariablesink.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 automationkit-0.5.0/source/packages/akit/interop/landscaping/__init__.py
--rwxr-xr-x   0        0        0    12880 2023-02-10 06:02:39.444142 automationkit-0.5.0/source/packages/akit/interop/landscaping/landscape.py
--rw-r--r--   0        0        0     9355 2023-01-21 17:29:41.202951 automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapedescription.py
--rw-r--r--   0        0        0    12757 2023-02-01 07:11:21.531092 automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapedevice.py
--rw-r--r--   0        0        0     3447 2023-02-13 00:34:51.752193 automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapedeviceextension.py
--rw-r--r--   0        0        0     1239 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapelayerbase.py
--rw-r--r--   0        0        0    23389 2023-01-23 06:05:11.875624 automationkit-0.5.0/source/packages/akit/interop/landscaping/layers/landscapeconfigurationlayer.py
--rw-r--r--   0        0        0     2605 2023-01-23 03:34:51.638434 automationkit-0.5.0/source/packages/akit/interop/landscaping/layers/landscapeintegrationlayer.py
--rw-r--r--   0        0        0    27545 2023-02-10 06:04:11.094479 automationkit-0.5.0/source/packages/akit/interop/landscaping/layers/landscapeoperationallayer.py
--rw-r--r--   0        0        0     2901 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/landscaping/topologydescription.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/serial/__init__.py
--rw-r--r--   0        0        0     6330 2023-02-20 16:45:57.121723 automationkit-0.5.0/source/packages/akit/interop/serial/serialtelnet.py
--rw-r--r--   0        0        0    98806 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/soap/Sonoswsdl-1.19.4-20190411.142401-3.wsdl
--rw-r--r--   0        0        0      540 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/__init__.py
--rw-r--r--   0        0        0      319 2023-02-20 16:48:13.568100 automationkit-0.5.0/source/packages/akit/interop/upnp/aliases.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/content/__init__.py
--rw-r--r--   0        0        0    15570 2023-02-20 16:46:16.842069 automationkit-0.5.0/source/packages/akit/interop/upnp/content/didllite.py
--rw-r--r--   0        0        0      557 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/devices/__init__.py
--rw-r--r--   0        0        0    14041 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/devices/upnpdevice.py
--rw-r--r--   0        0        0     1764 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/devices/upnpembeddeddevice.py
--rw-r--r--   0        0        0    44827 2023-02-14 00:06:24.094433 automationkit-0.5.0/source/packages/akit/interop/upnp/devices/upnprootdevice.py
--rw-r--r--   0        0        0      494 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/__init__.py
--rw-r--r--   0        0        0     9205 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/avtransport1serviceproxy.py
--rw-r--r--   0        0        0     2651 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/connectionmanager1serviceproxy.py
--rw-r--r--   0        0        0      508 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/dial1serviceproxy.py
--rw-r--r--   0        0        0     4201 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/renderingcontrol1serviceproxy.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEAR/__init__.py
--rw-r--r--   0        0        0     1838 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEAR/layer3forwarding1serviceproxy.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEARInc/__init__.py
--rw-r--r--   0        0        0     8506 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEARInc/wfawlanconfig1serviceproxy.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/__init__.py
--rw-r--r--   0        0        0    10842 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/alarmclock1serviceproxy.py
--rw-r--r--   0        0        0     4601 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/audioin1serviceproxy.py
--rw-r--r--   0        0        0    31349 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/avtransport1serviceproxy.py
--rw-r--r--   0        0        0     2900 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/connectionmanager1serviceproxy.py
--rw-r--r--   0        0        0    10802 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/contentdirectory1serviceproxy.py
--rw-r--r--   0        0        0    18636 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/deviceproperties1serviceproxy.py
--rw-r--r--   0        0        0     3112 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/groupmanagement1serviceproxy.py
--rw-r--r--   0        0        0     3933 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/grouprenderingcontrol1serviceproxy.py
--rw-r--r--   0        0        0     4518 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/htcontrol1serviceproxy.py
--rw-r--r--   0        0        0     2647 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/musicservices1serviceproxy.py
--rw-r--r--   0        0        0     1186 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/qplay1serviceproxy.py
--rw-r--r--   0        0        0     9591 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/queue1serviceproxy.py
--rw-r--r--   0        0        0    18702 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/renderingcontrol1serviceproxy.py
--rw-r--r--   0        0        0    10097 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/systemproperties1serviceproxy.py
--rw-r--r--   0        0        0     4151 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/virtuallinein1serviceproxy.py
--rw-r--r--   0        0        0     6122 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/zonegrouptopology1serviceproxy.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/__init__.py
--rw-r--r--   0        0        0     4394 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosdevice.py
--rw-r--r--   0        0        0     8216 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosplayer.py
--rw-r--r--   0        0        0      880 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps1.py
--rw-r--r--   0        0        0      886 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps11.py
--rw-r--r--   0        0        0      884 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps12.py
--rw-r--r--   0        0        0      882 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps13.py
--rw-r--r--   0        0        0      885 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps14.py
--rw-r--r--   0        0        0      888 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps15.py
--rw-r--r--   0        0        0      888 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps16.py
--rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps17.py
--rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps18.py
--rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps19.py
--rw-r--r--   0        0        0      885 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps22.py
--rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps23.py
--rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps24.py
--rw-r--r--   0        0        0      880 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps3.py
--rw-r--r--   0        0        0      886 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps34.py
--rw-r--r--   0        0        0      885 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps38.py
--rw-r--r--   0        0        0      883 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps5.py
--rw-r--r--   0        0        0      880 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps6.py
--rw-r--r--   0        0        0      881 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps9.py
--rw-r--r--   0        0        0      884 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpssub.py
--rw-r--r--   0        0        0      898 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp120.py
--rw-r--r--   0        0        0      895 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp80.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/__init__.py
--rw-r--r--   0        0        0     3502 2023-02-15 16:19:23.285785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
--rw-r--r--   0        0        0     6212 2023-02-15 16:19:23.293785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    11191 2023-02-15 16:19:23.333786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
--rw-r--r--   0        0        0    11586 2023-02-15 16:19:23.345786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
--rw-r--r--   0        0        0    14923 2023-02-15 16:19:23.293785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
--rw-r--r--   0        0        0    20191 2023-02-15 16:19:23.321786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
--rw-r--r--   0        0        0    13573 2023-02-15 16:19:23.369787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
--rw-r--r--   0        0        0    16766 2023-02-15 16:19:23.297785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
--rw-r--r--   0        0        0     6110 2023-02-15 16:19:23.373787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
--rw-r--r--   0        0        0    12558 2023-02-15 16:19:23.357787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
--rw-r--r--   0        0        0    17010 2023-02-15 16:19:23.341786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4564 2023-02-15 16:19:23.317785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
--rw-r--r--   0        0        0      620 2023-02-15 16:19:23.293785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
--rw-r--r--   0        0        0     4099 2023-02-15 16:19:23.317785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
--rw-r--r--   0        0        0    11320 2023-02-15 16:19:23.269784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    12938 2023-02-15 16:19:23.313785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4151 2023-02-15 16:19:23.293785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
--rw-r--r--   0        0        0     4151 2023-02-15 16:19:23.361786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
--rw-r--r--   0        0        0     5709 2023-02-15 16:19:23.313785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
--rw-r--r--   0        0        0     9443 2023-02-15 16:19:23.289785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
--rw-r--r--   0        0        0    11439 2023-02-15 16:19:23.297785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
--rw-r--r--   0        0        0    13524 2023-02-15 16:19:23.289785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
--rw-r--r--   0        0        0    23734 2023-02-15 16:19:23.273784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
--rw-r--r--   0        0        0     4419 2023-02-15 16:19:23.365787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
--rw-r--r--   0        0        0     7452 2023-02-15 16:19:23.325786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
--rw-r--r--   0        0        0    10860 2023-02-15 16:19:23.325786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
--rw-r--r--   0        0        0     7721 2023-02-15 16:19:23.305785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
--rw-r--r--   0        0        0     8818 2023-02-15 16:19:23.313785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
--rw-r--r--   0        0        0     9996 2023-02-15 16:19:23.377787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
--rw-r--r--   0        0        0     2033 2023-02-15 16:19:23.365787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
--rw-r--r--   0        0        0     3982 2023-02-15 16:19:23.377787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
--rw-r--r--   0        0        0     4949 2023-02-15 16:19:23.365787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
--rw-r--r--   0        0        0     3818 2023-02-15 16:19:23.377787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
--rw-r--r--   0        0        0     3156 2023-02-15 16:19:23.353786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     2029 2023-02-15 16:19:23.381787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
--rw-r--r--   0        0        0     3567 2023-02-15 16:19:23.353786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     3061 2023-02-15 16:19:23.305785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
--rw-r--r--   0        0        0     4676 2023-02-15 16:19:23.281784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
--rw-r--r--   0        0        0     9941 2023-02-15 16:19:23.377787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
--rw-r--r--   0        0        0     1772 2023-02-15 16:19:23.305785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
--rw-r--r--   0        0        0     8061 2023-02-15 16:19:23.269784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
--rw-r--r--   0        0        0     3921 2023-02-15 16:19:23.321786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
--rw-r--r--   0        0        0     3921 2023-02-15 16:19:23.309785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
--rw-r--r--   0        0        0    10230 2023-02-15 16:19:23.349786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
--rw-r--r--   0        0        0    10230 2023-02-15 16:19:23.277784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
--rw-r--r--   0        0        0     4665 2023-02-15 16:19:23.345786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
--rw-r--r--   0        0        0     5791 2023-02-15 16:19:23.309785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
--rw-r--r--   0        0        0    11106 2023-02-15 16:19:23.377787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
--rw-r--r--   0        0        0     1681 2023-02-15 16:19:23.301785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
--rw-r--r--   0        0        0     3278 2023-02-15 16:19:23.265784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
--rw-r--r--   0        0        0     2097 2023-02-15 16:19:23.277784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
--rw-r--r--   0        0        0     2702 2023-02-15 16:19:23.325786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
--rw-r--r--   0        0        0     4708 2023-02-15 16:19:23.373787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
--rw-r--r--   0        0        0     5204 2023-02-15 16:19:23.377787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
--rw-r--r--   0        0        0     5723 2023-02-15 16:19:23.361786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
--rw-r--r--   0        0        0     1741 2023-02-15 16:19:23.281784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
--rw-r--r--   0        0        0    20937 2023-02-15 16:19:23.301785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
--rw-r--r--   0        0        0    22550 2023-02-15 16:19:23.265784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
--rw-r--r--   0        0        0    26942 2023-02-15 16:19:23.265784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
--rw-r--r--   0        0        0     7326 2023-02-15 16:19:23.369787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
--rw-r--r--   0        0        0    11148 2023-02-15 16:19:23.301785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
--rw-r--r--   0        0        0    11148 2023-02-15 16:19:23.353786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
--rw-r--r--   0        0        0     9794 2023-02-15 16:19:23.309785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
--rw-r--r--   0        0        0    10315 2023-02-15 16:19:23.309785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
--rw-r--r--   0        0        0     2189 2023-02-15 16:19:23.365787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
--rw-r--r--   0        0        0     3247 2023-02-15 16:19:23.297785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
--rw-r--r--   0        0        0     4224 2023-02-15 16:19:23.305785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
--rw-r--r--   0        0        0     7776 2023-02-15 16:19:23.305785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     8122 2023-02-15 16:19:23.341786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
--rw-r--r--   0        0        0     6168 2023-02-15 16:19:23.305785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     1341 2023-02-15 16:19:23.345786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    12404 2023-02-15 16:19:23.329786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
--rw-r--r--   0        0        0    15204 2023-02-15 16:19:23.365787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
--rw-r--r--   0        0        0     5123 2023-02-15 16:19:23.325786 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
--rw-r--r--   0        0        0     6590 2023-02-15 16:19:23.265784 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    17121 2023-02-15 16:19:23.381787 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
--rw-r--r--   0        0        0    30981 2023-02-15 16:19:23.285785 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/__init__.py
--rw-r--r--   0        0        0      479 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/__init__.py
--rw-r--r--   0        0        0      451 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/NETGEAR/urn:schemas-upnp-org:device:LANDevice:1.xml
--rw-r--r--   0        0        0      446 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/NETGEAR/urn:schemas-upnp-org:device:WANDevice:1.xml
--rw-r--r--   0        0        0     2150 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaRenderer:1.xml
--rw-r--r--   0        0        0      834 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaServer:1.xml
--rw-r--r--   0        0        0     1282 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/MicrosoftCorporation/XboxOne.xml
--rw-r--r--   0        0        0     6551 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEAR/NETGEARR7400Router.xml
--rw-r--r--   0        0        0     1178 2022-12-08 19:53:16.284698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEARInc/NETGEARR7400.xml
--rw-r--r--   0        0        0     9941 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosAmp.xml
--rw-r--r--   0        0        0     9652 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosArc.xml
--rw-r--r--   0        0        0     9666 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBRAVO.xml
--rw-r--r--   0        0        0     9622 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBeam.xml
--rw-r--r--   0        0        0     9768 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosConnectAmp.xml
--rw-r--r--   0        0        0     9654 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosFury.xml
--rw-r--r--   0        0        0     9307 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosMove.xml
--rw-r--r--   0        0        0     9281 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosOne.xml
--rw-r--r--   0        0        0     9302 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay3.xml
--rw-r--r--   0        0        0     9668 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay5.xml
--rw-r--r--   0        0        0     9647 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybar.xml
--rw-r--r--   0        0        0     9668 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybase.xml
--rw-r--r--   0        0        0     9665 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPort.xml
--rw-r--r--   0        0        0     9298 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoam.xml
--rw-r--r--   0        0        0     9344 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoamSL.xml
--rw-r--r--   0        0        0     9192 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosSub.xml
--rw-r--r--   0        0        0     9603 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosZP80.xml
--rw-r--r--   0        0        0      358 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:dial-multiscreen-org:service:dial:1.xml
--rw-r--r--   0        0        0    15561 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:AVTransport:1.xml
--rw-r--r--   0        0        0     4280 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:ConnectionManager:1.xml
--rw-r--r--   0        0        0     4888 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:RenderingControl:1.xml
--rw-r--r--   0        0        0      826 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEAR/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
--rw-r--r--   0        0        0     4785 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEARInc/urn:schemas-wifialliance-org:service:WFAWLANConfig:1.xml
--rw-r--r--   0        0        0     1697 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-tencent-com:service:QPlay:1.xml
--rw-r--r--   0        0        0    14873 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AlarmClock:1.xml
--rw-r--r--   0        0        0     4385 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AudioIn:1.xml
--rw-r--r--   0        0        0    19452 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:DeviceProperties:1.xml
--rw-r--r--   0        0        0     4053 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:GroupManagement:1.xml
--rw-r--r--   0        0        0     4098 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:HTControl:1.xml
--rw-r--r--   0        0        0     2479 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:MusicServices:1.xml
--rw-r--r--   0        0        0    14284 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:SystemProperties:1.xml
--rw-r--r--   0        0        0     8663 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:ZoneGroupTopology:1.xml
--rw-r--r--   0        0        0      247 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
--rw-r--r--   0        0        0      280 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
--rw-r--r--   0        0        0      420 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
--rw-r--r--   0        0        0     1159 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
--rw-r--r--   0        0        0     1865 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
--rw-r--r--   0        0        0      459 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
--rw-r--r--   0        0        0      604 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
--rw-r--r--   0        0        0      208 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
--rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
--rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
--rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
--rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
--rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
--rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
--rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
--rw-r--r--   0        0        0      187 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
--rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
--rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
--rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
--rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
--rw-r--r--   0        0        0      300 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
--rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
--rw-r--r--   0        0        0      561 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
--rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
--rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
--rw-r--r--   0        0        0      419 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
--rw-r--r--   0        0        0      622 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
--rw-r--r--   0        0        0      416 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
--rw-r--r--   0        0        0      936 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
--rw-r--r--   0        0        0     1090 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
--rw-r--r--   0        0        0     1244 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
--rw-r--r--   0        0        0      338 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
--rw-r--r--   0        0        0      340 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
--rw-r--r--   0        0        0      490 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
--rw-r--r--   0        0        0    21478 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
--rw-r--r--   0        0        0    22506 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
--rw-r--r--   0        0        0    32819 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
--rw-r--r--   0        0        0     3894 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
--rw-r--r--   0        0        0     5779 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
--rw-r--r--   0        0        0    10054 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
--rw-r--r--   0        0        0    22061 2022-12-08 19:53:16.288698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
--rw-r--r--   0        0        0    27823 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
--rw-r--r--   0        0        0     5740 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
--rw-r--r--   0        0        0    15507 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
--rw-r--r--   0        0        0    22397 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
--rw-r--r--   0        0        0     4082 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
--rw-r--r--   0        0        0     2151 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
--rw-r--r--   0        0        0     5359 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
--rw-r--r--   0        0        0    11356 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
--rw-r--r--   0        0        0    12959 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
--rw-r--r--   0        0        0     7870 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
--rw-r--r--   0        0        0     6485 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
--rw-r--r--   0        0        0     8455 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
--rw-r--r--   0        0        0    14206 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
--rw-r--r--   0        0        0    15034 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
--rw-r--r--   0        0        0    17600 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
--rw-r--r--   0        0        0    27620 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
--rw-r--r--   0        0        0     4821 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
--rw-r--r--   0        0        0     7808 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
--rw-r--r--   0        0        0     8486 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
--rw-r--r--   0        0        0     4783 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
--rw-r--r--   0        0        0     6607 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
--rw-r--r--   0        0        0     8457 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
--rw-r--r--   0        0        0     2249 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
--rw-r--r--   0        0        0     3447 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
--rw-r--r--   0        0        0     5176 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
--rw-r--r--   0        0        0     2637 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
--rw-r--r--   0        0        0     4564 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
--rw-r--r--   0        0        0     3751 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
--rw-r--r--   0        0        0     3673 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
--rw-r--r--   0        0        0     2461 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
--rw-r--r--   0        0        0     4528 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
--rw-r--r--   0        0        0     7628 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
--rw-r--r--   0        0        0     1045 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
--rw-r--r--   0        0        0    15694 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
--rw-r--r--   0        0        0     3331 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
--rw-r--r--   0        0        0     3234 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
--rw-r--r--   0        0        0    12147 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
--rw-r--r--   0        0        0    12076 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
--rw-r--r--   0        0        0     4682 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
--rw-r--r--   0        0        0    13539 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
--rw-r--r--   0        0        0    25446 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
--rw-r--r--   0        0        0     1919 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
--rw-r--r--   0        0        0     3445 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
--rw-r--r--   0        0        0     2800 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
--rw-r--r--   0        0        0     3264 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
--rw-r--r--   0        0        0     4324 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
--rw-r--r--   0        0        0     4744 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
--rw-r--r--   0        0        0     6642 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
--rw-r--r--   0        0        0     2399 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
--rw-r--r--   0        0        0    24162 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
--rw-r--r--   0        0        0    25624 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
--rw-r--r--   0        0        0    29018 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
--rw-r--r--   0        0        0    13767 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
--rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
--rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
--rw-r--r--   0        0        0    13686 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
--rw-r--r--   0        0        0    14103 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
--rw-r--r--   0        0        0     1285 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
--rw-r--r--   0        0        0     2951 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
--rw-r--r--   0        0        0     3412 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
--rw-r--r--   0        0        0     7592 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
--rw-r--r--   0        0        0     8319 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
--rw-r--r--   0        0        0     4926 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
--rw-r--r--   0        0        0      754 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
--rw-r--r--   0        0        0    14359 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
--rw-r--r--   0        0        0    19829 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
--rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
--rw-r--r--   0        0        0     6730 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
--rw-r--r--   0        0        0    18555 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
--rw-r--r--   0        0        0    39224 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
--rw-r--r--   0        0        0    16824 2023-02-15 16:19:08.569407 automationkit-0.5.0/source/packages/akit/interop/upnp/generator/upnpgenerator.py
--rw-r--r--   0        0        0     2631 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/paths.py
--rw-r--r--   0        0        0      481 2022-12-08 19:53:16.292698 automationkit-0.5.0/source/packages/akit/interop/upnp/services/__init__.py
--rw-r--r--   0        0        0     5524 2023-02-20 16:48:01.083885 automationkit-0.5.0/source/packages/akit/interop/upnp/services/upnpdefaultvar.py
--rw-r--r--   0        0        0    26104 2023-01-26 08:29:15.573108 automationkit-0.5.0/source/packages/akit/interop/upnp/services/upnpserviceproxy.py
--rw-r--r--   0        0        0    11706 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/interop/upnp/soap.py
--rw-r--r--   0        0        0      736 2023-02-20 16:48:22.600256 automationkit-0.5.0/source/packages/akit/interop/upnp/upnpconstants.py
--rw-r--r--   0        0        0     2543 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/interop/upnp/upnperrors.py
--rw-r--r--   0        0        0    11117 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/interop/upnp/upnpfactory.py
--rw-r--r--   0        0        0    21734 2023-01-21 17:36:57.523900 automationkit-0.5.0/source/packages/akit/interop/upnp/upnpprotocol.py
--rw-r--r--   0        0        0      494 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/interop/upnp/xml/__init__.py
--rw-r--r--   0        0        0    20799 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/interop/upnp/xml/upnpdevice1.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/interop/wireless/__init__.py
--rw-r--r--   0        0        0     4141 2023-03-06 05:11:44.961781 automationkit-0.5.0/source/packages/akit/interop/wireless/channels.py
--rw-r--r--   0        0        0     2534 2023-02-20 16:49:37.737543 automationkit-0.5.0/source/packages/akit/interop/wireless/constants.py
--rw-r--r--   0        0        0      405 2023-02-20 16:48:52.304766 automationkit-0.5.0/source/packages/akit/interop/wireless/fastpingresult.py
--rw-r--r--   0        0        0      872 2023-02-20 16:48:59.744894 automationkit-0.5.0/source/packages/akit/interop/wireless/stationinfo.py
--rw-r--r--   0        0        0      810 2023-02-20 16:49:09.685064 automationkit-0.5.0/source/packages/akit/interop/wireless/wep.py
--rw-r--r--   0        0        0      869 2023-02-20 16:49:24.553318 automationkit-0.5.0/source/packages/akit/interop/wireless/wpa.py
--rw-r--r--   0        0        0      527 2023-03-17 22:19:43.706883 automationkit-0.5.0/source/packages/akit/jsos.py
--rw-r--r--   0        0        0     2792 2023-02-17 02:06:35.231504 automationkit-0.5.0/source/packages/akit/metadata.py
--rw-r--r--   0        0        0     3514 2023-02-20 16:52:04.212020 automationkit-0.5.0/source/packages/akit/monitoring/processmonitor.py
--rw-r--r--   0        0        0     5643 2023-02-20 16:52:10.288121 automationkit-0.5.0/source/packages/akit/monitoring/reportingservice.py
--rw-r--r--   0        0        0     2672 2023-02-20 16:52:14.620194 automationkit-0.5.0/source/packages/akit/monitoring/reportmonitor.py
--rw-r--r--   0        0        0      474 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/monitoring/scripts/platforms/linux/monitor_pid
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/monitoring/templates/processmonitor.html
--rw-r--r--   0        0        0      500 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/networking/__init__.py
--rw-r--r--   0        0        0      417 2023-02-20 16:52:24.424358 automationkit-0.5.0/source/packages/akit/networking/broadcast.py
--rw-r--r--   0        0        0     7135 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/networking/constants.py
--rw-r--r--   0        0        0     3460 2023-02-20 16:52:31.568478 automationkit-0.5.0/source/packages/akit/networking/httpserverthreadpool.py
--rw-r--r--   0        0        0     9204 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/networking/interfaces.py
--rw-r--r--   0        0        0     8678 2023-02-20 16:52:39.284607 automationkit-0.5.0/source/packages/akit/networking/multicast.py
--rw-r--r--   0        0        0     2179 2023-02-20 16:52:43.824683 automationkit-0.5.0/source/packages/akit/networking/resolution.py
--rw-r--r--   0        0        0     6566 2023-02-20 16:52:49.108771 automationkit-0.5.0/source/packages/akit/networking/simplewebserver.py
--rw-r--r--   0        0        0     1520 2023-02-20 16:52:53.660847 automationkit-0.5.0/source/packages/akit/networking/trafficcapturecontext.py
--rw-r--r--   0        0        0     4392 2023-02-20 16:52:59.308942 automationkit-0.5.0/source/packages/akit/networking/unicast.py
--rwxr-xr-x   0        0        0    10158 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/paths.py
--rw-r--r--   0        0        0     2852 2023-02-20 16:56:34.988514 automationkit-0.5.0/source/packages/akit/raisefor.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/readers/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/readers/linux/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/readers/linux/command/__init__.py
--rw-r--r--   0        0        0     1481 2023-02-20 16:53:10.085121 automationkit-0.5.0/source/packages/akit/readers/linux/command/ps.py
--rwxr-xr-x   0        0        0    13324 2023-02-17 23:10:00.323743 automationkit-0.5.0/source/packages/akit/recorders.py
--rwxr-xr-x   0        0        0    10708 2023-02-03 15:53:07.738902 automationkit-0.5.0/source/packages/akit/results.py
--rwxr-xr-x   0        0        0      960 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/taskbase.py
--rwxr-xr-x   0        0        0      959 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/templates/__init__.py
--rw-r--r--   0        0        0    78077 2023-03-02 06:14:46.409423 automationkit-0.5.0/source/packages/akit/templates/static/v0/testsummary.css
--rw-r--r--   0        0        0    38006 2023-03-02 06:15:41.846020 automationkit-0.5.0/source/packages/akit/templates/static/v0/testsummary.js
--rw-r--r--   0        0        0    23424 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/templates/static/v0/w3.css
--rw-r--r--   0        0        0     3190 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/templates/tabs/tab-images.html
--rw-r--r--   0        0        0     3385 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/templates/tabs/tab-sounds.html
--rwxr-xr-x   0        0        0     6732 2023-03-02 06:32:32.638419 automationkit-0.5.0/source/packages/akit/templates/testsummary.html
--rwxr-xr-x   0        0        0      544 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/testing/__init__.py
--rw-r--r--   0        0        0     1933 2023-02-20 16:53:40.485628 automationkit-0.5.0/source/packages/akit/testing/constraints.py
--rw-r--r--   0        0        0     4370 2023-02-20 16:53:47.517745 automationkit-0.5.0/source/packages/akit/testing/expressions.py
--rw-r--r--   0        0        0     1408 2023-02-20 16:53:52.149822 automationkit-0.5.0/source/packages/akit/testing/reflection.py
--rw-r--r--   0        0        0     1220 2023-02-20 00:46:52.316497 automationkit-0.5.0/source/packages/akit/testing/testplus/__init__.py
--rw-r--r--   0        0        0     4742 2023-01-26 04:04:47.642183 automationkit-0.5.0/source/packages/akit/testing/testplus/entrypoints.py
--rw-r--r--   0        0        0     7450 2023-02-20 16:54:10.130121 automationkit-0.5.0/source/packages/akit/testing/testplus/markers.py
--rw-r--r--   0        0        0     4028 2023-02-20 16:54:05.462043 automationkit-0.5.0/source/packages/akit/testing/testplus/parameters.py
--rw-r--r--   0        0        0     3277 2023-02-20 16:54:15.750214 automationkit-0.5.0/source/packages/akit/testing/testplus/queries.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/__init__.py
--rw-r--r--   0        0        0      408 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/integrationsource.py
--rw-r--r--   0        0        0     2735 2022-12-08 19:53:16.296698 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/parameterorigin.py
--rw-r--r--   0        0        0    10818 2023-01-26 03:57:11.180559 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/resourceregistry.py
--rw-r--r--   0        0        0    15978 2023-02-16 16:37:37.667216 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/resourcescope.py
--rw-r--r--   0        0        0      439 2023-02-05 23:36:28.700299 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/resourcesource.py
--rw-r--r--   0        0        0      537 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/scopesource.py
--rw-r--r--   0        0        0     1303 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/sourcebase.py
--rw-r--r--   0        0        0      623 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/testing/testplus/registration/unknownsource.py
--rw-r--r--   0        0        0      391 2023-02-20 16:54:20.910300 automationkit-0.5.0/source/packages/akit/testing/testplus/resourcelifespan.py
--rw-r--r--   0        0        0     6973 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/testing/testplus/resources.py
--rwxr-xr-x   0        0        0     8005 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/testing/testplus/scopecoupling.py
--rwxr-xr-x   0        0        0     9298 2023-02-10 06:14:58.794934 automationkit-0.5.0/source/packages/akit/testing/testplus/testcollector.py
--rw-r--r--   0        0        0     5115 2023-02-10 06:59:21.438953 automationkit-0.5.0/source/packages/akit/testing/testplus/testgroup.py
--rwxr-xr-x   0        0        0    17620 2023-02-17 23:06:27.929145 automationkit-0.5.0/source/packages/akit/testing/testplus/testjob.py
--rwxr-xr-x   0        0        0     4524 2023-02-09 22:27:08.127427 automationkit-0.5.0/source/packages/akit/testing/testplus/testref.py
--rw-r--r--   0        0        0    38166 2023-02-17 02:09:10.143486 automationkit-0.5.0/source/packages/akit/testing/testplus/testsequencer.py
--rw-r--r--   0        0        0    17481 2023-02-20 16:54:39.434607 automationkit-0.5.0/source/packages/akit/testing/testplus/verification.py
--rwxr-xr-x   0        0        0     6035 2023-01-25 17:53:53.625118 automationkit-0.5.0/source/packages/akit/testing/utilities.py
--rw-r--r--   0        0        0     6524 2023-02-20 16:56:43.860660 automationkit-0.5.0/source/packages/akit/timemachine.py
--rwxr-xr-x   0        0        0     7103 2023-01-27 16:12:24.390033 automationkit-0.5.0/source/packages/akit/timeouts.py
--rw-r--r--   0        0        0     8877 2023-03-11 05:15:15.284442 automationkit-0.5.0/source/packages/akit/waiting.py
--rw-r--r--   0        0        0        0 2023-01-25 16:55:15.635053 automationkit-0.5.0/source/packages/akit/wellknown/__init__.py
--rw-r--r--   0        0        0     1128 2023-02-20 16:54:54.654859 automationkit-0.5.0/source/packages/akit/wellknown/singletons.py
--rw-r--r--   0        0        0      303 2023-03-10 01:29:50.415382 automationkit-0.5.0/source/packages/akit/wellknownports.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/workflow/__init__.py
--rw-r--r--   0        0        0     2720 2023-01-15 13:31:47.440771 automationkit-0.5.0/source/packages/akit/workflow/entrypoints.py
--rw-r--r--   0        0        0     4484 2023-01-15 13:38:10.967670 automationkit-0.5.0/source/packages/akit/workflow/execution.py
--rw-r--r--   0        0        0        0 2023-01-15 05:47:46.525125 automationkit-0.5.0/source/packages/akit/workflow/tasks/__init__.py
--rw-r--r--   0        0        0     3616 2023-01-15 16:19:11.246722 automationkit-0.5.0/source/packages/akit/workflow/tasks/createenvironment.py
--rw-r--r--   0        0        0     1861 2023-01-15 06:38:46.840778 automationkit-0.5.0/source/packages/akit/workflow/tasks/embeddedpython.py
--rw-r--r--   0        0        0     1059 2023-01-15 06:39:11.257060 automationkit-0.5.0/source/packages/akit/workflow/tasks/gitcheckout.py
--rw-r--r--   0        0        0     1992 2023-01-15 06:39:04.556982 automationkit-0.5.0/source/packages/akit/workflow/tasks/runcommand.py
--rw-r--r--   0        0        0     2183 2023-01-15 06:38:56.548890 automationkit-0.5.0/source/packages/akit/workflow/tasks/shellscript.py
--rw-r--r--   0        0        0     1656 2023-01-15 06:37:20.407782 automationkit-0.5.0/source/packages/akit/workflow/tasks/taskbase.py
--rw-r--r--   0        0        0    11913 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xcollections.py
--rw-r--r--   0        0        0      556 2023-02-20 16:56:58.244896 automationkit-0.5.0/source/packages/akit/xconfiguration.py
--rw-r--r--   0        0        0      467 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/xcryptography/__init__.py
--rw-r--r--   0        0        0     1969 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/xcryptography/pkey.py
--rw-r--r--   0        0        0     6482 2022-12-08 19:53:16.272698 automationkit-0.5.0/source/packages/akit/xcryptography/x509.py
--rw-r--r--   0        0        0     4401 2023-02-20 16:57:03.144976 automationkit-0.5.0/source/packages/akit/xdebugger.py
--rw-r--r--   0        0        0     1418 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xenum.py
--rw-r--r--   0        0        0     6014 2023-02-20 16:57:10.837103 automationkit-0.5.0/source/packages/akit/xfeature.py
--rw-r--r--   0        0        0     4655 2023-03-11 03:41:48.245645 automationkit-0.5.0/source/packages/akit/xformatting.py
--rw-r--r--   0        0        0     1986 2023-03-16 21:57:31.426396 automationkit-0.5.0/source/packages/akit/xinspect.py
--rw-r--r--   0        0        0      550 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xlogging/__init__.py
--rw-r--r--   0        0        0    24838 2023-02-03 06:05:31.946933 automationkit-0.5.0/source/packages/akit/xlogging/foundations.py
--rw-r--r--   0        0        0    10390 2023-03-22 16:53:04.861736 automationkit-0.5.0/source/packages/akit/xlogging/scopemonitoring.py
--rw-r--r--   0        0        0     2256 2023-02-20 16:55:32.631486 automationkit-0.5.0/source/packages/akit/xml/parsing.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xmultiprocessing/__init__.py
--rw-r--r--   0        0        0     3514 2023-02-20 16:55:38.471583 automationkit-0.5.0/source/packages/akit/xmultiprocessing/smbserverprocess.py
--rw-r--r--   0        0        0     1027 2023-02-20 16:55:42.947656 automationkit-0.5.0/source/packages/akit/xmultiprocessing/webserverprocess.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xregex/__init__.py
--rw-r--r--   0        0        0    13244 2023-02-20 16:55:49.999773 automationkit-0.5.0/source/packages/akit/xregex/regexreader.py
--rw-r--r--   0        0        0      544 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xthreading/__init__.py
--rw-r--r--   0        0        0     3278 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xthreading/looper.py
--rw-r--r--   0        0        0     4911 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xthreading/looperpool.py
--rw-r--r--   0        0        0     3555 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xthreading/looperqueue.py
--rw-r--r--   0        0        0     5793 2022-12-08 19:53:16.300698 automationkit-0.5.0/source/packages/akit/xthreading/readwritelock.py
--rwxr-xr-x   0        0        0     2153 2023-02-05 22:33:18.961356 automationkit-0.5.0/source/packages/akit/xtime.py
--rw-r--r--   0        0        0      472 2023-02-20 16:57:20.933268 automationkit-0.5.0/source/packages/akit/xtraceback.py
--rw-r--r--   0        0        0    12613 1970-01-01 00:00:00.000000 automationkit-0.5.0/setup.py
--rw-r--r--   0        0        0    10080 1970-01-01 00:00:00.000000 automationkit-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-10 08:18:42.453518 automationkit-0.5.1/LICENSE.txt
+-rwxr-xr-x   0        0        0     8429 2023-03-26 18:03:35.445080 automationkit-0.5.1/README.md
+-rw-r--r--   0        0        0     1531 2023-04-19 05:46:34.684641 automationkit-0.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0      501 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/activation/__init__.py
+-rwxr-xr-x   0        0        0    10785 2023-03-17 17:44:00.403493 automationkit-0.5.1/source/packages/akit/activation/base.py
+-rw-r--r--   0        0        0     3158 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/activation/console.py
+-rw-r--r--   0        0        0     2352 2023-02-20 16:38:34.617539 automationkit-0.5.1/source/packages/akit/activation/service.py
+-rw-r--r--   0        0        0     1246 2023-02-20 16:40:19.955545 automationkit-0.5.1/source/packages/akit/activation/testrun.py
+-rwxr-xr-x   0        0        0     7749 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/aspects.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/__init__.py
+-rwxr-xr-x   0        0        0     2006 2023-02-20 17:00:06.783979 automationkit-0.5.1/source/packages/akit/cli/akitcommand.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      606 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/databases/__init__.py
+-rw-r--r--   0        0        0     1635 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/databases/automation.py
+-rw-r--r--   0        0        0      624 2023-01-15 20:20:46.496491 automationkit-0.5.1/source/packages/akit/cli/cmdtree/generators/__init__.py
+-rw-r--r--   0        0        0     3417 2023-01-25 17:04:25.895810 automationkit-0.5.1/source/packages/akit/cli/cmdtree/generators/upnp.py
+-rw-r--r--   0        0        0     4750 2023-01-23 05:04:42.854487 automationkit-0.5.1/source/packages/akit/cli/cmdtree/landscape.py
+-rw-r--r--   0        0        0      575 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/network/__init__.py
+-rw-r--r--   0        0        0      730 2023-03-16 03:38:01.488359 automationkit-0.5.1/source/packages/akit/cli/cmdtree/network/mdns.py
+-rw-r--r--   0        0        0     1987 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/network/upnp.py
+-rw-r--r--   0        0        0      572 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/servers/__init__.py
+-rw-r--r--   0        0        0     1468 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/servers/results_server.py
+-rw-r--r--   0        0        0      792 2023-01-15 20:15:04.705991 automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/__init__.py
+-rw-r--r--   0        0        0     2654 2023-02-20 16:59:46.891655 automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/constants.py
+-rw-r--r--   0        0        0     5729 2023-01-15 20:15:49.622323 automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/jobs.py
+-rw-r--r--   0        0        0     3730 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/query.py
+-rw-r--r--   0        0        0    12682 2023-02-20 18:25:00.841768 automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/run.py
+-rw-r--r--   0        0        0     2096 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/cli/cmdtree/utilities.py
+-rw-r--r--   0        0        0     3020 2023-01-15 20:12:48.600978 automationkit-0.5.1/source/packages/akit/cli/cmdtree/workflow.py
+-rw-r--r--   0        0        0     1707 2023-02-20 16:56:04.216007 automationkit-0.5.1/source/packages/akit/comparisons.py
+-rwxr-xr-x   0        0        0     2985 2023-02-05 22:33:03.153293 automationkit-0.5.1/source/packages/akit/compat.py
+-rw-r--r--   0        0        0     1187 2023-02-20 16:56:10.372109 automationkit-0.5.1/source/packages/akit/conversions.py
+-rw-r--r--   0        0        0      511 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/coupling/__init__.py
+-rw-r--r--   0        0        0      713 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/coupling/basecoupling.py
+-rw-r--r--   0        0        0     1562 2023-03-21 19:50:22.860805 automationkit-0.5.1/source/packages/akit/coupling/coordinatorcoupling.py
+-rw-r--r--   0        0        0     6560 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/coupling/coordinators/sshpoolcoordinatorintegration.py
+-rw-r--r--   0        0        0     7671 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/coupling/coordinators/upnpcoordinatorintegration.py
+-rw-r--r--   0        0        0     5468 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/coupling/coordinators/wirelesscoordinatorintegration.py
+-rwxr-xr-x   0        0        0     8306 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/coupling/integrationcoupling.py
+-rw-r--r--   0        0        0     6560 2023-03-21 19:50:22.860805 automationkit-0.5.1/source/packages/akit/coupling/sshpoolcoordinatorintegration.py
+-rw-r--r--   0        0        0     7465 2023-03-21 19:56:06.186465 automationkit-0.5.1/source/packages/akit/coupling/upnpcoordinatorintegration.py
+-rw-r--r--   0        0        0     5468 2023-03-21 19:50:22.860805 automationkit-0.5.1/source/packages/akit/coupling/wirelesscoordinatorintegration.py
+-rwxr-xr-x   0        0        0      492 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/datum/__init__.py
+-rw-r--r--   0        0        0     5286 2023-02-20 16:42:09.077603 automationkit-0.5.1/source/packages/akit/datum/dbconnection.py
+-rw-r--r--   0        0        0     3235 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/datum/dbio.py
+-rwxr-xr-x   0        0        0    11727 2023-03-04 03:52:34.313141 automationkit-0.5.1/source/packages/akit/datum/orm.py
+-rwxr-xr-x   0        0        0      515 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/environment/__init__.py
+-rwxr-xr-x   0        0        0     2994 2023-02-12 21:48:30.070383 automationkit-0.5.1/source/packages/akit/environment/configuration.py
+-rwxr-xr-x   0        0        0    12692 2023-02-05 22:33:31.781412 automationkit-0.5.1/source/packages/akit/environment/context.py
+-rw-r--r--   0        0        0     2358 2023-03-17 06:55:49.471603 automationkit-0.5.1/source/packages/akit/environment/contextpaths.py
+-rw-r--r--   0        0        0    14042 2023-02-20 18:40:35.027117 automationkit-0.5.1/source/packages/akit/environment/optionoverrides.py
+-rw-r--r--   0        0        0      367 2023-02-20 16:42:47.342310 automationkit-0.5.1/source/packages/akit/environment/system.py
+-rwxr-xr-x   0        0        0    10133 2023-03-10 16:22:08.505091 automationkit-0.5.1/source/packages/akit/environment/variables.py
+-rwxr-xr-x   0        0        0    22570 2023-03-21 03:23:41.039830 automationkit-0.5.1/source/packages/akit/exceptions.py
+-rw-r--r--   0        0        0     5106 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/extensible.py
+-rw-r--r--   0        0        0     3039 2023-02-20 16:56:19.052251 automationkit-0.5.1/source/packages/akit/extensionpoints.py
+-rw-r--r--   0        0        0     2954 2023-02-20 16:56:23.092318 automationkit-0.5.1/source/packages/akit/friendlyidentifier.py
+-rw-r--r--   0        0        0     2257 2023-03-03 14:34:20.424087 automationkit-0.5.1/source/packages/akit/interfaces/icommandrunner.py
+-rw-r--r--   0        0        0     1295 2023-03-03 14:39:50.955261 automationkit-0.5.1/source/packages/akit/interfaces/iexcludefilter.py
+-rw-r--r--   0        0        0     1288 2023-03-18 14:59:30.880461 automationkit-0.5.1/source/packages/akit/interfaces/iincludefilter.py
+-rwxr-xr-x   0        0        0      555 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/__init__.py
+-rwxr-xr-x   0        0        0      552 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/agents/__init__.py
+-rw-r--r--   0        0        0     1574 2023-02-20 16:43:24.374987 automationkit-0.5.1/source/packages/akit/interop/agents/dnsagent.py
+-rw-r--r--   0        0        0      890 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/agents/poweragents.py
+-rw-r--r--   0        0        0     8233 2023-03-26 18:03:35.449080 automationkit-0.5.1/source/packages/akit/interop/agents/serialagents.py
+-rwxr-xr-x   0        0        0    70773 2023-02-20 00:30:02.564939 automationkit-0.5.1/source/packages/akit/interop/agents/sshagent.py
+-rw-r--r--   0        0        0   117907 2023-02-20 16:43:50.383460 automationkit-0.5.1/source/packages/akit/interop/agents/wirelessapagent.py
+-rw-r--r--   0        0        0      608 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/clients/__init__.py
+-rw-r--r--   0        0        0     3683 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/clients/linuxclientintegration.py
+-rw-r--r--   0        0        0     3639 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/clients/windowsclientintegration.py
+-rw-r--r--   0        0        0      577 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/cluster/__init__.py
+-rw-r--r--   0        0        0     3609 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/cluster/clusterintegration.py
+-rw-r--r--   0        0        0     9144 2023-02-20 16:44:10.971831 automationkit-0.5.1/source/packages/akit/interop/concurrency/evolution.py
+-rw-r--r--   0        0        0      964 2023-02-20 16:44:15.315909 automationkit-0.5.1/source/packages/akit/interop/concurrency/procedurecontext.py
+-rw-r--r--   0        0        0      559 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/coordinators/__init__.py
+-rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/coordinators/coordinatorbase.py
+-rw-r--r--   0        0        0     3193 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/coordinators/powercoordinator.py
+-rw-r--r--   0        0        0     2591 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/coordinators/serialcoordinator.py
+-rw-r--r--   0        0        0    10379 2023-02-13 00:36:36.362837 automationkit-0.5.1/source/packages/akit/interop/coordinators/sshpoolcoordinator.py
+-rw-r--r--   0        0        0    55913 2023-03-16 03:58:50.510765 automationkit-0.5.1/source/packages/akit/interop/coordinators/upnpcoordinator.py
+-rw-r--r--   0        0        0     2812 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/coordinators/wirelessapcoordinator.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/credentials/__init__.py
+-rw-r--r--   0        0        0     1503 2023-02-25 04:10:12.127659 automationkit-0.5.1/source/packages/akit/interop/credentials/basecredential.py
+-rw-r--r--   0        0        0     2836 2023-02-25 04:19:08.322028 automationkit-0.5.1/source/packages/akit/interop/credentials/basiccredential.py
+-rw-r--r--   0        0        0     7520 2023-02-25 04:14:08.582552 automationkit-0.5.1/source/packages/akit/interop/credentials/credentialmanager.py
+-rw-r--r--   0        0        0     4832 2023-02-25 04:18:50.853830 automationkit-0.5.1/source/packages/akit/interop/credentials/sshcredential.py
+-rw-r--r--   0        0        0     2974 2023-02-25 04:18:59.901933 automationkit-0.5.1/source/packages/akit/interop/credentials/wifichoicecredential.py
+-rw-r--r--   0        0        0      519 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/__init__.py
+-rw-r--r--   0        0        0     2252 2023-03-16 15:58:21.513616 automationkit-0.5.1/source/packages/akit/interop/dns/dnsaddress.py
+-rw-r--r--   0        0        0      763 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/dnsapi.py
+-rw-r--r--   0        0        0    12410 2023-03-16 18:10:53.479049 automationkit-0.5.1/source/packages/akit/interop/dns/dnsconst.py
+-rw-r--r--   0        0        0     1030 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/dnserrors.py
+-rw-r--r--   0        0        0     2101 2023-03-16 15:58:21.513616 automationkit-0.5.1/source/packages/akit/interop/dns/dnshostinfo.py
+-rw-r--r--   0        0        0     9118 2023-03-16 16:22:49.474030 automationkit-0.5.1/source/packages/akit/interop/dns/dnsinboundmessage.py
+-rw-r--r--   0        0        0    15544 2023-03-16 17:00:25.492789 automationkit-0.5.1/source/packages/akit/interop/dns/dnsoutboundmessage.py
+-rw-r--r--   0        0        0     1842 2023-03-16 15:58:21.513616 automationkit-0.5.1/source/packages/akit/interop/dns/dnspointer.py
+-rw-r--r--   0        0        0     2266 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/dnsquestion.py
+-rw-r--r--   0        0        0      832 2023-03-16 05:21:20.896073 automationkit-0.5.1/source/packages/akit/interop/dns/dnsquestionresults.py
+-rw-r--r--   0        0        0     6896 2023-03-16 15:58:21.513616 automationkit-0.5.1/source/packages/akit/interop/dns/dnsrecord.py
+-rw-r--r--   0        0        0     3576 2023-03-16 15:58:35.037773 automationkit-0.5.1/source/packages/akit/interop/dns/dnsserver.py
+-rw-r--r--   0        0        0     2699 2023-03-16 15:58:21.513616 automationkit-0.5.1/source/packages/akit/interop/dns/dnsservice.py
+-rw-r--r--   0        0        0     1984 2023-03-16 15:58:21.513616 automationkit-0.5.1/source/packages/akit/interop/dns/dnstext.py
+-rw-r--r--   0        0        0     3713 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/dnsutil.py
+-rw-r--r--   0        0        0     2784 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/dnsvalidation.py
+-rw-r--r--   0        0        0     2756 2023-03-16 15:58:35.037773 automationkit-0.5.1/source/packages/akit/interop/dns/mdnscataloger.py
+-rw-r--r--   0        0        0     6263 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/mdnsservicecatalog.py
+-rw-r--r--   0        0        0     2505 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/dns/mdnsserviceinfo.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/eventsinking/__init__.py
+-rw-r--r--   0        0        0      787 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/eventsinking/enumerations.py
+-rw-r--r--   0        0        0    11897 2023-01-26 08:19:19.824084 automationkit-0.5.1/source/packages/akit/interop/eventsinking/eventedvariable.py
+-rw-r--r--   0        0        0     8080 2023-01-26 08:28:56.960950 automationkit-0.5.1/source/packages/akit/interop/eventsinking/eventedvariablesink.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 automationkit-0.5.1/source/packages/akit/interop/landscaping/__init__.py
+-rwxr-xr-x   0        0        0    12880 2023-02-10 06:02:39.444142 automationkit-0.5.1/source/packages/akit/interop/landscaping/landscape.py
+-rw-r--r--   0        0        0     9355 2023-01-21 17:29:41.202951 automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapedescription.py
+-rw-r--r--   0        0        0    12757 2023-02-01 07:11:21.531092 automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapedevice.py
+-rw-r--r--   0        0        0     3447 2023-02-13 00:34:51.752193 automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapedeviceextension.py
+-rw-r--r--   0        0        0     1239 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapelayerbase.py
+-rw-r--r--   0        0        0    23389 2023-01-23 06:05:11.875624 automationkit-0.5.1/source/packages/akit/interop/landscaping/layers/landscapeconfigurationlayer.py
+-rw-r--r--   0        0        0     2605 2023-01-23 03:34:51.638434 automationkit-0.5.1/source/packages/akit/interop/landscaping/layers/landscapeintegrationlayer.py
+-rw-r--r--   0        0        0    27545 2023-02-10 06:04:11.094479 automationkit-0.5.1/source/packages/akit/interop/landscaping/layers/landscapeoperationallayer.py
+-rw-r--r--   0        0        0     2901 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/landscaping/topologydescription.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/serial/__init__.py
+-rw-r--r--   0        0        0     6330 2023-02-20 16:45:57.121723 automationkit-0.5.1/source/packages/akit/interop/serial/serialtelnet.py
+-rw-r--r--   0        0        0    98806 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/soap/Sonoswsdl-1.19.4-20190411.142401-3.wsdl
+-rw-r--r--   0        0        0      540 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/__init__.py
+-rw-r--r--   0        0        0      319 2023-02-20 16:48:13.568100 automationkit-0.5.1/source/packages/akit/interop/upnp/aliases.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/content/__init__.py
+-rw-r--r--   0        0        0    15570 2023-02-20 16:46:16.842069 automationkit-0.5.1/source/packages/akit/interop/upnp/content/didllite.py
+-rw-r--r--   0        0        0      557 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/devices/__init__.py
+-rw-r--r--   0        0        0    14041 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/devices/upnpdevice.py
+-rw-r--r--   0        0        0     1764 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/devices/upnpembeddeddevice.py
+-rw-r--r--   0        0        0    44827 2023-02-14 00:06:24.094433 automationkit-0.5.1/source/packages/akit/interop/upnp/devices/upnprootdevice.py
+-rw-r--r--   0        0        0      494 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/__init__.py
+-rw-r--r--   0        0        0     9205 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/avtransport1serviceproxy.py
+-rw-r--r--   0        0        0     2651 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/connectionmanager1serviceproxy.py
+-rw-r--r--   0        0        0      508 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/dial1serviceproxy.py
+-rw-r--r--   0        0        0     4201 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/renderingcontrol1serviceproxy.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEAR/__init__.py
+-rw-r--r--   0        0        0     1838 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEAR/layer3forwarding1serviceproxy.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEARInc/__init__.py
+-rw-r--r--   0        0        0     8506 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEARInc/wfawlanconfig1serviceproxy.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/__init__.py
+-rw-r--r--   0        0        0    10842 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/alarmclock1serviceproxy.py
+-rw-r--r--   0        0        0     4601 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/audioin1serviceproxy.py
+-rw-r--r--   0        0        0    31349 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/avtransport1serviceproxy.py
+-rw-r--r--   0        0        0     2900 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/connectionmanager1serviceproxy.py
+-rw-r--r--   0        0        0    10802 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/contentdirectory1serviceproxy.py
+-rw-r--r--   0        0        0    18636 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/deviceproperties1serviceproxy.py
+-rw-r--r--   0        0        0     3112 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/groupmanagement1serviceproxy.py
+-rw-r--r--   0        0        0     3933 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/grouprenderingcontrol1serviceproxy.py
+-rw-r--r--   0        0        0     4518 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/htcontrol1serviceproxy.py
+-rw-r--r--   0        0        0     2647 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/musicservices1serviceproxy.py
+-rw-r--r--   0        0        0     1186 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/qplay1serviceproxy.py
+-rw-r--r--   0        0        0     9591 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/queue1serviceproxy.py
+-rw-r--r--   0        0        0    18702 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/renderingcontrol1serviceproxy.py
+-rw-r--r--   0        0        0    10097 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/systemproperties1serviceproxy.py
+-rw-r--r--   0        0        0     4151 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/virtuallinein1serviceproxy.py
+-rw-r--r--   0        0        0     6122 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/zonegrouptopology1serviceproxy.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/__init__.py
+-rw-r--r--   0        0        0     4394 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosdevice.py
+-rw-r--r--   0        0        0     8216 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosplayer.py
+-rw-r--r--   0        0        0      880 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps1.py
+-rw-r--r--   0        0        0      886 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps11.py
+-rw-r--r--   0        0        0      884 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps12.py
+-rw-r--r--   0        0        0      882 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps13.py
+-rw-r--r--   0        0        0      885 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps14.py
+-rw-r--r--   0        0        0      888 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps15.py
+-rw-r--r--   0        0        0      888 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps16.py
+-rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps17.py
+-rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps18.py
+-rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps19.py
+-rw-r--r--   0        0        0      885 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps22.py
+-rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps23.py
+-rw-r--r--   0        0        0      883 2022-12-08 19:53:16.280698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps24.py
+-rw-r--r--   0        0        0      880 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps3.py
+-rw-r--r--   0        0        0      886 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps34.py
+-rw-r--r--   0        0        0      885 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps38.py
+-rw-r--r--   0        0        0      883 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps5.py
+-rw-r--r--   0        0        0      880 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps6.py
+-rw-r--r--   0        0        0      881 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps9.py
+-rw-r--r--   0        0        0      884 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpssub.py
+-rw-r--r--   0        0        0      898 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp120.py
+-rw-r--r--   0        0        0      895 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp80.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/__init__.py
+-rw-r--r--   0        0        0     3502 2023-02-15 16:19:23.285785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
+-rw-r--r--   0        0        0     6212 2023-02-15 16:19:23.293785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    11191 2023-02-15 16:19:23.333786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0    11586 2023-02-15 16:19:23.345786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
+-rw-r--r--   0        0        0    14923 2023-02-15 16:19:23.293785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
+-rw-r--r--   0        0        0    20191 2023-02-15 16:19:23.321786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
+-rw-r--r--   0        0        0    13573 2023-02-15 16:19:23.369787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    16766 2023-02-15 16:19:23.297785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     6110 2023-02-15 16:19:23.373787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
+-rw-r--r--   0        0        0    12558 2023-02-15 16:19:23.357787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    17010 2023-02-15 16:19:23.341786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4564 2023-02-15 16:19:23.317785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
+-rw-r--r--   0        0        0      620 2023-02-15 16:19:23.293785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
+-rw-r--r--   0        0        0     4099 2023-02-15 16:19:23.317785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
+-rw-r--r--   0        0        0    11320 2023-02-15 16:19:23.269784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    12938 2023-02-15 16:19:23.313785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4151 2023-02-15 16:19:23.293785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
+-rw-r--r--   0        0        0     4151 2023-02-15 16:19:23.361786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
+-rw-r--r--   0        0        0     5709 2023-02-15 16:19:23.313785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
+-rw-r--r--   0        0        0     9443 2023-02-15 16:19:23.289785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
+-rw-r--r--   0        0        0    11439 2023-02-15 16:19:23.297785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
+-rw-r--r--   0        0        0    13524 2023-02-15 16:19:23.289785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
+-rw-r--r--   0        0        0    23734 2023-02-15 16:19:23.273784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
+-rw-r--r--   0        0        0     4419 2023-02-15 16:19:23.365787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
+-rw-r--r--   0        0        0     7452 2023-02-15 16:19:23.325786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
+-rw-r--r--   0        0        0    10860 2023-02-15 16:19:23.325786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
+-rw-r--r--   0        0        0     7721 2023-02-15 16:19:23.305785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
+-rw-r--r--   0        0        0     8818 2023-02-15 16:19:23.313785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
+-rw-r--r--   0        0        0     9996 2023-02-15 16:19:23.377787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
+-rw-r--r--   0        0        0     2033 2023-02-15 16:19:23.365787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
+-rw-r--r--   0        0        0     3982 2023-02-15 16:19:23.377787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
+-rw-r--r--   0        0        0     4949 2023-02-15 16:19:23.365787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
+-rw-r--r--   0        0        0     3818 2023-02-15 16:19:23.377787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
+-rw-r--r--   0        0        0     3156 2023-02-15 16:19:23.353786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     2029 2023-02-15 16:19:23.381787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
+-rw-r--r--   0        0        0     3567 2023-02-15 16:19:23.353786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     3061 2023-02-15 16:19:23.305785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
+-rw-r--r--   0        0        0     4676 2023-02-15 16:19:23.281784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
+-rw-r--r--   0        0        0     9941 2023-02-15 16:19:23.377787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
+-rw-r--r--   0        0        0     1772 2023-02-15 16:19:23.305785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
+-rw-r--r--   0        0        0     8061 2023-02-15 16:19:23.269784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
+-rw-r--r--   0        0        0     3921 2023-02-15 16:19:23.321786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
+-rw-r--r--   0        0        0     3921 2023-02-15 16:19:23.309785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
+-rw-r--r--   0        0        0    10230 2023-02-15 16:19:23.349786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
+-rw-r--r--   0        0        0    10230 2023-02-15 16:19:23.277784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
+-rw-r--r--   0        0        0     4665 2023-02-15 16:19:23.345786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
+-rw-r--r--   0        0        0     5791 2023-02-15 16:19:23.309785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
+-rw-r--r--   0        0        0    11106 2023-02-15 16:19:23.377787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
+-rw-r--r--   0        0        0     1681 2023-02-15 16:19:23.301785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
+-rw-r--r--   0        0        0     3278 2023-02-15 16:19:23.265784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
+-rw-r--r--   0        0        0     2097 2023-02-15 16:19:23.277784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
+-rw-r--r--   0        0        0     2702 2023-02-15 16:19:23.325786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
+-rw-r--r--   0        0        0     4708 2023-02-15 16:19:23.373787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
+-rw-r--r--   0        0        0     5204 2023-02-15 16:19:23.377787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
+-rw-r--r--   0        0        0     5723 2023-02-15 16:19:23.361786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
+-rw-r--r--   0        0        0     1741 2023-02-15 16:19:23.281784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
+-rw-r--r--   0        0        0    20937 2023-02-15 16:19:23.301785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
+-rw-r--r--   0        0        0    22550 2023-02-15 16:19:23.265784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
+-rw-r--r--   0        0        0    26942 2023-02-15 16:19:23.265784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
+-rw-r--r--   0        0        0     7326 2023-02-15 16:19:23.369787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
+-rw-r--r--   0        0        0    11148 2023-02-15 16:19:23.301785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
+-rw-r--r--   0        0        0    11148 2023-02-15 16:19:23.353786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
+-rw-r--r--   0        0        0     9794 2023-02-15 16:19:23.309785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
+-rw-r--r--   0        0        0    10315 2023-02-15 16:19:23.309785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
+-rw-r--r--   0        0        0     2189 2023-02-15 16:19:23.365787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
+-rw-r--r--   0        0        0     3247 2023-02-15 16:19:23.297785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
+-rw-r--r--   0        0        0     4224 2023-02-15 16:19:23.305785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
+-rw-r--r--   0        0        0     7776 2023-02-15 16:19:23.305785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     8122 2023-02-15 16:19:23.341786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
+-rw-r--r--   0        0        0     6168 2023-02-15 16:19:23.305785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     1341 2023-02-15 16:19:23.345786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    12404 2023-02-15 16:19:23.329786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
+-rw-r--r--   0        0        0    15204 2023-02-15 16:19:23.365787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
+-rw-r--r--   0        0        0     5123 2023-02-15 16:19:23.325786 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
+-rw-r--r--   0        0        0     6590 2023-02-15 16:19:23.265784 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    17121 2023-02-15 16:19:23.381787 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
+-rw-r--r--   0        0        0    30981 2023-02-15 16:19:23.285785 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/__init__.py
+-rw-r--r--   0        0        0      479 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/__init__.py
+-rw-r--r--   0        0        0      451 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/NETGEAR/urn:schemas-upnp-org:device:LANDevice:1.xml
+-rw-r--r--   0        0        0      446 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/NETGEAR/urn:schemas-upnp-org:device:WANDevice:1.xml
+-rw-r--r--   0        0        0     2150 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaRenderer:1.xml
+-rw-r--r--   0        0        0      834 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaServer:1.xml
+-rw-r--r--   0        0        0     1282 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/MicrosoftCorporation/XboxOne.xml
+-rw-r--r--   0        0        0     6551 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEAR/NETGEARR7400Router.xml
+-rw-r--r--   0        0        0     1178 2022-12-08 19:53:16.284698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEARInc/NETGEARR7400.xml
+-rw-r--r--   0        0        0     9941 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosAmp.xml
+-rw-r--r--   0        0        0     9652 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosArc.xml
+-rw-r--r--   0        0        0     9666 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBRAVO.xml
+-rw-r--r--   0        0        0     9622 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBeam.xml
+-rw-r--r--   0        0        0     9768 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosConnectAmp.xml
+-rw-r--r--   0        0        0     9654 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosFury.xml
+-rw-r--r--   0        0        0     9307 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosMove.xml
+-rw-r--r--   0        0        0     9281 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosOne.xml
+-rw-r--r--   0        0        0     9302 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay3.xml
+-rw-r--r--   0        0        0     9668 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay5.xml
+-rw-r--r--   0        0        0     9647 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybar.xml
+-rw-r--r--   0        0        0     9668 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybase.xml
+-rw-r--r--   0        0        0     9665 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPort.xml
+-rw-r--r--   0        0        0     9298 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoam.xml
+-rw-r--r--   0        0        0     9344 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoamSL.xml
+-rw-r--r--   0        0        0     9192 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosSub.xml
+-rw-r--r--   0        0        0     9603 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosZP80.xml
+-rw-r--r--   0        0        0      358 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:dial-multiscreen-org:service:dial:1.xml
+-rw-r--r--   0        0        0    15561 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:AVTransport:1.xml
+-rw-r--r--   0        0        0     4280 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:ConnectionManager:1.xml
+-rw-r--r--   0        0        0     4888 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:RenderingControl:1.xml
+-rw-r--r--   0        0        0      826 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEAR/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
+-rw-r--r--   0        0        0     4785 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEARInc/urn:schemas-wifialliance-org:service:WFAWLANConfig:1.xml
+-rw-r--r--   0        0        0     1697 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-tencent-com:service:QPlay:1.xml
+-rw-r--r--   0        0        0    14873 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AlarmClock:1.xml
+-rw-r--r--   0        0        0     4385 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AudioIn:1.xml
+-rw-r--r--   0        0        0    19452 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:DeviceProperties:1.xml
+-rw-r--r--   0        0        0     4053 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:GroupManagement:1.xml
+-rw-r--r--   0        0        0     4098 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:HTControl:1.xml
+-rw-r--r--   0        0        0     2479 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:MusicServices:1.xml
+-rw-r--r--   0        0        0    14284 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:SystemProperties:1.xml
+-rw-r--r--   0        0        0     8663 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:ZoneGroupTopology:1.xml
+-rw-r--r--   0        0        0      247 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
+-rw-r--r--   0        0        0      280 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
+-rw-r--r--   0        0        0      420 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
+-rw-r--r--   0        0        0     1159 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
+-rw-r--r--   0        0        0     1865 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
+-rw-r--r--   0        0        0      459 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
+-rw-r--r--   0        0        0      604 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
+-rw-r--r--   0        0        0      208 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
+-rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
+-rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
+-rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
+-rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
+-rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
+-rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
+-rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
+-rw-r--r--   0        0        0      187 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
+-rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
+-rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
+-rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
+-rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
+-rw-r--r--   0        0        0      300 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
+-rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
+-rw-r--r--   0        0        0      561 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
+-rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
+-rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
+-rw-r--r--   0        0        0      419 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
+-rw-r--r--   0        0        0      622 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
+-rw-r--r--   0        0        0      416 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
+-rw-r--r--   0        0        0      936 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
+-rw-r--r--   0        0        0     1090 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
+-rw-r--r--   0        0        0     1244 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
+-rw-r--r--   0        0        0      338 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
+-rw-r--r--   0        0        0      340 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
+-rw-r--r--   0        0        0      490 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
+-rw-r--r--   0        0        0    21478 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
+-rw-r--r--   0        0        0    22506 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
+-rw-r--r--   0        0        0    32819 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
+-rw-r--r--   0        0        0     3894 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
+-rw-r--r--   0        0        0     5779 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
+-rw-r--r--   0        0        0    10054 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
+-rw-r--r--   0        0        0    22061 2022-12-08 19:53:16.288698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
+-rw-r--r--   0        0        0    27823 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
+-rw-r--r--   0        0        0     5740 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
+-rw-r--r--   0        0        0    15507 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
+-rw-r--r--   0        0        0    22397 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
+-rw-r--r--   0        0        0     4082 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
+-rw-r--r--   0        0        0     2151 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
+-rw-r--r--   0        0        0     5359 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
+-rw-r--r--   0        0        0    11356 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
+-rw-r--r--   0        0        0    12959 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
+-rw-r--r--   0        0        0     7870 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
+-rw-r--r--   0        0        0     6485 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
+-rw-r--r--   0        0        0     8455 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
+-rw-r--r--   0        0        0    14206 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
+-rw-r--r--   0        0        0    15034 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
+-rw-r--r--   0        0        0    17600 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
+-rw-r--r--   0        0        0    27620 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
+-rw-r--r--   0        0        0     4821 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
+-rw-r--r--   0        0        0     7808 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
+-rw-r--r--   0        0        0     8486 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
+-rw-r--r--   0        0        0     4783 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
+-rw-r--r--   0        0        0     6607 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
+-rw-r--r--   0        0        0     8457 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
+-rw-r--r--   0        0        0     2249 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
+-rw-r--r--   0        0        0     3447 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
+-rw-r--r--   0        0        0     5176 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
+-rw-r--r--   0        0        0     2637 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
+-rw-r--r--   0        0        0     4564 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
+-rw-r--r--   0        0        0     3751 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
+-rw-r--r--   0        0        0     3673 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
+-rw-r--r--   0        0        0     2461 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
+-rw-r--r--   0        0        0     4528 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
+-rw-r--r--   0        0        0     7628 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
+-rw-r--r--   0        0        0     1045 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
+-rw-r--r--   0        0        0    15694 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
+-rw-r--r--   0        0        0     3331 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
+-rw-r--r--   0        0        0     3234 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
+-rw-r--r--   0        0        0    12147 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
+-rw-r--r--   0        0        0    12076 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
+-rw-r--r--   0        0        0     4682 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
+-rw-r--r--   0        0        0    13539 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
+-rw-r--r--   0        0        0    25446 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
+-rw-r--r--   0        0        0     1919 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
+-rw-r--r--   0        0        0     3445 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
+-rw-r--r--   0        0        0     2800 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
+-rw-r--r--   0        0        0     3264 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
+-rw-r--r--   0        0        0     4324 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
+-rw-r--r--   0        0        0     4744 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
+-rw-r--r--   0        0        0     6642 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
+-rw-r--r--   0        0        0     2399 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
+-rw-r--r--   0        0        0    24162 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
+-rw-r--r--   0        0        0    25624 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
+-rw-r--r--   0        0        0    29018 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
+-rw-r--r--   0        0        0    13767 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
+-rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
+-rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
+-rw-r--r--   0        0        0    13686 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
+-rw-r--r--   0        0        0    14103 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
+-rw-r--r--   0        0        0     1285 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
+-rw-r--r--   0        0        0     2951 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
+-rw-r--r--   0        0        0     3412 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
+-rw-r--r--   0        0        0     7592 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
+-rw-r--r--   0        0        0     8319 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
+-rw-r--r--   0        0        0     4926 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
+-rw-r--r--   0        0        0      754 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
+-rw-r--r--   0        0        0    14359 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
+-rw-r--r--   0        0        0    19829 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
+-rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
+-rw-r--r--   0        0        0     6730 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
+-rw-r--r--   0        0        0    18555 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
+-rw-r--r--   0        0        0    39224 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
+-rw-r--r--   0        0        0    16824 2023-02-15 16:19:08.569407 automationkit-0.5.1/source/packages/akit/interop/upnp/generator/upnpgenerator.py
+-rw-r--r--   0        0        0     2631 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/paths.py
+-rw-r--r--   0        0        0      481 2022-12-08 19:53:16.292698 automationkit-0.5.1/source/packages/akit/interop/upnp/services/__init__.py
+-rw-r--r--   0        0        0     5524 2023-02-20 16:48:01.083885 automationkit-0.5.1/source/packages/akit/interop/upnp/services/upnpdefaultvar.py
+-rw-r--r--   0        0        0    26104 2023-01-26 08:29:15.573108 automationkit-0.5.1/source/packages/akit/interop/upnp/services/upnpserviceproxy.py
+-rw-r--r--   0        0        0    11706 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/interop/upnp/soap.py
+-rw-r--r--   0        0        0      736 2023-02-20 16:48:22.600256 automationkit-0.5.1/source/packages/akit/interop/upnp/upnpconstants.py
+-rw-r--r--   0        0        0     2543 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/interop/upnp/upnperrors.py
+-rw-r--r--   0        0        0    11117 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/interop/upnp/upnpfactory.py
+-rw-r--r--   0        0        0    21734 2023-01-21 17:36:57.523900 automationkit-0.5.1/source/packages/akit/interop/upnp/upnpprotocol.py
+-rw-r--r--   0        0        0      494 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/interop/upnp/xml/__init__.py
+-rw-r--r--   0        0        0    20799 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/interop/upnp/xml/upnpdevice1.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/interop/wireless/__init__.py
+-rw-r--r--   0        0        0     4141 2023-03-06 05:11:44.961781 automationkit-0.5.1/source/packages/akit/interop/wireless/channels.py
+-rw-r--r--   0        0        0     2534 2023-02-20 16:49:37.737543 automationkit-0.5.1/source/packages/akit/interop/wireless/constants.py
+-rw-r--r--   0        0        0      405 2023-02-20 16:48:52.304766 automationkit-0.5.1/source/packages/akit/interop/wireless/fastpingresult.py
+-rw-r--r--   0        0        0      872 2023-02-20 16:48:59.744894 automationkit-0.5.1/source/packages/akit/interop/wireless/stationinfo.py
+-rw-r--r--   0        0        0      810 2023-02-20 16:49:09.685064 automationkit-0.5.1/source/packages/akit/interop/wireless/wep.py
+-rw-r--r--   0        0        0      869 2023-02-20 16:49:24.553318 automationkit-0.5.1/source/packages/akit/interop/wireless/wpa.py
+-rw-r--r--   0        0        0      527 2023-03-17 22:19:43.706883 automationkit-0.5.1/source/packages/akit/jsos.py
+-rw-r--r--   0        0        0     2792 2023-02-17 02:06:35.231504 automationkit-0.5.1/source/packages/akit/metadata.py
+-rw-r--r--   0        0        0     3514 2023-02-20 16:52:04.212020 automationkit-0.5.1/source/packages/akit/monitoring/processmonitor.py
+-rw-r--r--   0        0        0     5643 2023-02-20 16:52:10.288121 automationkit-0.5.1/source/packages/akit/monitoring/reportingservice.py
+-rw-r--r--   0        0        0     2672 2023-02-20 16:52:14.620194 automationkit-0.5.1/source/packages/akit/monitoring/reportmonitor.py
+-rw-r--r--   0        0        0      474 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/monitoring/scripts/platforms/linux/monitor_pid
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/monitoring/templates/processmonitor.html
+-rw-r--r--   0        0        0      500 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/networking/__init__.py
+-rw-r--r--   0        0        0      417 2023-02-20 16:52:24.424358 automationkit-0.5.1/source/packages/akit/networking/broadcast.py
+-rw-r--r--   0        0        0     7135 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/networking/constants.py
+-rw-r--r--   0        0        0     3460 2023-02-20 16:52:31.568478 automationkit-0.5.1/source/packages/akit/networking/httpserverthreadpool.py
+-rw-r--r--   0        0        0     9204 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/networking/interfaces.py
+-rw-r--r--   0        0        0     8678 2023-02-20 16:52:39.284607 automationkit-0.5.1/source/packages/akit/networking/multicast.py
+-rw-r--r--   0        0        0     2179 2023-02-20 16:52:43.824683 automationkit-0.5.1/source/packages/akit/networking/resolution.py
+-rw-r--r--   0        0        0     6566 2023-02-20 16:52:49.108771 automationkit-0.5.1/source/packages/akit/networking/simplewebserver.py
+-rw-r--r--   0        0        0     1520 2023-02-20 16:52:53.660847 automationkit-0.5.1/source/packages/akit/networking/trafficcapturecontext.py
+-rw-r--r--   0        0        0     4392 2023-02-20 16:52:59.308942 automationkit-0.5.1/source/packages/akit/networking/unicast.py
+-rwxr-xr-x   0        0        0    10160 2023-04-19 05:26:52.118301 automationkit-0.5.1/source/packages/akit/paths.py
+-rw-r--r--   0        0        0     2852 2023-02-20 16:56:34.988514 automationkit-0.5.1/source/packages/akit/raisefor.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/readers/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/readers/linux/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/readers/linux/command/__init__.py
+-rw-r--r--   0        0        0     1481 2023-02-20 16:53:10.085121 automationkit-0.5.1/source/packages/akit/readers/linux/command/ps.py
+-rwxr-xr-x   0        0        0    13324 2023-02-17 23:10:00.323743 automationkit-0.5.1/source/packages/akit/recorders.py
+-rwxr-xr-x   0        0        0    10708 2023-02-03 15:53:07.738902 automationkit-0.5.1/source/packages/akit/results.py
+-rwxr-xr-x   0        0        0      960 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/taskbase.py
+-rwxr-xr-x   0        0        0      959 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/templates/__init__.py
+-rw-r--r--   0        0        0    10399 2023-04-19 05:29:08.667263 automationkit-0.5.1/source/packages/akit/templates/static/v0/testsummary.css
+-rw-r--r--   0        0        0    38006 2023-03-02 06:15:41.846020 automationkit-0.5.1/source/packages/akit/templates/static/v0/testsummary.js
+-rw-r--r--   0        0        0    23424 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/templates/static/v0/w3.css
+-rw-r--r--   0        0        0     3190 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/templates/tabs/tab-images.html
+-rw-r--r--   0        0        0     3385 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/templates/tabs/tab-sounds.html
+-rwxr-xr-x   0        0        0     6715 2023-04-19 05:26:52.102301 automationkit-0.5.1/source/packages/akit/templates/testsummary.html
+-rwxr-xr-x   0        0        0      544 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/testing/__init__.py
+-rw-r--r--   0        0        0     1933 2023-02-20 16:53:40.485628 automationkit-0.5.1/source/packages/akit/testing/constraints.py
+-rw-r--r--   0        0        0     4370 2023-02-20 16:53:47.517745 automationkit-0.5.1/source/packages/akit/testing/expressions.py
+-rw-r--r--   0        0        0     1408 2023-02-20 16:53:52.149822 automationkit-0.5.1/source/packages/akit/testing/reflection.py
+-rw-r--r--   0        0        0     1220 2023-02-20 00:46:52.316497 automationkit-0.5.1/source/packages/akit/testing/testplus/__init__.py
+-rw-r--r--   0        0        0     4742 2023-01-26 04:04:47.642183 automationkit-0.5.1/source/packages/akit/testing/testplus/entrypoints.py
+-rw-r--r--   0        0        0     7450 2023-02-20 16:54:10.130121 automationkit-0.5.1/source/packages/akit/testing/testplus/markers.py
+-rw-r--r--   0        0        0     4028 2023-02-20 16:54:05.462043 automationkit-0.5.1/source/packages/akit/testing/testplus/parameters.py
+-rw-r--r--   0        0        0     3277 2023-02-20 16:54:15.750214 automationkit-0.5.1/source/packages/akit/testing/testplus/queries.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/__init__.py
+-rw-r--r--   0        0        0      408 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/integrationsource.py
+-rw-r--r--   0        0        0     2735 2022-12-08 19:53:16.296698 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/parameterorigin.py
+-rw-r--r--   0        0        0    10818 2023-01-26 03:57:11.180559 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/resourceregistry.py
+-rw-r--r--   0        0        0    15978 2023-02-16 16:37:37.667216 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/resourcescope.py
+-rw-r--r--   0        0        0      439 2023-02-05 23:36:28.700299 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/resourcesource.py
+-rw-r--r--   0        0        0      537 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/scopesource.py
+-rw-r--r--   0        0        0     1303 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/sourcebase.py
+-rw-r--r--   0        0        0      623 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/testing/testplus/registration/unknownsource.py
+-rw-r--r--   0        0        0      391 2023-02-20 16:54:20.910300 automationkit-0.5.1/source/packages/akit/testing/testplus/resourcelifespan.py
+-rw-r--r--   0        0        0     6973 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/testing/testplus/resources.py
+-rwxr-xr-x   0        0        0     8005 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/testing/testplus/scopecoupling.py
+-rwxr-xr-x   0        0        0     9298 2023-02-10 06:14:58.794934 automationkit-0.5.1/source/packages/akit/testing/testplus/testcollector.py
+-rw-r--r--   0        0        0     5115 2023-02-10 06:59:21.438953 automationkit-0.5.1/source/packages/akit/testing/testplus/testgroup.py
+-rwxr-xr-x   0        0        0    17620 2023-02-17 23:06:27.929145 automationkit-0.5.1/source/packages/akit/testing/testplus/testjob.py
+-rwxr-xr-x   0        0        0     4524 2023-02-09 22:27:08.127427 automationkit-0.5.1/source/packages/akit/testing/testplus/testref.py
+-rw-r--r--   0        0        0    38166 2023-02-17 02:09:10.143486 automationkit-0.5.1/source/packages/akit/testing/testplus/testsequencer.py
+-rw-r--r--   0        0        0    17481 2023-02-20 16:54:39.434607 automationkit-0.5.1/source/packages/akit/testing/testplus/verification.py
+-rwxr-xr-x   0        0        0     6035 2023-01-25 17:53:53.625118 automationkit-0.5.1/source/packages/akit/testing/utilities.py
+-rw-r--r--   0        0        0     6524 2023-02-20 16:56:43.860660 automationkit-0.5.1/source/packages/akit/timemachine.py
+-rwxr-xr-x   0        0        0     7103 2023-01-27 16:12:24.390033 automationkit-0.5.1/source/packages/akit/timeouts.py
+-rw-r--r--   0        0        0     8877 2023-03-11 05:15:15.284442 automationkit-0.5.1/source/packages/akit/waiting.py
+-rw-r--r--   0        0        0        0 2023-01-25 16:55:15.635053 automationkit-0.5.1/source/packages/akit/wellknown/__init__.py
+-rw-r--r--   0        0        0     1128 2023-02-20 16:54:54.654859 automationkit-0.5.1/source/packages/akit/wellknown/singletons.py
+-rw-r--r--   0        0        0      303 2023-03-10 01:29:50.415382 automationkit-0.5.1/source/packages/akit/wellknownports.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/workflow/__init__.py
+-rw-r--r--   0        0        0     2720 2023-01-15 13:31:47.440771 automationkit-0.5.1/source/packages/akit/workflow/entrypoints.py
+-rw-r--r--   0        0        0     4484 2023-01-15 13:38:10.967670 automationkit-0.5.1/source/packages/akit/workflow/execution.py
+-rw-r--r--   0        0        0        0 2023-01-15 05:47:46.525125 automationkit-0.5.1/source/packages/akit/workflow/tasks/__init__.py
+-rw-r--r--   0        0        0     3616 2023-01-15 16:19:11.246722 automationkit-0.5.1/source/packages/akit/workflow/tasks/createenvironment.py
+-rw-r--r--   0        0        0     1861 2023-01-15 06:38:46.840778 automationkit-0.5.1/source/packages/akit/workflow/tasks/embeddedpython.py
+-rw-r--r--   0        0        0     1059 2023-01-15 06:39:11.257060 automationkit-0.5.1/source/packages/akit/workflow/tasks/gitcheckout.py
+-rw-r--r--   0        0        0     1992 2023-01-15 06:39:04.556982 automationkit-0.5.1/source/packages/akit/workflow/tasks/runcommand.py
+-rw-r--r--   0        0        0     2183 2023-01-15 06:38:56.548890 automationkit-0.5.1/source/packages/akit/workflow/tasks/shellscript.py
+-rw-r--r--   0        0        0     1656 2023-01-15 06:37:20.407782 automationkit-0.5.1/source/packages/akit/workflow/tasks/taskbase.py
+-rw-r--r--   0        0        0    11913 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xcollections.py
+-rw-r--r--   0        0        0      556 2023-02-20 16:56:58.244896 automationkit-0.5.1/source/packages/akit/xconfiguration.py
+-rw-r--r--   0        0        0      467 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/xcryptography/__init__.py
+-rw-r--r--   0        0        0     1969 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/xcryptography/pkey.py
+-rw-r--r--   0        0        0     6482 2022-12-08 19:53:16.272698 automationkit-0.5.1/source/packages/akit/xcryptography/x509.py
+-rw-r--r--   0        0        0     4401 2023-02-20 16:57:03.144976 automationkit-0.5.1/source/packages/akit/xdebugger.py
+-rw-r--r--   0        0        0     1418 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xenum.py
+-rw-r--r--   0        0        0     6014 2023-02-20 16:57:10.837103 automationkit-0.5.1/source/packages/akit/xfeature.py
+-rw-r--r--   0        0        0     4655 2023-03-11 03:41:48.245645 automationkit-0.5.1/source/packages/akit/xformatting.py
+-rw-r--r--   0        0        0     1986 2023-03-16 21:57:31.426396 automationkit-0.5.1/source/packages/akit/xinspect.py
+-rw-r--r--   0        0        0      550 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xlogging/__init__.py
+-rw-r--r--   0        0        0    24838 2023-02-03 06:05:31.946933 automationkit-0.5.1/source/packages/akit/xlogging/foundations.py
+-rw-r--r--   0        0        0    10390 2023-03-22 16:53:04.861736 automationkit-0.5.1/source/packages/akit/xlogging/scopemonitoring.py
+-rw-r--r--   0        0        0     2256 2023-02-20 16:55:32.631486 automationkit-0.5.1/source/packages/akit/xml/parsing.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xmultiprocessing/__init__.py
+-rw-r--r--   0        0        0     3514 2023-02-20 16:55:38.471583 automationkit-0.5.1/source/packages/akit/xmultiprocessing/smbserverprocess.py
+-rw-r--r--   0        0        0     1027 2023-02-20 16:55:42.947656 automationkit-0.5.1/source/packages/akit/xmultiprocessing/webserverprocess.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xregex/__init__.py
+-rw-r--r--   0        0        0    13244 2023-02-20 16:55:49.999773 automationkit-0.5.1/source/packages/akit/xregex/regexreader.py
+-rw-r--r--   0        0        0      544 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xthreading/__init__.py
+-rw-r--r--   0        0        0     3278 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xthreading/looper.py
+-rw-r--r--   0        0        0     4911 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xthreading/looperpool.py
+-rw-r--r--   0        0        0     3555 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xthreading/looperqueue.py
+-rw-r--r--   0        0        0     5793 2022-12-08 19:53:16.300698 automationkit-0.5.1/source/packages/akit/xthreading/readwritelock.py
+-rwxr-xr-x   0        0        0     2153 2023-02-05 22:33:18.961356 automationkit-0.5.1/source/packages/akit/xtime.py
+-rw-r--r--   0        0        0      472 2023-02-20 16:57:20.933268 automationkit-0.5.1/source/packages/akit/xtraceback.py
+-rw-r--r--   0        0        0    12753 1970-01-01 00:00:00.000000 automationkit-0.5.1/setup.py
+-rw-r--r--   0        0        0    10220 1970-01-01 00:00:00.000000 automationkit-0.5.1/PKG-INFO
```

### Comparing `automationkit-0.5.0/LICENSE.txt` & `automationkit-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/README.md` & `automationkit-0.5.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -36,27 +36,27 @@
 ## Task and Test Integration Declaration and Assurance
 The **Automation Kit** utilizes its object model to allow tasks and tests to provide information about their associated integration points and scopes of execution to the automation framework.  This integration declaration mechanism allows the automation framework to provide an early scan of the integration pathways and provide levels of assurance as to the stability of the automation landscape early in the automation process.  This is vitally important as it eliminates the waist and noise that are often associated with automation runs that are performed against an automation Landscape that has broken, mis-configured or missing resources.
 
 ## Automation Job, Scope and Flow Control 
 The **Automation Kit** allows enterprise users to organize and customize the ordering of automation scope engagements and the flow of an automation job.  This provides the automation engineer the ability to control the engagement of automation scopes of execution and allows for optimal use of time and overlapping of scopes of execution in a test run.
 
 # Table of Contents
-1. [Automation Software Stack](http://automationmojo.com/automationkit/docs/usermanual/10-automation-software-stack.html)
-2. [Getting Started](http://automationmojo.com/automationkit/docs/usermanual/20-getting-started.html)
-3. [Automation Configuration](http://automationmojo.com/automationkit/docs/usermanual/30-automation-configuration.html)
-    1. [Landscape File](http://automationmojo.com/automationkit/docs/usermanual/31-landscape-file.html)
-    2. [Topology File](http://automationmojo.com/automationkit/docs/usermanual/32-topology-file.html)
-    2. [Runtime File](http://automationmojo.com/automationkit/docs/usermanual/33-runtime-file.html)
-    3. [Credentials File](http://automationmojo.com/automationkit/docs/usermanual/34-credentials-file.html)
-4. [TestRun Sequencing](http://automationmojo.com/automationkit/docs/usermanual/40-testrun-sequencing.html)
-    1. [Integration Couplings](http://automationmojo.com/automationkit/docs/usermanual/41-integration-couplings.html)
-    2. [Scope Couplings](http://automationmojo.com/automationkit/docs/usermanual/42-scope-couplings.html)
-5. [Functional Description](http://automationmojo.com/automationkit/docs/usermanual/50-functional-description.html)
-    1. [Activation and Startup](http://automationmojo.com/automationkit/docs/usermanual/51-activation-and-startup.html)
-    2. [Inter-Operability](http://automationmojo.com/automationkit/docs/usermanual/52-inter-operability.html)
-    3. [SSH Coordinator and Agent](http://automationmojo.com/automationkit/docs/usermanual/53-ssh-coordinator-and-agent.html)
-    4. [UPNP Coordinator and Agent](http://automationmojo.com/automationkit/docs/usermanual/54-upnp-coordinator-and-agent.html)
-6. [Workflow Orchestration](http://automationmojo.com/automationkit/docs/usermanual/60-workflow-orchestration.html)
-7. [Enterprise Extensibility](http://automationmojo.com/automationkit/docs/usermanual/70-enterprise-extensibility.html)
-8. [Command Line](http://automationmojo.com/automationkit/docs/usermanual/80-command-line.html)
-9. [Code Organization and Conventions](http://automationmojo.com/automationkit/docs/usermanual/90-code-organization-and-conventions.html)
-10. [Coding Standards](http://automationmojo.com/automationkit/docs/usermanual/100-coding-standards.html)
+1. [Automation Software Stack](http://automationmojo.com/static/automationkit/docs/usermanual/10-automation-software-stack.html)
+2. [Getting Started](http://automationmojo.com/static/automationkit/docs/usermanual/20-getting-started.html)
+3. [Automation Configuration](http://automationmojo.com/static/automationkit/docs/usermanual/30-automation-configuration.html)
+    1. [Landscape File](http://automationmojo.com/static/automationkit/docs/usermanual/31-landscape-file.html)
+    2. [Topology File](http://automationmojo.com/static/automationkit/docs/usermanual/32-topology-file.html)
+    2. [Runtime File](http://automationmojo.com/static/automationkit/docs/usermanual/33-runtime-file.html)
+    3. [Credentials File](http://automationmojo.com/static/automationkit/docs/usermanual/34-credentials-file.html)
+4. [TestRun Sequencing](http://automationmojo.com/static/automationkit/docs/usermanual/40-testrun-sequencing.html)
+    1. [Integration Couplings](http://automationmojo.com/static/automationkit/docs/usermanual/41-integration-couplings.html)
+    2. [Scope Couplings](http://automationmojo.com/static/automationkit/docs/usermanual/42-scope-couplings.html)
+5. [Functional Description](http://automationmojo.com/static/automationkit/docs/usermanual/50-functional-description.html)
+    1. [Activation and Startup](http://automationmojo.com/static/automationkit/docs/usermanual/51-activation-and-startup.html)
+    2. [Inter-Operability](http://automationmojo.com/static/automationkit/docs/usermanual/52-inter-operability.html)
+    3. [SSH Coordinator and Agent](http://automationmojo.com/static/automationkit/docs/usermanual/53-ssh-coordinator-and-agent.html)
+    4. [UPNP Coordinator and Agent](http://automationmojo.com/static/automationkit/docs/usermanual/54-upnp-coordinator-and-agent.html)
+6. [Workflow Orchestration](http://automationmojo.com/static/automationkit/docs/usermanual/60-workflow-orchestration.html)
+7. [Enterprise Extensibility](http://automationmojo.com/static/automationkit/docs/usermanual/70-enterprise-extensibility.html)
+8. [Command Line](http://automationmojo.com/static/automationkit/docs/usermanual/80-command-line.html)
+9. [Code Organization and Conventions](http://automationmojo.com/static/automationkit/docs/usermanual/90-code-organization-and-conventions.html)
+10. [Coding Standards](http://automationmojo.com/static/automationkit/docs/usermanual/100-coding-standards.html)
```

### Comparing `automationkit-0.5.0/pyproject.toml` & `automationkit-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "automationkit"
 description = "Automation Kit Test Framework"
-version = "0.5.00"
+version = "0.5.1"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `automationkit-0.5.0/source/packages/akit/activation/base.py` & `automationkit-0.5.1/source/packages/akit/activation/base.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/activation/console.py` & `automationkit-0.5.1/source/packages/akit/activation/console.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/activation/service.py` & `automationkit-0.5.1/source/packages/akit/activation/service.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/activation/testrun.py` & `automationkit-0.5.1/source/packages/akit/activation/testrun.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/aspects.py` & `automationkit-0.5.1/source/packages/akit/aspects.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/akitcommand.py` & `automationkit-0.5.1/source/packages/akit/cli/akitcommand.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/databases/__init__.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/databases/automation.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/databases/automation.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/generators/__init__.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/generators/upnp.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/generators/upnp.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/landscape.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/landscape.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/network/__init__.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/network/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/network/mdns.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/network/mdns.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/network/upnp.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/network/upnp.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/servers/__init__.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/servers/results_server.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/servers/results_server.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/__init__.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/constants.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/constants.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/jobs.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/jobs.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/query.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/query.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/testing/run.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/testing/run.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/utilities.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/utilities.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/cli/cmdtree/workflow.py` & `automationkit-0.5.1/source/packages/akit/cli/cmdtree/workflow.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/comparisons.py` & `automationkit-0.5.1/source/packages/akit/comparisons.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/compat.py` & `automationkit-0.5.1/source/packages/akit/compat.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/conversions.py` & `automationkit-0.5.1/source/packages/akit/conversions.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/basecoupling.py` & `automationkit-0.5.1/source/packages/akit/coupling/basecoupling.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/coordinatorcoupling.py` & `automationkit-0.5.1/source/packages/akit/coupling/coordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/coordinators/sshpoolcoordinatorintegration.py` & `automationkit-0.5.1/source/packages/akit/coupling/coordinators/sshpoolcoordinatorintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/coordinators/upnpcoordinatorintegration.py` & `automationkit-0.5.1/source/packages/akit/coupling/coordinators/upnpcoordinatorintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/coordinators/wirelesscoordinatorintegration.py` & `automationkit-0.5.1/source/packages/akit/coupling/coordinators/wirelesscoordinatorintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/integrationcoupling.py` & `automationkit-0.5.1/source/packages/akit/coupling/integrationcoupling.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/sshpoolcoordinatorintegration.py` & `automationkit-0.5.1/source/packages/akit/coupling/sshpoolcoordinatorintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/upnpcoordinatorintegration.py` & `automationkit-0.5.1/source/packages/akit/coupling/upnpcoordinatorintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/coupling/wirelesscoordinatorintegration.py` & `automationkit-0.5.1/source/packages/akit/coupling/wirelesscoordinatorintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/datum/dbconnection.py` & `automationkit-0.5.1/source/packages/akit/datum/dbconnection.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/datum/dbio.py` & `automationkit-0.5.1/source/packages/akit/datum/dbio.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/datum/orm.py` & `automationkit-0.5.1/source/packages/akit/datum/orm.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/environment/__init__.py` & `automationkit-0.5.1/source/packages/akit/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/environment/configuration.py` & `automationkit-0.5.1/source/packages/akit/environment/configuration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/environment/context.py` & `automationkit-0.5.1/source/packages/akit/environment/context.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/environment/contextpaths.py` & `automationkit-0.5.1/source/packages/akit/environment/contextpaths.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/environment/optionoverrides.py` & `automationkit-0.5.1/source/packages/akit/environment/optionoverrides.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/environment/variables.py` & `automationkit-0.5.1/source/packages/akit/environment/variables.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/exceptions.py` & `automationkit-0.5.1/source/packages/akit/exceptions.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/extensible.py` & `automationkit-0.5.1/source/packages/akit/extensible.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/extensionpoints.py` & `automationkit-0.5.1/source/packages/akit/extensionpoints.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/friendlyidentifier.py` & `automationkit-0.5.1/source/packages/akit/friendlyidentifier.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interfaces/icommandrunner.py` & `automationkit-0.5.1/source/packages/akit/interfaces/icommandrunner.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interfaces/iexcludefilter.py` & `automationkit-0.5.1/source/packages/akit/interfaces/iexcludefilter.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interfaces/iincludefilter.py` & `automationkit-0.5.1/source/packages/akit/interfaces/iincludefilter.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/agents/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/agents/dnsagent.py` & `automationkit-0.5.1/source/packages/akit/interop/agents/dnsagent.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/agents/poweragents.py` & `automationkit-0.5.1/source/packages/akit/interop/agents/poweragents.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/agents/serialagents.py` & `automationkit-0.5.1/source/packages/akit/interop/agents/serialagents.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 import telnetlib
 
 from akit.aspects import AspectsCmd
 from akit.compat import bytes_cast, str_cast
 
 from akit.interfaces.icommandrunner import ICommandRunner
 
-from akit.aspects import ActionPattern, AspectsCmd, LoggingPattern, DEFAULT_CMD_ASPECTS
+from akit.aspects import AspectsCmd, DEFAULT_CMD_ASPECTS
 
 class TcpSerialBase(ICommandRunner):
 
+    SERIAL_PROMPT=b"@@@&@@@&"
+    NORMAL_PROMPT=b"#"
+
     def __init__(self, host: str, port: int=22, aspects: AspectsCmd=DEFAULT_CMD_ASPECTS):
         self._host = host
         self._port = port
         self._aspects = aspects
         return
     
     def _create_connection(self) -> telnetlib.Telnet:
@@ -137,17 +140,14 @@
             BANNER:banner:\r\nser2net port \p device \d [\s] (Debian GNU/Linux)\r\n\r\n
 
             3333:telnet:0:/dev/ttyUSB0:115200 8DATABITS NONE 1STOPBIT banner
 
             
     """
 
-    SERIAL_PROMPT=b"@@@&@@@&"
-    NORMAL_PROMPT=b"#"
-
     def __init__(self, host, port:int=22, aspects: AspectsCmd=DEFAULT_CMD_ASPECTS):
         super().__init__(host, port=port, aspects=aspects)
         return
 
     def open_session(self, session_basis: Optional["ICommandRunner"] = None,
                      aspects: Optional[AspectsCmd] = None) -> "ICommandRunner": # pylint: disable=arguments-differ
         """
```

### Comparing `automationkit-0.5.0/source/packages/akit/interop/agents/sshagent.py` & `automationkit-0.5.1/source/packages/akit/interop/agents/sshagent.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/agents/wirelessapagent.py` & `automationkit-0.5.1/source/packages/akit/interop/agents/wirelessapagent.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/clients/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/clients/linuxclientintegration.py` & `automationkit-0.5.1/source/packages/akit/interop/clients/linuxclientintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/clients/windowsclientintegration.py` & `automationkit-0.5.1/source/packages/akit/interop/clients/windowsclientintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/cluster/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/cluster/clusterintegration.py` & `automationkit-0.5.1/source/packages/akit/interop/cluster/clusterintegration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/concurrency/evolution.py` & `automationkit-0.5.1/source/packages/akit/interop/concurrency/evolution.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/concurrency/procedurecontext.py` & `automationkit-0.5.1/source/packages/akit/interop/concurrency/procedurecontext.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/coordinators/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/coordinators/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/coordinators/coordinatorbase.py` & `automationkit-0.5.1/source/packages/akit/interop/coordinators/coordinatorbase.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/coordinators/powercoordinator.py` & `automationkit-0.5.1/source/packages/akit/interop/coordinators/powercoordinator.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/coordinators/serialcoordinator.py` & `automationkit-0.5.1/source/packages/akit/interop/coordinators/serialcoordinator.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/coordinators/sshpoolcoordinator.py` & `automationkit-0.5.1/source/packages/akit/interop/coordinators/sshpoolcoordinator.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/coordinators/upnpcoordinator.py` & `automationkit-0.5.1/source/packages/akit/interop/coordinators/upnpcoordinator.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/coordinators/wirelessapcoordinator.py` & `automationkit-0.5.1/source/packages/akit/interop/coordinators/wirelessapcoordinator.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/credentials/basecredential.py` & `automationkit-0.5.1/source/packages/akit/interop/credentials/basecredential.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/credentials/basiccredential.py` & `automationkit-0.5.1/source/packages/akit/interop/credentials/basiccredential.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/credentials/credentialmanager.py` & `automationkit-0.5.1/source/packages/akit/interop/credentials/credentialmanager.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/credentials/sshcredential.py` & `automationkit-0.5.1/source/packages/akit/interop/credentials/sshcredential.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/credentials/wifichoicecredential.py` & `automationkit-0.5.1/source/packages/akit/interop/credentials/wifichoicecredential.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsaddress.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsaddress.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsapi.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsapi.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsconst.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsconst.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnserrors.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnserrors.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnshostinfo.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnshostinfo.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsinboundmessage.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsinboundmessage.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsoutboundmessage.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsoutboundmessage.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnspointer.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnspointer.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsquestion.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsquestion.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsquestionresults.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsquestionresults.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsrecord.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsrecord.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsserver.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsserver.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsservice.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsservice.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnstext.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnstext.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsutil.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsutil.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/dnsvalidation.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/dnsvalidation.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/mdnscataloger.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/mdnscataloger.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/mdnsservicecatalog.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/mdnsservicecatalog.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/dns/mdnsserviceinfo.py` & `automationkit-0.5.1/source/packages/akit/interop/dns/mdnsserviceinfo.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/eventsinking/enumerations.py` & `automationkit-0.5.1/source/packages/akit/interop/eventsinking/enumerations.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/eventsinking/eventedvariable.py` & `automationkit-0.5.1/source/packages/akit/interop/eventsinking/eventedvariable.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/eventsinking/eventedvariablesink.py` & `automationkit-0.5.1/source/packages/akit/interop/eventsinking/eventedvariablesink.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/landscape.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/landscape.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapedescription.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapedescription.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapedevice.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapedevice.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapedeviceextension.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapedeviceextension.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/landscapelayerbase.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/landscapelayerbase.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/layers/landscapeconfigurationlayer.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/layers/landscapeconfigurationlayer.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/layers/landscapeintegrationlayer.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/layers/landscapeintegrationlayer.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/layers/landscapeoperationallayer.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/layers/landscapeoperationallayer.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/landscaping/topologydescription.py` & `automationkit-0.5.1/source/packages/akit/interop/landscaping/topologydescription.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/serial/serialtelnet.py` & `automationkit-0.5.1/source/packages/akit/interop/serial/serialtelnet.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/soap/Sonoswsdl-1.19.4-20190411.142401-3.wsdl` & `automationkit-0.5.1/source/packages/akit/interop/soap/Sonoswsdl-1.19.4-20190411.142401-3.wsdl`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/content/didllite.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/content/didllite.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/devices/__init__.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/devices/upnpdevice.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/devices/upnpdevice.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/devices/upnpembeddeddevice.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/devices/upnpembeddeddevice.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/devices/upnprootdevice.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/devices/upnprootdevice.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/avtransport1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/avtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/connectionmanager1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/connectionmanager1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/renderingcontrol1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/MicrosoftCorporation/renderingcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEAR/layer3forwarding1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEAR/layer3forwarding1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEARInc/wfawlanconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/NETGEARInc/wfawlanconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/alarmclock1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/alarmclock1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/audioin1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/audioin1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/avtransport1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/avtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/connectionmanager1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/connectionmanager1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/contentdirectory1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/contentdirectory1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/deviceproperties1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/deviceproperties1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/groupmanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/groupmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/grouprenderingcontrol1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/grouprenderingcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/htcontrol1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/htcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/musicservices1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/musicservices1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/qplay1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/qplay1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/queue1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/queue1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/renderingcontrol1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/renderingcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/systemproperties1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/systemproperties1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/virtuallinein1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/virtuallinein1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/zonegrouptopology1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/dynamic/services/SonosInc/zonegrouptopology1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosdevice.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosdevice.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosplayer.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/sonosplayer.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps1.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps1.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps11.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps11.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps12.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps12.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps13.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps13.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps14.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps14.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps15.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps15.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps16.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps16.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps17.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps17.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps18.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps18.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps19.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps19.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps22.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps22.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps23.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps23.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps24.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps24.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps3.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps3.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps34.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps34.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps38.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps38.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps5.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps5.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps6.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps6.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps9.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zps9.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpssub.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpssub.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp120.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp120.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp80.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/rootdevices/sonos/zpzp80.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaRenderer:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaRenderer:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaServer:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/embeddeddevices/SonosInc/urn:schemas-upnp-org:device:MediaServer:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/MicrosoftCorporation/XboxOne.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/MicrosoftCorporation/XboxOne.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEAR/NETGEARR7400Router.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEAR/NETGEARR7400Router.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEARInc/NETGEARR7400.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/NETGEARInc/NETGEARR7400.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosAmp.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosAmp.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosArc.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosArc.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBRAVO.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBRAVO.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBeam.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosBeam.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosConnectAmp.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosConnectAmp.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosFury.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosFury.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosMove.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosMove.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosOne.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosOne.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay3.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay3.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay5.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlay5.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybar.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybar.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybase.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPlaybase.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPort.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosPort.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoam.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoam.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoamSL.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosRoamSL.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosSub.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosSub.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosZP80.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/rootdevices/SonosInc/SonosZP80.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:AVTransport:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:AVTransport:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:ConnectionManager:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:ConnectionManager:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:RenderingControl:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/MicrosoftCorporation/urn:schemas-upnp-org:service:RenderingControl:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEAR/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEAR/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEARInc/urn:schemas-wifialliance-org:service:WFAWLANConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/NETGEARInc/urn:schemas-wifialliance-org:service:WFAWLANConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-tencent-com:service:QPlay:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-tencent-com:service:QPlay:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AlarmClock:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AlarmClock:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AudioIn:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:AudioIn:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:DeviceProperties:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:DeviceProperties:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:GroupManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:GroupManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:HTControl:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:HTControl:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:MusicServices:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:MusicServices:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:SystemProperties:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:SystemProperties:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:ZoneGroupTopology:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/dynamic/services/SonosInc/urn:schemas-upnp-org:service:ZoneGroupTopology:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/generator/upnpgenerator.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/generator/upnpgenerator.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/paths.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/paths.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/services/upnpdefaultvar.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/services/upnpdefaultvar.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/services/upnpserviceproxy.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/services/upnpserviceproxy.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/soap.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/soap.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/upnpconstants.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/upnpconstants.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/upnperrors.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/upnperrors.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/upnpfactory.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/upnpfactory.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/upnpprotocol.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/upnpprotocol.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/upnp/xml/upnpdevice1.py` & `automationkit-0.5.1/source/packages/akit/interop/upnp/xml/upnpdevice1.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/wireless/channels.py` & `automationkit-0.5.1/source/packages/akit/interop/wireless/channels.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/wireless/constants.py` & `automationkit-0.5.1/source/packages/akit/interop/wireless/constants.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/wireless/stationinfo.py` & `automationkit-0.5.1/source/packages/akit/interop/wireless/stationinfo.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/wireless/wep.py` & `automationkit-0.5.1/source/packages/akit/interop/wireless/wep.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/interop/wireless/wpa.py` & `automationkit-0.5.1/source/packages/akit/interop/wireless/wpa.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/jsos.py` & `automationkit-0.5.1/source/packages/akit/jsos.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/metadata.py` & `automationkit-0.5.1/source/packages/akit/metadata.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/monitoring/processmonitor.py` & `automationkit-0.5.1/source/packages/akit/monitoring/processmonitor.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/monitoring/reportingservice.py` & `automationkit-0.5.1/source/packages/akit/monitoring/reportingservice.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/monitoring/reportmonitor.py` & `automationkit-0.5.1/source/packages/akit/monitoring/reportmonitor.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/constants.py` & `automationkit-0.5.1/source/packages/akit/networking/constants.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/httpserverthreadpool.py` & `automationkit-0.5.1/source/packages/akit/networking/httpserverthreadpool.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/interfaces.py` & `automationkit-0.5.1/source/packages/akit/networking/interfaces.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/multicast.py` & `automationkit-0.5.1/source/packages/akit/networking/multicast.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/resolution.py` & `automationkit-0.5.1/source/packages/akit/networking/resolution.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/simplewebserver.py` & `automationkit-0.5.1/source/packages/akit/networking/simplewebserver.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/trafficcapturecontext.py` & `automationkit-0.5.1/source/packages/akit/networking/trafficcapturecontext.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/networking/unicast.py` & `automationkit-0.5.1/source/packages/akit/networking/unicast.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/paths.py` & `automationkit-0.5.1/source/packages/akit/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 
     global DIR_TESTRESULTS_DIRECTORY
 
     if DIR_TESTRESULTS_DIRECTORY is None:
         ctx = Context()
         configuration = ctx.lookup("/configuration")
 
-        tr_dir = configuration.lookup("/paths/testresults")
+        tr_dir = configuration.lookup("/paths/results/tests")
 
         DIR_TESTRESULTS_DIRECTORY = tr_dir
 
         if not os.path.exists(DIR_TESTRESULTS_DIRECTORY):
             os.makedirs(DIR_TESTRESULTS_DIRECTORY)
 
     return DIR_TESTRESULTS_DIRECTORY
```

### Comparing `automationkit-0.5.0/source/packages/akit/raisefor.py` & `automationkit-0.5.1/source/packages/akit/raisefor.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/readers/linux/command/ps.py` & `automationkit-0.5.1/source/packages/akit/readers/linux/command/ps.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/recorders.py` & `automationkit-0.5.1/source/packages/akit/recorders.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/results.py` & `automationkit-0.5.1/source/packages/akit/results.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/taskbase.py` & `automationkit-0.5.1/source/packages/akit/taskbase.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/templates/__init__.py` & `automationkit-0.5.1/source/packages/akit/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/templates/static/v0/testsummary.js` & `automationkit-0.5.1/source/packages/akit/templates/static/v0/testsummary.js`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/templates/static/v0/w3.css` & `automationkit-0.5.1/source/packages/akit/templates/static/v0/w3.css`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/templates/tabs/tab-images.html` & `automationkit-0.5.1/source/packages/akit/templates/tabs/tab-images.html`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/templates/tabs/tab-sounds.html` & `automationkit-0.5.1/source/packages/akit/templates/tabs/tab-sounds.html`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/templates/testsummary.html` & `automationkit-0.5.1/source/packages/akit/templates/testsummary.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         </script>
 
     </head>
     <body>
         <div class='section-header'>
             <div class='section-header'>
                 <div class="summary-banner">
-                    <div class="summary-banner-left image-sonos-banner-left"></div>
-                    <div class="summary-banner-middle image-sonos-banner-middle">
+                    <div class="summary-banner-left image-banner-left"></div>
+                    <div class="summary-banner-middle image-banner-middle">
                         <br/>
                         <br/>
                         <div style="width: auto; text-shadow: 5px 5px 6px black;">
                             <div class="summary-row" style="justify-content: flex-end;">
                                 <div style='color: whitesmoke' class="summary-label">Pod</div>
                                 <div style='color: whitesmoke' class="summary-value" id='summary-apod'>Automation Rig 2</div>
                                 <div style='color: whitesmoke' class="summary-label">Branch</div>
@@ -56,15 +56,15 @@
                                 <div style='color: whitesmoke' class="summary-label">Stop</div>
                                 <div style='color: whitesmoke' class="summary-value" id='summary-stop'>2019-09-21 22:43:08.195637</div>
                                 <div style='color: whitesmoke' class="summary-label">Status</div>
                                 <div style='color: whitesmoke' class="summary-value" id='summary-status'>RUNNING</div>
                             </div>
                         </div>
                     </div>
-                    <div class="summary-banner-right image-sonos-banner-right"></div>
+                    <div class="summary-banner-right image-banner-right"></div>
             </div>
             <br />
             <table class='summary-table'>
                     <tbody>
                         <tr class='summary-row'>
                             <td class='summary-label'>Errors</td><td id='summary-error' class='summary-value color-error'>0</td>
                             <td class='summary-label'>Failed</td><td id='summary-fail' class='summary-value color-fail'>0</td>
@@ -125,8 +125,8 @@
             <br/>
             <h2>Files</h2>
             <div id='container-files' class='ff-list'>
                 
             </div>
         </div>
     </body>
-</html>
+</html>
```

### Comparing `automationkit-0.5.0/source/packages/akit/testing/__init__.py` & `automationkit-0.5.1/source/packages/akit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/constraints.py` & `automationkit-0.5.1/source/packages/akit/testing/constraints.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/expressions.py` & `automationkit-0.5.1/source/packages/akit/testing/expressions.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/reflection.py` & `automationkit-0.5.1/source/packages/akit/testing/reflection.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/__init__.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/entrypoints.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/entrypoints.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/markers.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/markers.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/parameters.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/parameters.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/queries.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/queries.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/registration/parameterorigin.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/registration/parameterorigin.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/registration/resourceregistry.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/registration/resourceregistry.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/registration/resourcescope.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/registration/resourcescope.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/registration/scopesource.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/registration/scopesource.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/registration/sourcebase.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/registration/sourcebase.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/registration/unknownsource.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/registration/unknownsource.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/resources.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/resources.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/scopecoupling.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/scopecoupling.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/testcollector.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/testcollector.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/testgroup.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/testgroup.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/testjob.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/testjob.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/testref.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/testref.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/testsequencer.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/testsequencer.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/testplus/verification.py` & `automationkit-0.5.1/source/packages/akit/testing/testplus/verification.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/testing/utilities.py` & `automationkit-0.5.1/source/packages/akit/testing/utilities.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/timemachine.py` & `automationkit-0.5.1/source/packages/akit/timemachine.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/timeouts.py` & `automationkit-0.5.1/source/packages/akit/timeouts.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/waiting.py` & `automationkit-0.5.1/source/packages/akit/waiting.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/wellknown/singletons.py` & `automationkit-0.5.1/source/packages/akit/wellknown/singletons.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/entrypoints.py` & `automationkit-0.5.1/source/packages/akit/workflow/entrypoints.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/execution.py` & `automationkit-0.5.1/source/packages/akit/workflow/execution.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/tasks/createenvironment.py` & `automationkit-0.5.1/source/packages/akit/workflow/tasks/createenvironment.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/tasks/embeddedpython.py` & `automationkit-0.5.1/source/packages/akit/workflow/tasks/embeddedpython.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/tasks/gitcheckout.py` & `automationkit-0.5.1/source/packages/akit/workflow/tasks/gitcheckout.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/tasks/runcommand.py` & `automationkit-0.5.1/source/packages/akit/workflow/tasks/runcommand.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/tasks/shellscript.py` & `automationkit-0.5.1/source/packages/akit/workflow/tasks/shellscript.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/workflow/tasks/taskbase.py` & `automationkit-0.5.1/source/packages/akit/workflow/tasks/taskbase.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xcollections.py` & `automationkit-0.5.1/source/packages/akit/xcollections.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xconfiguration.py` & `automationkit-0.5.1/source/packages/akit/xconfiguration.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xcryptography/pkey.py` & `automationkit-0.5.1/source/packages/akit/xcryptography/pkey.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xcryptography/x509.py` & `automationkit-0.5.1/source/packages/akit/xcryptography/x509.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xdebugger.py` & `automationkit-0.5.1/source/packages/akit/xdebugger.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xenum.py` & `automationkit-0.5.1/source/packages/akit/xenum.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xfeature.py` & `automationkit-0.5.1/source/packages/akit/xfeature.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xformatting.py` & `automationkit-0.5.1/source/packages/akit/xformatting.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xinspect.py` & `automationkit-0.5.1/source/packages/akit/xinspect.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xlogging/__init__.py` & `automationkit-0.5.1/source/packages/akit/xlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xlogging/foundations.py` & `automationkit-0.5.1/source/packages/akit/xlogging/foundations.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xlogging/scopemonitoring.py` & `automationkit-0.5.1/source/packages/akit/xlogging/scopemonitoring.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xml/parsing.py` & `automationkit-0.5.1/source/packages/akit/xml/parsing.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xmultiprocessing/smbserverprocess.py` & `automationkit-0.5.1/source/packages/akit/xmultiprocessing/smbserverprocess.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xmultiprocessing/webserverprocess.py` & `automationkit-0.5.1/source/packages/akit/xmultiprocessing/webserverprocess.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xregex/regexreader.py` & `automationkit-0.5.1/source/packages/akit/xregex/regexreader.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xthreading/__init__.py` & `automationkit-0.5.1/source/packages/akit/xthreading/__init__.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xthreading/looper.py` & `automationkit-0.5.1/source/packages/akit/xthreading/looper.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xthreading/looperpool.py` & `automationkit-0.5.1/source/packages/akit/xthreading/looperpool.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xthreading/looperqueue.py` & `automationkit-0.5.1/source/packages/akit/xthreading/looperqueue.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xthreading/readwritelock.py` & `automationkit-0.5.1/source/packages/akit/xthreading/readwritelock.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/source/packages/akit/xtime.py` & `automationkit-0.5.1/source/packages/akit/xtime.py`

 * *Files identical despite different names*

### Comparing `automationkit-0.5.0/setup.py` & `automationkit-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,17 +113,17 @@
  'rope>=1.6.0,<2.0.0',
  'ssdp>=1.1.1,<2.0.0',
  'werkzeug>=2.2.2,<3.0.0',
  'zeroconf>=0.47.1,<0.48.0']
 
 setup_kwargs = {
     'name': 'automationkit',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Automation Kit Test Framework',
-    'long_description': '# Automation Kit Repository\n\nWelcome to the Automation Kit repository!\n\n\n*Note:* This package is progressing quickly but is not yet ready for full production environments.\n\n# Description\nThe **Automation Kit** is a python toolkit for building distributed automated task and testing systems.  It goes beyond the capabilities of other task and test automation frameworks by providing a hybrid approach that allows for dependency injection, similar to pytest, combined with and object oriented framework that can be utilized to easily customize the orchestration of tasks and tests across a collection of integrated resources.  Because the **Automation Kit** is built from the start with distributed automation in mind, it can help you quickly get distributed automated systems up and running that are based on a tested and proven set of object patterns and APIs.\n\n# Design Philosophies\nThis section covers some of the important design features of the **Automation Kit** framework.\n\n## Large Scale\nThe **Automation Kit** is designed for enterprise level distributed automation *"at scale"*.  The term *"at scale"* refers not only to a larger collection of enterprise resources but also refers to the fact that the **Automation Kit** helps to setup patterns that will support working in a very large code base.  The size of a code base that you might see associated with large enterprise level projects.  The **Automation Kit** supports working in large code bases by helping to establish good code organizational patterns and abstractions that support characteristics that:\n\n* make it easier to learn and work in the code base\n* make the code base easier to maintain\n* make it easier to share and reuse code\n\n## Faster Classification of Issues\nOne of the key philosophies behind the **Automation Kit** design is one of being able quickly and efficiently identify the nature of issues that come up during automation runs.  The **Automation Kit** initially classifies errors into one of four categories:\n\n* **Configuration** - We identify configuration issues quickly and classify them so as to ensure that resources are not waisted troubleshooting configuration related issues and that eronious test results or noise is not generated due to configuration related issues. We also want automation runs to fail out quickly if the automation configuration is not setup correctly, before waisting additional testing resources.\n* **Environment** - The **Automation Kit** performs an initial diagnostic scan of the automation landscape and all the resources declared to be necessary to run a series of tasks or tests in order to provide indications of environmental failures as early as possible.  This is important to ensure that we do not generate noise in automation results that are not related to the automation tasks or tests that might fail.  Just as with configuration, we want automation runs to fail out quickly if the automation environment is not setup correctly.\n* **Error** - The **Automation Kit** classifies un-expected errors, or errors that are not founded in an expectation of a result, as an **Error** condition.  This helps to ensure these errors are given an appropriate initial direction or indication that the issues is a problem in the automation code and not an issue in the code that is the target of the automation run.\n* **Failure** - The **AutomationKit** classifies failures that are associated with an expectation of behavior from a target under test as failures.  This allows for the proper initial classification of an issue as being a problem that is likely a failure in the code being targeted by the automation and the behavior or result it should have exhibited.\n\nHaving the initial classification of issues fall into one of these four categories helps to ensure that issues are easier to triage and assign to the appropriate party for investigation and resolution. It also helps to establish categories that can be used for data collection in order to better analyse the performance of test infrastructure, test code and product code.\n\n## Integration and Distributed Automation Support\nThe **Automation Kit** comes with enterprise level integration and distributed automation capabilities.  The framework utilizes a customize-able set of classes that guides enterprise users through a process of creating a very robust integration object model based on the roles that enterprise resources play in an automation landscape.\n\nThe declaration of a custom automation landscape is as simple as setting an environment variable or passing a command line flag declaring the python module that contains a custom landscape derived class.  The *Landscape* and *LandscapeDescription* derived classes work together to provide the **Automation Kit** with a description of the customized roles and integration mixin(s) that provide the connection between the tasks and test automation code.\n\n## Task and Test Integration Declaration and Assurance\nThe **Automation Kit** utilizes its object model to allow tasks and tests to provide information about their associated integration points and scopes of execution to the automation framework.  This integration declaration mechanism allows the automation framework to provide an early scan of the integration pathways and provide levels of assurance as to the stability of the automation landscape early in the automation process.  This is vitally important as it eliminates the waist and noise that are often associated with automation runs that are performed against an automation Landscape that has broken, mis-configured or missing resources.\n\n## Automation Job, Scope and Flow Control \nThe **Automation Kit** allows enterprise users to organize and customize the ordering of automation scope engagements and the flow of an automation job.  This provides the automation engineer the ability to control the engagement of automation scopes of execution and allows for optimal use of time and overlapping of scopes of execution in a test run.\n\n# Table of Contents\n1. [Automation Software Stack](http://automationmojo.com/automationkit/docs/usermanual/10-automation-software-stack.html)\n2. [Getting Started](http://automationmojo.com/automationkit/docs/usermanual/20-getting-started.html)\n3. [Automation Configuration](http://automationmojo.com/automationkit/docs/usermanual/30-automation-configuration.html)\n    1. [Landscape File](http://automationmojo.com/automationkit/docs/usermanual/31-landscape-file.html)\n    2. [Topology File](http://automationmojo.com/automationkit/docs/usermanual/32-topology-file.html)\n    2. [Runtime File](http://automationmojo.com/automationkit/docs/usermanual/33-runtime-file.html)\n    3. [Credentials File](http://automationmojo.com/automationkit/docs/usermanual/34-credentials-file.html)\n4. [TestRun Sequencing](http://automationmojo.com/automationkit/docs/usermanual/40-testrun-sequencing.html)\n    1. [Integration Couplings](http://automationmojo.com/automationkit/docs/usermanual/41-integration-couplings.html)\n    2. [Scope Couplings](http://automationmojo.com/automationkit/docs/usermanual/42-scope-couplings.html)\n5. [Functional Description](http://automationmojo.com/automationkit/docs/usermanual/50-functional-description.html)\n    1. [Activation and Startup](http://automationmojo.com/automationkit/docs/usermanual/51-activation-and-startup.html)\n    2. [Inter-Operability](http://automationmojo.com/automationkit/docs/usermanual/52-inter-operability.html)\n    3. [SSH Coordinator and Agent](http://automationmojo.com/automationkit/docs/usermanual/53-ssh-coordinator-and-agent.html)\n    4. [UPNP Coordinator and Agent](http://automationmojo.com/automationkit/docs/usermanual/54-upnp-coordinator-and-agent.html)\n6. [Workflow Orchestration](http://automationmojo.com/automationkit/docs/usermanual/60-workflow-orchestration.html)\n7. [Enterprise Extensibility](http://automationmojo.com/automationkit/docs/usermanual/70-enterprise-extensibility.html)\n8. [Command Line](http://automationmojo.com/automationkit/docs/usermanual/80-command-line.html)\n9. [Code Organization and Conventions](http://automationmojo.com/automationkit/docs/usermanual/90-code-organization-and-conventions.html)\n10. [Coding Standards](http://automationmojo.com/automationkit/docs/usermanual/100-coding-standards.html)\n',
+    'long_description': '# Automation Kit Repository\n\nWelcome to the Automation Kit repository!\n\n\n*Note:* This package is progressing quickly but is not yet ready for full production environments.\n\n# Description\nThe **Automation Kit** is a python toolkit for building distributed automated task and testing systems.  It goes beyond the capabilities of other task and test automation frameworks by providing a hybrid approach that allows for dependency injection, similar to pytest, combined with and object oriented framework that can be utilized to easily customize the orchestration of tasks and tests across a collection of integrated resources.  Because the **Automation Kit** is built from the start with distributed automation in mind, it can help you quickly get distributed automated systems up and running that are based on a tested and proven set of object patterns and APIs.\n\n# Design Philosophies\nThis section covers some of the important design features of the **Automation Kit** framework.\n\n## Large Scale\nThe **Automation Kit** is designed for enterprise level distributed automation *"at scale"*.  The term *"at scale"* refers not only to a larger collection of enterprise resources but also refers to the fact that the **Automation Kit** helps to setup patterns that will support working in a very large code base.  The size of a code base that you might see associated with large enterprise level projects.  The **Automation Kit** supports working in large code bases by helping to establish good code organizational patterns and abstractions that support characteristics that:\n\n* make it easier to learn and work in the code base\n* make the code base easier to maintain\n* make it easier to share and reuse code\n\n## Faster Classification of Issues\nOne of the key philosophies behind the **Automation Kit** design is one of being able quickly and efficiently identify the nature of issues that come up during automation runs.  The **Automation Kit** initially classifies errors into one of four categories:\n\n* **Configuration** - We identify configuration issues quickly and classify them so as to ensure that resources are not waisted troubleshooting configuration related issues and that eronious test results or noise is not generated due to configuration related issues. We also want automation runs to fail out quickly if the automation configuration is not setup correctly, before waisting additional testing resources.\n* **Environment** - The **Automation Kit** performs an initial diagnostic scan of the automation landscape and all the resources declared to be necessary to run a series of tasks or tests in order to provide indications of environmental failures as early as possible.  This is important to ensure that we do not generate noise in automation results that are not related to the automation tasks or tests that might fail.  Just as with configuration, we want automation runs to fail out quickly if the automation environment is not setup correctly.\n* **Error** - The **Automation Kit** classifies un-expected errors, or errors that are not founded in an expectation of a result, as an **Error** condition.  This helps to ensure these errors are given an appropriate initial direction or indication that the issues is a problem in the automation code and not an issue in the code that is the target of the automation run.\n* **Failure** - The **AutomationKit** classifies failures that are associated with an expectation of behavior from a target under test as failures.  This allows for the proper initial classification of an issue as being a problem that is likely a failure in the code being targeted by the automation and the behavior or result it should have exhibited.\n\nHaving the initial classification of issues fall into one of these four categories helps to ensure that issues are easier to triage and assign to the appropriate party for investigation and resolution. It also helps to establish categories that can be used for data collection in order to better analyse the performance of test infrastructure, test code and product code.\n\n## Integration and Distributed Automation Support\nThe **Automation Kit** comes with enterprise level integration and distributed automation capabilities.  The framework utilizes a customize-able set of classes that guides enterprise users through a process of creating a very robust integration object model based on the roles that enterprise resources play in an automation landscape.\n\nThe declaration of a custom automation landscape is as simple as setting an environment variable or passing a command line flag declaring the python module that contains a custom landscape derived class.  The *Landscape* and *LandscapeDescription* derived classes work together to provide the **Automation Kit** with a description of the customized roles and integration mixin(s) that provide the connection between the tasks and test automation code.\n\n## Task and Test Integration Declaration and Assurance\nThe **Automation Kit** utilizes its object model to allow tasks and tests to provide information about their associated integration points and scopes of execution to the automation framework.  This integration declaration mechanism allows the automation framework to provide an early scan of the integration pathways and provide levels of assurance as to the stability of the automation landscape early in the automation process.  This is vitally important as it eliminates the waist and noise that are often associated with automation runs that are performed against an automation Landscape that has broken, mis-configured or missing resources.\n\n## Automation Job, Scope and Flow Control \nThe **Automation Kit** allows enterprise users to organize and customize the ordering of automation scope engagements and the flow of an automation job.  This provides the automation engineer the ability to control the engagement of automation scopes of execution and allows for optimal use of time and overlapping of scopes of execution in a test run.\n\n# Table of Contents\n1. [Automation Software Stack](http://automationmojo.com/static/automationkit/docs/usermanual/10-automation-software-stack.html)\n2. [Getting Started](http://automationmojo.com/static/automationkit/docs/usermanual/20-getting-started.html)\n3. [Automation Configuration](http://automationmojo.com/static/automationkit/docs/usermanual/30-automation-configuration.html)\n    1. [Landscape File](http://automationmojo.com/static/automationkit/docs/usermanual/31-landscape-file.html)\n    2. [Topology File](http://automationmojo.com/static/automationkit/docs/usermanual/32-topology-file.html)\n    2. [Runtime File](http://automationmojo.com/static/automationkit/docs/usermanual/33-runtime-file.html)\n    3. [Credentials File](http://automationmojo.com/static/automationkit/docs/usermanual/34-credentials-file.html)\n4. [TestRun Sequencing](http://automationmojo.com/static/automationkit/docs/usermanual/40-testrun-sequencing.html)\n    1. [Integration Couplings](http://automationmojo.com/static/automationkit/docs/usermanual/41-integration-couplings.html)\n    2. [Scope Couplings](http://automationmojo.com/static/automationkit/docs/usermanual/42-scope-couplings.html)\n5. [Functional Description](http://automationmojo.com/static/automationkit/docs/usermanual/50-functional-description.html)\n    1. [Activation and Startup](http://automationmojo.com/static/automationkit/docs/usermanual/51-activation-and-startup.html)\n    2. [Inter-Operability](http://automationmojo.com/static/automationkit/docs/usermanual/52-inter-operability.html)\n    3. [SSH Coordinator and Agent](http://automationmojo.com/static/automationkit/docs/usermanual/53-ssh-coordinator-and-agent.html)\n    4. [UPNP Coordinator and Agent](http://automationmojo.com/static/automationkit/docs/usermanual/54-upnp-coordinator-and-agent.html)\n6. [Workflow Orchestration](http://automationmojo.com/static/automationkit/docs/usermanual/60-workflow-orchestration.html)\n7. [Enterprise Extensibility](http://automationmojo.com/static/automationkit/docs/usermanual/70-enterprise-extensibility.html)\n8. [Command Line](http://automationmojo.com/static/automationkit/docs/usermanual/80-command-line.html)\n9. [Code Organization and Conventions](http://automationmojo.com/static/automationkit/docs/usermanual/90-code-organization-and-conventions.html)\n10. [Coding Standards](http://automationmojo.com/static/automationkit/docs/usermanual/100-coding-standards.html)\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `automationkit-0.5.0/PKG-INFO` & `automationkit-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automationkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automation Kit Test Framework
 License: LICENSE.txt
 Keywords: automation,continuous-integration,distributed-test-framework,distributed-testing-tools,distributed-testing,upnp,test-automation,test-framework,testing,testing-tools
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -79,28 +79,28 @@
 ## Task and Test Integration Declaration and Assurance
 The **Automation Kit** utilizes its object model to allow tasks and tests to provide information about their associated integration points and scopes of execution to the automation framework.  This integration declaration mechanism allows the automation framework to provide an early scan of the integration pathways and provide levels of assurance as to the stability of the automation landscape early in the automation process.  This is vitally important as it eliminates the waist and noise that are often associated with automation runs that are performed against an automation Landscape that has broken, mis-configured or missing resources.
 
 ## Automation Job, Scope and Flow Control 
 The **Automation Kit** allows enterprise users to organize and customize the ordering of automation scope engagements and the flow of an automation job.  This provides the automation engineer the ability to control the engagement of automation scopes of execution and allows for optimal use of time and overlapping of scopes of execution in a test run.
 
 # Table of Contents
-1. [Automation Software Stack](http://automationmojo.com/automationkit/docs/usermanual/10-automation-software-stack.html)
-2. [Getting Started](http://automationmojo.com/automationkit/docs/usermanual/20-getting-started.html)
-3. [Automation Configuration](http://automationmojo.com/automationkit/docs/usermanual/30-automation-configuration.html)
-    1. [Landscape File](http://automationmojo.com/automationkit/docs/usermanual/31-landscape-file.html)
-    2. [Topology File](http://automationmojo.com/automationkit/docs/usermanual/32-topology-file.html)
-    2. [Runtime File](http://automationmojo.com/automationkit/docs/usermanual/33-runtime-file.html)
-    3. [Credentials File](http://automationmojo.com/automationkit/docs/usermanual/34-credentials-file.html)
-4. [TestRun Sequencing](http://automationmojo.com/automationkit/docs/usermanual/40-testrun-sequencing.html)
-    1. [Integration Couplings](http://automationmojo.com/automationkit/docs/usermanual/41-integration-couplings.html)
-    2. [Scope Couplings](http://automationmojo.com/automationkit/docs/usermanual/42-scope-couplings.html)
-5. [Functional Description](http://automationmojo.com/automationkit/docs/usermanual/50-functional-description.html)
-    1. [Activation and Startup](http://automationmojo.com/automationkit/docs/usermanual/51-activation-and-startup.html)
-    2. [Inter-Operability](http://automationmojo.com/automationkit/docs/usermanual/52-inter-operability.html)
-    3. [SSH Coordinator and Agent](http://automationmojo.com/automationkit/docs/usermanual/53-ssh-coordinator-and-agent.html)
-    4. [UPNP Coordinator and Agent](http://automationmojo.com/automationkit/docs/usermanual/54-upnp-coordinator-and-agent.html)
-6. [Workflow Orchestration](http://automationmojo.com/automationkit/docs/usermanual/60-workflow-orchestration.html)
-7. [Enterprise Extensibility](http://automationmojo.com/automationkit/docs/usermanual/70-enterprise-extensibility.html)
-8. [Command Line](http://automationmojo.com/automationkit/docs/usermanual/80-command-line.html)
-9. [Code Organization and Conventions](http://automationmojo.com/automationkit/docs/usermanual/90-code-organization-and-conventions.html)
-10. [Coding Standards](http://automationmojo.com/automationkit/docs/usermanual/100-coding-standards.html)
+1. [Automation Software Stack](http://automationmojo.com/static/automationkit/docs/usermanual/10-automation-software-stack.html)
+2. [Getting Started](http://automationmojo.com/static/automationkit/docs/usermanual/20-getting-started.html)
+3. [Automation Configuration](http://automationmojo.com/static/automationkit/docs/usermanual/30-automation-configuration.html)
+    1. [Landscape File](http://automationmojo.com/static/automationkit/docs/usermanual/31-landscape-file.html)
+    2. [Topology File](http://automationmojo.com/static/automationkit/docs/usermanual/32-topology-file.html)
+    2. [Runtime File](http://automationmojo.com/static/automationkit/docs/usermanual/33-runtime-file.html)
+    3. [Credentials File](http://automationmojo.com/static/automationkit/docs/usermanual/34-credentials-file.html)
+4. [TestRun Sequencing](http://automationmojo.com/static/automationkit/docs/usermanual/40-testrun-sequencing.html)
+    1. [Integration Couplings](http://automationmojo.com/static/automationkit/docs/usermanual/41-integration-couplings.html)
+    2. [Scope Couplings](http://automationmojo.com/static/automationkit/docs/usermanual/42-scope-couplings.html)
+5. [Functional Description](http://automationmojo.com/static/automationkit/docs/usermanual/50-functional-description.html)
+    1. [Activation and Startup](http://automationmojo.com/static/automationkit/docs/usermanual/51-activation-and-startup.html)
+    2. [Inter-Operability](http://automationmojo.com/static/automationkit/docs/usermanual/52-inter-operability.html)
+    3. [SSH Coordinator and Agent](http://automationmojo.com/static/automationkit/docs/usermanual/53-ssh-coordinator-and-agent.html)
+    4. [UPNP Coordinator and Agent](http://automationmojo.com/static/automationkit/docs/usermanual/54-upnp-coordinator-and-agent.html)
+6. [Workflow Orchestration](http://automationmojo.com/static/automationkit/docs/usermanual/60-workflow-orchestration.html)
+7. [Enterprise Extensibility](http://automationmojo.com/static/automationkit/docs/usermanual/70-enterprise-extensibility.html)
+8. [Command Line](http://automationmojo.com/static/automationkit/docs/usermanual/80-command-line.html)
+9. [Code Organization and Conventions](http://automationmojo.com/static/automationkit/docs/usermanual/90-code-organization-and-conventions.html)
+10. [Coding Standards](http://automationmojo.com/static/automationkit/docs/usermanual/100-coding-standards.html)
```


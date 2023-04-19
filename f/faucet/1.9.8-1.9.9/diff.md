# Comparing `tmp/faucet-1.9.8.tar.gz` & `tmp/faucet-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/faucet-1.9.8.tar", last modified: Fri Jun  7 03:37:39 2019, max compression
+gzip compressed data, was "dist/faucet-1.9.9.tar", last modified: Tue Jun 25 05:33:55 2019, max compression
```

## Comparing `faucet-1.9.8.tar` & `faucet-1.9.9.tar`

### file list

```diff
@@ -1,350 +1,352 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/hooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2019-06-07 03:36:45.000000 faucet-1.9.8/hooks/pre_build
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2019-06-07 03:36:45.000000 faucet-1.9.8/.dockerignore
--rw-rw-r--   0 travis    (2000) travis    (2000)    23324 2019-06-07 03:37:38.000000 faucet-1.9.8/ChangeLog
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2019-06-07 03:36:45.000000 faucet-1.9.8/Dockerfile.fuzz-packet
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/external_resources.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/recipe_book/
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/recipe_book/policy.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/recipe_book/routing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/recipe_book/forwarding.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/recipe_book/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/tutorials/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19044 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/tutorials/first_time.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    15605 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/tutorials/routing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     8477 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/tutorials/vlans.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    13123 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/tutorials/acls.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/tutorials/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    17927 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/tutorials/nfv_services.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    15004 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/developer_guide.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4828 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/architecture.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/noviflow/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3286 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/noviflow/README_noviflow.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/lagopus/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3638 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/lagopus/README_Lagopus.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/allied-telesis/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14234 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/allied-telesis/README_Allied_Telesis.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/northboundnetworks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1661 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/northboundnetworks/README_ZodiacFX.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      605 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/northboundnetworks/README_ZodiacGX.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)      697 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/northboundnetworks/conf-zodiac.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/ovs/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18223 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/ovs/faucet_ovs_test.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     6413 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/ovs/README_OVS-DPDK.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9332 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/cisco/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9521 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/cisco/README_Cisco.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      405 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/vendors/hpe/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17286 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/vendors/hpe/README_Aruba.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5281 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/intro.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)    34548 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/configuration.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     7099 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/source/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     1395 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/fuzzing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    13916 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/installation.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/release_notes/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3271 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/release_notes/1.9.0.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3303 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/release_notes/1.7.0.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3857 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/faq.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/autogen/
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/autogen/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      930 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/monitoring.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/_static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/_static/deployments/
--rw-rw-r--   0 travis    (2000) travis    (2000)  1106115 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/deployments/nznog17-virtual-network.jpg
--rw-rw-r--   0 travis    (2000) travis    (2000)    89120 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/deployments/ONF_Faucet_deploy1.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   984943 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/deployments/nznog17-physical-network.jpg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/_static/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/css/responsive-tables.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/_static/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)    58351 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/faucet-pipeline.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2421 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/faucet-pipeline.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   172474 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/tutorial-vlans.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)    47652 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/tutorial-ivr.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)   452164 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/gauge-snapshot2.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    51732 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/tutorial-acls.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)    23716 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/faucet-pipeline.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    77255 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/tutorial-bgp-routing.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)    87114 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/tutorial-nfv-services.svg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8466 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/8021X-conf-diagram.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)   467326 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/gauge-snapshot3.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    97737 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/faucet-architecture.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)   136689 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/gauge-nznog17.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    59007 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/tutorial-static-routing.svg
--rw-rw-r--   0 travis    (2000) travis    (2000)   285918 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/images/gauge-snapshot1.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/_static/tutorial/
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/tutorial/as_ns
--rw-rw-r--   0 travis    (2000) travis    (2000)     1086 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/tutorial/cleanup
--rw-rw-r--   0 travis    (2000) travis    (2000)      425 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/tutorial/add_tagged_interface
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/tutorial/create_ns
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docs/_static/grafana-dashboards/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14739 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/grafana-dashboards/faucet_port_statistics.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18897 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/grafana-dashboards/faucet_instrumentation.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    20170 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/_static/grafana-dashboards/faucet_inventory.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9402 2019-06-07 03:36:45.000000 faucet-1.9.8/docs/testing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2019-06-07 03:36:45.000000 faucet-1.9.8/.codecov.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2019-06-07 03:36:45.000000 faucet-1.9.8/fuzz-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2019-06-07 03:36:45.000000 faucet-1.9.8/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/adapters/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/adapters/vendors/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/adapters/vendors/rabbitmq/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/adapters/vendors/rabbitmq/hooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/hooks/pre_build
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/example_consumer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3473 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/test_rabbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      661 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/docker-compose-pi.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     6854 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/rabbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/docker-compose-rabbitmq.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      733 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/Dockerfile.pi
--rw-rw-r--   0 travis    (2000) travis    (2000)      655 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/docker-compose.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1636 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/vendors/rabbitmq/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-06-07 03:36:45.000000 faucet-1.9.8/adapters/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      830 2019-06-07 03:36:45.000000 faucet-1.9.8/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2232 2019-06-07 03:36:45.000000 faucet-1.9.8/docker-compose-pi.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      785 2019-06-07 03:37:39.000000 faucet-1.9.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-06-07 03:36:45.000000 faucet-1.9.8/Dockerfile.gauge
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      785 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/pbr.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7962 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2019-06-07 03:36:45.000000 faucet-1.9.8/Dockerfile.gauge.pi
--rw-rw-r--   0 travis    (2000) travis    (2000)      220 2019-06-07 03:36:45.000000 faucet-1.9.8/Dockerfile.faucet.pi
--rw-rw-r--   0 travis    (2000) travis    (2000)      185 2019-06-07 03:36:45.000000 faucet-1.9.8/test-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2538 2019-06-07 03:36:45.000000 faucet-1.9.8/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/debian/
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/watch
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/faucet-docs.docs
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/gauge.service
--rwxrwxr-x   0 travis    (2000) travis    (2000)      563 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/rules
--rw-rw-r--   0 travis    (2000) travis    (2000)      216 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/gauge.default
--rw-rw-r--   0 travis    (2000) travis    (2000)      135 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/changelog
--rw-rw-r--   0 travis    (2000) travis    (2000)      905 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/copyright
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/compat
--rw-rw-r--   0 travis    (2000) travis    (2000)     3438 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/control
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/debian/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/source/format
--rw-rw-r--   0 travis    (2000) travis    (2000)      204 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/faucet.install
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/faucet.default
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/faucet.service
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/gauge.install
--rw-rw-r--   0 travis    (2000) travis    (2000)       54 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/faucet-all-in-one.install
--rw-rw-r--   0 travis    (2000) travis    (2000)     1035 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/faucet.postinst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1035 2019-06-07 03:36:45.000000 faucet-1.9.8/debian/gauge.postinst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/git-hook/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      456 2019-06-07 03:36:45.000000 faucet-1.9.8/git-hook/pre-commit
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/gitlab/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      971 2019-06-07 03:36:45.000000 faucet-1.9.8/gitlab/deploy_deb.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2019-06-07 03:36:45.000000 faucet-1.9.8/hw_switch_config.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/travis/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3188 2019-06-07 03:36:45.000000 faucet-1.9.8/travis/runtests.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/images/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/images/vm/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      462 2019-06-07 03:36:45.000000 faucet-1.9.8/images/vm/build-faucet-vm.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2019-06-07 03:36:45.000000 faucet-1.9.8/images/vm/.gitignore
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/images/vm/elements/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/images/vm/elements/faucet-all-in-one/
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-06-07 03:36:45.000000 faucet-1.9.8/images/vm/elements/faucet-all-in-one/package-installs.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/images/vm/elements/faucet-all-in-one/install.d/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      924 2019-06-07 03:36:45.000000 faucet-1.9.8/images/vm/elements/faucet-all-in-one/install.d/02-install-faucet-gauge-prometheus-grafana
--rw-rw-r--   0 travis    (2000) travis    (2000)      210 2019-06-07 03:36:45.000000 faucet-1.9.8/images/vm/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/images/raspbian/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      571 2019-06-07 03:36:45.000000 faucet-1.9.8/images/raspbian/02-run.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4863 2019-06-07 03:36:45.000000 faucet-1.9.8/images/raspbian/build.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2340 2019-06-07 03:36:45.000000 faucet-1.9.8/images/raspbian/prerun.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2300 2019-06-07 03:36:45.000000 faucet-1.9.8/images/raspbian/common
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2019-06-07 03:36:45.000000 faucet-1.9.8/Dockerfile.faucet
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2019-06-07 03:36:45.000000 faucet-1.9.8/.pyup.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/etc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/etc/systemd/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/etc/systemd/system/
--rw-rw-r--   0 travis    (2000) travis    (2000)      355 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/systemd/system/prometheus.service
--rw-rw-r--   0 travis    (2000) travis    (2000)      419 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/systemd/system/gauge.service
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/systemd/system/faucet.service
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/etc/prometheus/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/prometheus/faucet.rules.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      862 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/prometheus/prometheus.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/prometheus/prometheus-docker-compose.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/etc/logrotate.d/
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/logrotate.d/gauge
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/logrotate.d/faucet
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/etc/default/
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/default/gauge
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/default/faucet
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/etc/faucet/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2704 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/faucet/acls.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/faucet/ryu.conf
--rw-rw-r--   0 travis    (2000) travis    (2000)     2339 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/faucet/faucet.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      965 2019-06-07 03:36:45.000000 faucet-1.9.8/etc/faucet/gauge.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1100 2019-06-07 03:37:39.000000 faucet-1.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2320 2019-06-07 03:36:45.000000 faucet-1.9.8/.gitlab-ci.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2282 2019-06-07 03:36:45.000000 faucet-1.9.8/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      129 2019-06-07 03:36:45.000000 faucet-1.9.8/Dockerfile.tests
--rw-rw-r--   0 travis    (2000) travis    (2000)     2136 2019-06-07 03:36:45.000000 faucet-1.9.8/docker-compose.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)    10912 2019-06-07 03:36:45.000000 faucet-1.9.8/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/docker/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      595 2019-06-07 03:36:45.000000 faucet-1.9.8/docker/fuzz_packet.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3705 2019-06-07 03:36:45.000000 faucet-1.9.8/docker/runtests.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      317 2019-06-07 03:36:45.000000 faucet-1.9.8/docker/pip_deps.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      700 2019-06-07 03:36:45.000000 faucet-1.9.8/docker/install-faucet.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      594 2019-06-07 03:36:45.000000 faucet-1.9.8/docker/fuzz_config.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      834 2019-06-07 03:36:45.000000 faucet-1.9.8/docker/localtest.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      220 2019-06-07 03:36:45.000000 faucet-1.9.8/docker/retrycmd.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2019-06-07 03:36:45.000000 faucet-1.9.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      416 2019-06-07 03:36:45.000000 faucet-1.9.8/Dockerfile.fuzz-config
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3278 2019-06-07 03:36:45.000000 faucet-1.9.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/clib/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4878 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/tcpdump_helper.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      538 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/clib_mininet_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20354 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/mininet_test_topo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7070 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/mininet_test_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   110574 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/mininet_test_base.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    26577 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/clib_mininet_test_main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12771 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/docker_host.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6135 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/clib_mininet_tests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-06-07 03:36:45.000000 faucet-1.9.8/clib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/faucet/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/meter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3516 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/prom_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10474 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valves_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30872 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_of.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7274 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/gauge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6100 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/router.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17605 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_host.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    59022 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/dp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18174 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/acl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9696 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_table.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6427 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/watcher_conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5774 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/watcher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6567 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/gauge_prom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9834 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8492 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9021 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23321 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/vlan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11872 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/config_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9508 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/gauge_influx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6037 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_util.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6087 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9829 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet_bgp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4503 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/tfm_pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27542 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_packet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1032 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_manager_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7027 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet_pipeline.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7794 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/fctl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2853 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet_experimental_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5129 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet_event.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_of_old.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13085 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet_dot1x.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7538 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/config_parser_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7490 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_ryuapp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12902 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/faucet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40232 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_route.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9036 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/gauge_pollers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17167 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_acl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72294 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29625 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/valve_flood.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2269 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/check_faucet_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14254 2019-06-07 03:36:45.000000 faucet-1.9.8/faucet/port.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      530 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/run_unit_tests.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      244 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/sysctls_for_tests.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      427 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/run_integration_tests.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/fuzzer/
--rw-rw-r--   0 travis    (2000) travis    (2000)      706 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/fake_packet.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/fuzzer/dict/
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/dict/packet.dict
--rw-rw-r--   0 travis    (2000) travis    (2000)     1572 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/dict/config.dict
--rw-rw-r--   0 travis    (2000) travis    (2000)      878 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/fuzz_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1655 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/display_packet_crash.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/fuzzer/packet/
--rw-rw-r--   0 travis    (2000) travis    (2000)      277 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/dns.ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/tcp.ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/arp.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/udp.ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/diameter.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      465 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/http.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/msger.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/arp.ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2885 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/icmp.ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/asap.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      109 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/tcp.ex3
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/lacp.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/tcp.ex4
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/igmpv2.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      193 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/irc.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/icmp.ex3
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/udp.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      925 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/http.ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/ipv6.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/icmp.ex4
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/tcp.ex5
--rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/dns.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)     2021 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/ipv4.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/udp.ex4
--rw-rw-r--   0 travis    (2000) travis    (2000)      933 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/icmp.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/tcp.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      311 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/irc.ex3
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/irc.ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/udp.ex3
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/aoe.ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/packet/asap.ex2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/fuzzer/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex6
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex11
--rw-rw-r--   0 travis    (2000) travis    (2000)      219 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex9
--rw-rw-r--   0 travis    (2000) travis    (2000)      585 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex1
--rw-rw-r--   0 travis    (2000) travis    (2000)      303 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex14
--rw-rw-r--   0 travis    (2000) travis    (2000)      412 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex5
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex2
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex10
--rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex12
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex7
--rw-rw-r--   0 travis    (2000) travis    (2000)      531 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex8
--rw-rw-r--   0 travis    (2000) travis    (2000)      360 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex4
--rw-rw-r--   0 travis    (2000) travis    (2000)      222 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/config/ex3
--rw-rw-r--   0 travis    (2000) travis    (2000)     1543 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/fuzzer/fuzz_packet.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/codecheck/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      439 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/codecheck/pytype.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      200 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/codecheck/pylint.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      605 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/codecheck/min_pylint.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      340 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/codecheck/src_files.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/integration/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      502 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/integration/mininet_main.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2360 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/integration/experimental_api_test_app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   262067 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/integration/mininet_tests.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/unit/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/unit/packaging/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4819 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/packaging/test_packaging.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/unit/gauge/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    35380 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/gauge/test_gauge.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4959 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/gauge/test_config_gauge.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1527 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/gauge/test_main.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-07 03:37:39.000000 faucet-1.9.8/tests/unit/faucet/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11277 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/test_check_config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1053 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/test_port.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8954 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/test_vlan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18585 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/fakeoftable.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1530 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/test_main.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)   108326 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/test_valve.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    79144 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/test_config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6497 2019-06-07 03:36:45.000000 faucet-1.9.8/tests/unit/faucet/test_fctl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      193 2019-06-07 03:36:45.000000 faucet-1.9.8/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      818 2019-06-07 03:37:38.000000 faucet-1.9.8/AUTHORS
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/hooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2019-06-25 05:32:59.000000 faucet-1.9.9/hooks/pre_build
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2019-06-25 05:32:59.000000 faucet-1.9.9/.dockerignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21210 2019-06-25 05:33:55.000000 faucet-1.9.9/ChangeLog
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2019-06-25 05:32:59.000000 faucet-1.9.9/Dockerfile.fuzz-packet
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      523 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/external_resources.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/recipe_book/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/recipe_book/policy.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/recipe_book/routing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/recipe_book/forwarding.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/recipe_book/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/tutorials/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19044 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/tutorials/first_time.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15605 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/tutorials/routing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8477 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/tutorials/vlans.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13123 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/tutorials/acls.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      115 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/tutorials/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17927 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/tutorials/nfv_services.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15004 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/developer_guide.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4828 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/architecture.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/noviflow/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3286 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/noviflow/README_noviflow.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/lagopus/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3638 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/lagopus/README_Lagopus.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/allied-telesis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14234 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/allied-telesis/README_Allied_Telesis.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/northboundnetworks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1661 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/northboundnetworks/README_ZodiacFX.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      605 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/northboundnetworks/README_ZodiacGX.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1292 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/northboundnetworks/conf-zodiac.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/ovs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18223 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/ovs/faucet_ovs_test.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6413 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/ovs/README_OVS-DPDK.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9332 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/cisco/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9521 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/cisco/README_Cisco.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      405 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/vendors/hpe/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17286 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/vendors/hpe/README_Aruba.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5281 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/intro.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34548 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/configuration.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7099 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/source/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1395 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/fuzzing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13916 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/installation.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/release_notes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3271 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/release_notes/1.9.0.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3303 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/release_notes/1.7.0.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3857 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/faq.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      308 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/autogen/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/autogen/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      930 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/monitoring.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/_static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/_static/deployments/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1106115 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/deployments/nznog17-virtual-network.jpg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89120 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/deployments/ONF_Faucet_deploy1.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   984943 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/deployments/nznog17-physical-network.jpg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/_static/css/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/css/responsive-tables.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/_static/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58351 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/faucet-pipeline.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2421 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/faucet-pipeline.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   172474 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/tutorial-vlans.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47652 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/tutorial-ivr.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)   452164 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/gauge-snapshot2.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51732 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/tutorial-acls.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23716 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/faucet-pipeline.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77255 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/tutorial-bgp-routing.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87114 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/tutorial-nfv-services.svg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8466 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/8021X-conf-diagram.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)   467326 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/gauge-snapshot3.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97737 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/faucet-architecture.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136689 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/gauge-nznog17.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    59007 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/tutorial-static-routing.svg
+-rw-rw-r--   0 travis    (2000) travis    (2000)   285918 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/images/gauge-snapshot1.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/_static/tutorial/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/tutorial/as_ns
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1086 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/tutorial/cleanup
+-rw-rw-r--   0 travis    (2000) travis    (2000)      425 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/tutorial/add_tagged_interface
+-rw-rw-r--   0 travis    (2000) travis    (2000)      409 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/tutorial/create_ns
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docs/_static/grafana-dashboards/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14739 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/grafana-dashboards/faucet_port_statistics.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18897 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/grafana-dashboards/faucet_instrumentation.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20170 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/_static/grafana-dashboards/faucet_inventory.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9402 2019-06-25 05:32:59.000000 faucet-1.9.9/docs/testing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      137 2019-06-25 05:32:59.000000 faucet-1.9.9/.codecov.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2019-06-25 05:32:59.000000 faucet-1.9.9/fuzz-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2019-06-25 05:32:59.000000 faucet-1.9.9/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/adapters/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/adapters/vendors/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/adapters/vendors/rabbitmq/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/adapters/vendors/rabbitmq/hooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/hooks/pre_build
+-rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/example_consumer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3473 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/test_rabbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      661 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/docker-compose-pi.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6854 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/rabbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      148 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/docker-compose-rabbitmq.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      733 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/Dockerfile.pi
+-rw-rw-r--   0 travis    (2000) travis    (2000)      655 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/docker-compose.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1636 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/vendors/rabbitmq/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-06-25 05:32:59.000000 faucet-1.9.9/adapters/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      830 2019-06-25 05:32:59.000000 faucet-1.9.9/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2233 2019-06-25 05:32:59.000000 faucet-1.9.9/docker-compose-pi.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      785 2019-06-25 05:33:55.000000 faucet-1.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-06-25 05:32:59.000000 faucet-1.9.9/Dockerfile.gauge
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      785 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/pbr.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7998 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2019-06-25 05:32:59.000000 faucet-1.9.9/Dockerfile.gauge.pi
+-rw-rw-r--   0 travis    (2000) travis    (2000)      220 2019-06-25 05:32:59.000000 faucet-1.9.9/Dockerfile.faucet.pi
+-rw-rw-r--   0 travis    (2000) travis    (2000)      178 2019-06-25 05:32:59.000000 faucet-1.9.9/test-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2538 2019-06-25 05:32:59.000000 faucet-1.9.9/Makefile
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/debian/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/watch
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/faucet-docs.docs
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/gauge.service
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      563 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/rules
+-rw-rw-r--   0 travis    (2000) travis    (2000)      216 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/gauge.default
+-rw-rw-r--   0 travis    (2000) travis    (2000)      135 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/changelog
+-rw-rw-r--   0 travis    (2000) travis    (2000)      905 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/copyright
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/compat
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3438 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/control
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/debian/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/source/format
+-rw-rw-r--   0 travis    (2000) travis    (2000)      204 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/faucet.install
+-rw-rw-r--   0 travis    (2000) travis    (2000)      224 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/faucet.default
+-rw-rw-r--   0 travis    (2000) travis    (2000)      421 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/faucet.service
+-rw-rw-r--   0 travis    (2000) travis    (2000)       35 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/gauge.install
+-rw-rw-r--   0 travis    (2000) travis    (2000)       54 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/faucet-all-in-one.install
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1035 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/faucet.postinst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1035 2019-06-25 05:32:59.000000 faucet-1.9.9/debian/gauge.postinst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/git-hook/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      456 2019-06-25 05:32:59.000000 faucet-1.9.9/git-hook/pre-commit
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/gitlab/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      971 2019-06-25 05:32:59.000000 faucet-1.9.9/gitlab/deploy_deb.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2019-06-25 05:32:59.000000 faucet-1.9.9/hw_switch_config.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/travis/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3188 2019-06-25 05:32:59.000000 faucet-1.9.9/travis/runtests.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/images/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/images/vm/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      462 2019-06-25 05:32:59.000000 faucet-1.9.9/images/vm/build-faucet-vm.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)       53 2019-06-25 05:32:59.000000 faucet-1.9.9/images/vm/.gitignore
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/images/vm/elements/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/images/vm/elements/faucet-all-in-one/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-06-25 05:32:59.000000 faucet-1.9.9/images/vm/elements/faucet-all-in-one/package-installs.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/images/vm/elements/faucet-all-in-one/install.d/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      924 2019-06-25 05:32:59.000000 faucet-1.9.9/images/vm/elements/faucet-all-in-one/install.d/02-install-faucet-gauge-prometheus-grafana
+-rw-rw-r--   0 travis    (2000) travis    (2000)      210 2019-06-25 05:32:59.000000 faucet-1.9.9/images/vm/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/images/raspbian/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      571 2019-06-25 05:32:59.000000 faucet-1.9.9/images/raspbian/02-run.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4863 2019-06-25 05:32:59.000000 faucet-1.9.9/images/raspbian/build.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2340 2019-06-25 05:32:59.000000 faucet-1.9.9/images/raspbian/prerun.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2300 2019-06-25 05:32:59.000000 faucet-1.9.9/images/raspbian/common
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2019-06-25 05:32:59.000000 faucet-1.9.9/Dockerfile.faucet
+-rw-rw-r--   0 travis    (2000) travis    (2000)      328 2019-06-25 05:32:59.000000 faucet-1.9.9/.renovaterc.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/etc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/etc/systemd/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/etc/systemd/system/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      355 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/systemd/system/prometheus.service
+-rw-rw-r--   0 travis    (2000) travis    (2000)      419 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/systemd/system/gauge.service
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/systemd/system/faucet.service
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/etc/prometheus/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/prometheus/faucet.rules.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      862 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/prometheus/prometheus.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/prometheus/prometheus-docker-compose.yml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/etc/logrotate.d/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      241 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/logrotate.d/gauge
+-rw-rw-r--   0 travis    (2000) travis    (2000)      243 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/logrotate.d/faucet
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/etc/default/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      215 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/default/gauge
+-rw-rw-r--   0 travis    (2000) travis    (2000)      223 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/default/faucet
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/etc/faucet/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2704 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/faucet/acls.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/faucet/ryu.conf
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2339 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/faucet/faucet.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      965 2019-06-25 05:32:59.000000 faucet-1.9.9/etc/faucet/gauge.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1100 2019-06-25 05:33:55.000000 faucet-1.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2320 2019-06-25 05:32:59.000000 faucet-1.9.9/.gitlab-ci.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2282 2019-06-25 05:32:59.000000 faucet-1.9.9/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      129 2019-06-25 05:32:59.000000 faucet-1.9.9/Dockerfile.tests
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2137 2019-06-25 05:32:59.000000 faucet-1.9.9/docker-compose.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10912 2019-06-25 05:32:59.000000 faucet-1.9.9/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/docker/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      595 2019-06-25 05:32:59.000000 faucet-1.9.9/docker/fuzz_packet.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3859 2019-06-25 05:32:59.000000 faucet-1.9.9/docker/runtests.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      576 2019-06-25 05:32:59.000000 faucet-1.9.9/docker/pip_deps.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      700 2019-06-25 05:32:59.000000 faucet-1.9.9/docker/install-faucet.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      594 2019-06-25 05:32:59.000000 faucet-1.9.9/docker/fuzz_config.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      834 2019-06-25 05:32:59.000000 faucet-1.9.9/docker/localtest.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      220 2019-06-25 05:32:59.000000 faucet-1.9.9/docker/retrycmd.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2019-06-25 05:32:59.000000 faucet-1.9.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      416 2019-06-25 05:32:59.000000 faucet-1.9.9/Dockerfile.fuzz-config
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3278 2019-06-25 05:32:59.000000 faucet-1.9.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/clib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4878 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/tcpdump_helper.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      538 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/clib_mininet_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24254 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/mininet_test_topo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7070 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/mininet_test_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110699 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/mininet_test_base.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    27264 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/clib_mininet_test_main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12771 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/docker_host.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6135 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/clib_mininet_tests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-06-25 05:32:59.000000 faucet-1.9.9/clib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/faucet/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/meter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3516 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/prom_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10474 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valves_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30904 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_of.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7274 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/gauge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6100 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/router.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17391 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_host.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    59022 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/dp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18174 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/acl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9696 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_table.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6427 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/watcher_conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5774 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/watcher.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6567 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/gauge_prom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9834 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8492 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_pipeline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9021 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23321 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/vlan.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11872 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/config_parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9508 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/gauge_influx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6037 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_util.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6087 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9829 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet_bgp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4503 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/tfm_pipeline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27542 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_packet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1032 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_manager_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      439 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7027 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet_pipeline.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7794 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/fctl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2853 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet_experimental_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5129 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet_event.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_of_old.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13435 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet_dot1x.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7538 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/config_parser_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7490 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_ryuapp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12902 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/faucet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40263 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_route.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9036 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/gauge_pollers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17167 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_acl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71402 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30088 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/valve_flood.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2269 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/check_faucet_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15024 2019-06-25 05:32:59.000000 faucet-1.9.9/faucet/port.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      530 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/run_unit_tests.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      244 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/sysctls_for_tests.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      427 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/run_integration_tests.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/fuzzer/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      706 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/fake_packet.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/fuzzer/dict/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/dict/packet.dict
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1572 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/dict/config.dict
+-rw-rw-r--   0 travis    (2000) travis    (2000)      878 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/fuzz_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1655 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/display_packet_crash.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/fuzzer/packet/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      277 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/dns.ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/tcp.ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      121 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/arp.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/udp.ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/diameter.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      465 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/http.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/msger.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/arp.ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2885 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/icmp.ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/asap.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      109 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/tcp.ex3
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/lacp.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/tcp.ex4
+-rw-rw-r--   0 travis    (2000) travis    (2000)      121 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/igmpv2.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      193 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/irc.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/icmp.ex3
+-rw-rw-r--   0 travis    (2000) travis    (2000)      121 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/udp.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      925 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/http.ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      381 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/ipv6.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/icmp.ex4
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/tcp.ex5
+-rw-rw-r--   0 travis    (2000) travis    (2000)      169 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/dns.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2021 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/ipv4.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      147 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/udp.ex4
+-rw-rw-r--   0 travis    (2000) travis    (2000)      933 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/icmp.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/tcp.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      311 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/irc.ex3
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/irc.ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/udp.ex3
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/aoe.ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/packet/asap.ex2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/fuzzer/config/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      179 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex6
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex11
+-rw-rw-r--   0 travis    (2000) travis    (2000)      219 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex9
+-rw-rw-r--   0 travis    (2000) travis    (2000)      585 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      303 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex14
+-rw-rw-r--   0 travis    (2000) travis    (2000)      412 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex5
+-rw-rw-r--   0 travis    (2000) travis    (2000)      188 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      783 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex10
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex12
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex7
+-rw-rw-r--   0 travis    (2000) travis    (2000)      531 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex8
+-rw-rw-r--   0 travis    (2000) travis    (2000)      360 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex4
+-rw-rw-r--   0 travis    (2000) travis    (2000)      222 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/config/ex3
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1543 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/fuzzer/fuzz_packet.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/codecheck/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      439 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/codecheck/pytype.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      200 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/codecheck/pylint.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      605 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/codecheck/min_pylint.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      340 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/codecheck/src_files.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/integration/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      502 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/integration/mininet_main.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2360 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/integration/experimental_api_test_app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   261309 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/integration/mininet_tests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/unit/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/unit/packaging/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4819 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/packaging/test_packaging.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/unit/gauge/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    35380 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/gauge/test_gauge.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4959 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/gauge/test_config_gauge.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1527 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/gauge/test_main.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/unit/clib/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4754 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/clib/test_topo.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-06-25 05:33:55.000000 faucet-1.9.9/tests/unit/faucet/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11277 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/test_check_config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1053 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/test_port.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8954 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/test_vlan.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18585 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/fakeoftable.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1530 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/test_main.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)   108358 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/test_valve.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    80659 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/test_config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6497 2019-06-25 05:32:59.000000 faucet-1.9.9/tests/unit/faucet/test_fctl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      193 2019-06-25 05:32:59.000000 faucet-1.9.9/.readthedocs.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      881 2019-06-25 05:33:55.000000 faucet-1.9.9/AUTHORS
```

### Comparing `faucet-1.9.8/ChangeLog` & `faucet-1.9.9/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,66 @@
 CHANGES
 =======
 
+1.9.9
+-----
+
+* self
+* Reauth test can fail if more attempts occur than the hard coded timeout expects
+* Making LACP resp rate configurable
+* Config unit test cases for lacp\_resp\_interval
+* config unit tests for LLDP src mac validation
+* Upgrade Chewie Version to 0.0.18
+* Change API between Chewie and Faucet to use KWARGS
+* FIX: Use acl\_manager directly instead of Valve inside Faucet\_Dot1x
+* Set :preserveSemverRanges for renovatebot
+* Bump README to 1.9.9
+* Update dependency pytype to v2019.6.21
+* Allow fixed or random ordering for port\_map
+* Update prom/prometheus Docker tag to v2.10.0
+* Simulated hardware switch also needs all IP functionality deconfigured
+* First pass at a "silence" sanity check; must hear no unexpected packets in test environment where all hosts are deconfigured
+* Remove debugging print()
+* set/type
+* Generate flowdel for potentially stale existing port specific flood rule
+* Update dependency prometheus\_client to v0.7.1
+* Update faucet/prometheus-pi Docker tag to v2.10.0
+* Update dependency sphinx to v2.1.2
+* Add missing :
+* Remove port out pcp
+* Should not fall through to default flood rule if stack port is not up
+* Move ARP loop test to standard stack test base
+* Make ARP test broadcast test more robust by testing both directions and ensure ARP cache cleared
+* Also check no leaked p=0
+* Move pcp set to vlan
+* Only test
+* pyup -> renovate
+* Configure .renovaterc.json
+* Add renovate.json
+* conf-zodiac.sh: set Zodiac and OF controller network details
+* FAUCET can send truncated ICMP6 echo replies
+* update grafana to 6.2.4
+* err -> out
+* Pin exabgp to 4.0.10
+* Update apt dependency for python3-prometheus-client
+* Update prometheus\_client from 0.6.0 to 0.7.0
+* Update sphinx from 2.1.0 to 2.1.1
+* Making LACP resp rate configurable
+* LLDP src validation
+* test\_topo.py tests clib rather than faucet
+* Simplify get\_config() in mininet\_tests.py
+
 1.9.8
 -----
 
 * Changing age calculation for LACP response
 * Fix LLDP redundant logging
 * Log error for types
 * Fix missing parsing of optional hw\_switch\_config.yaml parameters
+* setup 1.9.9
 * README 1.9.8
 * self.threads continually grows leading to high CPU. thread schedule jitter can be a float for better load distribution
 * Fix crash when optional include file does not exist
 
 1.9.7
 -----
 
@@ -156,18 +205,14 @@
 * Remove hard coding of string remote ports
 * one\_stack\_port\_down() handles offset
 * Remove unused port\_map\_rev
 * Incremental support for stack/offset port numbering
 * Verify empty caps is more verbose
 * Add offset for stacking
 * Fix two broken switch vendor URLs in the docs
-* Handle empty yaml\_conf
-* Add explicit switch start\_port
-* Remove diag prints
-* Remap function should actually only annotate
 * Set minimum performance bar at 100M
 * Mirror packets with consistent perspective based on mirrored port
 * Add mirror perf tests
 * Update pytype from 2019.4.12 to 2019.4.19
 * changed a few too many
 * event notif no longer experimental; closes #1312
 * fixes #2913
@@ -270,21 +315,14 @@
 * Update BGP docs for bgp dict
 * BGP sub-dict
 * Remove broken bgp\_neighbor aliases
 * Remove unused dp BGP attributes
 * set\_defaults() can set defaults for sub-dicts
 * Docs for routing tutorial
 * Docs for router
-* Re-enable BGP config checks for DP
-* pylint
-* Incremental bgp\_vlan to remove BGP entirely from VLANs
-* bgp\_vlans()
-* coldstart\_conf() needs to handle routers
-* Re order VLAN BGP attributes
-* Remove unused bgp\_local\_address
 * pytype
 * Should use yaml.safe\_load()
 * Remove dl\_dst output action from ACLs (which did not work anymore anyway)
 * Use relative time comparison profiling config parsing performance
 * Update pytype from 2019.3.8 to 2019.3.15
 * Prevent running faucet on python versions earlier than 3.5
 * Update apt package to require faucet versions 1.9+
@@ -354,39 +392,17 @@
 * Skip running a script to speed up pypi deploys
 * Move codechecks back inside docker
 * Run deploy build stage as python instead of the default (ruby)
 
 1.8.35
 ------
 
-* Optimize travis runs
-* Workaround ping -I behavior change, and add retries resolving down nexthops and comparing VLAN/port learn counters
-* Allow 8021x tests to work with freeradius 2 and 3
-* Run unit tests in parallel
-* Standardise parallel arguments
-* Default to python 3.6
-* exact mask check needs to check value is string
-* Handle OFAs that don't drop redundant exact masks from matches
-* pylint & pytype
-* 2to3 no longer needed
-* Don't need to explicitly install python-debian any longer
 * Preversion 1.8.36
-* Update control
 * README 1.8.35
-* port up not automatically called by StringDP based test. Need to defeat automatic hardware port remapping for TunnelTest
-* Update test-requirements.txt
-* Add SVG version of faucet-pipeline diagram
 * valve: add miss\_goto table to next\_tables label
-* Remove table numbers from pipeline diagram
-* Update prometheus\_client from 0.5.0 to 0.6.0
-* Update scapy from 2.4.0 to 2.4.2
-* valve: add next\_tables label to config\_table\_names
-* docs/developer\_guide: more files to copy
-* docs/architecture: remove table numbers
-* Correct non port 1-4 references in TunnelTest
 * check auth doesnt occur via wpa status and ping fail
 * pytype multiple syntax
 * pytype
 * Update test-requirements.txt
 * Update scapy from 2.4.0 to 2.4.2
 * Update pytype from 2019.1.30 to 2019.2.13
 * Update python-debian from 0.1.33 to 0.1.34
@@ -477,56 +493,28 @@
 * Upgrade to prometheus:v2.6.1 and grafana:5.4.3
 * Automatically lookup ubuntu/debian releases for CI package push
 * Kill even unhealthy controllers
 * Ensure \_start\_faucet() not multiply called
 * unintended array copy can cause hardware tests for stacking to fail due to using the wrong hardware ports
 * check\_config\_file should handle no file
 * Log print enhancement. 1.yaml format; 2.involve skipped cases; 3.involve sanity test results
-* ftctl should andle bad URL or content
-* Make ValvePipeline aware of hairpinning flag
 * Move port status handler to ValvesManager
 * Split up packet receive handler
-* update pika version; use alpine image for management
-* Upgrade to pytype 2019.1.18
-* Lack of explicit LACP down messages is confusing. Explicitly test flapping LACP
-* More tutorial tidyups
-* Add svg2pdfconverter so that SVGs can be rendered in LaTeX
-* Update faucet tutorial series for LCA2019
 * pylint
 * VLAN internal reservation
 * Valve tests with fakeOFtable
 * tunnel acl flowmods created by acl manager
 * pylint
 * Add Faucet port tunnel ACL implementation, packets from a port can be sent to a port on another DP via the tunnel path
 
 1.8.32
 ------
 
 * Preversion 1.8.33
 * README 1.8.32
-* Test that flows for newly added port are sent
-* Need to track op status for all ports the DP reports, even if they are not configured currently. The user might configure them later and we need their opstatus to decide whether to program flows for new ports
-* ping -> macvlan\_ping
-* Wrap net.ping() and net.pingAll() so they have reasonable timeouts (decrease test run time)
-* sphinx==1.8.3
-* Control dot1x acls using acl manager
-* Use acl\_manager to add and remove authed\_mac addresses
-* Include acl\_manager in valve members
-* use manager to install port acls
-* Use acl manager to install vlan acls
-* Create acl manager and use it to install dp acls
-* pytype upgrade to 2018.12.21
-* Explicitly explain that running hardware tests under virtualization is not supported
-* Use pipeline for accept instructions in acls
-
-1.8.31
-------
-
-* Preversion 1.8.32
-* Bump README
 * BUGFIX: Chewie port never comes back up
 * Include unit test to catch faulty instructions
 * change formatter for ports < 65535
 * Generate prometheus metric tables better
 * Need sphinx 1.8
 * Import new apidoc main()
 * Fix table overflow/wrapping issue in rtd theme with CSS
@@ -561,50 +549,20 @@
 * use pipeline for building goto instructions
 * add accept\_to\_classification function to ValvePipeline
 * Test VLAN PCP match and set
 * Upgrade docker images
 * Remove more Zodiac references
 * Prometheus metrics of type counter now end with \_total
 * Update packaging metadata
-* Enable group support for stacking
 * Remove ZodiacFX tests, which were never really used (and Zodiac switches now not commercially supported)
-* Mark groups and stacking together not yet supported
-* Flood manager should only send port specific rules, if those roles differ from broadcast rules
 * update supported EAP Types in docs
 * user port\_no# instead of hardcoded number
 * initialise egress\_table in ValvePipeline
 * move override output port initialising to ValveHostManager
-* include add\_port in ValveManagerBase
 * Tweak codecov settings
-* use self.port\_labels() instead of constructing dict by hand
-* debugging, reorder order of success checks
-* rename prometheus variable to match the best practice for counters
-* retry the prometheus poll 5 times
-* Notify Chewie of port status events
 * BUGFIX - Deny Port on 802.1x Failure
 * Hash config files for changes if stat didn't change
 * Preversion 1.8.29
 
 1.8.28
 ------
 
-* README 1.8.28
-* Update Vendor page for AT products
-* Remove more hardcoded port maps in 8021X tests
-* Remove hard coded port assignments in 802.1x
-* Mount /var/lib/docker on host to avoid docker-in-docker fs problems
-* Upgrade travis VM to xenial
-* port\_labels() needs to be smart enough to remap ports for hardware
-* Always use latest version of docker-ce
-* Move run-travis-test.sh to travis directory
-* pytype issue #133 is now fixed
-* Refresh grafana dashboards
-* pylint
-* Disable mirror port in group test which implicitly disables group mode
-* When flooding to a port that is being mirrored, the mirrored packet must not have a tag if the mirrored port is untagged
-* Require combinatorial flood rules when mirroring VLAN
-* pylint
-* stack ports must use "b" convention
-* Ports always begin with b
-* Use boilerplate config where possible
-* Update prometheus rules
-* Send CONFIG\_CHANGE success message
```

### Comparing `faucet-1.9.8/docs/external_resources.rst` & `faucet-1.9.9/docs/external_resources.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/tutorials/first_time.rst` & `faucet-1.9.9/docs/tutorials/first_time.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/tutorials/routing.rst` & `faucet-1.9.9/docs/tutorials/routing.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/tutorials/vlans.rst` & `faucet-1.9.9/docs/tutorials/vlans.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/tutorials/acls.rst` & `faucet-1.9.9/docs/tutorials/acls.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/tutorials/nfv_services.rst` & `faucet-1.9.9/docs/tutorials/nfv_services.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/developer_guide.rst` & `faucet-1.9.9/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/architecture.rst` & `faucet-1.9.9/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/noviflow/README_noviflow.rst` & `faucet-1.9.9/docs/vendors/noviflow/README_noviflow.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/lagopus/README_Lagopus.rst` & `faucet-1.9.9/docs/vendors/lagopus/README_Lagopus.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/allied-telesis/README_Allied_Telesis.rst` & `faucet-1.9.9/docs/vendors/allied-telesis/README_Allied_Telesis.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/northboundnetworks/README_ZodiacFX.rst` & `faucet-1.9.9/docs/vendors/northboundnetworks/README_ZodiacFX.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/northboundnetworks/README_ZodiacGX.rst` & `faucet-1.9.9/docs/vendors/northboundnetworks/README_ZodiacGX.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/ovs/faucet_ovs_test.png` & `faucet-1.9.9/docs/vendors/ovs/faucet_ovs_test.png`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/ovs/README_OVS-DPDK.rst` & `faucet-1.9.9/docs/vendors/ovs/README_OVS-DPDK.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst` & `faucet-1.9.9/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/cisco/README_Cisco.rst` & `faucet-1.9.9/docs/vendors/cisco/README_Cisco.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/vendors/hpe/README_Aruba.rst` & `faucet-1.9.9/docs/vendors/hpe/README_Aruba.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/intro.rst` & `faucet-1.9.9/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/Makefile` & `faucet-1.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/configuration.rst` & `faucet-1.9.9/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/conf.py` & `faucet-1.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/fuzzing.rst` & `faucet-1.9.9/docs/fuzzing.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/installation.rst` & `faucet-1.9.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/release_notes/1.9.0.rst` & `faucet-1.9.9/docs/release_notes/1.9.0.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/release_notes/1.7.0.rst` & `faucet-1.9.9/docs/release_notes/1.7.0.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/faq.rst` & `faucet-1.9.9/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/index.rst` & `faucet-1.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/monitoring.rst` & `faucet-1.9.9/docs/monitoring.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/deployments/nznog17-virtual-network.jpg` & `faucet-1.9.9/docs/_static/deployments/nznog17-virtual-network.jpg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/deployments/ONF_Faucet_deploy1.png` & `faucet-1.9.9/docs/_static/deployments/ONF_Faucet_deploy1.png`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/deployments/nznog17-physical-network.jpg` & `faucet-1.9.9/docs/_static/deployments/nznog17-physical-network.jpg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/faucet-pipeline.svg` & `faucet-1.9.9/docs/_static/images/faucet-pipeline.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/faucet-pipeline.txt` & `faucet-1.9.9/docs/_static/images/faucet-pipeline.txt`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/tutorial-vlans.svg` & `faucet-1.9.9/docs/_static/images/tutorial-vlans.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/tutorial-ivr.svg` & `faucet-1.9.9/docs/_static/images/tutorial-ivr.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/gauge-snapshot2.png` & `faucet-1.9.9/docs/_static/images/gauge-snapshot2.png`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/tutorial-acls.svg` & `faucet-1.9.9/docs/_static/images/tutorial-acls.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/faucet-pipeline.png` & `faucet-1.9.9/docs/_static/images/faucet-pipeline.png`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/tutorial-bgp-routing.svg` & `faucet-1.9.9/docs/_static/images/tutorial-bgp-routing.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/tutorial-nfv-services.svg` & `faucet-1.9.9/docs/_static/images/tutorial-nfv-services.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/8021X-conf-diagram.svg` & `faucet-1.9.9/docs/_static/images/8021X-conf-diagram.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/gauge-snapshot3.png` & `faucet-1.9.9/docs/_static/images/gauge-snapshot3.png`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/faucet-architecture.svg` & `faucet-1.9.9/docs/_static/images/faucet-architecture.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/gauge-nznog17.png` & `faucet-1.9.9/docs/_static/images/gauge-nznog17.png`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/tutorial-static-routing.svg` & `faucet-1.9.9/docs/_static/images/tutorial-static-routing.svg`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/images/gauge-snapshot1.png` & `faucet-1.9.9/docs/_static/images/gauge-snapshot1.png`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/tutorial/cleanup` & `faucet-1.9.9/docs/_static/tutorial/cleanup`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/grafana-dashboards/faucet_port_statistics.json` & `faucet-1.9.9/docs/_static/grafana-dashboards/faucet_port_statistics.json`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/grafana-dashboards/faucet_instrumentation.json` & `faucet-1.9.9/docs/_static/grafana-dashboards/faucet_instrumentation.json`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/_static/grafana-dashboards/faucet_inventory.json` & `faucet-1.9.9/docs/_static/grafana-dashboards/faucet_inventory.json`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docs/testing.rst` & `faucet-1.9.9/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/Dockerfile` & `faucet-1.9.9/adapters/vendors/rabbitmq/Dockerfile`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/example_consumer.py` & `faucet-1.9.9/adapters/vendors/rabbitmq/example_consumer.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/test_rabbit.py` & `faucet-1.9.9/adapters/vendors/rabbitmq/test_rabbit.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/docker-compose-pi.yaml` & `faucet-1.9.9/adapters/vendors/rabbitmq/docker-compose-pi.yaml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/rabbit.py` & `faucet-1.9.9/adapters/vendors/rabbitmq/rabbit.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/Dockerfile.pi` & `faucet-1.9.9/adapters/vendors/rabbitmq/Dockerfile.pi`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/docker-compose.yaml` & `faucet-1.9.9/adapters/vendors/rabbitmq/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/adapters/vendors/rabbitmq/README.rst` & `faucet-1.9.9/adapters/vendors/rabbitmq/README.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/CONTRIBUTING.rst` & `faucet-1.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docker-compose-pi.yaml` & `faucet-1.9.9/docker-compose-pi.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,29 @@
             INFLUXDB_INIT_PWD: 'faucet'
 
     prometheus:
         restart: always
         build:
             context: https://github.com/faucetsdn/docker-prometheus.git
             dockerfile: Dockerfile.pi
-        image: 'faucet/prometheus-pi:2.9.2'
+        image: 'faucet/prometheus-pi:2.10.0'
         user: 'root'
         ports:
             - '9090:9090'
         volumes:
             - '${FAUCET_PREFIX}/opt/prometheus/:/prometheus'
             - './etc/prometheus/prometheus-docker-compose.yml:/etc/prometheus/prometheus.yml'
             - './etc/prometheus/faucet.rules.yml:/etc/prometheus/faucet.rules.yml'
         links:
             - faucet
             - gauge
 
     grafana:
         restart: always
-        image: 'grafana/grafana-arm32v7-linux:6.2.0'
+        image: 'grafana/grafana-arm32v7-linux:6.2.4'
         user: 'root'
         ports:
             - '3000:3000'
         volumes:
             - '${FAUCET_PREFIX}/opt/grafana:/var/lib/grafana'
         links:
             - influxdb
```

### Comparing `faucet-1.9.8/PKG-INFO` & `faucet-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: faucet
-Version: 1.9.8
+Version: 1.9.9
 Summary: Faucet is an OpenFlow controller that implements a layer 2 and layer 3 switch.
 Home-page: https://faucet.nz
 Author: Faucet development team
 Author-email: faucet-dev@list.waikato.ac.nz
 License: Apache-2
 Description: UNKNOWN
 Keywords: openflow
```

### Comparing `faucet-1.9.8/faucet.egg-info/PKG-INFO` & `faucet-1.9.9/faucet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: faucet
-Version: 1.9.8
+Version: 1.9.9
 Summary: Faucet is an OpenFlow controller that implements a layer 2 and layer 3 switch.
 Home-page: https://faucet.nz
 Author: Faucet development team
 Author-email: faucet-dev@list.waikato.ac.nz
 License: Apache-2
 Description: UNKNOWN
 Keywords: openflow
```

### Comparing `faucet-1.9.8/faucet.egg-info/SOURCES.txt` & `faucet-1.9.9/faucet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .codecov.yml
 .dockerignore
 .gitlab-ci.yml
-.pyup.yml
 .readthedocs.yml
+.renovaterc.json
 .travis.yml
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 Dockerfile.faucet
 Dockerfile.faucet.pi
 Dockerfile.fuzz-config
@@ -271,14 +271,15 @@
 tests/fuzzer/packet/udp.ex1
 tests/fuzzer/packet/udp.ex2
 tests/fuzzer/packet/udp.ex3
 tests/fuzzer/packet/udp.ex4
 tests/integration/experimental_api_test_app.py
 tests/integration/mininet_main.py
 tests/integration/mininet_tests.py
+tests/unit/clib/test_topo.py
 tests/unit/faucet/fakeoftable.py
 tests/unit/faucet/test_check_config.py
 tests/unit/faucet/test_config.py
 tests/unit/faucet/test_fctl.py
 tests/unit/faucet/test_main.py
 tests/unit/faucet/test_port.py
 tests/unit/faucet/test_valve.py
```

### Comparing `faucet-1.9.8/Makefile` & `faucet-1.9.9/Makefile`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/debian/rules` & `faucet-1.9.9/debian/rules`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/debian/copyright` & `faucet-1.9.9/debian/copyright`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/debian/control` & `faucet-1.9.9/debian/control`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 Package: python3-faucet
 Architecture: all
 Depends: python3-oslo.config (>= 1:3.9~),
          python3-influxdb (>= 2.12.0),
          python3-msgpack (>= 0.4.2),
          python3-networkx (>= 1.9),
          python3-pbr (>= 1.9),
-         python3-prometheus-client (>= 0.6.0), python3-prometheus-client (<< 0.6.1),
+         python3-prometheus-client (>= 0.7.1), python3-prometheus-client (<< 0.7.2),
          python3-yaml (>= 3.1.1),
          python3-eventlet (>= 0.24.1), python3-eventlet (<< 0.24.2),
          python3-ryu (>= 4.32), python3-ryu (<< 4.33),
          python3-beka (>= 0.3.3), python3-beka (<< 0.3.4),
-         python3-chewie (>= 0.0.17), python3-chewie (<< 0.0.18),
+         python3-chewie (>= 0.0.18), python3-chewie (<< 0.0.19),
          python3-pytricia (>= 1.0.0),
          python3:any (>= 3.5~),
 Suggests: python-faucet-doc, faucet, gauge
 Description: source code for faucet and gauge (Python3)
  Python3 library that contains the source code for the Faucet open source
  OpenFlow controller, see faucet and gauge packages for further information.
  .
```

### Comparing `faucet-1.9.8/debian/faucet.postinst` & `faucet-1.9.9/debian/faucet.postinst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/debian/gauge.postinst` & `faucet-1.9.9/debian/gauge.postinst`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/gitlab/deploy_deb.sh` & `faucet-1.9.9/gitlab/deploy_deb.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/hw_switch_config.yaml` & `faucet-1.9.9/hw_switch_config.yaml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/travis/runtests.sh` & `faucet-1.9.9/travis/runtests.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/images/vm/elements/faucet-all-in-one/install.d/02-install-faucet-gauge-prometheus-grafana` & `faucet-1.9.9/images/vm/elements/faucet-all-in-one/install.d/02-install-faucet-gauge-prometheus-grafana`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/images/raspbian/02-run.sh` & `faucet-1.9.9/images/raspbian/02-run.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/images/raspbian/build.sh` & `faucet-1.9.9/images/raspbian/build.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/images/raspbian/prerun.sh` & `faucet-1.9.9/images/raspbian/prerun.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/images/raspbian/common` & `faucet-1.9.9/images/raspbian/common`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/etc/prometheus/faucet.rules.yml` & `faucet-1.9.9/etc/prometheus/faucet.rules.yml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/etc/prometheus/prometheus.yml` & `faucet-1.9.9/etc/prometheus/prometheus.yml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/etc/faucet/acls.yaml` & `faucet-1.9.9/etc/faucet/acls.yaml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/etc/faucet/faucet.yaml` & `faucet-1.9.9/etc/faucet/faucet.yaml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/etc/faucet/gauge.yaml` & `faucet-1.9.9/etc/faucet/gauge.yaml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/setup.cfg` & `faucet-1.9.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = faucet
-version = 1.9.8
+version = 1.9.9
 summary = Faucet is an OpenFlow controller that implements a layer 2 and layer 3 switch.
 license = Apache-2
 author = Faucet development team
 author-email = faucet-dev@list.waikato.ac.nz
 home-page = https://faucet.nz
 platform = any
 classifier =
```

### Comparing `faucet-1.9.8/.gitlab-ci.yml` & `faucet-1.9.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/.travis.yml` & `faucet-1.9.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docker-compose.yaml` & `faucet-1.9.9/docker-compose.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,29 @@
             INFLUXDB_DB: 'faucet'
             INFLUXDB_HTTP_AUTH_ENABLED: 'true'
             INFLUXDB_ADMIN_USER: 'faucet'
             INFLUXDB_ADMIN_PASSWORD: 'faucet'
 
     prometheus:
         restart: always
-        image: 'prom/prometheus:v2.9.2'
+        image: 'prom/prometheus:v2.10.0'
         user: 'root'
         ports:
             - '9090:9090'
         volumes:
             - '${FAUCET_PREFIX}/opt/prometheus/:/prometheus'
             - './etc/prometheus/prometheus-docker-compose.yml:/etc/prometheus/prometheus.yml'
             - './etc/prometheus/faucet.rules.yml:/etc/prometheus/faucet.rules.yml'
         links:
             - faucet
             - gauge
 
     grafana:
         restart: always
-        image: 'grafana/grafana:6.2.0'
+        image: 'grafana/grafana:6.2.4'
         user: 'root'
         ports:
             - '3000:3000'
         volumes:
             - '${FAUCET_PREFIX}/opt/grafana:/var/lib/grafana'
         links:
             - influxdb
```

### Comparing `faucet-1.9.8/LICENSE` & `faucet-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docker/fuzz_packet.sh` & `faucet-1.9.9/docker/fuzz_packet.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docker/runtests.sh` & `faucet-1.9.9/docker/runtests.sh`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DEPCHECK=1
 MINCOVERAGE=85
 
 set -e  # quit on error
 
 # allow user to skip parts of docker test
 # this wrapper script only cares about -n, -u, -i, others passed to test suite.
-while getopts "cdijknsux" o $FAUCET_TESTS; do
+while getopts "cdijknsuxo" o $FAUCET_TESTS; do
   case "${o}" in
         i)
             # run only integration tests
             UNITTESTS=0
             DEPCHECK=0
             ;;
         n)
@@ -109,14 +109,19 @@
   for p in `seq 2 5` ; do
     HWP="hwp$p"
     PHWP="p$HWP"
     ip link add dev $HWP type veth peer name $PHWP &&
       ifconfig $PHWP up &&
       ovs-vsctl add-port hwbr $PHWP -- set interface $PHWP ofport_request=$p ||
       exit 1
+    for i in $HWP $PHWP ; do
+      echo 1 > /proc/sys/net/ipv6/conf/$i/disable_ipv6
+      ip -4 addr flush dev $i
+      ip -6 addr flush dev $i
+    done
     DP_PORTS="  ${p}: ${HWP}${N}${DP_PORTS}"
   done
   cat > /tmp/hw_switch_config.yaml << EOL
 hw_switch: True
 hardware: 'Open vSwitch'
 of_port: 6653
 gauge_of_port: 6654
```

### Comparing `faucet-1.9.8/docker/install-faucet.sh` & `faucet-1.9.9/docker/install-faucet.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docker/fuzz_config.sh` & `faucet-1.9.9/docker/fuzz_config.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/docker/localtest.sh` & `faucet-1.9.9/docker/localtest.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/README.rst` & `faucet-1.9.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Faucet
 ======
 
-:version: 1.9.8
+:version: 1.9.9
 
 .. image:: https://travis-ci.com/faucetsdn/faucet.svg?branch=master
     :target: https://travis-ci.com/faucetsdn/faucet
 
 .. image:: https://codecov.io/gh/faucetsdn/faucet/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/faucetsdn/faucet
```

### Comparing `faucet-1.9.8/setup.py` & `faucet-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/clib/tcpdump_helper.py` & `faucet-1.9.9/clib/tcpdump_helper.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/clib/clib_mininet_test.py` & `faucet-1.9.9/clib/clib_mininet_test.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/clib/mininet_test_topo.py` & `faucet-1.9.9/clib/mininet_test_topo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Topology components for FAUCET Mininet unit tests."""
 
+from collections import namedtuple
 import os
 import socket
 import string
 import shutil
 import subprocess
 import time
 
@@ -18,14 +19,15 @@
 from mininet.node import OVSSwitch
 
 from clib import mininet_test_util
 
 
 # TODO: this should be configurable (e.g for randomization)
 SWITCH_START_PORT = 5
+HW_OFFSET = 16  # Must be > max(dp_ports)
 
 
 class FaucetHost(CPULimitedHost):
     """Base Mininet Host class, for Mininet-based tests."""
 
     pass
 
@@ -120,14 +122,20 @@
 
 class FaucetSwitchTopo(Topo):
     """FAUCET switch topology that contains a software switch."""
 
     CPUF = 0.5
     DELAY = '1ms'
 
+    def __init__(self, *args, **kwargs):
+        self.dpid_names = {}  # maps dpids to switch names
+        self.switch_dpids = {}  # maps switch names to dpids
+        self.switch_ports = {}  # maps switch names to port lists
+        super().__init__(*args, **kwargs)
+
     @staticmethod
     def _get_sid_prefix(ports_served):
         """Return a unique switch/host prefix for a test."""
         # Linux tools require short interface names.
         id_chars = ''.join(sorted(string.ascii_letters + string.digits)) # pytype: disable=module-attr
         id_a = int(ports_served / len(id_chars))
         id_b = ports_served - (id_a * len(id_chars))
@@ -149,66 +157,121 @@
         """Add a single extended test host."""
         host_name = 'e%s%1.1u' % (sid_prefix, host_n + 1)
         return self.addHost(name=host_name, cls=e_cls, host_n=host_n, tmpdir=tmpdir)
 
     def _add_faucet_switch(self, sid_prefix, dpid, hw_dpid, ovs_type):
         """Add a FAUCET switch."""
         switch_cls = FaucetSwitch
+        switch_name = 's%s' % sid_prefix
+        self.switch_dpids[switch_name] = dpid
+        self.dpid_names[dpid] = switch_name
         if hw_dpid and hw_dpid == dpid:
             remap_dpid = str(int(dpid) + 1)
-            output('bridging hardware switch DPID %s (%x) dataplane via OVS DPID %s (%x)' % (
+            output('bridging hardware switch DPID %s (%x) dataplane via OVS DPID %s (%x)\n' % (
                 dpid, int(dpid), remap_dpid, int(remap_dpid)))
             dpid = remap_dpid
             switch_cls = NoControllerFaucetSwitch
-        switch_name = 's%s' % sid_prefix
         return self.addSwitch(
             name=switch_name,
             cls=switch_cls,
             datapath=ovs_type,
             dpid=mininet_test_util.mininet_dpid(dpid))
 
-    def _add_links(self, switch, hosts, links_per_host, start_port):
-        port = start_port
+    # Hardware switch port virtualization through
+    # transparent OVS attachment bridge/patch panel
+    #
+    # Since FAUCET is talking to the hardware switch, it needs
+    # to use the hardware switch's OpenFlow ports, rather than
+    # the OpenFlow ports of the (transparent) OVS attachment bridge.
+
+    def hw_remap_port(self, dpid, port):
+        """Map OVS attachment bridge port number -> HW port number if necessary"""
+        if dpid != self.hw_dpid:
+            return port
+        assert self.hw_ports
+        return self.hw_ports[port - self.start_port]
+
+    peer_link = namedtuple('peer_link', 'port peer_dpid peer_port')
+
+    def hw_remap_peer_link(self, dpid, link):
+        """Remap HW port numbers -> OVS port numbers in link if necessary"""
+        port = self.hw_remap_port(dpid, link.port)
+        peer_port = self.hw_remap_port(link.peer_dpid, link.peer_port)
+        return self.peer_link(port, link.peer_dpid, peer_port)
+
+    def dpid_ports(self, dpid):
+        """Return port list for dpid, remapping if necessary"""
+        name = self.dpid_names[dpid]
+        ports = self.switch_ports[name]
+        return [self.hw_remap_port(dpid, port) for port in ports]
+
+    @staticmethod
+    def extend_port_order(port_order=None, max_length=16):
+        """Extend port_order to max_length if needed"""
+        if not port_order:
+            port_order = []
+        return port_order + list(range(len(port_order), max_length + 1))
+
+    def _add_links(self, switch, hosts, links_per_host):
+        self.switch_ports.setdefault(switch, [])
+        index = 0
         for host in hosts:
             for _ in range(links_per_host):
                 # Order of switch/host is important, since host may be in a container.
+                port = self.start_port + self.port_order[index]
                 self.addLink(switch, host, port1=port, delay=self.DELAY, use_htb=True)
-                port += 1
-        return port
+                # Keep track of switch ports
+                self.switch_ports.setdefault(switch, [])
+                self.switch_ports[switch].append(port)
+                index += 1
+        return index
 
     def build(self, ovs_type, ports_sock, test_name, dpids,
               n_tagged=0, tagged_vid=100, n_untagged=0, links_per_host=0,
-              n_extended=0, e_cls=None, tmpdir=None, hw_dpid=None,
-              host_namespace=None, start_port=SWITCH_START_PORT):
+              n_extended=0, e_cls=None, tmpdir=None, hw_dpid=None, switch_map=None,
+              host_namespace=None, start_port=SWITCH_START_PORT, port_order=None,
+              get_serialno=mininet_test_util.get_serialno):
         if not host_namespace:
             host_namespace = {}
-
+        self.hw_dpid = hw_dpid
+        self.hw_ports = sorted(switch_map) if switch_map else []
+        self.start_port = start_port
+        maxlength = n_tagged + n_untagged + n_extended
+        self.port_order = self.extend_port_order(port_order, maxlength)
         for dpid in dpids:
-            serialno = mininet_test_util.get_serialno(
-                ports_sock, test_name)
+            serialno = get_serialno(ports_sock, test_name)
             sid_prefix = self._get_sid_prefix(serialno)
-            for host_n in range(n_tagged):
-                self._add_tagged_host(sid_prefix, tagged_vid, host_n)
-            for host_n in range(n_untagged):
-                self._add_untagged_host(sid_prefix, host_n, host_namespace.get(host_n, True))
-            for host_n in range(n_extended):
-                self._add_extended_host(sid_prefix, host_n, e_cls, tmpdir)
+            tagged = [self._add_tagged_host(sid_prefix, tagged_vid, host_n)
+                      for host_n in range(n_tagged)]
+            untagged = [self._add_untagged_host(sid_prefix, host_n, host_namespace.get(host_n, True))
+                        for host_n in range(n_untagged)]
+            extended = [self._add_extended_host(sid_prefix, host_n, e_cls, tmpdir)
+                        for host_n in range(n_extended)]
             switch = self._add_faucet_switch(sid_prefix, dpid, hw_dpid, ovs_type)
-            self._add_links(switch, self.hosts(), links_per_host, start_port)
+            self._add_links(switch, tagged + untagged + extended, links_per_host)
 
 
 class FaucetStringOfDPSwitchTopo(FaucetSwitchTopo):
     """String of datapaths each with hosts with a single FAUCET controller."""
 
     switch_to_switch_links = 1
 
+    def dpid_peer_links(self, dpid):
+        """Return peer_link list for dpid, remapping if necessary"""
+        name = self.dpid_names[dpid]
+        links = [self.hw_remap_peer_link(dpid, link) for link in self.switch_peer_links[name]]
+        return links
+
     def build(self, ovs_type, ports_sock, test_name, dpids,
               n_tagged=0, tagged_vid=100, n_untagged=0,
               links_per_host=0, switch_to_switch_links=1,
-              hw_dpid=None, stack_ring=False, start_port=SWITCH_START_PORT):
+              hw_dpid=None, switch_map=None,
+              stack_ring=False, start_port=SWITCH_START_PORT,
+              port_order=None, get_serialno=mininet_test_util.get_serialno):
+
         """
 
                                Hosts
                                ||||
                                ||||
                  +----+       +----+       +----+
               ---+1   |       |1234|       |   1+---
@@ -226,44 +289,59 @@
         * s switches (above S = 3; for S > 3, switches are added to the chain)
         * (n_tagged + n_untagged) hosts per switch
         * (n_tagged + n_untagged + 1) links on switches 0 and s-1,
           with final link being inter-switch
         * (n_tagged + n_untagged + 2) links on switches 0 < n < s-1,
           with final two links being inter-switch
         """
-        def addLinks(src, dst, switch_ports): # pylint: disable=invalid-name
+        def addLinks(src, dst, next_index): # pylint: disable=invalid-name
+            """Add peer links from src switch to dst switch"""
+            self.switch_peer_links.setdefault(src, [])
+            self.switch_peer_links.setdefault(dst, [])
+            dpid1, dpid2 = self.switch_dpids[src], self.switch_dpids[dst]
             for _ in range(self.switch_to_switch_links):
-                self.addLink(src, dst, port1=switch_ports[src], port2=switch_ports[dst])
-                switch_ports[src] += 1
-                switch_ports[dst] += 1
-
-        first_switch = None
-        last_switch = None
+                index1, index2 = next_index[src], next_index[dst]
+                port1, port2 = [self.start_port + self.port_order[i] for i in (index1, index2)]
+                self.addLink(src, dst, port1=port1, port2=port2)
+                # Update port and link lists
+                self.switch_ports[src].append(port1)
+                self.switch_ports[dst].append(port2)
+                self.switch_peer_links[src].append(self.peer_link(port1, dpid2, port2))
+                self.switch_peer_links[dst].append(self.peer_link(port2, dpid1, port1))
+                # Update next indices on src and dest
+                next_index[src] += 1
+                next_index[dst] += 1
+
+        self.hw_dpid = hw_dpid
+        self.hw_ports = sorted(switch_map) if switch_map else []
+        self.start_port = start_port
         self.switch_to_switch_links = switch_to_switch_links
-        switch_ports = {}
+        max_ports = (n_tagged + n_untagged) * links_per_host + 2*switch_to_switch_links
+        self.port_order = self.extend_port_order(port_order, max_ports)
+        self.switch_peer_links = {}
+
+        first_switch, last_switch, next_index = None, None, {}
         for dpid in dpids:
-            serialno = mininet_test_util.get_serialno(
-                ports_sock, test_name)
+            serialno = get_serialno(ports_sock, test_name)
             sid_prefix = self._get_sid_prefix(serialno)
-            hosts = []
-            for host_n in range(n_tagged):
-                hosts.append(self._add_tagged_host(sid_prefix, tagged_vid, host_n))
-            for host_n in range(n_untagged):
-                hosts.append(self._add_untagged_host(sid_prefix, host_n))
+            tagged = [self._add_tagged_host(sid_prefix, tagged_vid, host_n)
+                      for host_n in range(n_tagged)]
+            untagged = [self._add_untagged_host(sid_prefix, host_n)
+                        for host_n in range(n_untagged)]
             switch = self._add_faucet_switch(sid_prefix, dpid, hw_dpid, ovs_type)
-            switch_ports[switch] = self._add_links(switch, hosts, links_per_host, start_port)
+            next_index[switch] = self._add_links(switch, tagged + untagged, links_per_host)
             if first_switch is None:
                 first_switch = switch
             else:
                 # Add a switch-to-switch link with the previous switch,
                 # if this isn't the first switch in the topology.
-                addLinks(last_switch, switch, switch_ports)
+                addLinks(last_switch, switch, next_index)
             last_switch = switch
         if stack_ring:
-            addLinks(first_switch, last_switch, switch_ports)
+            addLinks(first_switch, last_switch, next_index)
 
 
 class BaseFAUCET(Controller):
     """Base class for FAUCET and Gauge controllers."""
 
     # Set to True to have cProfile output to controller log.
     CPROFILE = False
```

### Comparing `faucet-1.9.8/clib/mininet_test_util.py` & `faucet-1.9.9/clib/mininet_test_util.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/clib/mininet_test_base.py` & `faucet-1.9.9/clib/mininet_test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,22 +115,21 @@
     cpn_ipv6 = False
     config_ports = {}
     env = collections.defaultdict(dict)
     rand_dpids = set()
     event_sock = None
     faucet_config_path = None
 
-    def __init__(self, name, config, root_tmpdir, ports_sock, max_test_load):
+    def __init__(self, name, config, root_tmpdir, ports_sock, max_test_load, port_order=None):
         super(FaucetTestBase, self).__init__(name)
         self.config = config
         self.root_tmpdir = root_tmpdir
         self.ports_sock = ports_sock
         self.max_test_load = max_test_load
-        start_port = mininet_test_topo.SWITCH_START_PORT
-        self.port_map = {'port_%u' % (port + 1): port + start_port for port in range(4)}
+        self.port_order = port_order
 
     def rand_dpid(self):
         reserved_range = 100
         while True:
             dpid = random.randint(1, (2**32 - reserved_range)) + reserved_range
             if dpid not in self.rand_dpids:
                 self.rand_dpids.add(dpid)
@@ -180,20 +179,15 @@
                 if 'ctl_privkey' in self.config:
                     self.ctl_privkey = self.config['ctl_privkey']
                 if 'ctl_cert' in self.config:
                     self.ctl_cert = self.config['ctl_cert']
                 if 'ca_certs' in self.config:
                     self.ca_certs = self.config['ca_certs']
                 dp_ports = self.config['dp_ports']
-                self.port_map = {}
-                self.switch_map = {}
-                for i, switch_port in enumerate(sorted(dp_ports), start=1):
-                    test_port_name = 'port_%u' % i
-                    self.port_map[test_port_name] = switch_port
-                    self.switch_map[test_port_name] = dp_ports[switch_port]
+                self.switch_map = dp_ports.copy()
 
     def _set_vars(self):
         self._set_prom_port()
         self._set_log_level()
 
     def _set_log_level(self, name='faucet'):
         self._set_var(name, 'FAUCET_LOG_LEVEL', str(self.LOG_LEVEL))
@@ -327,15 +321,17 @@
             for switch in self.net.switches:
                 switch.cmd('%s del-controller %s' % (self.VSCTL, switch.name))
             self.net.stop()
 
     def setUp(self):
         self.tmpdir = self._tmpdir_name()
         self._set_static_vars()
-        self.topo_class = mininet_test_topo.FaucetSwitchTopo
+        self.topo_class = partial(
+            mininet_test_topo.FaucetSwitchTopo, port_order=self.port_order,
+            switch_map=self.switch_map)
         if self.hw_switch:
             self.hw_dpid = mininet_test_util.str_int_dpid(self.dpid)
             self.dpid = self.hw_dpid
         else:
             self.dpid = self.rand_dpid()
 
     def hostns(self, host):
@@ -387,18 +383,17 @@
             oferrors,
             msg='log has OFPErrorMsgs: %s' % oferrors)
 
     def _attach_physical_switch(self):
         """Bridge a physical switch into test topology."""
         switch = self.net.switches[0]
         self.assertEqual('', switch.cmd('ebtables --f OUTPUT'))
-        mapped_base = max(len(self.switch_map), len(self.port_map))
         phys_macs = set()
-        for i, test_host_port in enumerate(sorted(self.switch_map)):
-            port_i = i + 1
+        mapped_base = len(self.switch_map)
+        for port_i, test_host_port in enumerate(sorted(self.switch_map), start=1):
             mapped_port_i = mapped_base + port_i
             phys_port = Intf(self.switch_map[test_host_port], node=switch)
             phys_mac = netifaces.ifaddresses(phys_port.name)[netifaces.AF_LINK][0]['addr']
             self.assertFalse(phys_mac in phys_macs, 'duplicate physical MAC %s' % phys_mac)
             phys_macs.add(phys_mac)
             for phys_cmd in (
                     'ip link set dev %s up' % phys_port,
@@ -418,21 +413,30 @@
             switch.cmd('%s add-flow %s in_port=%u,eth_dst=%s,priority=2,actions=drop' % (
                 self.OFCTL, switch.name, port_i, phys_mac))
             for port_pair in ((port_i, mapped_port_i), (mapped_port_i, port_i)):
                 in_port, out_port = port_pair
                 switch.cmd('%s add-flow %s in_port=%u,priority=1,actions=output:%u' % (
                     self.OFCTL, switch.name, in_port, out_port))
 
+    def create_port_map(self, dpid):
+        """Return a port map {'port_1': port...} for a dpid in self.topo"""
+        ports = self.topo.dpid_ports(dpid)
+        port_map = { 'port_%d' % i: port for i,  port in enumerate(ports, start=1)}
+        return port_map
+
     def start_net(self):
         """Start Mininet network."""
         controller_intf = 'lo'
         controller_ipv6 = False
         if self.hw_switch:
             controller_intf = self.cpn_intf
             controller_ipv6 = self.cpn_ipv6
+        if not self.port_map:
+            # Sometimes created in build_net for config purposes, sometimes not
+            self.port_map = self.create_port_map(self.dpid)
         self._start_faucet(controller_intf, controller_ipv6)
         self.pre_start_net()
         if self.hw_switch:
             self._attach_physical_switch()
         self._wait_debug_log()
         for port_no in self._dp_ports():
             self.set_port_up(port_no, wait=False)
@@ -1438,26 +1442,26 @@
                             hello_template % (unicast_mac1, unicast_mac2),
                             host.defaultIntf(),
                             count=3)))],
                 timeout=5, vflags='-vv', packets=1)
             self.verify_no_packets(tcpdump_txt)
 
     def verify_controller_fping(self, host, faucet_vip,
-                                total_packets=100, packet_interval_ms=100):
+                                total_packets=100, packet_interval_ms=100, size=64):
         fping_bin = 'fping'
         if faucet_vip.version == 6:
             fping_bin = 'fping6'
-        fping_cli = '%s -s -c %u -i %u -p 1 -T 1 %s' % (
-            fping_bin, total_packets, packet_interval_ms, faucet_vip.ip)
+        fping_cli = '%s -s -b %u -c %u -i %u -p 1 -T 1 %s' % (
+            fping_bin, size, total_packets, packet_interval_ms, faucet_vip.ip)
         timeout = int(((1000.0 / packet_interval_ms) * total_packets) * 1.5)
         fping_out = host.cmd(mininet_test_util.timeout_cmd(
             fping_cli, timeout))
         error('%s: %s' % (self._test_name(), fping_out))
         self.assertTrue(
-            not re.search(r'\s+0 ICMP Echo Replies received', fping_out),
+            re.search(r'\s+[1-9][0-9]* ICMP Echo Replies received', fping_out),
             msg=fping_out)
 
     def verify_learn_counters(self, vlan, ports, verify_neighbors=False):
         for _ in range(3):
             vlan_hosts_learned = self.scrape_prometheus_var(
                 'vlan_hosts_learned',
                 {'vlan': str(vlan)})
@@ -2184,39 +2188,39 @@
         first_host.setMAC(second_host_mac)
         second_host.setMAC(first_host_mac)
 
     def start_exabgp(self, exabgp_conf, timeout=30, log_prefix=''):
         """Start exabgp process on controller host."""
         exabgp_conf_file_name = os.path.join(self.tmpdir, '%sexabgp.conf' % log_prefix)
         exabgp_log = os.path.join(self.tmpdir, '%sexabgp.log' % log_prefix)
-        exabgp_err = os.path.join(self.tmpdir, '%sexabgp.err' % log_prefix)
+        exabgp_out = os.path.join(self.tmpdir, '%sexabgp.out' % log_prefix)
         exabgp_env = ' '.join((
             'exabgp.daemon.user=root',
             'exabgp.log.all=true',
             'exabgp.log.level=DEBUG',
             'exabgp.log.destination=%s' % exabgp_log,
         ))
         bgp_port = self.config_ports['bgp_port']
         exabgp_conf = exabgp_conf % {'bgp_port': bgp_port}
         with open(exabgp_conf_file_name, 'w') as exabgp_conf_file:
             exabgp_conf_file.write(exabgp_conf)
         controller = self._get_controller()
         # Ensure exabgp only attempts one connection.
         exabgp_cmd = mininet_test_util.timeout_cmd(
-            'exabgp %s --once -d 2> %s > /dev/null &' % (
-                exabgp_conf_file_name, exabgp_err), 300)
+            'exabgp %s --once -d 2>&1 > %s &' % (
+                exabgp_conf_file_name, exabgp_out), 300)
         exabgp_cli = 'env %s %s' % (exabgp_env, exabgp_cmd)
         controller.cmd(exabgp_cli)
         for _ in range(timeout):
             if os.path.exists(exabgp_log):
                 break
             time.sleep(1)
         self.assertTrue(
             os.path.exists(exabgp_log), msg='exabgp (%s) did not start' % exabgp_cli)
-        return (exabgp_log, exabgp_err)
+        return (exabgp_log, exabgp_out)
 
     def wait_bgp_up(self, neighbor, vlan, exabgp_log, exabgp_err):
         """Wait for BGP to come up."""
         label_values = {
             'neighbor': neighbor,
             'vlan': vlan,
         }
```

### Comparing `faucet-1.9.8/clib/clib_mininet_test_main.py` & `faucet-1.9.9/clib/clib_mininet_test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -206,21 +206,21 @@
             if version.parse(binary_version) < version.parse(binary_minversion):
                 print('%s version %s is less than required version %s' % (
                     required_binary, binary_version, binary_minversion))
                 return False
     return True
 
 
-def make_suite(tc_class, hw_config, root_tmpdir, ports_sock, max_test_load):
+def make_suite(tc_class, hw_config, root_tmpdir, ports_sock, max_test_load, port_order):
     """Compose test suite based on test class names."""
     testloader = unittest.TestLoader()
     testnames = testloader.getTestCaseNames(tc_class)
     suite = unittest.TestSuite()
     for name in testnames:
-        suite.addTest(tc_class(name, hw_config, root_tmpdir, ports_sock, max_test_load))
+        suite.addTest(tc_class(name, hw_config, root_tmpdir, ports_sock, max_test_load, port_order))
     return suite
 
 
 def pipeline_superset_report(decoded_pcap_logs):
     """Report on matches, instructions, and actions by table from tshark logs."""
 
     def parse_flow(flow_lines):
@@ -366,15 +366,15 @@
 
 
 def max_loadavg():
     return int(multiprocessing.cpu_count() * 1.5)
 
 
 def expand_tests(module, requested_test_classes, excluded_test_classes,
-                 hw_config, root_tmpdir, ports_sock, serial):
+                 hw_config, root_tmpdir, ports_sock, serial, port_order):
     sanity_test_suites = []
     single_test_suites = []
     parallel_test_suites = []
 
     for full_name, test_obj in inspect.getmembers(sys.modules[module]):
         test_name = full_name.split('.')[-1]
         if not inspect.isclass(test_obj):
@@ -384,15 +384,15 @@
         if excluded_test_classes and test_name in excluded_test_classes:
             continue
         if test_name.endswith('Test') and test_name.startswith('Faucet'):
             if not filter_test_hardware(test_obj, hw_config):
                 continue
             print('adding test %s' % test_name)
             test_suite = make_suite(
-                test_obj, hw_config, root_tmpdir, ports_sock, max_loadavg())
+                test_obj, hw_config, root_tmpdir, ports_sock, max_loadavg(), port_order)
             if test_name.startswith('FaucetSanity'):
                 sanity_test_suites.append(test_suite)
             else:
                 if serial or test_name.startswith('FaucetSingle') or test_obj.NETNS:
                     single_test_suites.append(test_suite)
                 else:
                     parallel_test_suites.append(test_suite)
@@ -591,15 +591,15 @@
                 for test_dir in test_dirs:
                     test_name = os.path.basename(test_dir)
                     if dumpfail:
                         dump_failed_test(test_name, test_dir)
 
 
 def run_tests(module, hw_config, requested_test_classes, dumpfail,
-              keep_logs, serial, excluded_test_classes, report_json_filename):
+              keep_logs, serial, excluded_test_classes, report_json_filename, port_order):
     """Actually run the test suites, potentially in parallel."""
     if hw_config is not None:
         print('Testing hardware, forcing test serialization')
         serial = True
     root_tmpdir = tempfile.mkdtemp(prefix='faucet-tests-', dir='/var/tmp')
     print('Logging test results in %s' % root_tmpdir)
     start_free_ports = 10
@@ -607,15 +607,15 @@
     if serial:
         start_free_ports = 5
         min_free_ports = 5
     ports_sock = start_port_server(root_tmpdir, start_free_ports, min_free_ports)
     print('test ports server started')
     sanity_tests, single_tests, parallel_tests = expand_tests(
         module, requested_test_classes, excluded_test_classes,
-        hw_config, root_tmpdir, ports_sock, serial)
+        hw_config, root_tmpdir, ports_sock, serial, port_order)
     resultclass = FaucetCleanupResult
     if keep_logs:
         resultclass = FaucetResult
     all_successful = False
     sanity_result = run_sanity_test_suite(root_tmpdir, resultclass, sanity_tests)
     if sanity_result.wasSuccessful():
         all_successful = run_test_suites(
@@ -644,57 +644,75 @@
     parser.add_argument(
         '-d', '--dumpfail', action='store_true', help='dump logs for failed tests')
     parser.add_argument(
         '-k', '--keep_logs', action='store_true', help='keep logs even for OK tests')
     parser.add_argument(
         '-n', '--nocheck', action='store_true', help='skip dependency check')
     parser.add_argument(
+        '-o', '--order', default='random',
+        help='port order for tests: 0,1,2,3 | random (default: random)')
+    parser.add_argument(
         '-i', '--integration', default=True, action='store_true', help='run integration tests')
     parser.add_argument(
         '-s', '--serial', action='store_true', help='run tests serially')
     parser.add_argument(
         '-j', '--jsonreport', help='write a json file with test results')
     parser.add_argument(
         '-x', help='list of test classes to exclude')
 
     excluded_test_classes = []
     report_json_filename = None
 
     try:
         args, requested_test_classes = parser.parse_known_args(sys.argv[1:])
-    except(KeyError, IndexError):
+        if args.order == 'random':
+            port_order = list(range(4))
+            random.shuffle(port_order)
+        else:
+            port_order = [int(s) for s in args.order.split(',')]
+        if sorted(port_order) != sorted(range(len(port_order))):
+            print('Port order should be a permutation of 0,1,2,3')
+            raise ValueError
+    except(KeyError, IndexError, ValueError):
         parser.print_usage()
         sys.exit(-1)
 
     if args.jsonreport:
         report_json_filename = args.jsonreport
     if args.x:
         excluded_test_classes = args.x.split(',')
+
+
     return (
         requested_test_classes, args.clean, args.dumpfail,
         args.keep_logs, args.nocheck, args.serial,
-        excluded_test_classes, report_json_filename)
+        excluded_test_classes, report_json_filename, port_order)
 
 
 def test_main(module):
     """Test main."""
     setLogLevel('error')
     print('testing module %s' % module)
+
     (requested_test_classes, clean, dumpfail, keep_logs, nocheck,
-     serial, excluded_test_classes, report_json_filename) = parse_args()
+     serial, excluded_test_classes, report_json_filename, port_order) = parse_args()
 
     if clean:
         print('Cleaning up test interfaces, processes and openvswitch '
               'configuration from previous test runs')
         Cleanup.cleanup()
         sys.exit(0)
+
     if nocheck:
         print('Skipping dependency checks')
     else:
         if not check_dependencies():
             print('dependency check failed. check required library/binary '
                   'list in header of this script')
             sys.exit(-1)
+
+    print("port order: -o", ','.join(str(i) for i in port_order))
+
     hw_config = import_hw_config()
     run_tests(
         module, hw_config, requested_test_classes, dumpfail,
-        keep_logs, serial, excluded_test_classes, report_json_filename)
+        keep_logs, serial, excluded_test_classes, report_json_filename, port_order)
```

### Comparing `faucet-1.9.8/clib/docker_host.py` & `faucet-1.9.9/clib/docker_host.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/clib/clib_mininet_tests.py` & `faucet-1.9.9/clib/clib_mininet_tests.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/meter.py` & `faucet-1.9.9/faucet/meter.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/prom_client.py` & `faucet-1.9.9/faucet/prom_client.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valves_manager.py` & `faucet-1.9.9/faucet/valves_manager.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_of.py` & `faucet-1.9.9/faucet/valve_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 MIN_VID = 1
 MAX_VID = 4095
 VLAN_GROUP_OFFSET = MAX_VID + 1
 ROUTE_GROUP_OFFSET = VLAN_GROUP_OFFSET * 2
 OFP_VERSIONS = [ofp.OFP_VERSION]
 OFP_IN_PORT = ofp.OFPP_IN_PORT
-MAX_PACKET_IN_BYTES = 128
+MAX_PACKET_IN_BYTES = 160 # largest packet is icmp6 echo.
 ECTP_ETH_TYPE = 0x9000
 
 OFERROR_TYPE_CODE = {
     0: ('OFPET_HELLO_FAILED', {
         ofp.OFPHFC_INCOMPATIBLE: 'OFPHFC_INCOMPATIBLE',
         ofp.OFPHFC_EPERM: 'OFPHFC_EPERM'}),
     1: ('OFPET_BAD_REQUEST', {
```

### Comparing `faucet-1.9.8/faucet/gauge.py` & `faucet-1.9.9/faucet/gauge.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/router.py` & `faucet-1.9.9/faucet/router.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_host.py` & `faucet-1.9.9/faucet/valve_host.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,20 +201,15 @@
             ofmsgs.extend(self.delete_host_from_vlan(eth_src, vlan))
 
         # Associate this MAC with source port.
         src_match = self.eth_src_table.match(
             in_port=port.number, vlan=vlan, eth_src=eth_src)
         src_priority = self.host_priority - 1
 
-        mark_port = self.has_externals and not port.stack
-
         inst = []
-        if mark_port:
-            vlan_pcp = 0 if port.loop_protect_external else 1
-            inst.append(valve_of.apply_actions([self.eth_src_table.set_field(vlan_pcp=vlan_pcp)]))
 
         if port.override_output_port:
             inst.append(valve_of.apply_actions([
                 valve_of.output_port(port.override_output_port.number)]))
         else:
             inst.append(self.eth_src_table.goto(self.output_table))
 
@@ -229,15 +224,15 @@
         # If we are refreshing only and not in hairpin mode, leave existing eth_dst alone.
         if refresh_rules and not hairpinning:
             return ofmsgs
 
         loop_protect_field = None
         if port.tagged_vlans and port.loop_protect_external and self.stack:
             loop_protect_field = 0
-        elif mark_port:
+        elif self.has_externals and not port.stack:
             loop_protect_field = 1
 
         # Output packets for this MAC to specified port.
         vlan_pcp = 1 if self.has_externals else None
         ofmsgs.append(self.eth_dst_table.flowmod(
             self.eth_dst_table.match(vlan=vlan, eth_dst=eth_src, vlan_pcp=vlan_pcp),
             priority=self.host_priority,
```

### Comparing `faucet-1.9.8/faucet/dp.py` & `faucet-1.9.9/faucet/dp.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/acl.py` & `faucet-1.9.9/faucet/acl.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_table.py` & `faucet-1.9.9/faucet/valve_table.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/watcher_conf.py` & `faucet-1.9.9/faucet/watcher_conf.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/watcher.py` & `faucet-1.9.9/faucet/watcher.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/gauge_prom.py` & `faucet-1.9.9/faucet/gauge_prom.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/faucet_metrics.py` & `faucet-1.9.9/faucet/faucet_metrics.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_pipeline.py` & `faucet-1.9.9/faucet/valve_pipeline.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/conf.py` & `faucet-1.9.9/faucet/conf.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/vlan.py` & `faucet-1.9.9/faucet/vlan.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/config_parser.py` & `faucet-1.9.9/faucet/config_parser.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/gauge_influx.py` & `faucet-1.9.9/faucet/gauge_influx.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_util.py` & `faucet-1.9.9/faucet/valve_util.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/__main__.py` & `faucet-1.9.9/faucet/__main__.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/faucet_bgp.py` & `faucet-1.9.9/faucet/faucet_bgp.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/tfm_pipeline.py` & `faucet-1.9.9/faucet/tfm_pipeline.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_packet.py` & `faucet-1.9.9/faucet/valve_packet.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_manager_base.py` & `faucet-1.9.9/faucet/valve_manager_base.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/faucet_pipeline.py` & `faucet-1.9.9/faucet/faucet_pipeline.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/fctl.py` & `faucet-1.9.9/faucet/fctl.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/faucet_experimental_api.py` & `faucet-1.9.9/faucet/faucet_experimental_api.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/faucet_event.py` & `faucet-1.9.9/faucet/faucet_event.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_of_old.py` & `faucet-1.9.9/faucet/valve_of_old.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/faucet_dot1x.py` & `faucet-1.9.9/faucet/faucet_dot1x.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,26 +102,28 @@
 
     def log_port_event(self, event_type, port_type, valve, port_num):
         """Log a dot1x port event"""
         valve.dot1x_event({event_type: {'dp_id': valve.dp.dp_id,
                                         'port': port_num,
                                         'port_type': port_type}})
 
-    def auth_handler(self, address, port_id, vlan_name, filter_id):
+    def auth_handler(self, address, port_id, *args, **kwargs):
         """Callback for when a successful auth happens."""
         address_str = str(address)
         valve, dot1x_port = self._get_valve_and_port(port_id)
         port_num = dot1x_port.number
 
         self.log_auth_event(valve, port_num, address_str, 'success')
-        flowmods = self._get_login_flowmod(dot1x_port, valve, address_str, vlan_name)
+        flowmods = self._get_login_flowmod(dot1x_port, valve, address_str,
+                                           kwargs.get('vlan_name', None))
 
         if flowmods:
             self._send_flow_msgs(valve, flowmods)
 
+
     def logoff_handler(self, address, port_id):
         """Callback for when an EAP logoff happens."""
         address_str = str(address)
         valve, dot1x_port = self._get_valve_and_port(port_id)
         port_num = dot1x_port.number
 
         self.log_auth_event(valve, port_num, address_str, 'logoff')
@@ -218,18 +220,19 @@
             dot1x_port (Port):
             nfv_sw_port (Port):
             valve (Valve):
 
         Returns:
             list
         """
+        acl_manager = valve.acl_manager
         if dot1x_port.running():
             valve_index = self.dp_id_to_valve_index[dp_id]
             mac = get_mac_str(valve_index, dot1x_port.number)
-            return valve.create_dot1x_flow_pair(
+            return acl_manager.create_dot1x_flow_pair(
                 dot1x_port.number, nfv_sw_port.number, mac)
         return []
 
     def port_down(self, dp_id, dot1x_port, nfv_sw_port):
         """
         Remove the acls added by FaucetDot1x.get_port_acls
         Args:
@@ -243,21 +246,22 @@
         valve_index = self.dp_id_to_valve_index[dp_id]
         port_num = dot1x_port.number
 
         mac = get_mac_str(valve_index, port_num)
         self._dot1x_speaker.port_down(mac)
 
         valve = self._valves[dp_id]
+        acl_manager = valve.acl_manager
         self.log_port_event("PORT_DOWN", 'supplicant', valve, port_num)
 
         flowmods = []
         flowmods.extend(self._del_authenticated_flowmod(dot1x_port, valve, mac))
         flowmods.extend(self._del_unauthenticated_flowmod(dot1x_port, valve))
         # NOTE: The flow_pair are not included in unauthed flowmod
-        flowmods.extend(valve.del_dot1x_flow_pair(dot1x_port.number, nfv_sw_port.number, mac))
+        flowmods.extend(acl_manager.del_dot1x_flow_pair(dot1x_port.number, nfv_sw_port.number, mac))
         return flowmods
 
     def reset(self, valves):
         """Set up a dot1x speaker."""
         self._valves = valves
         dot1x_valves = [
             valve for valve in valves.values() if valve.dp.dot1x and valve.dp.dot1x_ports()]
@@ -307,50 +311,57 @@
 
         return flowmods
 
     def _add_authenticated_flowmod(self, dot1x_port, valve, mac_str, vlan_name):
         """Return flowmods for successful authentication on port"""
         port_num = dot1x_port.number
         flowmods = []
+        acl_manager = valve.acl_manager
 
         if dot1x_port.dot1x_acl:
             auth_acl, _ = self._get_acls(valve.dp)
-            flowmods.extend(valve.add_port_acl(auth_acl, port_num, mac_str))
+            flowmods.extend(acl_manager.add_port_acl(auth_acl, port_num, mac_str))
         else:
-            flowmods.extend(valve.add_authed_mac(port_num, mac_str))
+            flowmods.extend(acl_manager.add_authed_mac(port_num, mac_str))
 
         if vlan_name:
             flowmods.extend(valve.add_dot1x_native_vlan(port_num, mac_str, vlan_name))
 
         return flowmods
 
     def _del_authenticated_flowmod(self, dot1x_port, valve, mac_str):
         """Return flowmods for deleting authentication flows from a port"""
         flowmods = []
         port_num = dot1x_port.number
+        acl_manager = valve.acl_manager
+
         if dot1x_port.dot1x_acl:
             auth_acl, _ = self._get_acls(valve.dp)
-            flowmods.extend(valve.del_port_acl(auth_acl, port_num, mac_str))
+            flowmods.extend(acl_manager.del_port_acl(auth_acl, port_num, mac_str))
         else:
-            flowmods.extend(valve.del_authed_mac(port_num, mac_str))
+            flowmods.extend(acl_manager.del_authed_mac(port_num, mac_str))
 
         flowmods.extend(valve.del_dot1x_native_vlan(port_num, mac_str))
 
         return flowmods
 
     def _add_unauthenticated_flowmod(self, dot1x_port, valve, mac_str=None):
         """Return flowmods default on a port"""
         flowmods = []
+        acl_manager = valve.acl_manager
+
         if dot1x_port.dot1x_acl:
             _, noauth_acl = self._get_acls(valve.dp)
-            flowmods.extend(valve.add_port_acl(noauth_acl, dot1x_port.number, mac_str))
+            flowmods.extend(acl_manager.add_port_acl(noauth_acl, dot1x_port.number, mac_str))
 
         return flowmods
 
     def _del_unauthenticated_flowmod(self, dot1x_port, valve, mac_str=None):
         """Return flowmods for deleting default / unauthenticated flows from a port"""
         flowmods = []
+        acl_manager = valve.acl_manager
+
         if dot1x_port.dot1x_acl:
             _, noauth_acl = self._get_acls(valve.dp)
-            flowmods.extend(valve.del_port_acl(noauth_acl, dot1x_port.number, mac_str))
+            flowmods.extend(acl_manager.del_port_acl(noauth_acl, dot1x_port.number, mac_str))
 
         return flowmods
```

### Comparing `faucet-1.9.8/faucet/config_parser_util.py` & `faucet-1.9.9/faucet/config_parser_util.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_ryuapp.py` & `faucet-1.9.9/faucet/valve_ryuapp.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/faucet.py` & `faucet-1.9.9/faucet/faucet.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_route.py` & `faucet-1.9.9/faucet/valve_route.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,15 +833,15 @@
     """Implement IPv6 FIB."""
 
     IPV = 6
     ETH_TYPE = valve_of.ether.ETH_TYPE_IPV6
     ICMP_TYPE = valve_of.inet.IPPROTO_ICMPV6
     CONTROL_ETH_TYPES = (valve_of.ether.ETH_TYPE_IPV6,) # type: ignore
     IP_PKT = ipv6.ipv6
-
+    ICMP6_ECHO_SIZE = 160
 
     @staticmethod
     def _gw_resolve_pkt():
         return valve_packet.nd_request
 
     @staticmethod
     def _gw_respond_pkt():
@@ -874,15 +874,15 @@
         ofmsgs.append(self.vip_table.flowcontroller(
             self.vip_table.match(
                 eth_type=self.ETH_TYPE,
                 eth_dst=vlan.faucet_mac,
                 nw_proto=valve_of.inet.IPPROTO_ICMPV6,
                 icmpv6_type=icmpv6.ICMPV6_ECHO_REQUEST),
             priority=priority,
-            max_len=self.ICMP_SIZE))
+            max_len=self.ICMP6_ECHO_SIZE))
         # IPv6 NA unicast to FAUCET.
         ofmsgs.append(self.vip_table.flowcontroller(
             self.vip_table.match(
                 eth_type=self.ETH_TYPE,
                 eth_dst=vlan.faucet_mac,
                 nw_proto=valve_of.inet.IPPROTO_ICMPV6,
                 icmpv6_type=icmpv6.ND_NEIGHBOR_ADVERT),
```

### Comparing `faucet-1.9.8/faucet/gauge_pollers.py` & `faucet-1.9.9/faucet/gauge_pollers.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve_acl.py` & `faucet-1.9.9/faucet/valve_acl.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/valve.py` & `faucet-1.9.9/faucet/valve.py`

 * *Files 2% similar despite different names*

```diff
@@ -649,17 +649,17 @@
         vlan_table = self.dp.tables['vlan']
         actions = copy.copy(mirror_act)
         match_vlan = vlan
         if push_vlan:
             actions.extend(valve_of.push_vlan_act(
                 vlan_table, vlan.vid))
             match_vlan = NullVLAN()
-        elif self.dp.stack and self.dp.stack.get('externals', False) and port.loop_protect_external:
-            # Ensure loop protection field cleared on external port.
-            actions.append(valve_of.set_field(**{STACK_LOOP_PROTECT_FIELD: 0}))
+        if vlan.loop_protect_external_ports():
+            vlan_pcp = 0 if port.loop_protect_external else 1
+            actions.append(valve_of.set_field(**{STACK_LOOP_PROTECT_FIELD: vlan_pcp}))
         inst = [
             valve_of.apply_actions(actions),
             vlan_table.goto(self._find_forwarding_table(vlan))]
         return vlan_table.flowmod(
             vlan_table.match(in_port=port.number, vlan=match_vlan),
             priority=self.dp.low_priority,
             inst=inst
@@ -955,16 +955,15 @@
                             pkt_meta.port.dyn_lacp_up, lacp_pkt.actor_state_synchronization,
                             lacp_pkt.actor_system, pkt_meta.port.lacp,
                             pkt_meta.log()))
                     if lacp_pkt.actor_state_synchronization:
                         ofmsgs_by_valve[self].extend(self.lacp_up(pkt_meta.port))
                     else:
                         ofmsgs_by_valve[self].extend(self.lacp_down(pkt_meta.port))
-                # TODO: make LACP response rate limit configurable.
-                if lacp_pkt_change or (age is not None and age > 1):
+                if lacp_pkt_change or (age is not None and age > self.dp.ports[pkt_meta.port.number].lacp_resp_interval):
                     ofmsgs_by_valve[self].extend(self._lacp_actions(lacp_pkt, pkt_meta.port, now))
                     pkt_meta.port.dyn_lacp_last_resp_time = now
                 pkt_meta.port.dyn_last_lacp_pkt = lacp_pkt
                 pkt_meta.port.dyn_lacp_updated_time = now
                 other_lag_ports = [
                     port for port in self.dp.ports.values()
                     if port.lacp == pkt_meta.port.lacp and port.dyn_last_lacp_pkt]
@@ -1024,26 +1023,30 @@
         if not lldp_pkt:
             return {}
 
         port = pkt_meta.port
         (remote_dp_id, remote_dp_name,
          remote_port_id, remote_port_state) = valve_packet.parse_faucet_lldp(
              lldp_pkt, self.dp.faucet_dp_mac)
-        
+
         port.dyn_lldp_beacon_recv_time = now
         if port.dyn_lldp_beacon_recv_state != remote_port_state:
             chassis_id = str(self.dp.faucet_dp_mac)
             if remote_port_state:
                 self.logger.info('LLDP on %s, %s from %s (remote %s, port %u) state %s' % (chassis_id, port, pkt_meta.eth_src, valve_util.dpid_log(remote_dp_id), remote_port_id, remote_port_state))
             port.dyn_lldp_beacon_recv_state = remote_port_state
 
+        peer_mac_src = self.dp.ports[port.number].lldp_peer_mac
+        if peer_mac_src and peer_mac_src != pkt_meta.eth_src:
+            self.logger.warning('Unexpected LLDP peer. Received pkt from %s instead of %s' % (pkt_meta.eth_src, peer_mac_src))
+        
         ofmsgs_by_valve = {}
         if remote_dp_id and remote_port_id:
-            self.logger.debug('FAUCET LLDP from %s (remote %s, port %u)' % (
-                pkt_meta.log(), valve_util.dpid_log(remote_dp_id), remote_port_id))
+            self.logger.debug('FAUCET LLDP on %s from %s (remote %s, port %u)' % (
+                port, pkt_meta.eth_src, valve_util.dpid_log(remote_dp_id), remote_port_id))
             ofmsgs_by_valve.update(self._verify_stack_lldp(
                 port, now, other_valves,
                 remote_dp_id, remote_dp_name,
                 remote_port_id, remote_port_state))
         else:
             self.logger.debug('LLDP on %s from %s: %s' % (port, pkt_meta.eth_src, str(lldp_pkt)))
         return ofmsgs_by_valve
@@ -1506,38 +1509,14 @@
             ofmsgs = []
         if restart_type is not None:
             self._inc_var('faucet_config_reload_%s' % restart_type)
             self.logger.info('%s starting' % restart_type)
         self._notify({'CONFIG_CHANGE': {'restart_type': restart_type}})
         return ofmsgs
 
-    def add_authed_mac(self, port_num, mac):
-        """Add authed mac address"""
-        # TODO: track dynamic auth state.
-        return self.acl_manager.add_authed_mac(port_num, mac)
-
-    def del_authed_mac(self, port_num, mac=None):
-        return self.acl_manager.del_authed_mac(port_num, mac)
-
-    def del_port_acl(self, acl, port_num, mac=None):
-        """Return ACL openflow rules for removing port with acl"""
-        return self.acl_manager.del_port_acl(acl, port_num, mac)
-
-    def add_port_acl(self, acl, port_num, mac=None):
-        """Return ACL openflow rules for port with acl"""
-        return self.acl_manager.add_port_acl(acl, port_num, mac)
-
-    def create_dot1x_flow_pair(self, port_num, nfv_sw_port_num, mac):
-        """Return flowmods for creating dot1x flow pair"""
-        return self.acl_manager.create_dot1x_flow_pair(port_num, nfv_sw_port_num, mac)
-
-    def del_dot1x_flow_pair(self, port_num, nfv_sw_port_num, mac):
-        """Return flowmods for deleting dot1x flow pair"""
-        return self.acl_manager.del_dot1x_flow_pair(port_num, nfv_sw_port_num, mac)
-
     def _del_native_vlan(self, port):
         vlan_table = self.dp.tables['vlan']
         ofmsg = vlan_table.flowdel(
             vlan_table.match(in_port=port.number, vlan=port.native_vlan),
             priority=self.dp.low_priority,
         )
         return [ofmsg]
```

### Comparing `faucet-1.9.8/faucet/valve_flood.py` & `faucet-1.9.9/faucet/valve_flood.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,59 +147,65 @@
         if port.dyn_phys_up:
             flood_acts = self._build_flood_rule_actions(
                 vlan, exclude_unicast, port, exclude_all_external)
             flood_acts, port_output_ports, port_non_output_acts = self._output_non_output_actions(
                 flood_acts)
         return (flood_acts, port_output_ports, port_non_output_acts)
 
-    def _build_flood_rule_for_port(self, vlan, eth_dst, eth_dst_mask, # pylint: disable=too-many-arguments
-                                   command, port, flood_acts, add_match=None):
-        ofmsgs = []
+    def _build_flood_match_priority(self, port, vlan, eth_dst, eth_dst_mask, add_match):
+        flood_priority = self._vlan_flood_priority(eth_dst_mask) + 1
         if add_match is None:
             add_match = {}
-        flood_priority = self._vlan_flood_priority(eth_dst_mask) + 1
         match = self.flood_table.match(
             vlan=vlan, in_port=port.number,
             eth_dst=eth_dst, eth_dst_mask=eth_dst_mask,
             **add_match)
-        ofmsgs = self._build_flood_rule(match, command, flood_acts, flood_priority)
-        return ofmsgs
+        return (flood_priority, match)
+
+    def _build_flood_rule_for_port(self, vlan, eth_dst, eth_dst_mask, # pylint: disable=too-many-arguments
+                                   command, port, flood_acts, add_match=None):
+        flood_priority, match = self._build_flood_match_priority(
+            port, vlan, eth_dst, eth_dst_mask, add_match)
+        return self._build_flood_rule(match, command, flood_acts, flood_priority)
 
     def _build_mask_flood_rules(self, vlan, eth_dst, eth_dst_mask, # pylint: disable=too-many-arguments
                                 exclude_unicast, command):
         ofmsgs = []
         if self.combinatorial_port_flood:
             for port in self._vlan_all_ports(vlan, exclude_unicast):
                 flood_acts, port_output_ports, _ = self._build_flood_acts_for_port(
                     vlan, exclude_unicast, port)
                 if port_output_ports:
-                    port_flood_ofmsg = self._build_flood_rule_for_port(
-                        vlan, eth_dst, eth_dst_mask, command, port, flood_acts)
-                    ofmsgs.append(port_flood_ofmsg)
+                    ofmsgs.append(self._build_flood_rule_for_port(
+                        vlan, eth_dst, eth_dst_mask, command, port, flood_acts))
         else:
             vlan_flood_ofmsg, vlan_flood_acts = self._build_flood_rule_for_vlan(
-                vlan, eth_dst, eth_dst_mask,
-                exclude_unicast, command)
+                vlan, eth_dst, eth_dst_mask, exclude_unicast, command)
             if not self.use_group_table:
                 ofmsgs.append(vlan_flood_ofmsg)
             flood_acts, vlan_output_ports, vlan_non_output_acts = self._output_non_output_actions(
                 vlan_flood_acts)
             for port in self._vlan_all_ports(vlan, exclude_unicast):
                 (flood_acts,
                  port_output_ports,
                  port_non_output_acts) = self._build_flood_acts_for_port(
                      vlan, exclude_unicast, port)
-                if port_output_ports:
-                    port_output_ports.add(port.number)
-                    if (vlan_output_ports == port_output_ports and
-                            vlan_non_output_acts == port_non_output_acts):
-                        continue
-                    port_flood_ofmsg = self._build_flood_rule_for_port(
-                        vlan, eth_dst, eth_dst_mask, command, port, flood_acts)
-                    ofmsgs.append(port_flood_ofmsg)
+                if not port_output_ports:
+                    continue
+                if (vlan_output_ports - set([port.number]) == port_output_ports
+                        and vlan_non_output_acts == port_non_output_acts):
+                    # Delete a potentially existing port specific flow
+                    # TODO: optimize, avoid generating delete for port if no existing flow.
+                    flood_priority, match = self._build_flood_match_priority(
+                        port, vlan, eth_dst, eth_dst_mask, add_match=None)
+                    ofmsgs.append(self.flood_table.flowdel(
+                        match=match, priority=flood_priority))
+                else:
+                    ofmsgs.append(self._build_flood_rule_for_port(
+                        vlan, eth_dst, eth_dst_mask, command, port, flood_acts))
         return ofmsgs
 
     def _build_multiout_flood_rules(self, vlan, command):
         """Build flooding rules for a VLAN without using groups."""
         ofmsgs = []
         for unicast_eth_dst, eth_dst, eth_dst_mask in self.FLOOD_DSTS:
             if unicast_eth_dst and not vlan.unicast_flood:
@@ -317,29 +323,29 @@
             port for port, port_peer_distance in port_peer_distances
             if port_peer_distance < my_root_distance]
         self.away_from_root_stack_ports = [
             port for port, port_peer_distance in port_peer_distances
             if port_peer_distance > my_root_distance]
         self.stack_size = self.stack.get('longest_path_to_root_len', None)
         self.externals = self.stack.get('externals', False)
-        self.ext_flood_needed = []
-        self.ext_flood_not_needed = []
+        self._set_ext_port_flag = []
+        self._set_nonext_port_flag = []
         if self.externals:
-            self.ext_flood_needed = [self._set_ext_flag(self.EXT_PORT_FLAG)]
-            self.ext_flood_not_needed = [self._set_ext_flag(self.NONEXT_PORT_FLAG)]
+            self._set_ext_port_flag = [self._set_ext_flag(self.EXT_PORT_FLAG)]
+            self._set_nonext_port_flag = [self._set_ext_flag(self.NONEXT_PORT_FLAG)]
 
     def _flood_actions_size2(self, in_port, external_ports,
                              away_flood_actions, toward_flood_actions, local_flood_actions):
         if not in_port or in_port in self.stack_ports:
             flood_prefix = []
         else:
             if in_port.loop_protect_external:
-                flood_prefix = self.ext_flood_not_needed
+                flood_prefix = self._set_nonext_port_flag
             else:
-                flood_prefix = self.ext_flood_needed
+                flood_prefix = self._set_ext_port_flag
 
         # Special case for stack with maximum distance 2 - we don't need to reflect off of the root.
         flood_actions = (
             flood_prefix + away_flood_actions + local_flood_actions)
 
         if self._dp_is_root():
             # Default strategy is flood locally and to non-roots.
@@ -368,57 +374,57 @@
         return flood_actions
 
     def _flood_actions(self, in_port, external_ports,
                        away_flood_actions, toward_flood_actions, local_flood_actions):
         # General case for stack with maximum distance > 2
         if self._dp_is_root():
             flood_actions = (
-                self.ext_flood_needed + away_flood_actions + local_flood_actions)
+                self._set_ext_port_flag + away_flood_actions + local_flood_actions)
 
             if in_port:
                 if in_port in self.away_from_root_stack_ports:
                     # Packet from a non-root switch, flood locally and to all non-root switches
                     # (reflect it).
                     flood_actions = (
                         away_flood_actions + [valve_of.output_in_port()] + local_flood_actions)
                     # If we have external ports, let the non-roots know they don't have to
                     # flood externally.
                     if external_ports:
-                        flood_actions = self.ext_flood_not_needed + flood_actions
+                        flood_actions = self._set_nonext_port_flag + flood_actions
                     else:
-                        flood_actions = self.ext_flood_needed + flood_actions
+                        flood_actions = self._set_ext_port_flag + flood_actions
                 elif external_ports:
                     # Packet from an external switch, locally. As above, let the non-roots
                     # know they don't have to flood externally again.
                     flood_actions = (
-                        self.ext_flood_not_needed + away_flood_actions + local_flood_actions)
+                        self._set_nonext_port_flag + away_flood_actions + local_flood_actions)
 
         else:
             # Default non-root strategy is flood towards root.
-            flood_actions = self.ext_flood_needed + toward_flood_actions
+            flood_actions = self._set_ext_port_flag + toward_flood_actions
 
             if in_port:
                 # Packet from switch further away, flood it to the root.
                 if in_port in self.away_from_root_stack_ports:
                     flood_actions = toward_flood_actions
                 # Packet from the root.
                 elif in_port in self.towards_root_stack_ports:
                     # If we have external ports, and packet hasn't already been flooded
                     # externally, flood it externally before passing it to further away switches,
                     # and mark it flooded.
                     if external_ports:
                         flood_actions = (
-                            self.ext_flood_not_needed + away_flood_actions + local_flood_actions)
+                            self._set_nonext_port_flag + away_flood_actions + local_flood_actions)
                     else:
                         flood_actions = (
-                            away_flood_actions + self.ext_flood_not_needed + local_flood_actions)
+                            away_flood_actions + self._set_nonext_port_flag + local_flood_actions)
                 # Packet from external port, locally. Mark it already flooded externally and
                 # flood to root (it came from an external switch so keep it within the stack).
                 elif in_port.loop_protect_external:
-                    flood_actions = self.ext_flood_not_needed + toward_flood_actions
+                    flood_actions = self._set_nonext_port_flag + toward_flood_actions
 
         return flood_actions
 
     def _build_flood_rule_actions(self, vlan, exclude_unicast, in_port, exclude_all_external=False):
         """Calculate flooding destinations based on this DP's position.
 
         If a standalone switch, then flood to local VLAN ports.
@@ -511,50 +517,47 @@
                 # If external flag is set, flood to external ports, otherwise exclude them.
                 for ext_port_flag, exclude_all_external in (
                         (self.NONEXT_PORT_FLAG, True),
                         (self.EXT_PORT_FLAG, False)):
                     flood_acts, port_output_ports, _ = self._build_flood_acts_for_port(
                         vlan, exclude_unicast, port, exclude_all_external=exclude_all_external)
                     if not port_output_ports:
-                        continue
+                        flood_acts = []
                     port_flood_ofmsg = self._build_flood_rule_for_port(
                         vlan, eth_dst, eth_dst_mask, command, port, flood_acts,
                         add_match={STACK_LOOP_PROTECT_FIELD: ext_port_flag})
                     ofmsgs.append(port_flood_ofmsg)
             else:
                 flood_acts, port_output_ports, _ = self._build_flood_acts_for_port(
                     vlan, exclude_unicast, port)
                 if not port_output_ports:
-                    continue
+                    flood_acts = []
                 port_flood_ofmsg = self._build_flood_rule_for_port(
                     vlan, eth_dst, eth_dst_mask, command, port, flood_acts)
                 ofmsgs.append(port_flood_ofmsg)
             if not self._dp_is_root():
                 # Drop bridge local traffic immediately.
                 bridge_local_match = {
                     'in_port': port.number,
                     'vlan': vlan,
                     'eth_dst': valve_packet.BRIDGE_GROUP_ADDRESS,
-                    'eth_dst_mask': valve_packet.BRIDGE_GROUP_MASK
-                    }
+                    'eth_dst_mask': valve_packet.BRIDGE_GROUP_MASK}
                 ofmsgs.extend(self.pipeline.filter_packets(
                     bridge_local_match, priority_offset=self.classification_offset))
                 # Because stacking uses reflected broadcasts from the root,
                 # don't try to learn broadcast sources from stacking ports.
                 if eth_dst is not None:
                     match = {
                         'in_port': port.number,
                         'vlan': vlan,
                         'eth_dst': eth_dst,
-                        'eth_dst_mask': eth_dst_mask
-                        }
+                        'eth_dst_mask': eth_dst_mask}
                     ofmsgs.extend(self.pipeline.select_packets(
                         self.flood_table, match,
-                        priority_offset=self.classification_offset
-                        ))
+                        priority_offset=self.classification_offset))
         return ofmsgs
 
     def _dp_is_root(self):
         """Return True if this datapath is the root of the stack."""
         return 'priority' in self.stack
 
     def _edge_dp_for_host(self, other_valves, pkt_meta):
```

### Comparing `faucet-1.9.8/faucet/check_faucet_config.py` & `faucet-1.9.9/faucet/check_faucet_config.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/faucet/port.py` & `faucet-1.9.9/faucet/port.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from faucet.conf import Conf, InvalidConfigError, test_config_condition
 from faucet import valve_of
+import netaddr
 
 STACK_STATE_ADMIN_DOWN = 0
 STACK_STATE_INIT = 1
 STACK_STATE_DOWN = 2
 STACK_STATE_UP = 3
 
 
@@ -56,26 +57,30 @@
         # if True, then switch unicast between hosts on this port (eg WiFi radio).
         'lacp': 0,
         # if non 0 (LAG ID), experimental LACP support enabled on this port.
         'lacp_active': False,
         # experimental active LACP
         'lacp_passthrough': None,
         # If set, fail the lacp on this port if any of the peer ports are down.
+        'lacp_resp_interval': 1,
+        # Min time since last LACP response. Used to control rate of responce for LACP
         'loop_protect': False,
         # if True, do simple (host/access port) loop protection on this port.
         'loop_protect_external': False,
         # if True, do external (other switch) loop protection on this port.
         'output_only': False,
         # if True, all packets input from this port are dropped.
         'lldp_beacon': {},
         # LLDP beacon configuration for this port.
         'opstatus_reconf': True,
         # If True, configure pipeline if operational status of port changes.
         'receive_lldp': False,
         # If True, receive LLDP on this port.
+        'lldp_peer_mac': None,
+        # If set, validates src MAC address of incoming LLDP packets
         'override_output_port': None,
         # If set, packets are sent to this other port.
         'max_lldp_lost': 3,
         # threshold before marking a stack port as down
         'dot1x': False,
         # If true, block this port until a successful 802.1x auth
         'dot1x_acl': False,
@@ -97,20 +102,22 @@
         'stack': dict,
         'max_hosts': int,
         'hairpin': bool,
         'hairpin_unicast': bool,
         'lacp': int,
         'lacp_active': bool,
         'lacp_passthrough': list,
+        'lacp_resp_interval': int,
         'loop_protect': bool,
         'loop_protect_external': bool,
         'output_only': bool,
         'lldp_beacon': dict,
         'opstatus_reconf': bool,
         'receive_lldp': bool,
+        'lldp_peer_mac': str,
         'override_output_port': (str, int),
         'dot1x': bool,
         'dot1x_acl': bool,
         'max_lldp_lost': int,
     }
 
     stack_defaults_types = {
@@ -140,28 +147,30 @@
         self.dp_id = None
         self.enabled = None
         self.hairpin = None
         self.hairpin_unicast = None
         self.lacp = None
         self.lacp_active = None
         self.lacp_passthrough = None
+        self.lacp_resp_interval = None
         self.loop_protect = None
         self.loop_protect_external = None
         self.max_hosts = None
         self.max_lldp_lost = None
         self.mirror = None
         self.name = None
         self.native_vlan = None
         self.number = None
         self.op_status_reconf = None
         self.opstatus_reconf = None
         self.output_only = None
         self.override_output_port = None
         self.permanent_learn = None
         self.receive_lldp = None
+        self.lldp_peer_mac = None
         self.stack = {}
         self.unicast_flood = None
 
         self.dyn_dot1x_native_vlan = None
         self.dyn_lacp_up = None
         self.dyn_lacp_updated_time = None
         self.dyn_lacp_last_resp_time = None
@@ -231,14 +240,20 @@
             for stack_config in list(self.stack_defaults_types.keys()):
                 test_config_condition(stack_config not in self.stack, (
                     'stack %s must be defined' % stack_config))
             # LLDP always enabled for stack ports.
             self.receive_lldp = True
             if not self.lldp_beacon_enabled():
                 self.lldp_beacon.update({'enable': True})
+        if self.lacp_resp_interval is not None:
+            test_config_condition(self.lacp_resp_interval > 65535 or self.lacp_resp_interval < 0.3, 
+                    ('interval must be atleast 0.3 and less than 65536'))
+        if self.lldp_peer_mac:
+            test_config_condition(not netaddr.valid_mac(self.lldp_peer_mac), (
+                'invalid MAC address %s' % self.lldp_peer_mac))
 
         if self.lldp_beacon:
             self._check_conf_types(
                 self.lldp_beacon, self.lldp_beacon_defaults_types)
             self.lldp_beacon = self._set_unknown_conf(
                 self.lldp_beacon, self.lldp_beacon_defaults_types)
             if self.lldp_beacon_enabled():
```

### Comparing `faucet-1.9.8/tests/run_unit_tests.sh` & `faucet-1.9.9/tests/run_unit_tests.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/fake_packet.py` & `faucet-1.9.9/tests/fuzzer/fake_packet.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/dict/config.dict` & `faucet-1.9.9/tests/fuzzer/dict/config.dict`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/fuzz_config.py` & `faucet-1.9.9/tests/fuzzer/fuzz_config.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/display_packet_crash.py` & `faucet-1.9.9/tests/fuzzer/display_packet_crash.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/packet/msger.ex1` & `faucet-1.9.9/tests/fuzzer/packet/msger.ex1`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/packet/icmp.ex2` & `faucet-1.9.9/tests/fuzzer/packet/icmp.ex2`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/packet/http.ex2` & `faucet-1.9.9/tests/fuzzer/packet/http.ex2`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/packet/ipv4.ex1` & `faucet-1.9.9/tests/fuzzer/packet/ipv4.ex1`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/packet/icmp.ex1` & `faucet-1.9.9/tests/fuzzer/packet/icmp.ex1`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/config/ex1` & `faucet-1.9.9/tests/fuzzer/config/ex1`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/config/ex10` & `faucet-1.9.9/tests/fuzzer/config/ex10`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/config/ex12` & `faucet-1.9.9/tests/fuzzer/config/ex12`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/config/ex8` & `faucet-1.9.9/tests/fuzzer/config/ex8`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/fuzzer/fuzz_packet.py` & `faucet-1.9.9/tests/fuzzer/fuzz_packet.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/codecheck/min_pylint.sh` & `faucet-1.9.9/tests/codecheck/min_pylint.sh`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/integration/experimental_api_test_app.py` & `faucet-1.9.9/tests/integration/experimental_api_test_app.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/integration/mininet_tests.py` & `faucet-1.9.9/tests/integration/mininet_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -814,22 +814,22 @@
         self.set_port_up(port_no1)
         self.wait_8021x_flows(port_no1)
         self.try_8021x(
             self.eapol1_host, port_no1, self.wpasupplicant_conf_1, and_logoff=False)
 
         self.wait_8021x_success_flows(self.eapol1_host, port_no1)
 
-        self.assertEqual(
-            1,
-            self.scrape_prometheus_var('port_dot1x_success_total', labels=port_labels1, default=0))
-        time.sleep(50)
-
-        self.assertEqual(
-            4,
-            self.scrape_prometheus_var('port_dot1x_success_total', labels=port_labels1, default=0))
+        for expected_total in range(1, 4):
+            for _ in range(self.SESSION_TIMEOUT * 2):
+                total = self.scrape_prometheus_var(
+                    'port_dot1x_success_total', labels=port_labels1, default=0)
+                if total == expected_total:
+                    break
+                time.sleep(1)
+            self.assertEquals(expected_total, total, msg='failed to successfully re-auth')
 
 
 class Faucet8021XConfigReloadTest(Faucet8021XBaseTest):
 
     def test_untagged(self):
         port_no1 = self.port_map['port_1']
         port_no2 = self.port_map['port_2']
@@ -1627,20 +1627,21 @@
         self.fail('DP port %u not healthy (%s)' % (dp_port, port_desc))
 
     def test_portmap(self):
         prom_desc = self.scrape_prometheus(
             controller='faucet', var='of_dp_desc_stats')
         self.assertIsNotNone(prom_desc, msg='Cannot scrape of_dp_desc_stats')
         error('DP: %s\n' % prom_desc[0])
-        for i, host in enumerate(self.net.hosts):
-            in_port = 'port_%u' % (i + 1)
+        error('port_map: %s\n' % self.port_map)
+        for i, host in enumerate(self.net.hosts, start=1):
+            in_port = 'port_%u' % i
             dp_port = self.port_map[in_port]
-            if in_port in self.switch_map:
+            if dp_port in self.switch_map:
                 error('verifying cabling for %s: host %s -> dp %u\n' % (
-                    in_port, self.switch_map[in_port], dp_port))
+                    in_port, self.switch_map[dp_port], dp_port))
             else:
                 error('verifying host %s -> dp %s\n' % (
                     in_port, dp_port))
             self.verify_dp_port_healthy(dp_port)
             self.require_host_learned(host, in_port=dp_port)
         learned = self.prom_macs_learned()
         self.assertEqual(
@@ -1661,14 +1662,28 @@
             listening_int = [line for line in ss_out if int_re.match(line)]
             self.assertFalse(
                 len(listening_int),
                 msg=(msg_template % '\n'.join(listening_int)))
         if listening_all:
             print('Warning: %s' % (msg_template % '\n'.join(listening_all)))
 
+    def test_silence(self):
+        # Make all test hosts silent and ensure we hear no other packets.
+        for host in self.net.hosts:
+            self.host_drop_all_ips(host)
+            host.cmd('echo 1 > /proc/sys/net/ipv6/conf/%s/disable_ipv6' % host.defaultIntf())
+        for host in self.net.hosts:
+            tcpdump_filter = ''
+            tcpdump_txt = self.tcpdump_helper(
+                host, tcpdump_filter, [], timeout=10, vflags='-vv', packets=1)
+            self.tcpdump_rx_packets(tcpdump_txt, 0)
+            self.assertTrue(
+                self.tcpdump_rx_packets(tcpdump_txt, 0),
+                msg='got unexpected packet from test switch: %s' % tcpdump_txt)
+
 
 class FaucetUntaggedPrometheusGaugeTest(FaucetUntaggedTest):
     """Testing Gauge Prometheus"""
 
     GAUGE_CONFIG_DBS = """
     prometheus:
         type: 'prometheus'
@@ -2435,15 +2450,15 @@
         cache_update_guard_time: 1
         idle_dst: False
 """ + CONFIG_BOILER_UNTAGGED
 
 
 class FaucetSingleL3LearnMACsOnPortTest(FaucetUntaggedTest):
 
-    # TODO: currently set to accomodate least hardware
+    # TODO: currently set to accommodate least hardware
     def _max_hosts():
         return 512
 
     MAX_HOSTS = _max_hosts()
     TEST_IPV4_NET = '10.0.0.0'
     TEST_IPV4_PREFIX = 16 # must hold more than MAX_HOSTS + 4
     LEARN_IPV4 = '10.0.254.254'
@@ -2484,15 +2499,15 @@
             '%s/%s' % (self.TEST_IPV4_NET, self.TEST_IPV4_PREFIX))
         learn_ip = ipaddress.IPv4Address(self.LEARN_IPV4)
         self.verify_learning(test_net, learn_ip, 64, self.MAX_HOSTS)
 
 
 class FaucetSingleL2LearnMACsOnPortTest(FaucetUntaggedTest):
 
-    # TODO: currently set to accomodate least hardware
+    # TODO: currently set to accommodate least hardware
     def _max_hosts():
         return 1024
 
     MAX_HOSTS = _max_hosts()
     TEST_IPV4_NET = '10.0.0.0'
     TEST_IPV4_PREFIX = 16 # must hold more than MAX_HOSTS + 4
     LEARN_IPV4 = '10.0.0.1'
@@ -5179,40 +5194,64 @@
         self.verify_broadcast()
         self.verify_no_bcast_to_self()
 
 
 class FaucetTaggedExtLoopProtectTest(FaucetTaggedTest):
 
 
+    CONFIG_GLOBAL = """
+acls:
+    pcp_force:
+        - rule:
+            vlan_vid: 100
+            actions:
+                output:
+                    set_fields:
+                        - vlan_pcp: 1
+                allow: 1
+"""
+
     CONFIG = """
         interfaces:
             %(port_1)d:
                 tagged_vlans: [100]
                 loop_protect_external: True
+                acl_in: pcp_force
             %(port_2)d:
                 tagged_vlans: [100]
                 loop_protect_external: True
             %(port_3)d:
                 tagged_vlans: [100]
             %(port_4)d:
                 tagged_vlans: [100]
 """
 
+    def _verify_link(self, hosts=None, expected=True):
+        from_port=hosts[0]
+        to_port=hosts[1]
+        tcpdump_filter = 'ether src %s' % from_port.MAC()
+        tcpdump_txt = self.tcpdump_helper(
+            to_port, tcpdump_filter, [
+                lambda: from_port.cmd(
+                    'ping -c3 %s' % to_port.IP())], root_intf=True, packets=2)
+        if expected:
+            self.assertTrue(re.search('vlan 100, p 1,', tcpdump_txt))
+            self.assertFalse(re.search('vlan 100, p 0,', tcpdump_txt))
+        else:
+            self.assertFalse(re.search('vlan 100,', tcpdump_txt))
+        self.verify_broadcast(hosts, expected)
+        self.verify_unicast(hosts, expected)
+
     def test_tagged(self):
         ext_port1, ext_port2, int_port1, int_port2 = self.net.hosts
-        self.verify_broadcast(hosts=(ext_port1, ext_port2), broadcast_expected=False)
-        self.verify_broadcast(hosts=(ext_port1, int_port1), broadcast_expected=True)
-        self.verify_broadcast(hosts=(int_port1, int_port2), broadcast_expected=True)
-        self.one_ipv4_ping(ext_port1, int_port2.IP())
-        tcpdump_filter = 'ether dst %s' % int_port2.MAC()
-        tcpdump_txt = self.tcpdump_helper(
-            ext_port1, tcpdump_filter, [
-                lambda: ext_port1.cmd(
-                    'ping -c3 %s' % int_port2.IP())], root_intf=True, packets=1)
-        self.assertTrue(re.search('vlan 100, p 0,', tcpdump_txt))
+        self._verify_link(hosts=(ext_port1, ext_port2), expected=False)
+        self._verify_link(hosts=(ext_port1, int_port2), expected=True)
+        self._verify_link(hosts=(ext_port2, int_port2), expected=True)
+        self._verify_link(hosts=(int_port1, ext_port2), expected=True)
+        self._verify_link(hosts=(int_port1, int_port2), expected=True)
 
 
 class FaucetTaggedWithUntaggedTest(FaucetTaggedTest):
 
     N_UNTAGGED = 0
     N_TAGGED = 4
     LINKS_PER_HOST = 1
@@ -6359,84 +6398,71 @@
     LINKS_PER_HOST = 1
     VID = 100
     CONFIG = None
     GROUP_TABLE = False
     dpids = None
     topo = None
 
-    def non_host_ports(self, dpid):
-        if self.NUM_DPS <= 2 and dpid == self.dpid:
-            min_non_host_ports = self.MAX_HOSTS - self.NUM_HOSTS
-            first_non_host_port = min_non_host_ports + 1
-            last_non_host_port = first_non_host_port + min_non_host_ports - 1
-            return [self.port_map['port_%u' % port]
-                    for port in range(first_non_host_port, last_non_host_port + 1)]
-        min_non_host_ports = 2
-        first_non_host_port = self.NUM_HOSTS + mininet_test_topo.SWITCH_START_PORT
-        last_non_host_port = first_non_host_port + min_non_host_ports - 1
-        return [port for port in range(first_non_host_port, last_non_host_port + 1)]
-
-    def hw_port_map_offset(self, port_no):
-        remap_port_no = (port_no - mininet_test_topo.SWITCH_START_PORT) + 1
-        return self.port_map['port_%u' % remap_port_no]
-
-    def hw_remap_all_ports(self, config):
-        return {self.hw_port_map_offset(port_no): config
-                for port_no, config in config.items()}
+    def non_host_links(self, dpid):
+        return self.topo.dpid_peer_links(dpid)
 
     @staticmethod
     def get_config_header(_config_global, _debug_log, _dpid, _hardware):
         """Don't generate standard config file header."""
         return ''
 
+    def acls(self):
+        return {}
+
+    def acl_in_dp(self):
+        return {}
+
     def build_net(self, stack=False, n_dps=1,
                   n_tagged=0, tagged_vid=100,
                   n_untagged=0, untagged_vid=100,
                   include=None, include_optional=None,
-                  acls=None, acl_in_dp=None,
                   switch_to_switch_links=1, hw_dpid=None,
                   stack_ring=False, lacp=False, use_external=False):
         """Set up Mininet and Faucet for the given topology."""
         if include is None:
             include = []
         if include_optional is None:
             include_optional = []
-        if acls is None:
-            acls = {}
-        if acl_in_dp is None:
-            acl_in_dp = {}
         self.dpids = [str(self.rand_dpid()) for _ in range(n_dps)]
         self.dpids[0] = self.dpid
         self.topo = mininet_test_topo.FaucetStringOfDPSwitchTopo(
             self.OVS_TYPE,
             self.ports_sock,
             dpids=self.dpids,
             n_tagged=n_tagged,
             tagged_vid=tagged_vid,
             n_untagged=n_untagged,
             links_per_host=self.LINKS_PER_HOST,
             switch_to_switch_links=switch_to_switch_links,
             test_name=self._test_name(),
-            hw_dpid=hw_dpid,
+            hw_dpid=hw_dpid, switch_map=self.switch_map,
             stack_ring=stack_ring,
+            port_order=self.port_order
         )
+        self.port_maps = {dpid: self.create_port_map(dpid) for dpid in self.dpids}
+        self.port_map = self.port_maps[self.dpid]
         self.CONFIG = self.get_config(
             self.dpids,
             hw_dpid,
             stack,
             self.hardware,
             self.debug_log_path,
             n_tagged,
             tagged_vid,
             n_untagged,
             untagged_vid,
             include,
             include_optional,
-            acls,
-            acl_in_dp,
+            self.acls(),
+            self.acl_in_dp(),
             stack_ring,
             lacp,
             use_external,
         )
 
     def get_config(self, dpids=None, hw_dpid=None, stack=False, hardware=None, ofchannel_log=None,
                    n_tagged=0, tagged_vid=0, n_untagged=0, untagged_vid=0,
@@ -6449,14 +6475,16 @@
             include = []
         if include_optional is None:
             include_optional = []
         if acls is None:
             acls = {}
         if acl_in_dp is None:
             acl_in_dp = {}
+        dpid_names = {}
+        dpname_to_dpkey = {}
 
         def dp_name(i):
             return 'faucet-%i' % (i + 1)
 
         def add_vlans(n_tagged, tagged_vid, n_untagged, untagged_vid):
             vlans_config = {}
             if n_untagged:
@@ -6471,171 +6499,128 @@
                 }
             return vlans_config
 
         def add_acl_to_port(name, port, interfaces_config):
             if name in acl_in_dp and port in acl_in_dp[name]:
                 interfaces_config[port]['acl_in'] = acl_in_dp[name][port]
 
-        def add_dp_to_dp_ports(name, dp_config, port, interfaces_config, i,
-                               dpid_count, stack, n_tagged, tagged_vid,
-                               n_untagged, untagged_vid):
-
-            # Add configuration for the switch-to-switch links
-            # (0 for a single switch, 1 for an end switch, 2 for middle switches).
-            first_dp = i == 0
-            second_dp = i == 1
-            last_dp = i == dpid_count - 1
-            end_dp = first_dp or last_dp
-            first_stack_port = port
-            peer_dps = []
-            if dpid_count > 1:
-                if end_dp:
-                    if first_dp:
-                        peer_dps = [i + 1]
-                    else:
-                        peer_dps = [i - 1]
+        def add_dp_to_dp_ports(name, dpid, dp_config, interfaces_config, stack,
+                               n_tagged, tagged_vid, n_untagged, untagged_vid):
+            for link in self.topo.dpid_peer_links(dpid):
+                port, peer_dpid, peer_port = link.port, link.peer_dpid, link.peer_port
+                interfaces_config[port] = {}
+                if stack:
+                    # make this a stacking link.
+                    interfaces_config[port].update(
+                        {
+                            'stack': {
+                                'dp': dpid_names[peer_dpid],
+                                'port': peer_port}
+                        })
                 else:
-                    peer_dps = [i - 1, i + 1]
+                    # not a stack - make this a trunk.
+                    tagged_vlans = []
+                    if n_tagged:
+                        tagged_vlans.append(tagged_vid)
+                    if n_untagged and untagged_vid not in tagged_vlans:
+                        tagged_vlans.append(untagged_vid)
+                    if tagged_vlans:
+                        interfaces_config[port]['tagged_vlans'] = tagged_vlans
+                    if lacp:
+                        interfaces_config[port].update(
+                            {'lacp': 1, 'lacp_active': True})
+                add_acl_to_port(name, port, interfaces_config)
 
-                if dpid_count > 2:
-                    if first_dp and stack and stack_ring:
-                        peer_dps.append(dpid_count - 1)
-                    if last_dp and stack and stack_ring:
-                        peer_dps.append(0)
-
-                # TODO: make per test configurable
-                dp_config['lacp_timeout'] = 10
-
-                # TODO: make the stacking root configurable
-                if stack and first_dp:
-                    dp_config['stack'] = {
-                        'priority': 1
-                    }
-                for peer_dp in peer_dps:
-                    if (dpid_count <= 2 or (first_dp and peer_dp != dpid_count - 1) or second_dp
-                            or (not end_dp and peer_dp > i)):
-                        peer_stack_port_base = first_stack_port
-                    else:
-                        peer_stack_port_base = first_stack_port + self.topo.switch_to_switch_links
-                    for stack_dp_port in range(self.topo.switch_to_switch_links):
-                        peer_port = peer_stack_port_base + stack_dp_port
-                        interfaces_config[port] = {}
-                        if stack:
-                            # make this a stacking link.
-                            interfaces_config[port].update(
-                                {
-                                    'stack': {
-                                        'dp': dp_name(peer_dp),
-                                        'port': peer_port}
-                                })
-                        else:
-                            # not a stack - make this a trunk.
-                            tagged_vlans = []
-                            if n_tagged and n_untagged and n_tagged != n_untagged:
-                                tagged_vlans = [tagged_vid, untagged_vid]
-                            elif ((n_tagged and not n_untagged) or
-                                  (n_tagged and n_untagged and tagged_vid == untagged_vid)):
-                                tagged_vlans = [tagged_vid]
-                            elif n_untagged and not n_tagged:
-                                tagged_vlans = [untagged_vid]
-                            if tagged_vlans:
-                                interfaces_config[port]['tagged_vlans'] = tagged_vlans
-                            if lacp:
-                                interfaces_config[port].update(
-                                    {'lacp': 1, 'lacp_active': True})
-                        add_acl_to_port(name, port, interfaces_config)
-                        port += 1
+            # TODO: make per test configurable
+            dp_config['lacp_timeout'] = 10
+
+            # TODO: make the stacking root configurable
+            first_dp = dpid == self.dpid
+            if stack and first_dp:
+                dp_config['stack'] = {
+                    'priority': 1
+                }
 
-        def add_dp(name, dpid, hw_dpid, i, dpid_count, stack,
+        def add_dp(name, dpid, hw_dpid, i, stack,
                    n_tagged, tagged_vid, n_untagged, untagged_vid,
-                   dpname_to_dpkey, use_external):
-            dpid_ofchannel_log = None
-            if ofchannel_log is not None:
-                dpid_ofchannel_log = ofchannel_log + str(i)
-            dp_hardware = hardware
-            if dpid != hw_dpid:
-                dp_hardware = 'Open vSwitch'
+                   use_external):
             dp_config = {
                 'dp_id': int(dpid),
-                'hardware': dp_hardware,
-                'ofchannel_log': dpid_ofchannel_log,
+                'hardware': hardware if dpid == hw_dpid else 'Open vSwitch',
+                'ofchannel_log': ofchannel_log + str(i) if ofchannel_log else None,
                 'interfaces': {},
                 'lldp_beacon': {'send_interval': 5, 'max_per_interval': 5},
                 'group_table': self.GROUP_TABLE,
             }
 
             interfaces_config = {}
-            port = mininet_test_topo.SWITCH_START_PORT
+            index = 1
 
-            for n_port in range(1, n_tagged + 1):
+            for n_port in range(n_tagged):
+                port = self.port_maps[dpid]['port_%d' % index]
                 interfaces_config[port] = {
                     'tagged_vlans': [tagged_vid],
-                    'loop_protect_external': (use_external and n_port < n_tagged),
+                    'loop_protect_external': (use_external and n_port != n_tagged - 1),
                 }
                 add_acl_to_port(name, port, interfaces_config)
-                port += 1
+                index += 1
 
-            for n_port in range(1, n_untagged + 1):
+            for n_port in range(n_untagged):
+                port = self.port_maps[dpid]['port_%d' % index]
                 interfaces_config[port] = {
                     'native_vlan': untagged_vid,
-                    'loop_protect_external': (use_external and n_port < n_untagged),
+                    'loop_protect_external': (use_external and n_port != n_untagged - 1),
                 }
                 add_acl_to_port(name, port, interfaces_config)
-                port += 1
+                index += 1
 
-            add_dp_to_dp_ports(
-                name, dp_config, port, interfaces_config, i, dpid_count, stack,
-                n_tagged, tagged_vid, n_untagged, untagged_vid)
+            add_dp_to_dp_ports(name, dpid, dp_config, interfaces_config, stack,
+                               n_tagged, tagged_vid, n_untagged, untagged_vid)
 
             for portno, config in list(interfaces_config.items()):
                 stack = config.get('stack', None)
                 if stack:
                     peer_dp = stack['dp']
                     peer_portno = stack['port']
-                    peer_dpid, _ = dpname_to_dpkey[peer_dp]
-                    if hw_dpid == peer_dpid:
-                        peer_portno = self.hw_port_map_offset(portno)
+                    peer_dpid = dpname_to_dpkey[peer_dp]
                     if 'stack' not in interfaces_config[portno]:
                         interfaces_config[portno]['stack'] = {}
                     interfaces_config[portno]['stack'].update({
                         'port': 'b%u' % peer_portno})
 
-            if hw_dpid == dpid:
-                interfaces_config = self.hw_remap_all_ports(interfaces_config)
-
             dp_config['interfaces'] = interfaces_config
-
             return dp_config
 
+
+        ### Create config
+
         config = {'version': 2}
 
         if include:
             config['include'] = list(include)
 
         if include_optional:
             config['include-optional'] = list(include_optional)
 
-        config['vlans'] = add_vlans(
-            n_tagged, tagged_vid, n_untagged, untagged_vid)
-
+        config['vlans'] = add_vlans(n_tagged, tagged_vid, n_untagged, untagged_vid)
         config['acls'] = acls.copy()
-
-        dpid_count = len(dpids)
         config['dps'] = {}
-        dpname_to_dpkey = {
-            dp_name(i): (dpid, i) for i, dpid in enumerate(dpids, start=0)}
 
-        for name, dpkey in dpname_to_dpkey.items():
-            dpid, i = dpkey
+        for i, dpid in enumerate(dpids):
+            dpid_names[dpid] = name = dp_name(i)
+            dpname_to_dpkey[name] = dpid
+
+        for i, dpid in enumerate(dpids):
+            name = dpid_names[dpid]
             config['dps'][name] = add_dp(
-                name, dpid, hw_dpid, i, dpid_count, stack,
+                name, dpid, hw_dpid, i, stack,
                 n_tagged, tagged_vid, n_untagged, untagged_vid,
-                dpname_to_dpkey, use_external)
-
-        return yaml.dump(config, default_flow_style=False)
+                use_external)
+        config_text = yaml.dump(config, default_flow_style=False)
+        return config_text
 
     def verify_no_cable_errors(self):
         i = 0
         for dpid in self.dpids:
             i += 1
             labels = {'dp_id': '0x%x' % int(dpid), 'dp_name': 'faucet-%u' % i}
             self.assertEqual(
@@ -6673,26 +6658,43 @@
                 default=None, dpid=False, timeout=timeout):
             self.fail('did not get expected dpid %x port %u port_stack_state %u' % (
                 int(dpid), port_no, status))
 
     def verify_all_stack_up(self):
         for i, dpid in enumerate(self.dpids, start=1):
             dp_name = 'faucet-%u' % i
-            for port_no in self.non_host_ports(dpid):
+            for link in self.non_host_links(dpid):
                 self.wait_for_stack_port_status(
-                    dpid, dp_name, port_no, 3) # up
+                    dpid, dp_name, link.port, 3) # up
+
+    def verify_stack_has_no_loop(self):
+        num_arp_expected = self.topo.switch_to_switch_links * 2
+        for ping_host, tcpdump_host in (
+                (self.net.hosts[0], self.net.hosts[-1]),
+                (self.net.hosts[-1], self.net.hosts[0])):
+            tcpdump_filter = 'arp and ether src %s' % ping_host.MAC()
+            tcpdump_txt = self.tcpdump_helper(
+                tcpdump_host, tcpdump_filter, [
+                    lambda: ping_host.cmd('arp -d %s' % tcpdump_host.IP()),
+                    lambda: ping_host.cmd('ping -c1 %s' % tcpdump_host.IP())],
+                packets=(num_arp_expected+1))
+            num_arp_received = len(re.findall(
+                'who-has %s tell %s' % (tcpdump_host.IP(), ping_host.IP()), tcpdump_txt))
+            self.assertTrue(num_arp_received)
+            self.assertLessEqual(num_arp_received, num_arp_expected)
 
     def verify_all_stack_hosts(self):
         for _ in range(2):
             self.verify_all_stack_up()
             self.verify_no_cable_errors()
             self.verify_stack_hosts()
             self.verify_traveling_dhcp_mac()
             self.verify_unicast_not_looped()
             self.verify_no_bcast_to_self()
+            self.verify_stack_has_no_loop()
             self.flap_all_switch_ports()
 
 
 class FaucetStringOfDPUntaggedTest(FaucetStringOfDPTest):
 
     NUM_DPS = 3
 
@@ -6737,16 +6739,16 @@
             n_tagged=self.NUM_HOSTS,
             tagged_vid=self.VID,
             switch_to_switch_links=2)
         self.start_net()
 
     def verify_one_stack_down(self, stack_offset_port, coldstart=False):
         self.retry_net_ping()
-        stack_port = self.non_host_ports(self.dpid)[stack_offset_port]
-        remote_stack_port = self.non_host_ports(self.dpids[1])[stack_offset_port]
+        stack_port = self.non_host_links(self.dpid)[stack_offset_port].port
+        remote_stack_port = self.non_host_links(self.dpid)[stack_offset_port].peer_port
         self.set_port_down(stack_port, wait=False)
         # self.dpids[1] is the intermediate switch.
         self.set_port_down(remote_stack_port, self.dpids[1], wait=False)
         # test case where one link is down when coldstarted.
         if coldstart:
             self.coldstart_conf()
         self.verify_stack_hosts(verify_bridge_local_rule=False)
@@ -6800,29 +6802,34 @@
 
     def wait_for_lacp_port_down(self, port_no, dpid, dp_name):
         self.wait_for_lacp_status(port_no, 0, dpid, dp_name)
 
     def wait_for_lacp_port_up(self, port_no, dpid, dp_name):
         self.wait_for_lacp_status(port_no, 1, dpid, dp_name)
 
+    # We sort non_host_links by port because FAUCET sorts its ports
+    # and only floods out of the first active LACP port in that list
+
     def wait_for_all_lacp_up(self):
-        first_lacp_port, second_lacp_port = self.non_host_ports(self.dpid)
-        remote_first_lacp_port = self.non_host_ports(self.dpids[1])[0]
+        first_link, second_link = sorted(self.non_host_links(self.dpid))
+        first_lacp_port, second_lacp_port = first_link.port, second_link.port
+        remote_first_lacp_port = first_link.peer_port
         self.wait_for_lacp_port_up(first_lacp_port, self.dpid, self.DP_NAME)
         self.wait_for_lacp_port_up(second_lacp_port, self.dpid, self.DP_NAME)
         self.wait_until_matching_flow(
             self.match_bcast, self._FLOOD_TABLE, actions=[self.action_str % first_lacp_port])
         self.wait_until_matching_flow(
             self.match_bcast, self._FLOOD_TABLE, actions=[self.action_str % remote_first_lacp_port],
             dpid=self.dpids[1])
 
     def test_lacp_port_down(self):
         """LACP to switch to a working port when the primary port fails."""
-        first_lacp_port, second_lacp_port = self.non_host_ports(self.dpid)
-        remote_first_lacp_port, remote_second_lacp_port = self.non_host_ports(self.dpids[1])
+        first_link, second_link = sorted(self.non_host_links(self.dpid))
+        first_lacp_port, second_lacp_port = first_link.port, second_link.port
+        remote_first_lacp_port, remote_second_lacp_port = first_link.peer_port, second_link.peer_port
         self.wait_for_all_lacp_up()
         self.retry_net_ping()
         self.set_port_down(first_lacp_port, wait=False)
         self.wait_for_lacp_port_down(first_lacp_port, self.dpid, self.DP_NAME)
         self.wait_for_lacp_port_down(remote_first_lacp_port, self.dpids[1], 'faucet-2')
         self.wait_until_matching_flow(
             self.match_bcast, self._FLOOD_TABLE, actions=[self.action_str % second_lacp_port])
@@ -6839,17 +6846,17 @@
             self.verify_stack_hosts()
             self.flap_all_switch_ports()
 
     def test_dyn_fail(self):
         """Test lacp fail on reload with dynamic lacp status."""
 
         conf = self._get_faucet_conf()
-        src_port = self.non_host_ports(self.dpids[0])[0]
-        dst_port = self.non_host_ports(self.dpids[0])[1]
-        fail_port = self.non_host_ports(self.dpids[1])[0]
+        first_link, second_link = sorted(self.non_host_links(self.dpid))
+        src_port, dst_port = first_link.port, second_link.port
+        fail_port = first_link.peer_port
 
         self.wait_for_lacp_port_up(src_port, self.dpids[0], 'faucet-1')
         self.wait_for_lacp_port_up(dst_port, self.dpids[0], 'faucet-1')
 
         conf['dps']['faucet-2']['interfaces'][fail_port]['lacp'] = 0
         conf['dps']['faucet-2']['interfaces'][fail_port]['lacp_active'] = False
         self.reload_conf(conf, self.faucet_config_path, restart=True,
@@ -6858,18 +6865,17 @@
         self.wait_for_lacp_port_down(src_port, self.dpids[0], 'faucet-1')
         self.wait_for_lacp_port_up(dst_port, self.dpids[0], 'faucet-1')
 
     def test_passthrough(self):
         """Test lacp passthrough on port fail."""
 
         conf = self._get_faucet_conf()
-        src_port = self.non_host_ports(self.dpids[0])[0]
-        dst_port = self.non_host_ports(self.dpids[0])[1]
-        fail_port = self.non_host_ports(self.dpids[1])[0]
-        end_port = self.non_host_ports(self.dpids[1])[1]
+        first_link, second_link = self.non_host_links(self.dpid)
+        src_port, dst_port = first_link.port, second_link.port
+        fail_port, end_port = first_link.peer_port, second_link.peer_port
 
         conf['dps']['faucet-1']['interfaces'][dst_port]['lacp_passthrough'] = [src_port]
         conf['dps']['faucet-1']['interfaces'][dst_port]['loop_protect_external'] = True
         conf['dps']['faucet-1']['interfaces'][dst_port]['lacp'] = 2
         conf['dps']['faucet-1']['interfaces'][src_port]['loop_protect_external'] = True
         conf['dps']['faucet-2']['interfaces'][fail_port]['loop_protect_external'] = True
         conf['dps']['faucet-2']['interfaces'][end_port]['loop_protect_external'] = True
@@ -6942,15 +6948,15 @@
         self._mark_external(False)
 
         # Part 3: Make sure things are the same after reload.
         self._connections_aye() # After reload
 
     def _mark_external(self, protect_external):
         conf = self._get_faucet_conf()
-        loop_port = self.non_host_ports(self.dpids[1])[0]
+        loop_port = self.non_host_links(self.dpids[1])[0].port
         conf['dps']['faucet-2']['interfaces'][loop_port]['loop_protect_external'] = protect_external
         self.reload_conf(
             conf, self.faucet_config_path,
             restart=True, cold_start=False, change_expected=True)
 
     def _verify_link(self, hosts=None, expected=True):
         self.verify_broadcast(hosts, expected)
@@ -7001,27 +7007,16 @@
             stack_ring=True)
         self.start_net()
         self.first_host = self.net.hosts[0]
         self.second_host = self.net.hosts[1]
         self.fifth_host = self.net.hosts[4]
         self.last_host = self.net.hosts[self.NUM_HOSTS * self.NUM_DPS - 1]
 
-    def verify_stack_has_no_loop(self):
-        tcpdump_filter = 'ether src %s' % self.first_host.MAC()
-        tcpdump_txt = self.tcpdump_helper(
-            self.first_host, tcpdump_filter, [
-                lambda: self.last_host.cmd('ping -c1 %s' % self.first_host.IP())],
-            packets=self.topo.switch_to_switch_links * 5)
-        num_arp_expected = self.topo.switch_to_switch_links * 2
-        num_arp_received = len(re.findall(
-            'who-has %s tell %s' % (self.first_host.IP(), self.last_host.IP()), tcpdump_txt))
-        self.assertLessEqual(num_arp_received, num_arp_expected)
-
     def one_stack_port_down(self):
-        port = self.non_host_ports(self.dpid)[1]
+        port = self.non_host_links(self.dpid)[1].port
         self.set_port_down(port, self.dpid)
         self.wait_for_stack_port_status(self.dpid, self.DP_NAME, port, 2) # down
 
     def test_untagged(self):
         """Stack loop prevention works and hosts can ping each others."""
         self.verify_all_stack_up()
         self.verify_stack_has_no_loop()
@@ -7042,56 +7037,58 @@
 
 class FaucetSingleStackAclControlTest(FaucetStringOfDPTest):
     """Test ACL control of stacked datapaths with untagged hosts."""
 
     NUM_DPS = 3
     NUM_HOSTS = 3
 
-    ACLS = {
+    def acls(self):
+        map1, map2, map3 = [self.port_maps[dpid] for dpid in self.dpids]
+        return {
         1: [
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'nw_dst': '10.0.0.2',
                 'actions': {
                     'output': {
-                        'port': mininet_test_topo.SWITCH_START_PORT + 1
+                        'port': map1['port_2']
                     }
                 },
             }},
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'dl_dst': 'ff:ff:ff:ff:ff:ff',
                 'actions': {
                     'output': {
                         'ports': [
-                            mininet_test_topo.SWITCH_START_PORT + 1,
-                            mininet_test_topo.SWITCH_START_PORT + 3]
+                            map1['port_2'],
+                            map1['port_4']]
                     }
                 },
             }},
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'actions': {
                     'output': {
-                        'port': mininet_test_topo.SWITCH_START_PORT + 3
+                        'port': map1['port_4']
                     }
                 },
             }},
             {'rule': {
                 'actions': {
                     'allow': 1,
                 },
             }},
         ],
         2: [
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'actions': {
                     'output': {
-                        'port': mininet_test_topo.SWITCH_START_PORT + 4
+                        'port': map2['port_5']
                     }
                 },
             }},
             {'rule': {
                 'actions': {
                     'allow': 1,
                 },
@@ -7099,24 +7096,24 @@
         ],
         3: [
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'nw_dst': '10.0.0.7',
                 'actions': {
                     'output': {
-                        'port': mininet_test_topo.SWITCH_START_PORT
+                        'port': map3['port_1']
                     }
                 },
             }},
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'dl_dst': 'ff:ff:ff:ff:ff:ff',
                 'actions': {
                     'output': {
-                        'ports': [mininet_test_topo.SWITCH_START_PORT]
+                        'ports': [map3['port_1']]
                     }
                 },
             }},
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'actions': {
                     'allow': 0,
@@ -7127,38 +7124,38 @@
                     'allow': 1,
                 },
             }},
         ],
     }
 
     # DP-to-acl_in port mapping.
-    ACL_IN_DP = {
+    def acl_in_dp(self):
+        map1, map2, map3 = [self.port_maps[dpid] for dpid in self.dpids]
+        return {
         'faucet-1': {
             # Port 1, acl_in = 1
-            mininet_test_topo.SWITCH_START_PORT: 1,
+            map1['port_1']: 1,
         },
         'faucet-2': {
             # Port 4, acl_in = 2
-            mininet_test_topo.SWITCH_START_PORT + 3: 2,
+            map2['port_4']: 2,
         },
         'faucet-3': {
             # Port 4, acl_in = 3
-            mininet_test_topo.SWITCH_START_PORT + 3: 3,
+            map3['port_4']: 3,
         },
     }
 
     def setUp(self): # pylint: disable=invalid-name
         super(FaucetSingleStackAclControlTest, self).setUp()
         self.build_net(
             stack=True,
             n_dps=self.NUM_DPS,
             n_untagged=self.NUM_HOSTS,
             untagged_vid=self.VID,
-            acls=self.ACLS,
-            acl_in_dp=self.ACL_IN_DP,
             )
         self.start_net()
 
     def test_unicast(self):
         """Hosts in stack topology can appropriately reach each other over unicast."""
         hosts = self.net.hosts
         self.verify_tp_dst_notblocked(5000, hosts[0], hosts[1], table_id=None)
@@ -7179,15 +7176,16 @@
 
 class FaucetStringOfDPACLOverrideTest(FaucetStringOfDPTest):
 
     NUM_DPS = 1
     NUM_HOSTS = 2
 
     # ACL rules which will get overridden.
-    ACLS = {
+    def acls(self):
+        return {
         1: [
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'ip_proto': 6,
                 'tcp_dst': 5001,
                 'actions': {
                     'allow': 1,
@@ -7207,15 +7205,16 @@
                 },
             }},
         ],
     }
 
     # ACL rules which get put into an include-optional
     # file, then reloaded into FAUCET.
-    ACLS_OVERRIDE = {
+    def acls_override(self):
+        return {
         1: [
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'ip_proto': 6,
                 'tcp_dst': 5001,
                 'actions': {
                     'allow': 0,
@@ -7234,65 +7233,67 @@
                     'allow': 1,
                 },
             }},
         ],
     }
 
     # DP-to-acl_in port mapping.
-    ACL_IN_DP = {
+    def acl_in_dp(self):
+        port_1 = self.port_map['port_1']
+        return {
         'faucet-1': {
             # First port, acl_in = 1
-            mininet_test_topo.SWITCH_START_PORT: 1,
+            port_1: 1,
         },
     }
 
     def setUp(self): # pylint: disable=invalid-name
         super(FaucetStringOfDPACLOverrideTest, self).setUp()
         self.acls_config = os.path.join(self.tmpdir, 'acls.yaml')
         missing_config = os.path.join(self.tmpdir, 'missing_config.yaml')
         self.build_net(
             n_dps=self.NUM_DPS,
             n_untagged=self.NUM_HOSTS,
             untagged_vid=self.VID,
             include_optional=[self.acls_config, missing_config],
-            acls=self.ACLS,
-            acl_in_dp=self.ACL_IN_DP,
         )
         self.start_net()
 
     def test_port5001_blocked(self):
         """Test that TCP port 5001 is blocked."""
         self.ping_all_when_learned()
         first_host, second_host = self.net.hosts[0:2]
         self.verify_tp_dst_notblocked(5001, first_host, second_host)
         with open(self.acls_config, 'w') as config_file:
-            config_file.write(self.get_config(acls=self.ACLS_OVERRIDE))
+            config_file.write(self.get_config(acls=self.acls_override()))
         self.verify_faucet_reconf(cold_start=False, change_expected=True)
         self.verify_tp_dst_blocked(5001, first_host, second_host)
         self.verify_no_cable_errors()
 
     def test_port5002_notblocked(self):
         """Test that TCP port 5002 is not blocked."""
         self.ping_all_when_learned()
         first_host, second_host = self.net.hosts[0:2]
         self.verify_tp_dst_blocked(5002, first_host, second_host)
         with open(self.acls_config, 'w') as config_file:
-            config_file.write(self.get_config(acls=self.ACLS_OVERRIDE))
+            config_file.write(self.get_config(acls=self.acls_override()))
         self.verify_faucet_reconf(cold_start=False, change_expected=True)
         self.verify_tp_dst_notblocked(5002, first_host, second_host)
         self.verify_no_cable_errors()
 
 
 class FaucetTunnelSameDpTest(FaucetStringOfDPTest):
 
     NUM_DPS = 2
     NUM_HOSTS = 2
     SWITCH_TO_SWITCH_LINKS = 2
     VID = 100
-    ACLS = {
+
+    def acls(self):
+        return {
         1: [
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'ip_proto': 1,
                 'actions': {
                     'allow': 0,
                     'output': {
@@ -7301,33 +7302,33 @@
                             'tunnel_id': 200,
                             'dp': 'faucet-1',
                             'port': 'b%(port_2)d'}
                     }
                 }
             }}
         ]
-    }
+        }
 
     # DP-to-acl_in port mapping.
-    ACL_IN_DP = {
+    def acl_in_dp(self):
+        port_1 = self.port_map['port_1']
+        return {
         'faucet-1': {
             # First port 1, acl_in = 1
-            mininet_test_topo.SWITCH_START_PORT: 1,
+            port_1: 1,
+        }
         }
-    }
 
     def setUp(self): # pylint: disable=invalid-name
         super(FaucetTunnelSameDpTest, self).setUp()
         self.build_net(
             stack=True,
             n_dps=self.NUM_DPS,
             n_untagged=self.NUM_HOSTS,
             untagged_vid=self.VID,
-            acls=self.ACLS,
-            acl_in_dp=self.ACL_IN_DP,
             switch_to_switch_links=self.SWITCH_TO_SWITCH_LINKS,
             hw_dpid=self.hw_dpid,
         )
         self.start_net()
 
     def verify_tunnel_established(self, src_host, dst_host, other_host, packets=3):
         """Verify ICMP packets tunnelled from src to dst."""
@@ -7354,50 +7355,53 @@
 
 class FaucetTunnelTest(FaucetStringOfDPTest):
 
     NUM_DPS = 2
     NUM_HOSTS = 2
     SWITCH_TO_SWITCH_LINKS = 2
     VID = 100
-    ACLS = {
+    def acls(self):
+        dpid2 = self.dpids[1]
+        port2_1 = self.port_maps[dpid2]['port_1']
+        return {
         1: [
             {'rule': {
                 'dl_type': IPV4_ETH,
                 'ip_proto': 1,
                 'actions': {
                     'allow': 0,
                     'output': {
                         'tunnel': {
                             'type': 'vlan',
                             'tunnel_id': 200,
                             'dp': 'faucet-2',
-                            'port': mininet_test_topo.SWITCH_START_PORT}
+                            'port': port2_1}
                     }
                 }
             }}
         ]
     }
 
     # DP-to-acl_in port mapping.
-    ACL_IN_DP = {
+    def acl_in_dp(self,):
+        port_1 = self.port_map['port_1']
+        return {
         'faucet-1': {
             # First port 1, acl_in = 1
-            mininet_test_topo.SWITCH_START_PORT: 1,
+            port_1: 1,
+        }
         }
-    }
 
     def setUp(self): # pylint: disable=invalid-name
         super(FaucetTunnelTest, self).setUp()
         self.build_net(
             stack=True,
             n_dps=self.NUM_DPS,
             n_untagged=self.NUM_HOSTS,
             untagged_vid=self.VID,
-            acls=self.ACLS,
-            acl_in_dp=self.ACL_IN_DP,
             switch_to_switch_links=self.SWITCH_TO_SWITCH_LINKS,
             hw_dpid=self.hw_dpid,
         )
         self.start_net()
 
     def verify_tunnel_established(self, src_host, dst_host, other_host, packets=3):
         """Verify ICMP packets tunnelled from src to dst."""
@@ -7425,15 +7429,15 @@
         self.verify_all_stack_up()
         src_host, other_host, dst_host = self.net.hosts[:3]
         self.verify_tunnel_established(src_host, dst_host, other_host)
 
     def test_tunnel_path_rerouted(self):
         """Test a tunnel path is rerouted when a stack is down."""
         self.verify_all_stack_up()
-        first_stack_port = self.non_host_ports(self.dpid)[0]
+        first_stack_port = self.non_host_links(self.dpid)[0].port
         self.one_stack_port_down(first_stack_port)
         src_host, other_host, dst_host = self.net.hosts[:3]
         self.verify_tunnel_established(src_host, dst_host, other_host, packets=10)
 
 
 class FaucetGroupTableTest(FaucetUntaggedTest):
```

### Comparing `faucet-1.9.8/tests/unit/packaging/test_packaging.py` & `faucet-1.9.9/tests/unit/packaging/test_packaging.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/gauge/test_gauge.py` & `faucet-1.9.9/tests/unit/gauge/test_gauge.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/gauge/test_config_gauge.py` & `faucet-1.9.9/tests/unit/gauge/test_config_gauge.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/gauge/test_main.py` & `faucet-1.9.9/tests/unit/gauge/test_main.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/faucet/test_check_config.py` & `faucet-1.9.9/tests/unit/faucet/test_check_config.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/faucet/test_port.py` & `faucet-1.9.9/tests/unit/faucet/test_port.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/faucet/test_vlan.py` & `faucet-1.9.9/tests/unit/faucet/test_vlan.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/faucet/fakeoftable.py` & `faucet-1.9.9/tests/unit/faucet/fakeoftable.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/faucet/test_main.py` & `faucet-1.9.9/tests/unit/faucet/test_main.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/tests/unit/faucet/test_valve.py` & `faucet-1.9.9/tests/unit/faucet/test_valve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1562,15 +1562,16 @@
         filter_id = 'block_http'
         for handler in (
                 self.dot1x.logoff_handler,
                 self.dot1x.failure_handler):
             handler(
                 '0e:00:00:00:00:ff', faucet_dot1x.get_mac_str(valve_index, port_no))
         self.dot1x.auth_handler(
-            '0e:00:00:00:00:ff', faucet_dot1x.get_mac_str(valve_index, port_no), vlan_name, filter_id)
+            '0e:00:00:00:00:ff', faucet_dot1x.get_mac_str(valve_index, port_no),
+            vlan_name=vlan_name, filter_id=filter_id)
 
 
 class ValveDot1xACLSmokeTestCase(ValveDot1xSmokeTestCase):
     """Smoke test to check dot1x can be initialized."""
     ACL_CONFIG = """
 acls:
     auth_acl:
```

### Comparing `faucet-1.9.8/tests/unit/faucet/test_config.py` & `faucet-1.9.9/tests/unit/faucet/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,14 +648,31 @@
                     system_name: port_system
                     port_descr: port_description
                     org_tlvs:
                         - {oui: 0x12bb, subtype: 2, info: "01406500"}
 """
         self.check_config_success(config, cp.dp_parser)
 
+    def test_lldp_peer_mac_valid(self):
+        """Test minimal valid LLDP config."""
+        config = """
+vlans:
+    office:
+        vid: 100
+dps:
+    sw1:
+        dp_id: 0x1
+        interfaces:
+            testing:
+                number: 1
+                native_vlan: office
+                lldp_peer_mac: '11:22:33:44:55:66'
+"""
+        self.check_config_success(config, cp.dp_parser)
+
     def test_interface_ranges_lldp(self):
         """Verify lldp config works when using interface ranges"""
         config = """
 vlans:
     office:
         vid: 100
     guest:
@@ -1716,14 +1733,48 @@
         dp_id: 0xfffffffffffffffffffffffffffffffff
         interfaces:
             1:
                 native_vlan: office
 """
         self.check_config_failure(config, cp.dp_parser)
 
+    def test_lacp_resp_interval_too_big(self):
+        """Test DP ID is valid."""
+        config = """
+vlans:
+    office:
+        vid: 100
+dps:
+    sw1:
+        dp_id: 0x1
+        interfaces:
+            1:
+                native_vlan: office
+                lacp_resp_interval: 0xfffffffffffffffffffffffffffffffff
+
+"""
+        self.check_config_failure(config, cp.dp_parser)
+
+    def test_lacp_resp_interval_zero(self):
+        """Test DP ID is valid."""
+        config = """
+vlans:
+    office:
+        vid: 100
+dps:
+    sw1:
+        dp_id: 0x1
+        interfaces:
+            1:
+                native_vlan: office
+                lacp_resp_interval: 0
+
+"""
+        self.check_config_failure(config, cp.dp_parser)
+
     def test_invalid_vid(self):
         """Test VID is valid."""
         config = """
 vlans:
     office:
         vid: 10000
 dps:
@@ -2950,14 +3001,31 @@
         interfaces:
             testing:
                 number: 1
                 native_vlan: office
 """
         self.check_config_failure(config, cp.dp_parser)
 
+    def test_lldp_peer_mac_invalid(self):
+        """Test minimal invalid DP config."""
+        config = """
+vlans:
+    office:
+        vid: 100
+dps:
+    sw1:
+        dp_id: 0x1
+        interfaces:
+            testing:
+                number: 1
+                native_vlan: office
+                lldp_peer_mac: '11:22:33:44:55:66:77:88'
+"""
+        self.check_config_failure(config, cp.dp_parser)
+        
     def test_vlan_route_missing_value_invalid(self):
         """Test new vlan route format fails when missing value"""
         config = """
 vlans:
     office:
         vid: 100
         routes:
```

### Comparing `faucet-1.9.8/tests/unit/faucet/test_fctl.py` & `faucet-1.9.9/tests/unit/faucet/test_fctl.py`

 * *Files identical despite different names*

### Comparing `faucet-1.9.8/AUTHORS` & `faucet-1.9.9/AUTHORS`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Anurag Porripireddi <anuragprdi@google.com>
-Bill Fisher <william.w.fisher@gmail.com>
 Bob Lantz <rlantz@cs.stanford.edu>
 Brad Cowie <brad@gizmoguy.net.nz>
 Brad Cowie <brad@wand.net.nz>
 Charlie Lewis <clewis@iqt.org>
 Christophe Rene <crene@cisco.com>
 Christopher Lorier <chris.lorier@reannz.co.nz>
 Ewen McNeill <ewen@naos.co.nz>
 Josh Bailey <anarkiwi@users.noreply.github.com>
 Josh Bailey <joshb@google.com>
 KitL <clorier@gmail.com>
+Mark Wutzke <mwutzke@users.noreply.github.com>
 Michael Baird <michaelb_111@hotmail.com>
 Michael Washer <michael.washer@icloud.com>
+Renovate Bot <bot@renovateapp.com>
 Simeon Miteff <simeon.miteff@gmail.com>
 Trevor Pering <peringknife@google.com>
 Trung Truong <trungdtbk@gmail.com>
 Yiding Xu <yiding.xu@gmail.com>
 cglewis <clewis@iqt.org>
+clorier <50934868+clorier@users.noreply.github.com>
 m@b <mab68@students.waikato.ac.nz>
 mab68 <mab68@students.waikato.ac.nz>
 pyup-bot <github-bot@pyup.io>
-rahul217 <rahul217@gmail.com>
```


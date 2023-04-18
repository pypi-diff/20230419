# Comparing `tmp/c65chewie-1.0.3.tar.gz` & `tmp/c65chewie-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c65chewie-1.0.3.tar", last modified: Thu Oct 13 18:57:21 2022, max compression
+gzip compressed data, was "c65chewie-1.0.4.tar", last modified: Tue Apr 18 22:28:48 2023, max compression
```

## Comparing `c65chewie-1.0.3.tar` & `c65chewie-1.0.4.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.273969 c65chewie-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.245967 c65chewie-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.253968 c65chewie-1.0.3/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.253968 c65chewie-1.0.3/.github/workflows/disabled/
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.github/workflows/disabled/release-debian.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.github/workflows/release-docker.yml
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.github/workflows/release-python.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.github/workflows/tests-codecheck.yml
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.github/workflows/tests-integration.yml
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.github/workflows/tests-unit.yml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.github/workflows/tests-yaml-lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.renovaterc.json
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-13 18:57:16.000000 c65chewie-1.0.3/.stickler.yml
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-13 18:57:20.000000 c65chewie-1.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-13 18:57:20.000000 c65chewie-1.0.3/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-10-13 18:57:16.000000 c65chewie-1.0.3/Dockerfile.chewie
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-13 18:57:16.000000 c65chewie-1.0.3/Dockerfile.freeradius
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-10-13 18:57:16.000000 c65chewie-1.0.3/Dockerfile.fuzz
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-13 18:57:16.000000 c65chewie-1.0.3/Dockerfile.wpasupplicant
--rw-r--r--   0 runner    (1001) docker     (121)    10758 2022-10-13 18:57:16.000000 c65chewie-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-13 18:57:21.273969 c65chewie-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-10-13 18:57:16.000000 c65chewie-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-10-13 18:57:16.000000 c65chewie-1.0.3/build_docs.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.253968 c65chewie-1.0.3/c65chewie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-13 18:57:21.000000 c65chewie-1.0.3/c65chewie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.257968 c65chewie-1.0.3/chewie/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/auth_8021x.py
--rw-r--r--   0 runner    (1001) docker     (121)    19852 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/chewie.py
--rw-r--r--   0 runner    (1001) docker     (121)     8676 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/eap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/ethernet_packet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/mac_address.py
--rw-r--r--   0 runner    (1001) docker     (121)    12739 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/message_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/nfv_sockets.py
--rw-r--r--   0 runner    (1001) docker     (121)    14498 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/radius.py
--rw-r--r--   0 runner    (1001) docker     (121)     9787 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/radius_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     8618 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/radius_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4692 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/radius_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/radius_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.261968 c65chewie-1.0.3/chewie/state_machines/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/state_machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/state_machines/abstract_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)    37477 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/state_machines/eap_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     9922 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/state_machines/mab_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/timer_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-10-13 18:57:16.000000 c65chewie-1.0.3/chewie/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-13 18:57:16.000000 c65chewie-1.0.3/codecheck-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.261968 c65chewie-1.0.3/debian/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-13 18:57:16.000000 c65chewie-1.0.3/debian/README.source
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-13 18:57:16.000000 c65chewie-1.0.3/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-13 18:57:16.000000 c65chewie-1.0.3/debian/compat
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-10-13 18:57:16.000000 c65chewie-1.0.3/debian/control
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-10-13 18:57:16.000000 c65chewie-1.0.3/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (121)       96 2022-10-13 18:57:16.000000 c65chewie-1.0.3/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.261968 c65chewie-1.0.3/debian/source/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 18:57:16.000000 c65chewie-1.0.3/debian/source/format
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.261968 c65chewie-1.0.3/docker/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docker/fuzz_packet.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      575 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docker/pip_deps.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      220 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docker/retrycmd.sh
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docker/run_integration_tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.265968 c65chewie-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docs/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-13 18:57:16.000000 c65chewie-1.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.249968 c65chewie-1.0.3/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.265968 c65chewie-1.0.3/etc/freeradius/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/etc/freeradius/certs/
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/01.pem
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/02.pem
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8444 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/README
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/bootstrap
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/ca.cnf
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/ca.der
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/ca.key
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/ca.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/client.cnf
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/client.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/client.csr
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/client.key
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/client.p12
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/client.pem
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/dh
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/index.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/index.txt.attr
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/index.txt.attr.old
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/index.txt.old
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/passwords.mk
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/serial
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/serial.old
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/server.cnf
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/server.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/server.csr
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/server.key
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/server.p12
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/server.pem
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/user@example.org.pem
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/certs/xpextensions
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/clients.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/etc/freeradius/default/
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/default/eap
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/default/inner-eap
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/default/tls
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/freeradius/users
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/etc/hostapd/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/hostapd/hostapd.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/etc/wpasupplicant/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/etc/wpasupplicant/cert/
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/wpasupplicant/cert/ca.pem
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/wpasupplicant/cert/user@example.org.pem
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/wpasupplicant/wired-md5.conf
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/wpasupplicant/wired-peap.conf
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/wpasupplicant/wired-tls.conf
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-13 18:57:16.000000 c65chewie-1.0.3/etc/wpasupplicant/wired-ttls.conf
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-13 18:57:16.000000 c65chewie-1.0.3/fuzz-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-13 18:57:16.000000 c65chewie-1.0.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     2060 2022-10-13 18:57:16.000000 c65chewie-1.0.3/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-13 18:57:21.273969 c65chewie-1.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      494 2022-10-13 18:57:16.000000 c65chewie-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.249968 c65chewie-1.0.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/test/codecheck/
--rwxr-xr-x   0 runner    (1001) docker     (121)      354 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/codecheck/min_pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      234 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/codecheck/pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      670 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/codecheck/src_files.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/test/fuzzer/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.269968 c65chewie-1.0.3/test/fuzzer/dict/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/dict/packet.dict
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.273969 c65chewie-1.0.3/test/fuzzer/eap_packet/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/eap_packet/eap-md5.ex1
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/eap_packet/eap-start.ex1
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/eap_packet/eap-success.ex1
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/eap_packet/eap-tls.ex1
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/fuzz_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.273969 c65chewie-1.0.3/test/fuzzer/radius_packet/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/radius_packet/access-accept.ex1
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/radius_packet/access-challenge.ex1
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/radius_packet/access-challenge.ex2
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/fuzzer/radius_packet/access-reject.ex1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.273969 c65chewie-1.0.3/test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)    10209 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/integration/base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/integration/test_eap.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/integration/test_mab.py
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/integration/test_radius_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 18:57:21.273969 c65chewie-1.0.3/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_auth_8021x.py
--rw-r--r--   0 runner    (1001) docker     (121)    20873 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_chewie.py
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_chewie_mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_eap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_ethernet_packet.py
--rw-r--r--   0 runner    (1001) docker     (121)    24746 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_full_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     5471 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_mab_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_mac_address.py
--rw-r--r--   0 runner    (1001) docker     (121)    23173 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_message_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    40548 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test/unit/test_radius.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-13 18:57:16.000000 c65chewie-1.0.3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.130614 c65chewie-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.118614 c65chewie-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.118614 c65chewie-1.0.4/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.118614 c65chewie-1.0.4/.github/workflows/disabled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/workflows/disabled/release-debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/workflows/release-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/workflows/release-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/workflows/tests-codecheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/workflows/tests-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/workflows/tests-unit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.github/workflows/tests-yaml-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-18 22:28:45.000000 c65chewie-1.0.4/.stickler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 22:28:47.000000 c65chewie-1.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 22:28:47.000000 c65chewie-1.0.4/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-18 22:28:45.000000 c65chewie-1.0.4/Dockerfile.chewie
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 22:28:45.000000 c65chewie-1.0.4/Dockerfile.freeradius
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 22:28:45.000000 c65chewie-1.0.4/Dockerfile.fuzz
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 22:28:45.000000 c65chewie-1.0.4/Dockerfile.wpasupplicant
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-18 22:28:45.000000 c65chewie-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-18 22:28:48.130614 c65chewie-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-18 22:28:45.000000 c65chewie-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-18 22:28:45.000000 c65chewie-1.0.4/build_docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.118614 c65chewie-1.0.4/c65chewie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-18 22:28:47.000000 c65chewie-1.0.4/c65chewie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-18 22:28:48.000000 c65chewie-1.0.4/c65chewie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:28:47.000000 c65chewie-1.0.4/c65chewie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 22:28:47.000000 c65chewie-1.0.4/c65chewie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:28:47.000000 c65chewie-1.0.4/c65chewie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 22:28:47.000000 c65chewie-1.0.4/c65chewie.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:28:47.000000 c65chewie-1.0.4/c65chewie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 22:28:47.000000 c65chewie-1.0.4/c65chewie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.118614 c65chewie-1.0.4/chewie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/auth_8021x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/chewie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/eap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/ethernet_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/mac_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/message_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/nfv_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/radius_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/radius_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/radius_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/radius_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.122614 c65chewie-1.0.4/chewie/state_machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/state_machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/state_machines/abstract_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37477 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/state_machines/eap_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/state_machines/mab_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/timer_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-18 22:28:45.000000 c65chewie-1.0.4/chewie/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 22:28:45.000000 c65chewie-1.0.4/codecheck-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.122614 c65chewie-1.0.4/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-18 22:28:45.000000 c65chewie-1.0.4/debian/README.source
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 22:28:45.000000 c65chewie-1.0.4/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-18 22:28:45.000000 c65chewie-1.0.4/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 22:28:45.000000 c65chewie-1.0.4/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-18 22:28:45.000000 c65chewie-1.0.4/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-18 22:28:45.000000 c65chewie-1.0.4/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.122614 c65chewie-1.0.4/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 22:28:45.000000 c65chewie-1.0.4/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.122614 c65chewie-1.0.4/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docker/fuzz_packet.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docker/pip_deps.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docker/retrycmd.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docker/run_integration_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.122614 c65chewie-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docs/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 22:28:45.000000 c65chewie-1.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.114613 c65chewie-1.0.4/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.122614 c65chewie-1.0.4/etc/freeradius/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/etc/freeradius/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/01.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/02.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/README
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/bootstrap
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/ca.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/ca.der
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/client.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/client.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/client.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/client.key
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/client.p12
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/client.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/dh
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/index.txt.attr
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/index.txt.attr.old
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/index.txt.old
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/passwords.mk
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/serial
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/serial.old
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/server.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/server.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/server.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/server.key
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/server.p12
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/server.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/user@example.org.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/certs/xpextensions
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/clients.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/etc/freeradius/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/default/eap
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/default/inner-eap
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/default/tls
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/freeradius/users
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/etc/hostapd/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/hostapd/hostapd.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/etc/wpasupplicant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/etc/wpasupplicant/cert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/wpasupplicant/cert/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/wpasupplicant/cert/user@example.org.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/wpasupplicant/wired-md5.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/wpasupplicant/wired-peap.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/wpasupplicant/wired-tls.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-18 22:28:45.000000 c65chewie-1.0.4/etc/wpasupplicant/wired-ttls.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-18 22:28:45.000000 c65chewie-1.0.4/fuzz-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:28:45.000000 c65chewie-1.0.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-18 22:28:45.000000 c65chewie-1.0.4/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-18 22:28:48.130614 c65chewie-1.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-04-18 22:28:45.000000 c65chewie-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.114613 c65chewie-1.0.4/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/test/codecheck/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/codecheck/min_pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/codecheck/pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/codecheck/src_files.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/test/fuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/test/fuzzer/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/dict/packet.dict
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/test/fuzzer/eap_packet/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/eap_packet/eap-md5.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/eap_packet/eap-start.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/eap_packet/eap-success.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/eap_packet/eap-tls.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/fuzz_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.126614 c65chewie-1.0.4/test/fuzzer/radius_packet/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/radius_packet/access-accept.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/radius_packet/access-challenge.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/radius_packet/access-challenge.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/fuzzer/radius_packet/access-reject.ex1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.130614 c65chewie-1.0.4/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/integration/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/integration/test_eap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/integration/test_mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/integration/test_radius_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:28:48.130614 c65chewie-1.0.4/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_auth_8021x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_chewie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_chewie_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_eap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_ethernet_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_full_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_mab_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_mac_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_message_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40548 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test/unit/test_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:28:45.000000 c65chewie-1.0.4/test-requirements.txt
```

### Comparing `c65chewie-1.0.3/.github/workflows/disabled/release-debian.yml` & `c65chewie-1.0.4/.github/workflows/disabled/release-debian.yml`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/.github/workflows/release-docker.yml` & `c65chewie-1.0.4/.github/workflows/release-docker.yml`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/.github/workflows/release-python.yml` & `c65chewie-1.0.4/.github/workflows/release-python.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
       - name: Set up python-${{ env.RELEASE_PY_VER }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ env.RELEASE_PY_VER }}
       - name: Build python package
         run: python3 setup.py sdist
       - name: Publish python package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.5.1
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `c65chewie-1.0.3/.github/workflows/tests-codecheck.yml` & `c65chewie-1.0.4/.github/workflows/tests-codecheck.yml`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,15 @@
           ./test/codecheck/pylint.sh
 
   pytype:
     name: Pytype
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        # TODO: pytype does not yet support python 3.10: https://github.com/google/pytype/issues/1022
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.8, 3.9, '3.10']
     steps:
       - name: Checkout repo
         uses: actions/checkout@v3
       - name: Set up python-${{ env.CODECHECK_PY_VER }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ env.CODECHECK_PY_VER }}
```

### Comparing `c65chewie-1.0.3/.github/workflows/tests-unit.yml` & `c65chewie-1.0.4/.github/workflows/tests-unit.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   unit-tests:
     name: Unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.8, 3.9, '3.10', 3.11]
     steps:
       - name: Checkout repo
         uses: actions/checkout@v3
       - name: Set up python-${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `c65chewie-1.0.3/LICENSE` & `c65chewie-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/PKG-INFO` & `c65chewie-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: c65chewie
-Version: 1.0.3
+Version: 1.0.4
 Summary: A bare-bones EAPOL/802.1x implementation
 Home-page: https://github.com/faucetsdn/chewie
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache-2
 Description: UNKNOWN
 Keywords: 802.1x,dot1x,eap,eapol,radius,authentication,aaa
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `c65chewie-1.0.3/README.md` & `c65chewie-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Chewie
 
-[![Build Status](https://github.com/faucetsdn/chewie/workflows/Unit%20tests/badge.svg?branch=master)](https://github.com/faucetsdn/chewie/actions?query=workflow%3A%22Unit+tests%22)
-[![Test Coverage](https://codecov.io/gh/faucetsdn/chewie/branch/master/graph/badge.svg)](https://codecov.io/gh/faucetsdn/chewie)
+[![Build Status](https://github.com/faucetsdn/chewie/workflows/Unit%20tests/badge.svg?branch=main)](https://github.com/faucetsdn/chewie/actions?query=workflow%3A%22Unit+tests%22)
+[![Test Coverage](https://codecov.io/gh/faucetsdn/chewie/branch/main/graph/badge.svg)](https://codecov.io/gh/faucetsdn/chewie)
 
 ## Chewie - EAPOL / 802.1x
 Chewie is an EAPOL/802.1x implementation in Python.
 It is designed to work on it's own but primarily as a module for [The Faucet Project](https://github.com/faucetsdn/faucet)
 which is an open-source SDN controller implementation in Python.
 
 ### Supported Features:
```

### Comparing `c65chewie-1.0.3/build_docs.sh` & `c65chewie-1.0.4/build_docs.sh`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/c65chewie.egg-info/PKG-INFO` & `c65chewie-1.0.4/c65chewie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: c65chewie
-Version: 1.0.3
+Version: 1.0.4
 Summary: A bare-bones EAPOL/802.1x implementation
 Home-page: https://github.com/faucetsdn/chewie
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache-2
 Description: UNKNOWN
 Keywords: 802.1x,dot1x,eap,eapol,radius,authentication,aaa
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `c65chewie-1.0.3/c65chewie.egg-info/SOURCES.txt` & `c65chewie-1.0.4/c65chewie.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .codecov.yml
 .pylintrc
 .readthedocs.yml
-.renovaterc.json
 .stickler.yml
 AUTHORS
 ChangeLog
 Dockerfile.chewie
 Dockerfile.freeradius
 Dockerfile.fuzz
 Dockerfile.wpasupplicant
@@ -16,14 +15,15 @@
 docker-compose.yaml
 fuzz-requirements.txt
 requirements.txt
 run_tests.sh
 setup.cfg
 setup.py
 test-requirements.txt
+.github/dependabot.yml
 .github/workflows/release-docker.yml
 .github/workflows/release-python.yml
 .github/workflows/tests-codecheck.yml
 .github/workflows/tests-integration.yml
 .github/workflows/tests-unit.yml
 .github/workflows/tests-yaml-lint.yml
 .github/workflows/disabled/release-debian.yml
```

### Comparing `c65chewie-1.0.3/chewie/__main__.py` & `c65chewie-1.0.4/chewie/__main__.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/auth_8021x.py` & `c65chewie-1.0.4/chewie/auth_8021x.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/chewie.py` & `c65chewie-1.0.4/chewie/chewie.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/eap.py` & `c65chewie-1.0.4/chewie/eap.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/ethernet_packet.py` & `c65chewie-1.0.4/chewie/ethernet_packet.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/event.py` & `c65chewie-1.0.4/chewie/event.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/mac_address.py` & `c65chewie-1.0.4/chewie/mac_address.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/message_parser.py` & `c65chewie-1.0.4/chewie/message_parser.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/nfv_sockets.py` & `c65chewie-1.0.4/chewie/nfv_sockets.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/radius.py` & `c65chewie-1.0.4/chewie/radius.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/radius_attributes.py` & `c65chewie-1.0.4/chewie/radius_attributes.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/radius_datatypes.py` & `c65chewie-1.0.4/chewie/radius_datatypes.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/radius_lifecycle.py` & `c65chewie-1.0.4/chewie/radius_lifecycle.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/radius_socket.py` & `c65chewie-1.0.4/chewie/radius_socket.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/state_machines/abstract_state_machine.py` & `c65chewie-1.0.4/chewie/state_machines/abstract_state_machine.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/state_machines/eap_state_machine.py` & `c65chewie-1.0.4/chewie/state_machines/eap_state_machine.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/state_machines/mab_state_machine.py` & `c65chewie-1.0.4/chewie/state_machines/mab_state_machine.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/timer_scheduler.py` & `c65chewie-1.0.4/chewie/timer_scheduler.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/chewie/utils.py` & `c65chewie-1.0.4/chewie/utils.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/debian/control` & `c65chewie-1.0.4/debian/control`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
                python3-all,
                python3-setuptools,
                python3-eventlet,
                python3-transitions,
                python3-pbr (>= 1.9),
 Standards-Version: 3.9.6
 Homepage: https://github.com/faucetsdn/chewie
-X-Python3-Version: >= 3.7
+X-Python3-Version: >= 3.8
 Vcs-Git: https://github.com/faucetsdn/chewie.git
 Vcs-Browser: https://github.com/faucetsdn/chewie
 
 Package: python3-chewie
 Architecture: all
 Depends: ${python3:Depends},
-         python3:any (>= 3.7~),
+         python3:any (>= 3.8~),
          ${misc:Depends}
 Description: Chewie is an EAPOL/802.1x implementation in Python.
  .
  This package installs the library for Python 3.
```

### Comparing `c65chewie-1.0.3/debian/copyright` & `c65chewie-1.0.4/debian/copyright`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/docker/fuzz_packet.sh` & `c65chewie-1.0.4/docker/fuzz_packet.sh`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/docker/pip_deps.sh` & `c65chewie-1.0.4/docker/pip_deps.sh`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/docker-compose.yaml` & `c65chewie-1.0.4/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/docs/Makefile` & `c65chewie-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/docs/conf.py` & `c65chewie-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/docs/development.rst` & `c65chewie-1.0.4/docs/development.rst`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/docs/intro.rst` & `c65chewie-1.0.4/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/01.pem` & `c65chewie-1.0.4/etc/freeradius/certs/01.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/02.pem` & `c65chewie-1.0.4/etc/freeradius/certs/02.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/Makefile` & `c65chewie-1.0.4/etc/freeradius/certs/Makefile`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/README` & `c65chewie-1.0.4/etc/freeradius/certs/README`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/bootstrap` & `c65chewie-1.0.4/etc/freeradius/certs/bootstrap`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/ca.cnf` & `c65chewie-1.0.4/etc/freeradius/certs/ca.cnf`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/ca.der` & `c65chewie-1.0.4/etc/freeradius/certs/ca.der`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/ca.key` & `c65chewie-1.0.4/etc/freeradius/certs/ca.key`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/ca.pem` & `c65chewie-1.0.4/etc/freeradius/certs/ca.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/client.cnf` & `c65chewie-1.0.4/etc/freeradius/certs/client.cnf`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/client.crt` & `c65chewie-1.0.4/etc/freeradius/certs/client.crt`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/client.csr` & `c65chewie-1.0.4/etc/freeradius/certs/client.csr`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/client.key` & `c65chewie-1.0.4/etc/freeradius/certs/client.key`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/client.p12` & `c65chewie-1.0.4/etc/freeradius/certs/client.p12`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/client.pem` & `c65chewie-1.0.4/etc/freeradius/certs/client.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/dh` & `c65chewie-1.0.4/etc/freeradius/certs/dh`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/server.cnf` & `c65chewie-1.0.4/etc/freeradius/certs/server.cnf`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/server.crt` & `c65chewie-1.0.4/etc/freeradius/certs/server.crt`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/server.csr` & `c65chewie-1.0.4/etc/freeradius/certs/server.csr`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/server.key` & `c65chewie-1.0.4/etc/freeradius/certs/server.key`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/server.p12` & `c65chewie-1.0.4/etc/freeradius/certs/server.p12`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/server.pem` & `c65chewie-1.0.4/etc/freeradius/certs/server.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/user@example.org.pem` & `c65chewie-1.0.4/etc/freeradius/certs/user@example.org.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/certs/xpextensions` & `c65chewie-1.0.4/etc/freeradius/certs/xpextensions`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/default/eap` & `c65chewie-1.0.4/etc/freeradius/default/eap`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/default/tls` & `c65chewie-1.0.4/etc/freeradius/default/tls`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/freeradius/users` & `c65chewie-1.0.4/etc/freeradius/users`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/wpasupplicant/cert/ca.pem` & `c65chewie-1.0.4/etc/wpasupplicant/cert/ca.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/etc/wpasupplicant/cert/user@example.org.pem` & `c65chewie-1.0.4/etc/wpasupplicant/cert/user@example.org.pem`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/run_tests.sh` & `c65chewie-1.0.4/run_tests.sh`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/setup.cfg` & `c65chewie-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/codecheck/src_files.sh` & `c65chewie-1.0.4/test/codecheck/src_files.sh`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/fuzzer/README.rst` & `c65chewie-1.0.4/test/fuzzer/README.rst`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/fuzzer/eap_packet/eap-tls.ex1` & `c65chewie-1.0.4/test/fuzzer/eap_packet/eap-tls.ex1`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/fuzzer/fuzz_packet.py` & `c65chewie-1.0.4/test/fuzzer/fuzz_packet.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/fuzzer/radius_packet/access-challenge.ex2` & `c65chewie-1.0.4/test/fuzzer/radius_packet/access-challenge.ex2`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/integration/base_test.py` & `c65chewie-1.0.4/test/integration/base_test.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/integration/test_eap.py` & `c65chewie-1.0.4/test/integration/test_eap.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/integration/test_mab.py` & `c65chewie-1.0.4/test/integration/test_mab.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/integration/test_radius_attributes.py` & `c65chewie-1.0.4/test/integration/test_radius_attributes.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/helpers.py` & `c65chewie-1.0.4/test/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_auth_8021x.py` & `c65chewie-1.0.4/test/unit/test_auth_8021x.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_chewie.py` & `c65chewie-1.0.4/test/unit/test_chewie.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_chewie_mocks.py` & `c65chewie-1.0.4/test/unit/test_chewie_mocks.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_eap.py` & `c65chewie-1.0.4/test/unit/test_eap.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_ethernet_packet.py` & `c65chewie-1.0.4/test/unit/test_ethernet_packet.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_full_state_machine.py` & `c65chewie-1.0.4/test/unit/test_full_state_machine.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_mab_state_machine.py` & `c65chewie-1.0.4/test/unit/test_mab_state_machine.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_mac_address.py` & `c65chewie-1.0.4/test/unit/test_mac_address.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_message_parser.py` & `c65chewie-1.0.4/test/unit/test_message_parser.py`

 * *Files identical despite different names*

### Comparing `c65chewie-1.0.3/test/unit/test_radius.py` & `c65chewie-1.0.4/test/unit/test_radius.py`

 * *Files identical despite different names*


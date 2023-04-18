# Comparing `tmp/dallinger-9.5.0.tar.gz` & `tmp/dallinger-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dallinger-9.5.0.tar", last modified: Wed Mar 29 05:44:13 2023, max compression
+gzip compressed data, was "dallinger-9.6.0.tar", last modified: Tue Apr 18 22:00:43 2023, max compression
```

## Comparing `dallinger-9.5.0.tar` & `dallinger-9.6.0.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.965340 dallinger-9.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-29 05:43:37.000000 dallinger-9.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-29 05:43:37.000000 dallinger-9.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-29 05:44:13.965340 dallinger-9.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-29 05:43:37.000000 dallinger-9.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-29 05:44:09.000000 dallinger-9.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-03-29 05:43:37.000000 dallinger-9.5.0/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.933340 dallinger-9.5.0/dallinger/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/bots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.937340 dallinger-9.5.0/dallinger/command_line/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/command_line/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/command_line/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/command_line/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/command_line/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/command_line/docker_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/command_line/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.937340 dallinger-9.5.0/dallinger/default_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/default_configs/.dallingerconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/default_configs/global_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/default_configs/local_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.937340 dallinger-9.5.0/dallinger/dev_server/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/dev_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/dev_server/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.937340 dallinger-9.5.0/dallinger/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/heroku.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/prepare_docker_image.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.937340 dallinger-9.5.0/dallinger/docker/ssh_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/ssh_templates/docker-compose-server.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/docker/wheel_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)    59122 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.937340 dallinger-9.5.0/dallinger/experiment_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26990 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    57902 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiment_server/worker_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.937340 dallinger-9.5.0/dallinger/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.929340 dallinger-9.5.0/dallinger/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.941340 dallinger-9.5.0/dallinger/frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.941340 dallinger-9.5.0/dallinger/frontend/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/css/dallinger.css
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/css/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.941340 dallinger-9.5.0/dallinger/frontend/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.941340 dallinger-9.5.0/dallinger/frontend/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/dallinger2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/dallinger2.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.929340 dallinger-9.5.0/dallinger/frontend/static/scripts/fingerprintjs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.941340 dallinger-9.5.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/network-monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/require.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/reqwest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/spin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/store+json2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/tracker.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.941340 dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.929340 dallinger-9.5.0/dallinger/frontend/static/vis@4.17.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.945340 dallinger-9.5.0/dallinger/frontend/static/vis@4.17.0/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.945340 dallinger-9.5.0/dallinger/frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.945340 dallinger-9.5.0/dallinger/frontend/templates/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/base/ad.html
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/base/consent.html
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/base/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/base/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/base/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/dashboard_database.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/dashboard_develop.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/dashboard_heroku.html
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/dashboard_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/dashboard_lifecycle.html
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/dashboard_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/dashboard_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/error-complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/exit_recruiter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/exit_recruiter_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/exit_recruiter_prolific.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/launch.html
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/frontend/templates/waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.949340 dallinger-9.5.0/dallinger/heroku/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/heroku/Procfile
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/heroku/Procfile_no_clock
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/heroku/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/heroku/rq_gevent_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/heroku/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/heroku/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/pytest_dallinger.py
--rw-r--r--   0 runner    (1001) docker     (123)    63882 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/redis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.933340 dallinger-9.5.0/dallinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-29 05:44:13.000000 dallinger-9.5.0/dallinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-03-29 05:44:13.000000 dallinger-9.5.0/dallinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 05:44:13.000000 dallinger-9.5.0/dallinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-29 05:44:13.000000 dallinger-9.5.0/dallinger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 05:44:13.000000 dallinger-9.5.0/dallinger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-29 05:44:13.000000 dallinger-9.5.0/dallinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-29 05:44:13.000000 dallinger-9.5.0/dallinger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.949340 dallinger-9.5.0/dallinger_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger_scripts/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger_scripts/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-29 05:43:37.000000 dallinger-9.5.0/dallinger_scripts/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-03-29 05:43:38.000000 dallinger-9.5.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.949340 dallinger-9.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.953340 dallinger-9.5.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.957340 dallinger-9.5.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
--rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/Dallinger AWS Group.png
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/burst.png
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/chain.png
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/class_chart.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/corner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/delayed.png
--rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/directories.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/empty.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/front_back_layout.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/full.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/grid.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/grid_mini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/grid_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/heroku.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_static/star.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.957340 dallinger-9.5.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/acknowledgments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/aws_etc_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/build_demo_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/building_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/command_line_utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/communicating_with_the_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/contributing_to_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/creating_an_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/dallinger_the_scientist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/demo_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/demoing_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/demos_on_heroku.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/developing_dallinger_setup_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/docker_only.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/docker_support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/docker_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/email_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/experiment_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/extra_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/installing_dallinger_for_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/javascript_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/learning_to_use_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/monitoring_a_live_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/postico_and_postgres.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/private_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/python_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/recruitment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/registration_on_OSF.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/required_experiment_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/rewarding_participants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/running_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/running_the_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/scheduled_tasks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.961341 dallinger-9.5.0/docs/source/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/info.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/network.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/node.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/notification.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/participant.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/transformation.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/transmission.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/schemas/vector.csvs
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/the_experiment_class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/vagrant_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/waiting_rooms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/web_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-03-29 05:43:38.000000 dallinger-9.5.0/docs/source/writing_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-03-29 05:43:38.000000 dallinger-9.5.0/incubator.png
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-03-29 05:43:38.000000 dallinger-9.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-29 05:44:13.965340 dallinger-9.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-29 05:43:38.000000 dallinger-9.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:13.965340 dallinger-9.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_bots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40472 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39003 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)    42528 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    76131 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_griduniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27061 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_replay_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-03-29 05:43:38.000000 dallinger-9.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.988801 dallinger-9.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-18 21:59:55.000000 dallinger-9.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 21:59:55.000000 dallinger-9.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-18 22:00:43.988801 dallinger-9.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-18 21:59:55.000000 dallinger-9.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-18 22:00:38.000000 dallinger-9.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-04-18 21:59:55.000000 dallinger-9.6.0/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.900801 dallinger-9.6.0/dallinger/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/bots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.904801 dallinger-9.6.0/dallinger/command_line/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/docker_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.904801 dallinger-9.6.0/dallinger/default_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/default_configs/.dallingerconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/default_configs/global_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/default_configs/local_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.904801 dallinger-9.6.0/dallinger/dev_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/dev_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/dev_server/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.908801 dallinger-9.6.0/dallinger/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/heroku.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/prepare_docker_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.908801 dallinger-9.6.0/dallinger/docker/ssh_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-server.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/wheel_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.912801 dallinger-9.6.0/dallinger/experiment_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27557 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57902 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/worker_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.912801 dallinger-9.6.0/dallinger/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.884801 dallinger-9.6.0/dallinger/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.912801 dallinger-9.6.0/dallinger/frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.916801 dallinger-9.6.0/dallinger/frontend/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/css/dallinger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.916801 dallinger-9.6.0/dallinger/frontend/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.920801 dallinger-9.6.0/dallinger/frontend/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.880801 dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.920801 dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/network-monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/require.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/reqwest.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/spin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/store+json2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.924801 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.880801 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.924801 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.932801 dallinger-9.6.0/dallinger/frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.932801 dallinger-9.6.0/dallinger/frontend/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/ad.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_database.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_develop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_heroku.html
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_lifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/error-complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_prolific.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/launch.html
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.936801 dallinger-9.6.0/dallinger/heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/Procfile
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/Procfile_no_clock
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/rq_gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    68520 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/pytest_dallinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64023 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/redis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.900801 dallinger-9.6.0/dallinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.936801 dallinger-9.6.0/dallinger_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-04-18 21:59:55.000000 dallinger-9.6.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.940801 dallinger-9.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.960801 dallinger-9.6.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.972801 dallinger-9.6.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/Dallinger AWS Group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/burst.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/chain.png
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/class_chart.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/corner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/delayed.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/directories.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/empty.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/front_back_layout.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/full.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/grid.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/grid_mini.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/grid_small.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/heroku.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/star.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.972801 dallinger-9.6.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/acknowledgments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/aws_etc_keys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/build_demo_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/building_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/command_line_utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/communicating_with_the_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/contributing_to_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/creating_an_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/dallinger_the_scientist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/demo_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/demoing_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/demos_on_heroku.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/developing_dallinger_setup_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/docker_only.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/docker_support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/docker_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/email_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/experiment_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/extra_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/installing_dallinger_for_users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/javascript_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/learning_to_use_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/monitoring_a_live_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/postico_and_postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/private_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/python_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/recruitment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/registration_on_OSF.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/required_experiment_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/rewarding_participants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/running_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/running_the_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/scheduled_tasks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.976801 dallinger-9.6.0/docs/source/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/info.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/network.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/node.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/notification.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/participant.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/transformation.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/transmission.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/vector.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/the_experiment_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/vagrant_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/waiting_rooms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/web_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/writing_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-04-18 21:59:55.000000 dallinger-9.6.0/incubator.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-18 21:59:55.000000 dallinger-9.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 22:00:43.988801 dallinger-9.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-18 21:59:55.000000 dallinger-9.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.988801 dallinger-9.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40472 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42354 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76131 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_griduniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_replay_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_utils.py
```

### Comparing `dallinger-9.5.0/LICENSE` & `dallinger-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/PKG-INFO` & `dallinger-9.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.5.0
+Version: 9.6.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.5.0/README.md` & `dallinger-9.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/README.rst` & `dallinger-9.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/constraints.txt` & `dallinger-9.6.0/dev-requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    ./scripts/update_dependencies.sh
 #
 
-    # via -r constraints.in
+    # via -r dev-requirements.in
 alabaster==0.7.13
     # via
     #   dallinger
     #   sphinx
 anyio==3.6.2
     # via jupyter-server
 apscheduler==3.10.1
@@ -25,35 +25,34 @@
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 async-generator==1.10
     # via trio
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   jsonschema
     #   outcome
-    #   pytest
     #   trio
 babel==2.12.1
     # via sphinx
 backcall==0.2.0
     # via ipython
 bcrypt==4.0.1
     # via paramiko
-beautifulsoup4==4.12.0
+beautifulsoup4==4.12.2
     # via nbconvert
-black==23.1.0
+black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
-boto3==1.26.100
+boto3==1.26.115
     # via dallinger
-botocore==1.29.100
+botocore==1.29.115
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -83,32 +82,29 @@
 click==8.1.3
     # via
     #   black
     #   dallinger
     #   flask
     #   pip-tools
     #   rq
-codecov==2.1.12
-    # via dallinger
 colorama==0.4.6
     # via tox
 comm==0.1.3
     # via ipykernel
-coverage==7.2.2
+coverage==7.2.3
     # via
-    #   codecov
     #   coverage-pth
     #   dallinger
 coverage-pth==0.0.2
     # via dallinger
-cryptography==40.0.1
+cryptography==40.0.2
     # via
     #   paramiko
     #   pyopenssl
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via
     #   nbconvert
     #   odfpy
@@ -126,19 +122,19 @@
 exceptiongroup==1.1.1
     # via
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.3.1
+faker==18.4.0
     # via dallinger
 fastjsonschema==2.16.3
     # via nbformat
-filelock==3.10.7
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
 flask==2.2.3
     # via
@@ -171,15 +167,15 @@
     #   dallinger
     #   gevent
     #   sqlalchemy
 gunicorn==20.1.0
     # via dallinger
 h11==0.14.0
     # via wsproto
-heroku3==5.2.0
+heroku3==5.2.1
     # via dallinger
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
@@ -193,15 +189,15 @@
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
     #   nbclassic
     #   notebook
     #   qtconsole
-ipython==8.11.0
+ipython==8.12.0
     # via
     #   ipykernel
     #   ipywidgets
     #   jupyter-console
 ipython-genutils==0.2.0
     # via
     #   nbclassic
@@ -238,15 +234,15 @@
     # via jsonschema
 jsonschema==4.17.3
     # via
     #   jupyter-events
     #   nbformat
 jupyter==1.0.0
     # via dallinger
-jupyter-client==8.1.0
+jupyter-client==8.2.0
     # via
     #   ipykernel
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   notebook
@@ -306,19 +302,19 @@
     # via nbconvert
 mock==5.0.0
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==1.0.0
     # via dallinger
-nbclassic==0.5.3
+nbclassic==0.5.5
     # via notebook
-nbclient==0.7.2
+nbclient==0.7.3
     # via nbconvert
-nbconvert==7.2.10
+nbconvert==7.3.1
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
 nbformat==5.8.0
     # via
@@ -330,42 +326,42 @@
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
 nodeenv==1.7.0
     # via pre-commit
-notebook==6.5.3
+notebook==6.5.4
     # via jupyter
 notebook-shim==0.2.2
     # via nbclassic
 numpy==1.24.2
     # via pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   docker
     #   ipykernel
     #   jupyter-server
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
 paramiko==3.1.0
     # via
@@ -377,42 +373,42 @@
     # via black
 pexpect==4.8.0
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via dallinger
 platformdirs==3.2.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via dallinger
 prometheus-client==0.16.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 prompt-toolkit==3.0.38
     # via
     #   ipython
     #   jupyter-console
-psutil==5.9.4
+psutil==5.9.5
     # via
     #   dallinger
     #   ipykernel
-psycopg2==2.9.5
+psycopg2==2.9.6
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
@@ -424,15 +420,15 @@
     #   flake8
 pycparser==2.21
     # via cffi
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   ipython
     #   jupyter-console
     #   nbconvert
     #   qtconsole
     #   sphinx
 pynacl==1.5.0
@@ -445,15 +441,15 @@
     # via tox
 pyproject-hooks==1.0.0
     # via build
 pyrsistent==0.19.3
     # via jsonschema
 pysocks==1.7.1
     # via urllib3
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   dallinger
     #   pytest-rerunfailures
 pytest-rerunfailures==11.1.2
     # via dallinger
 python-dateutil==2.8.2
     # via
@@ -461,15 +457,15 @@
     #   botocore
     #   faker
     #   heroku3
     #   jupyter-client
     #   pandas
 python-json-logger==2.0.7
     # via jupyter-events
-pytz==2023.2
+pytz==2023.3
     # via
     #   apscheduler
     #   pandas
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
 pyyaml==6.0
     # via
@@ -482,25 +478,24 @@
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   qtconsole
-qtconsole==5.4.1
+qtconsole==5.4.2
     # via jupyter
-qtpy==2.3.0
+qtpy==2.3.1
     # via qtconsole
-redis==4.5.3
+redis==4.5.4
     # via
     #   dallinger
     #   rq
 requests==2.28.2
     # via
-    #   codecov
     #   dallinger
     #   docker
     #   heroku3
     #   sphinx
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
@@ -533,15 +528,15 @@
     # via
     #   anyio
     #   trio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via trio
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
 sphinx==6.1.3
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
@@ -596,23 +591,23 @@
     # via
     #   black
     #   build
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tornado==6.2
+tornado==6.3
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.8
+tox==4.4.12
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -630,16 +625,18 @@
     #   qtconsole
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.2
     # via selenium
-tzdata==2023.2
-    # via pytz-deprecation-shim
+tzdata==2023.3
+    # via
+    #   pandas
+    #   pytz-deprecation-shim
 tzlocal==4.3
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
     #   dallinger
```

### Comparing `dallinger-9.5.0/dallinger/__init__.py` & `dallinger-9.6.0/dallinger/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/bots.py` & `dallinger-9.6.0/dallinger/bots.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,28 +43,50 @@
         if not URL:
             return
         logger.info("Creating bot with URL: %s." % URL)
         self.URL = URL
 
         parts = urllib.parse.urlparse(URL)
         query = urllib.parse.parse_qs(parts.query)
+
         if not assignment_id:
-            assignment_id = query.get("assignment_id", [""])[0]
+            # Dallinger experiments are not always consistent in whether the participant recruitment URL
+            # uses snake_case or camelCase. This code accepts either format.
+            assignment_id = self.get_from_query(
+                query, ["assignment_id", "assignmentId"]
+            )
+
         if not participant_id:
-            participant_id = query.get("participant_id", [""])[0]
+            participant_id = self.get_from_query(
+                query, ["participant_id", "participantId"]
+            )
+
+        if not worker_id:
+            worker_id = self.get_from_query(query, ["worker_id", "workerId"])
+
         if not hit_id:
-            hit_id = query.get("hit_id", [""])[0]
+            hit_id = self.get_from_query(query, ["hit_id", "hitId"])
+
         self.assignment_id = assignment_id
-        if not worker_id:
-            worker_id = query.get("worker_id", [""])[0]
         self.participant_id = participant_id
-        self.hit_id = hit_id
         self.worker_id = worker_id
+        self.hit_id = hit_id
+
         self.unique_id = worker_id + ":" + assignment_id
 
+    @staticmethod
+    def get_from_query(query, args):
+        for arg in args:
+            try:
+                return query[arg][0]
+            except KeyError:
+                pass
+
+        return ""
+
     def log(self, msg):
         logger.info("{}: {}".format(self.participant_id, msg))
 
     @cached_property
     def driver(self):
         """Returns a Selenium WebDriver instance of the type requested in the
         configuration."""
```

### Comparing `dallinger-9.5.0/dallinger/command_line/__init__.py` & `dallinger-9.6.0/dallinger/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/command_line/appdirs.py` & `dallinger-9.6.0/dallinger/command_line/appdirs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/command_line/config.py` & `dallinger-9.6.0/dallinger/command_line/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/command_line/develop.py` & `dallinger-9.6.0/dallinger/command_line/develop.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/command_line/docker.py` & `dallinger-9.6.0/dallinger/command_line/docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/command_line/docker_ssh.py` & `dallinger-9.6.0/dallinger/command_line/docker_ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
         ssh_host = server_info["host"]
         ssh_user = server_info.get("user")
         executor = Executor(ssh_host, user=ssh_user, app=app)
         # Prepare a tunnel to be able to pass a postgresql URL to the databse
         # on the remote docker container. First we need to find the IP of the
         # container running docker
         postgresql_remote_ip = executor.run(
-            "docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' dallinger_postgresql_1"
+            "docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' dallinger-postgresql-1"
         ).strip()
         # Now we start the tunnel
         tunnel = SSHTunnelForwarder(
             ssh_host,
             ssh_username=ssh_user,
             remote_bind_address=(postgresql_remote_ip, 5432),
         )
```

### Comparing `dallinger-9.5.0/dallinger/command_line/utils.py` & `dallinger-9.6.0/dallinger/command_line/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/config.py` & `dallinger-9.6.0/dallinger/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/data.py` & `dallinger-9.6.0/dallinger/data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/default_configs/global_config_defaults.txt` & `dallinger-9.6.0/dallinger/default_configs/global_config_defaults.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/deployment.py` & `dallinger-9.6.0/dallinger/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/dev_server/app.py` & `dallinger-9.6.0/dallinger/dev_server/app.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/docker/deployment.py` & `dallinger-9.6.0/dallinger/docker/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/docker/docker-compose.yml.j2` & `dallinger-9.6.0/dallinger/docker/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2` & `dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/docker/ssh_templates/docker-compose-server.yml` & `dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-server.yml`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/docker/tools.py` & `dallinger-9.6.0/dallinger/docker/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/docker/wheel_filename.py` & `dallinger-9.6.0/dallinger/docker/wheel_filename.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/experiment.py` & `dallinger-9.6.0/dallinger/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,36 +13,43 @@
 import uuid
 import warnings
 from collections import Counter, OrderedDict
 from contextlib import contextmanager
 from functools import wraps
 from importlib import import_module
 from operator import itemgetter
+from typing import List, Optional, Union
 
 import requests
 from cached_property import cached_property
 from flask import Blueprint
-from sqlalchemy import and_, create_engine, distinct, func
-from sqlalchemy.orm import scoped_session, sessionmaker
+from sqlalchemy import Table, and_, create_engine, func
+from sqlalchemy.orm import scoped_session, sessionmaker, undefer
 from sqlalchemy.orm.exc import MultipleResultsFound, NoResultFound
 
-from dallinger import models, recruiters
+from dallinger import db, models, recruiters
 from dallinger.config import LOCAL_CONFIG, get_config, initialize_experiment_package
 from dallinger.data import (
     Data,
     export,
     find_experiment_export,
     ingest_zip,
     is_registered,
 )
 from dallinger.data import load as data_load
-from dallinger.db import db_url, init_db
+from dallinger.db import (
+    Base,
+    db_url,
+    get_mapped_class,
+    get_polymorphic_mapping,
+    init_db,
+)
 from dallinger.heroku.tools import HerokuApp
 from dallinger.information import Gene, Meme, State
-from dallinger.models import Info, Network, Node, Participant, Transformation, Vector
+from dallinger.models import Info, Network, Node, Participant, Transformation
 from dallinger.networks import Empty
 from dallinger.nodes import Agent, Environment, Source
 from dallinger.transformations import Compression, Mutation, Replication, Response
 from dallinger.utils import deferred_route_decorator, struct_to_html
 
 logger = logging.getLogger(__file__)
 
@@ -973,125 +980,150 @@
                     ("count", transformations.count()),
                     ("failed", transformations.filter_by(failed=True).count()),
                 )
             )
 
         return stats
 
-    @staticmethod
-    def count_active_complete_failed(entities):
-        n_pending = 0
-        n_completed = 0
-        n_failed = 0
-        for entity in entities:
-            if entity.failed is False:
-                is_pending = (
-                    issubclass(entity.__class__, Info) and entity.contents is None
-                )
-                if is_pending:
-                    n_pending += 1
-                else:
-                    n_completed += 1
-            else:
-                n_failed += 1
-        return n_pending, n_completed, n_failed
+    def network_structure(
+        self,
+        network_roles=None,
+        network_ids=None,
+        collapsed=False,
+        transformations=False,
+    ):
+        networks = self.summarize_table("network", network_roles, network_ids)
+
+        nodes = self.summarize_table(
+            "node",
+            network_roles,
+            network_ids,
+            cls_filter=(lambda cls: issubclass(cls, Source)) if collapsed else None,
+        )
 
-    def network_structure(self, **kw):
-        network_ids = {i[0] for i in self.session.query(distinct(Network.id)).all()}
-        if "network_roles" in kw:
-            network_ids = {
-                i[0]
-                for i in self.session.query(distinct(Network.id)).filter(
-                    Network.role.in_(kw["network_roles"])
+        if collapsed:
+            vectors = []
+            infos = []
+            participants = []
+            trans = []
+        else:
+            vectors = self.summarize_table("vector", network_roles, network_ids)
+            infos = self.summarize_table("info", network_roles, network_ids)
+            participants = self.summarize_table("participant")
+
+            if transformations:
+                trans = self.summarize_table(
+                    "transformation", network_roles, network_ids
                 )
-            }
-        if "network_ids" in kw:
-            network_ids = network_ids.intersection(int(v) for v in kw["network_ids"])
+            else:
+                trans = []
 
-        network_ids = sorted(network_ids)  # default sorting is by id
+        return {
+            "networks": networks,
+            "nodes": nodes,
+            "vectors": vectors,
+            "infos": infos,
+            "participants": participants,
+            "trans": trans,
+        }
 
-        jnetworks = []
-        for network in Network.query.filter(Network.id.in_(network_ids)).all():
-            (
-                n_pending_infos,
-                n_completed_infos,
-                n_failed_infos,
-            ) = self.count_active_complete_failed(network.all_infos)
-            _, n_completed_nodes, n_failed_nodes = self.count_active_complete_failed(
-                network.all_nodes
-            )
+    def summarize_table(
+        self,
+        table: Union[Table, str],
+        network_roles: Optional[List] = None,
+        network_ids: Optional[List] = None,
+        cls_filter: Optional[callable] = None,
+    ):
+        """
+        Summarizes a given database table.
 
-            jnetworks.append(
-                {
-                    **network.__json__(),
-                    "n_pending_infos": n_pending_infos,
-                    "n_completed_infos": n_completed_infos,
-                    "n_failed_infos": n_failed_infos,
-                    "n_completed_nodes": n_completed_nodes,
-                    "n_failed_nodes": n_failed_nodes,
-                }
-            )
+        :param table: Table to be summarized
+        :param network_roles: Optionally restrict output to objects from networks with these roles
+        :param network_ids: Optionally restrict output to objects from networks with these IDs
+        :param cls_filter: Optional lambda function that returns ``False`` for classes that should be excluded
+
+        Returns a list of JSON-style dictionaries produced by calling ``.__json__()`` on every object
+        retrieved from the table.
+        """
+        objects = self.pull_table(
+            table=table,
+            polymorphic_identity=None,
+            network_roles=network_roles,
+            network_ids=network_ids,
+            cls_filter=cls_filter,
+        )
+        return [obj.__json__() for obj in objects]
 
-        if "collapsed" in kw:
-            # Collapsed view shows Source nodes only
-            jnodes = [
-                n.__json__()
-                for n in Source.query.filter(Node.network_id.in_(network_ids))
-                .order_by(Source.id)
-                .all()
-            ]
-            jinfos = jparticipants = jtransformations = jvectors = []
-        else:
-            jnodes = [
-                n.__json__()
-                for n in Node.query.filter(Node.network_id.in_(network_ids))
-                .order_by(Node.id)
-                .all()
-            ]
-            jinfos = [
-                n.__json__()
-                for n in Info.query.filter(Info.network_id.in_(network_ids))
-                .order_by(Info.id)
-                .all()
-            ]
-            # We don't filter participants because they aren't directly connected to specific networks
-            jparticipants = [
-                n.__json__() for n in Participant.query.order_by(Participant.id).all()
+    def pull_table(
+        self,
+        table: Union[Table, str],
+        polymorphic_identity: Optional[str] = None,
+        network_roles: Optional[List] = None,
+        network_ids: Optional[List] = None,
+        cls_filter: Optional[callable] = None,
+    ):
+        """
+        Downloads every object in the specified table.
+        For efficiency, the SQL queries are batched by the values of the polymorphic identity column ``type``
+        if it is present.
+
+        :param table: Table to be summarized
+        :param polymorphic_identity: Optionally restrict output to a given polymorphic identity (i.e. ``type`` value)
+        :param network_roles: Optionally restrict output to objects from networks with these roles
+        :param network_ids: Optionally restrict output to objects from networks with these IDs
+        :param cls_filter: Optional lambda function that returns ``False`` for classes that should be excluded
+
+        Returns a list of database-mapped objects.
+        """
+        if isinstance(table, str):
+            table = Base.metadata.tables[table]
+
+        if polymorphic_identity is None and "type" in table.columns:
+            observed_types = [
+                r.type for r in db.session.query(table.columns.type).distinct().all()
             ]
-            jtransformations = []
-            if kw.get("transformations"):
-                jtransformations = [
-                    n.__json__()
-                    for n in Transformation.query.filter(
-                        Transformation.network_id.in_(network_ids)
-                    )
-                    .order_by(Transformation.id)
-                    .all()
-                ]
-
-            jvectors = [
-                {
-                    "origin_id": v.origin_id,
-                    "destination_id": v.destination_id,
-                    "id": v.id,
-                    "failed": v.failed,
-                }
-                for v in Vector.query.filter(Vector.network_id.in_(network_ids))
-                .order_by(Vector.id)
-                .all()
+            obj_by_type = [
+                self.pull_table(
+                    table,
+                    polymorphic_identity=_type,
+                    network_roles=network_roles,
+                    network_ids=network_ids,
+                    cls_filter=cls_filter,
+                )
+                for _type in observed_types
             ]
+            return [obj for sublist in obj_by_type for obj in sublist]
 
-        return {
-            "networks": jnetworks,
-            "nodes": jnodes,
-            "vectors": jvectors,
-            "infos": jinfos,
-            "participants": jparticipants,
-            "trans": jtransformations,
-        }
+        if polymorphic_identity is None:
+            cls = get_mapped_class(table)
+        else:
+            assert "type" in table.columns
+            cls = get_polymorphic_mapping(table)[polymorphic_identity]
+
+        if cls_filter is not None and not cls_filter(cls):
+            return
+
+        query = cls.query
+
+        if polymorphic_identity is not None:
+            query = query.filter(cls.type == polymorphic_identity)
+
+        if network_roles is not None:
+            query = query.filter(Network.role.in_(network_roles))
+
+        if network_ids is not None:
+            query = query.filter(Network.id.in_(network_ids))
+
+        if network_roles is not None or network_ids is not None:
+            if "network_id" in table.columns:
+                query = query.join(Network, cls.network_id == Network.id)
+
+        primary_keys = [c.name for c in table.primary_key.columns]
+
+        return query.order_by(*primary_keys).options(undefer("*")).all()
 
     def node_visualization_options(self):
         """Provides custom vis.js configuration options for the
         Network Monitoring Dashboard.
 
         :returns: A dict with `vis.js option values <https://visjs.github.io/vis-network/docs/network/#options>`__
         """
@@ -1112,48 +1144,53 @@
         model = getattr(models, object_type, None)
         if model is not None:
             obj = self.session.query(model).get(int(obj_id))
             if getattr(obj, "visualization_html", None):
                 return obj.visualization_html
         return ""
 
-    def table_data(self, **kw):
+    def table_data(
+        self, table: str = "participant", polymorphic_identity: Optional[str] = None
+    ):
         """Generates DataTablesJS data and configuration for the experiment. The data
         is compiled from the models' ``__json__`` methods, and can be customized by either
         overriding this method or using the ``json_data`` method on the model to return
         additional serializable data.
 
-        :param \**kw: arguments passed in from the request. The ``model_type`` parameter
-                      takes a ``str`` or iterable and queries all objects of those types,
-                      ordered by ``id``.
+        :param table: table to query
+
+        :param polymorphic_identity: optional polymorphic identity (corresponds to the ``type`` column)
+
         :returns: Returns a ``dict`` with DataTablesJS data and configuration, filters using
                   arbitrary keyword arguments. Should contain ``data`` and ``columns`` keys
                   at least, with ``columns`` containing data for all fields on all returned
                   objects.
         """  # noqa
         rows = []
         found_columns = set()
         columns = []
-        model_types = kw.get("model_type", ["Participant"])
-        if hasattr(model_types, "strip"):
-            model_types = [model_types]
-
-        for model_type in model_types:
-            model = getattr(models, model_type, None)
-            for obj in model.query.order_by(model.id).all():
-                data = obj.__json__()
-                # Add participant worker_id to data, we normally leave it out of
-                # JSON renderings
-                if model_type == "Participant":
-                    data["worker_id"] = obj.worker_id
-                rows.append(data)
-                for key in data:
-                    if key not in found_columns:
-                        columns.append({"name": key, "data": key})
-                        found_columns.add(key)
+
+        table = Base.metadata.tables[table]
+
+        if polymorphic_identity == "None":
+            polymorphic_identity = None
+
+        objects = self.pull_table(table, polymorphic_identity=polymorphic_identity)
+
+        for obj in objects:
+            data = obj.__json__()
+            # Add participant worker_id to data, we normally leave it out of
+            # JSON renderings
+            if table.name == "participant":
+                data["worker_id"] = obj.worker_id
+            rows.append(data)
+            for key in data:
+                if key not in found_columns:
+                    columns.append({"name": key, "data": key})
+                    found_columns.add(key)
 
         # Make sure every row has an entry for every column
         for col in found_columns:
             for row in rows:
                 if col not in row:
                     row[col] = None
```

### Comparing `dallinger-9.5.0/dallinger/experiment_server/dashboard.py` & `dallinger-9.6.0/dallinger/experiment_server/dashboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from tzlocal import get_localzone
 from wtforms import BooleanField, HiddenField, PasswordField, StringField, SubmitField
 from wtforms.validators import DataRequired, ValidationError
 
 import dallinger.db
 from dallinger import recruiters
 from dallinger.config import get_config
+from dallinger.db import get_all_mapped_classes
 from dallinger.heroku.tools import HerokuApp
 from dallinger.utils import deferred_route_decorator
 
 from .utils import date_handler, error_response, success_response
 
 logger = logging.getLogger(__name__)
 
@@ -197,30 +198,26 @@
         route_check = frozenset((route_name, "dashboard." + route_name))
         self.tabs = [t for t in self.tabs if t.route_name not in route_check]
 
     def __iter__(self):
         return iter(self.tabs)
 
 
-BROWSEABLE_MODELS = [
-    "Info",
-    "Network",
-    "Node",
-    "Participant",
-    "Question",
-    "Transformation",
-    "Transmission",
-    "Notification",
-]
-
-
 def database_children():
-    for model_type in BROWSEABLE_MODELS:
+    mapped_classes = list(get_all_mapped_classes().items())
+    mapped_classes.sort(key=lambda x: x[0])
+    for cls_name, cls_info in mapped_classes:
         yield DashboardTab(
-            model_type + "s", "dashboard.database", None, {"model_type": model_type}
+            cls_name,
+            "dashboard.database",
+            None,
+            {
+                "table": cls_info["table"],
+                "polymorphic_identity": cls_info["polymorphic_identity"],
+            },
         )
 
 
 dashboard_tabs = DashboardTabs(
     [
         DashboardTab("Home", "dashboard.index"),
         DashboardTab("Heroku", "dashboard.heroku"),
@@ -705,23 +702,38 @@
 
     return datatables_options
 
 
 @dashboard.route("/database")
 @login_required
 def database():
+    from dallinger.db import get_polymorphic_mapping
     from dallinger.experiment_server.experiment_server import Experiment, session
 
-    title = "Database View"
     exp = Experiment(session)
-    model_type = request.args.get("model_type")
-    if model_type:
-        title = "Database View: {}s".format(model_type)
+
+    table = request.args.get("table", None)
+    polymorphic_identity = request.args.get("polymorphic_identity", None)
+
+    if polymorphic_identity == "None":
+        polymorphic_identity = None
+
+    if table is None and polymorphic_identity is None:
+        table = "participant"
+
+    if polymorphic_identity is not None:
+        assert table is not None
+        cls = get_polymorphic_mapping(table)[polymorphic_identity]
+        label = cls.__name__
+    else:
+        label = table.capitalize()
+
+    title = "Database View: {}".format(label)
     datatables_options = prep_datatables_options(
-        exp.table_data(**request.args.to_dict(flat=False))
+        exp.table_data(**request.args.to_dict())
     )
     columns = [
         c.get("name") or c["data"]
         for c in datatables_options.get("columns", [])
         if c.get("data")
     ]
```

### Comparing `dallinger-9.5.0/dallinger/experiment_server/experiment_server.py` & `dallinger-9.6.0/dallinger/experiment_server/experiment_server.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/experiment_server/gunicorn.py` & `dallinger-9.6.0/dallinger/experiment_server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/experiment_server/replay.py` & `dallinger-9.6.0/dallinger/experiment_server/replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/experiment_server/sockets.py` & `dallinger-9.6.0/dallinger/experiment_server/sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/experiment_server/utils.py` & `dallinger-9.6.0/dallinger/experiment_server/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/experiment_server/worker_events.py` & `dallinger-9.6.0/dallinger/experiment_server/worker_events.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/experiments/__init__.py` & `dallinger-9.6.0/dallinger/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/css/bootstrap.min.css` & `dallinger-9.6.0/dallinger/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/css/dashboard.css` & `dallinger-9.6.0/dallinger/frontend/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/bootstrap.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/clipboard.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/dallinger2.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/dallinger2.test.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.test.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/network-monitor.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/network-monitor.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/popper.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/popper.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/reconnecting-websocket.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/reconnecting-websocket.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/require.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/require.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/reqwest.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/reqwest.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/spin.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/spin.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/store+json2.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/store+json2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/tracker.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/tracker.js.map` & `dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js.map`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/load-tracker.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/load-tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js` & `dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css` & `dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js` & `dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/base/ad.html` & `dallinger-9.6.0/dallinger/frontend/templates/base/ad.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/base/consent.html` & `dallinger-9.6.0/dallinger/frontend/templates/base/consent.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/base/dashboard.html` & `dallinger-9.6.0/dallinger/frontend/templates/base/dashboard.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/base/layout.html` & `dallinger-9.6.0/dallinger/frontend/templates/base/layout.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/base/questionnaire.html` & `dallinger-9.6.0/dallinger/frontend/templates/base/questionnaire.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/dashboard_database.html` & `dallinger-9.6.0/dallinger/frontend/templates/dashboard_database.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/dashboard_develop.html` & `dallinger-9.6.0/dallinger/frontend/templates/dashboard_develop.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/dashboard_home.html` & `dallinger-9.6.0/dallinger/frontend/templates/dashboard_home.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/dashboard_lifecycle.html` & `dallinger-9.6.0/dallinger/frontend/templates/dashboard_lifecycle.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/dashboard_monitor.html` & `dallinger-9.6.0/dallinger/frontend/templates/dashboard_monitor.html`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                         <label for="sortBy">Sort networks by</label>
                         <div class="input-group mb-3">
                             <select class="form-control" id="sortBy">
                                 <option value="network_id">Network ID</option>
                                 <option value="n_pending_infos">Number of pending infos</option>
                                 <option value="n_completed_infos">Number of completed infos</option>
                                 <option value="n_failed_infos">Number of failed infos</option>
-                                <option value="n_completed_nodes">Number of completed nodes</option>
+                                <option value="n_alive_nodes">Number of completed nodes</option>
                                 <option value="n_failed_nodes">Number of failed nodes</option>
                             </select>
                             <div class="input-group-append">
                                 <div class="btn-group btn-group-toggle" id="order" data-toggle="buttons">
 
                                     <label class="btn btn-secondary active">
                                         <input type="radio" name="options" checked>
```

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/dashboard_mturk.html` & `dallinger-9.6.0/dallinger/frontend/templates/dashboard_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/error-complete.html` & `dallinger-9.6.0/dallinger/frontend/templates/error-complete.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/error.html` & `dallinger-9.6.0/dallinger/frontend/templates/error.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/exit_recruiter.html` & `dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/exit_recruiter_mturk.html` & `dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/exit_recruiter_prolific.html` & `dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_prolific.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/login.html` & `dallinger-9.6.0/dallinger/frontend/templates/login.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/frontend/templates/waiting.html` & `dallinger-9.6.0/dallinger/frontend/templates/waiting.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/heroku/clock.py` & `dallinger-9.6.0/dallinger/heroku/clock.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/heroku/rq_gevent_worker.py` & `dallinger-9.6.0/dallinger/heroku/rq_gevent_worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/heroku/tools.py` & `dallinger-9.6.0/dallinger/heroku/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/jupyter.py` & `dallinger-9.6.0/dallinger/jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/models.py` & `dallinger-9.6.0/dallinger/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,20 @@
     Enum,
     Float,
     ForeignKey,
     Integer,
     String,
     Text,
     and_,
+    func,
     or_,
 )
 from sqlalchemy.dialects.postgresql import JSONB
-from sqlalchemy.orm import relationship, validates
-from sqlalchemy.sql.expression import false
+from sqlalchemy.orm import column_property, relationship, validates
+from sqlalchemy.sql.expression import false, select
 
 from .db import Base
 
 DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%f"
 
 
 def timenow():
@@ -470,20 +471,25 @@
             len(self.vectors()),
             len(self.infos()),
             len(self.transmissions()),
             len(self.transformations()),
         )
 
     def json_data(self):
-        """Return json description of a participant."""
+        """Return json description of a network."""
         return {
             "type": self.type,
             "max_size": self.max_size,
             "full": self.full,
             "role": self.role,
+            "n_pending_infos": self.n_pending_infos,
+            "n_completed_infos": self.n_completed_infos,
+            "n_failed_infos": self.n_failed_infos,
+            "n_alive_nodes": self.n_alive_nodes,
+            "n_failed_nodes": self.n_failed_nodes,
             "object_type": "Network",
         }
 
     """ ###################################
     Methods that get things about a Network
     ################################### """
 
@@ -1528,14 +1534,17 @@
 
     #: the network the info is in
     network = relationship(Network, foreign_keys=[network_id], backref="all_infos")
 
     #: the contents of the info. Must be stored as a String.
     contents = Column(Text(), default=None)
 
+    #: whether the info is 'complete', i.e. has received its contents
+    complete = Column(Boolean(), default=False)
+
     def __init__(self, origin, contents=None, details=None, failed=False):
         """Create an info."""
         # check the origin hasn't failed
         if origin.failed and not failed:
             raise ValueError(
                 "Only failed Infos can be added to {}, as it has failed".format(origin)
             )
@@ -1553,14 +1562,23 @@
     @validates("contents")
     def _write_once(self, key, value):
         existing = getattr(self, key)
         if existing is not None:
             raise ValueError("The contents of an info is write-once.")
         return value
 
+    def __setattr__(self, key, value):
+        super().__setattr__(key, value)
+        if key != "complete":
+            self.check_complete()
+
+    def check_complete(self):
+        if self.contents is not None:
+            self.complete = True
+
     def __repr__(self):
         """The string representation of an info."""
         return "Info-{}-{}".format(self.id, self.type)
 
     def json_data(self):
         """The json representation of an info."""
         return {
@@ -1845,15 +1863,70 @@
 
     # the assignment is from AWS the notification pertains to
     assignment_id = Column(String, nullable=False)
 
     # the type of notification
     event_type = Column(String, nullable=False)
 
+    def json_data(self):
+        """The json representation of a notification."""
+        return {
+            "assignment_id": self.assignment_id,
+            "event_type": self.event_type,
+        }
+
 
 class Recruitment(Base, SharedMixin):
     """A record of a request to recruit a participant."""
 
     __tablename__ = "recruitment"
 
     #: A String, the nickname of the recruiter used.
     recruiter_id = Column(String(50), nullable=True)
+
+
+Network.n_pending_infos = column_property(
+    select(func.count(Info.id))
+    .where(
+        Info.network_id == Network.id,
+        ~Info.failed,
+        ~Info.complete,
+    )
+    .scalar_subquery()
+)
+
+Network.n_completed_infos = column_property(
+    select(func.count(Info.id))
+    .where(
+        Info.network_id == Network.id,
+        ~Info.failed,
+        Info.complete,
+    )
+    .scalar_subquery()
+)
+
+Network.n_failed_infos = column_property(
+    select(func.count(Info.id))
+    .where(
+        Info.network_id == Network.id,
+        Info.failed,
+    )
+    .scalar_subquery()
+)
+
+Network.n_alive_nodes = column_property(
+    select(func.count(Node.id))
+    .where(
+        Node.network_id == Network.id,
+        ~Node.failed,
+    )
+    .scalar_subquery()
+)
+
+Network.n_failed_nodes = column_property(
+    select(func.count(Node.id))
+    .where(
+        Node.network_id == Network.id,
+        Node.failed,
+    )
+    .scalar_subquery()
+)
```

### Comparing `dallinger-9.5.0/dallinger/mturk.py` & `dallinger-9.6.0/dallinger/mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/networks.py` & `dallinger-9.6.0/dallinger/networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/nodes.py` & `dallinger-9.6.0/dallinger/nodes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/notifications.py` & `dallinger-9.6.0/dallinger/notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/processes.py` & `dallinger-9.6.0/dallinger/processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/prolific.py` & `dallinger-9.6.0/dallinger/prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/pytest_dallinger.py` & `dallinger-9.6.0/dallinger/pytest_dallinger.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/recruiters.py` & `dallinger-9.6.0/dallinger/recruiters.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,14 +378,18 @@
             "entry_information": entry_information,
         }
 
         return participant_data
 
     def recruit(self, n: int = 1):
         """Recruit `n` new participants to an existing Prolific Study"""
+        if not self.config.get("auto_recruit"):
+            logger.info("auto_recruit is False: recruitment suppressed")
+            return
+
         return self.prolificservice.add_participants_to_study(
             study_id=self.current_study_id, number_to_add=n
         )
 
     def approve_hit(self, assignment_id: str):
         """Approve a participant's assignment/submission on Prolific"""
         try:
```

### Comparing `dallinger-9.5.0/dallinger/redis_utils.py` & `dallinger-9.6.0/dallinger/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/registration.py` & `dallinger-9.6.0/dallinger/registration.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/transformations.py` & `dallinger-9.6.0/dallinger/transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger/utils.py` & `dallinger-9.6.0/dallinger/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger.egg-info/PKG-INFO` & `dallinger-9.6.0/dallinger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.5.0
+Version: 9.6.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.5.0/dallinger.egg-info/SOURCES.txt` & `dallinger-9.6.0/dallinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dallinger.egg-info/requires.txt` & `dallinger-9.6.0/dallinger.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 pandas
 tablib[all]
 
 [dev]
 alabaster
 black
 bumpversion
-codecov
 coverage
 coverage_pth
 flake8
 isort
 mock==5.0.0
 myst-parser
 pre-commit
```

### Comparing `dallinger-9.5.0/dallinger_scripts/worker.py` & `dallinger-9.6.0/dallinger_scripts/worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/dev-requirements.txt` & `dallinger-9.6.0/constraints.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    ./scripts/update_dependencies.sh
 #
 
-    # via -r dev-requirements.in
+    # via -r constraints.in
 alabaster==0.7.13
     # via
     #   dallinger
     #   sphinx
 anyio==3.6.2
     # via jupyter-server
 apscheduler==3.10.1
@@ -25,35 +25,34 @@
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 async-generator==1.10
     # via trio
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   jsonschema
     #   outcome
-    #   pytest
     #   trio
 babel==2.12.1
     # via sphinx
 backcall==0.2.0
     # via ipython
 bcrypt==4.0.1
     # via paramiko
-beautifulsoup4==4.12.0
+beautifulsoup4==4.12.2
     # via nbconvert
-black==23.1.0
+black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
-boto3==1.26.100
+boto3==1.26.115
     # via dallinger
-botocore==1.29.100
+botocore==1.29.115
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -83,32 +82,29 @@
 click==8.1.3
     # via
     #   black
     #   dallinger
     #   flask
     #   pip-tools
     #   rq
-codecov==2.1.12
-    # via dallinger
 colorama==0.4.6
     # via tox
 comm==0.1.3
     # via ipykernel
-coverage==7.2.2
+coverage==7.2.3
     # via
-    #   codecov
     #   coverage-pth
     #   dallinger
 coverage-pth==0.0.2
     # via dallinger
-cryptography==40.0.1
+cryptography==40.0.2
     # via
     #   paramiko
     #   pyopenssl
-debugpy==1.6.6
+debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via
     #   nbconvert
     #   odfpy
@@ -126,19 +122,19 @@
 exceptiongroup==1.1.1
     # via
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.3.1
+faker==18.4.0
     # via dallinger
 fastjsonschema==2.16.3
     # via nbformat
-filelock==3.10.7
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
 flask==2.2.3
     # via
@@ -171,15 +167,15 @@
     #   dallinger
     #   gevent
     #   sqlalchemy
 gunicorn==20.1.0
     # via dallinger
 h11==0.14.0
     # via wsproto
-heroku3==5.2.0
+heroku3==5.2.1
     # via dallinger
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
@@ -193,15 +189,15 @@
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
     #   nbclassic
     #   notebook
     #   qtconsole
-ipython==8.11.0
+ipython==8.12.0
     # via
     #   ipykernel
     #   ipywidgets
     #   jupyter-console
 ipython-genutils==0.2.0
     # via
     #   nbclassic
@@ -238,15 +234,15 @@
     # via jsonschema
 jsonschema==4.17.3
     # via
     #   jupyter-events
     #   nbformat
 jupyter==1.0.0
     # via dallinger
-jupyter-client==8.1.0
+jupyter-client==8.2.0
     # via
     #   ipykernel
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   notebook
@@ -306,19 +302,19 @@
     # via nbconvert
 mock==5.0.0
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==1.0.0
     # via dallinger
-nbclassic==0.5.3
+nbclassic==0.5.5
     # via notebook
-nbclient==0.7.2
+nbclient==0.7.3
     # via nbconvert
-nbconvert==7.2.10
+nbconvert==7.3.1
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
 nbformat==5.8.0
     # via
@@ -330,42 +326,42 @@
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
 nodeenv==1.7.0
     # via pre-commit
-notebook==6.5.3
+notebook==6.5.4
     # via jupyter
 notebook-shim==0.2.2
     # via nbclassic
 numpy==1.24.2
     # via pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   docker
     #   ipykernel
     #   jupyter-server
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
 paramiko==3.1.0
     # via
@@ -377,42 +373,42 @@
     # via black
 pexpect==4.8.0
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via dallinger
 platformdirs==3.2.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via dallinger
 prometheus-client==0.16.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 prompt-toolkit==3.0.38
     # via
     #   ipython
     #   jupyter-console
-psutil==5.9.4
+psutil==5.9.5
     # via
     #   dallinger
     #   ipykernel
-psycopg2==2.9.5
+psycopg2==2.9.6
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
@@ -424,15 +420,15 @@
     #   flake8
 pycparser==2.21
     # via cffi
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   ipython
     #   jupyter-console
     #   nbconvert
     #   qtconsole
     #   sphinx
 pynacl==1.5.0
@@ -445,15 +441,15 @@
     # via tox
 pyproject-hooks==1.0.0
     # via build
 pyrsistent==0.19.3
     # via jsonschema
 pysocks==1.7.1
     # via urllib3
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   dallinger
     #   pytest-rerunfailures
 pytest-rerunfailures==11.1.2
     # via dallinger
 python-dateutil==2.8.2
     # via
@@ -461,15 +457,15 @@
     #   botocore
     #   faker
     #   heroku3
     #   jupyter-client
     #   pandas
 python-json-logger==2.0.7
     # via jupyter-events
-pytz==2023.2
+pytz==2023.3
     # via
     #   apscheduler
     #   pandas
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
 pyyaml==6.0
     # via
@@ -482,25 +478,24 @@
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   qtconsole
-qtconsole==5.4.1
+qtconsole==5.4.2
     # via jupyter
-qtpy==2.3.0
+qtpy==2.3.1
     # via qtconsole
-redis==4.5.3
+redis==4.5.4
     # via
     #   dallinger
     #   rq
 requests==2.28.2
     # via
-    #   codecov
     #   dallinger
     #   docker
     #   heroku3
     #   sphinx
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
@@ -533,15 +528,15 @@
     # via
     #   anyio
     #   trio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via trio
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
 sphinx==6.1.3
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
@@ -596,23 +591,23 @@
     # via
     #   black
     #   build
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tornado==6.2
+tornado==6.3
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.8
+tox==4.4.12
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -630,16 +625,18 @@
     #   qtconsole
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.2
     # via selenium
-tzdata==2023.2
-    # via pytz-deprecation-shim
+tzdata==2023.3
+    # via
+    #   pandas
+    #   pytz-deprecation-shim
 tzlocal==4.3
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
     #   dallinger
```

### Comparing `dallinger-9.5.0/docs/Makefile` & `dallinger-9.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/make.bat` & `dallinger-9.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.eot` & `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.eot`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.svg` & `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.svg`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf` & `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/AvenirLTStd-Book_gdi.woff` & `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.woff`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/Dallinger AWS Group.png` & `dallinger-9.6.0/docs/source/_static/Dallinger AWS Group.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/barplot.png` & `dallinger-9.6.0/docs/source/_static/barplot.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/burst.png` & `dallinger-9.6.0/docs/source/_static/burst.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/chain.png` & `dallinger-9.6.0/docs/source/_static/chain.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/class_chart.jpg` & `dallinger-9.6.0/docs/source/_static/class_chart.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/corner.jpg` & `dallinger-9.6.0/docs/source/_static/corner.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/custom.css` & `dallinger-9.6.0/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/delayed.png` & `dallinger-9.6.0/docs/source/_static/delayed.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/directories.jpg` & `dallinger-9.6.0/docs/source/_static/directories.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/empty.jpg` & `dallinger-9.6.0/docs/source/_static/empty.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/front_back_layout.jpg` & `dallinger-9.6.0/docs/source/_static/front_back_layout.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/full.png` & `dallinger-9.6.0/docs/source/_static/full.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/grid.png` & `dallinger-9.6.0/docs/source/_static/grid.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/grid_mini.png` & `dallinger-9.6.0/docs/source/_static/grid_mini.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/grid_small.png` & `dallinger-9.6.0/docs/source/_static/grid_small.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/heroku.jpg` & `dallinger-9.6.0/docs/source/_static/heroku.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/_static/star.png` & `dallinger-9.6.0/docs/source/_static/star.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/aws_etc_keys.rst` & `dallinger-9.6.0/docs/source/aws_etc_keys.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/build_demo_docs.py` & `dallinger-9.6.0/docs/source/build_demo_docs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/building_documentation.rst` & `dallinger-9.6.0/docs/source/building_documentation.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/classes.rst` & `dallinger-9.6.0/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/command_line_utility.rst` & `dallinger-9.6.0/docs/source/command_line_utility.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/communicating_with_the_server.rst` & `dallinger-9.6.0/docs/source/communicating_with_the_server.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/conf.py` & `dallinger-9.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/configuration.rst` & `dallinger-9.6.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/contributing_to_dallinger.rst` & `dallinger-9.6.0/docs/source/contributing_to_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/creating_an_experiment.rst` & `dallinger-9.6.0/docs/source/creating_an_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/demo_index.rst` & `dallinger-9.6.0/docs/source/demo_index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/demoing_dallinger.rst` & `dallinger-9.6.0/docs/source/demoing_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/demos_on_heroku.rst` & `dallinger-9.6.0/docs/source/demos_on_heroku.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/developing_dallinger_setup_guide.rst` & `dallinger-9.6.0/docs/source/developing_dallinger_setup_guide.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/docker_only.rst` & `dallinger-9.6.0/docs/source/docker_only.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/docker_support.rst` & `dallinger-9.6.0/docs/source/docker_support.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/docker_tutorial.rst` & `dallinger-9.6.0/docs/source/docker_tutorial.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/email_setup.rst` & `dallinger-9.6.0/docs/source/email_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/experiment_data.rst` & `dallinger-9.6.0/docs/source/experiment_data.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/extra_configuration.rst` & `dallinger-9.6.0/docs/source/extra_configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/index.rst` & `dallinger-9.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/installing_dallinger_for_users.rst` & `dallinger-9.6.0/docs/source/installing_dallinger_for_users.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/javascript_api.rst` & `dallinger-9.6.0/docs/source/javascript_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/learning_to_use_dallinger.rst` & `dallinger-9.6.0/docs/source/learning_to_use_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/monitoring_a_live_experiment.rst` & `dallinger-9.6.0/docs/source/monitoring_a_live_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/networks.rst` & `dallinger-9.6.0/docs/source/networks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/postico_and_postgres.rst` & `dallinger-9.6.0/docs/source/postico_and_postgres.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/private_repo.rst` & `dallinger-9.6.0/docs/source/private_repo.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/python_module.rst` & `dallinger-9.6.0/docs/source/python_module.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/recruitment.rst` & `dallinger-9.6.0/docs/source/recruitment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/required_experiment_files.rst` & `dallinger-9.6.0/docs/source/required_experiment_files.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/rewarding_participants.rst` & `dallinger-9.6.0/docs/source/rewarding_participants.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/running_bots.rst` & `dallinger-9.6.0/docs/source/running_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/running_the_tests.rst` & `dallinger-9.6.0/docs/source/running_the_tests.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/scheduled_tasks.rst` & `dallinger-9.6.0/docs/source/scheduled_tasks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/spelling_wordlist.txt` & `dallinger-9.6.0/docs/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/the_experiment_class.rst` & `dallinger-9.6.0/docs/source/the_experiment_class.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/troubleshooting.rst` & `dallinger-9.6.0/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/vagrant_setup.rst` & `dallinger-9.6.0/docs/source/vagrant_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/waiting_rooms.rst` & `dallinger-9.6.0/docs/source/waiting_rooms.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/web_api.rst` & `dallinger-9.6.0/docs/source/web_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/docs/source/writing_bots.rst` & `dallinger-9.6.0/docs/source/writing_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/incubator.png` & `dallinger-9.6.0/incubator.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/requirements.txt` & `dallinger-9.6.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     # via -r requirements.in
 apscheduler==3.10.1
     # via dallinger
 async-generator==1.10
     # via trio
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   outcome
     #   trio
-boto3==1.26.100
+boto3==1.26.115
     # via dallinger
-botocore==1.29.100
+botocore==1.29.115
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -38,21 +38,21 @@
     # via requests
 click==8.1.3
     # via
     #   dallinger
     #   flask
     #   pip-tools
     #   rq
-cryptography==40.0.1
+cryptography==40.0.2
     # via pyopenssl
 exceptiongroup==1.1.1
     # via
     #   trio
     #   trio-websocket
-faker==18.3.1
+faker==18.4.0
     # via dallinger
 flask==2.2.3
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
@@ -79,15 +79,15 @@
     #   dallinger
     #   gevent
     #   sqlalchemy
 gunicorn==20.1.0
     # via dallinger
 h11==0.14.0
     # via wsproto
-heroku3==5.2.0
+heroku3==5.2.1
     # via dallinger
 idna==3.4
     # via
     #   requests
     #   trio
 itsdangerous==2.1.2
     # via
@@ -104,23 +104,23 @@
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
     #   wtforms
 outcome==1.2.0
     # via trio
-packaging==23.0
+packaging==23.1
     # via build
 pexpect==4.8.0
     # via dallinger
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via dallinger
-psutil==5.9.4
+psutil==5.9.5
     # via dallinger
-psycopg2==2.9.5
+psycopg2==2.9.6
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 ptyprocess==0.7.0
     # via pexpect
 pycparser==2.21
     # via cffi
@@ -131,19 +131,19 @@
 pysocks==1.7.1
     # via urllib3
 python-dateutil==2.8.2
     # via
     #   botocore
     #   faker
     #   heroku3
-pytz==2023.2
+pytz==2023.3
     # via apscheduler
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
-redis==4.5.3
+redis==4.5.4
     # via
     #   dallinger
     #   rq
 requests==2.28.2
     # via
     #   dallinger
     #   heroku3
@@ -181,15 +181,15 @@
     #   pyproject-hooks
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.2
     # via selenium
-tzdata==2023.2
+tzdata==2023.3
     # via pytz-deprecation-shim
 tzlocal==4.3
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
```

### Comparing `dallinger-9.5.0/setup.py` & `dallinger-9.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 
 setup_args = dict(
     name="dallinger",
     packages=["dallinger", "dallinger_scripts"],
-    version="9.5.0",
+    version="9.6.0",
     description="Laboratory automation for the behavioral and social sciences",
     long_description=README,
     long_description_content_type="text/markdown",
     url="http://github.com/Dallinger/Dallinger",
     maintainer="Jordan Suchow",
     maintainer_email="suchow@berkeley.edu",
     license="MIT",
@@ -93,15 +93,14 @@
             "pandas",
             "tablib[all]",
         ],
         "dev": [
             "alabaster",
             "black",
             "bumpversion",
-            "codecov",
             "coverage",
             "coverage_pth",
             "flake8",
             "isort",
             "mock==5.0.0",
             "myst-parser",
             "pre-commit",
```

### Comparing `dallinger-9.5.0/tests/test_agents.py` & `dallinger-9.6.0/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_api.py` & `dallinger-9.6.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_bots.py` & `dallinger-9.6.0/tests/test_bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_cli_config.py` & `dallinger-9.6.0/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_command_line.py` & `dallinger-9.6.0/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_config.py` & `dallinger-9.6.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_dashboard.py` & `dallinger-9.6.0/tests/test_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,14 +497,15 @@
         source2 = a.source(network=network2)
         info1 = a.info(origin=source, contents="contents1")
         info2 = a.info(origin=source, contents="contents2")
         info3 = a.info(origin=source2, contents="contents3")
         info4 = a.info(origin=source2, contents="contents3")
         a.transformation(info_in=info1, info_out=info2)
         a.transformation(info_in=info3, info_out=info4)
+        db_session.commit()
         yield exp
 
     def test_network_structure(self, a, db_session):
         from dallinger.experiment_server.experiment_server import Experiment
         from dallinger.models import Network
 
         exp = Experiment(db_session)
@@ -677,55 +678,55 @@
 
 @pytest.mark.usefixtures("experiment_dir_merged")
 class TestDashboardDatabase(object):
     def test_requires_login(self, webapp):
         assert webapp.get("/dashboard/database").status_code == 401
 
     def test_render(self, active_config, webapp_admin):
-        resp = webapp_admin.get("/dashboard/database?model_type=Network")
+        resp = webapp_admin.get("/dashboard/database?table=network")
 
         assert resp.status_code == 200
-        assert "<h1>Database View: Networks</h1>" in resp.data.decode("utf8")
+        assert "<h1>Database View: Network</h1>" in resp.data.decode("utf8")
 
     def test_table_data(self, a, db_session):
         from dallinger.experiment_server.experiment_server import Experiment
         from dallinger.models import Network
 
         exp = Experiment(db_session)
 
         network = Network.query.all()[0]
 
-        table = exp.table_data(model_type=["Network"])
+        table = exp.table_data(table="network")
         assert len(table["data"]) == 1
         assert table["data"][0]["id"] == network.id
         assert table["data"][0]["role"] == network.role
         assert len(table["columns"]) > 2
         for col in table["columns"]:
             if col["data"] == "role":
                 assert col == {"data": "role", "name": "role"}
                 break
         else:
             raise KeyError("'role' not in Network columns")
 
         source = a.source(network=network)
 
-        table = exp.table_data(model_type="Node")
+        table = exp.table_data(table="node")
         assert len(table["data"]) == 1
         assert table["data"][0]["id"] == source.id
         assert table["data"][0]["type"] == source.type
         assert len(table["columns"]) > 2
         for col in table["columns"]:
             if col["data"] == "id":
                 assert col == {"data": "id", "name": "id"}
                 break
         else:
             raise KeyError("'id' not in Node columns")
 
         p = a.participant()
-        table = exp.table_data(model_type="Participant")
+        table = exp.table_data(table="participant")
         assert len(table["data"]) == 1
         assert table["data"][0]["id"] == p.id
         assert table["data"][0]["type"] == p.type
         assert table["data"][0]["worker_id"] == p.worker_id
         assert table["data"][0]["recruiter"] == p.recruiter_id
         assert len(table["columns"]) == len(table["data"][0])
 
@@ -878,15 +879,15 @@
         assert row2["col1_display"] == "&lt;script&gt;alert();&lt;/script&gt;"
 
     def test_database_output(self, a, active_config, mock_renderer):
         import json
 
         webapp, renderer = mock_renderer
         p = a.participant()
-        webapp.get("/dashboard/database?model_type=Participant")
+        webapp.get("/dashboard/database?table=participant")
         renderer.assert_called_once()
         render_args = renderer.call_args[1]
         dt_options = json.loads(render_args["datatables_options"])
         # We have two sets of buttons, exports and actions
         exports = dt_options["buttons"][0]
         actions = dt_options["buttons"][1]
         assert actions["text"] == "Actions"
@@ -910,34 +911,34 @@
         assert participant_data["id"] == p.id
         assert participant_data["object_type"] == "Participant"
         assert participant_data["assignment_id"] == p.assignment_id
 
     def test_actions_with_mturk(self, a, active_config, mock_renderer):
         webapp, renderer = mock_renderer
         active_config.extend({"mode": "live", "recruiter": "mturk"})
-        webapp.get("/dashboard/database?model_type=Participant")
+        webapp.get("/dashboard/database?table=participant")
         render_args = renderer.call_args[1]
         assert render_args["is_sandbox"] is False
 
         active_config.extend({"mode": "sandbox", "recruiter": "mturk"})
-        webapp.get("/dashboard/database?model_type=Participant")
+        webapp.get("/dashboard/database?table=participant")
         render_args = renderer.call_args[1]
         assert render_args["is_sandbox"] is True
 
     def test_output_with_custom_actions(self, a, active_config, mock_renderer):
         import json
 
         webapp, renderer = mock_renderer
         with mock.patch(
             "dallinger.experiment.Experiment.dashboard_database_actions"
         ) as actions:
             actions.return_value = [
                 {"name": "special_action", "title": "Special Action"}
             ]
-            webapp.get("/dashboard/database?model_type=Participant")
+            webapp.get("/dashboard/database?table=participant")
             render_args = renderer.call_args[1]
             dt_options = json.loads(render_args["datatables_options"])
             actions = dt_options["buttons"][1]
             assert actions["buttons"] == [
                 {
                     "extend": "route_action",
                     "text": "Special Action",
```

### Comparing `dallinger-9.5.0/tests/test_data.py` & `dallinger-9.6.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_db.py` & `dallinger-9.6.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_demos.py` & `dallinger-9.6.0/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_deployment.py` & `dallinger-9.6.0/tests/test_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -982,15 +982,14 @@
         )
         p.logfile = sys.stdout
         try:
             p.expect_exact("Server is running", timeout=240)
             p.expect_exact("Recruitment is complete", timeout=180)
             p.expect_exact("'status': 'success'", timeout=120)
             p.expect_exact("Experiment completed", timeout=10)
-            p.expect_exact("Container bartlett1932-web-1         Stopped", timeout=30)
             p.expect(pexpect.EOF)
         finally:
             try:
                 p.sendcontrol("c")
                 p.read()
             except IOError:
                 pass
@@ -1014,15 +1013,14 @@
             p.expect("New participant requested.*", 50)
             Bot(re.search("http://[^ \n\r]+", p.after).group()).run_experiment()
             p.expect("New participant requested.*", 50)
             Bot(re.search("http://[^ \n\r]+", p.after).group()).run_experiment()
             p.expect_exact("Recruitment is complete", timeout=240)
             p.expect_exact("'status': 'success'", timeout=120)
             p.expect_exact("Experiment completed", timeout=20)
-            p.expect_exact("Container bartlett1932-web-1         Stopped", timeout=20)
             p.expect(pexpect.EOF)
         finally:
             try:
                 p.sendcontrol("c")
                 p.read()
             except IOError:
                 pass
```

### Comparing `dallinger-9.5.0/tests/test_docker.py` & `dallinger-9.6.0/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_environments.py` & `dallinger-9.6.0/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_experiment.py` & `dallinger-9.6.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_experiment_server.py` & `dallinger-9.6.0/tests/test_experiment_server.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_griduniverse.py` & `dallinger-9.6.0/tests/test_griduniverse.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_heroku.py` & `dallinger-9.6.0/tests/test_heroku.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_information.py` & `dallinger-9.6.0/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_jupyter.py` & `dallinger-9.6.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_models.py` & `dallinger-9.6.0/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 from datetime import datetime
 
 import six
 from pytest import mark, raises
 
 from dallinger import models, nodes
+from dallinger.db import Base, get_all_mapped_classes, get_polymorphic_mapping
 from dallinger.information import Gene
 from dallinger.nodes import Agent, Source
 from dallinger.transformations import Mutation
 
 
 @mark.slow
 class TestModels(object):
@@ -104,14 +105,19 @@
             "time_of_death": None,
             "property1": None,
             "property2": None,
             "property3": None,
             "property4": None,
             "property5": None,
             "details": {},
+            "n_alive_nodes": 3,
+            "n_failed_nodes": 0,
+            "n_completed_infos": 2,
+            "n_pending_infos": 0,
+            "n_failed_infos": 0,
             "object_type": "Network",
         }
 
         # test nodes()
         for n in [node, agent, source]:
             assert n in net.nodes()
 
@@ -751,7 +757,64 @@
         participant_json = participant.__json__()
         assert "details" in participant_json
         assert participant_json["details"].get("data") == "something"
 
         # make sure private data is not in there
         assert "unique_id" not in participant_json
         assert "worker_id" not in participant_json
+
+    def test_get_all_mapped_classes(self, db_session):
+        net = models.Network()
+        participant = models.Participant(
+            recruiter_id="hotair",
+            worker_id=str(1),
+            hit_id=str(1),
+            assignment_id=str(1),
+            mode="test",
+        )
+
+        db_session.add(net)
+        db_session.add(participant)
+        db_session.commit()
+
+        node = models.Node(network=net)
+        agent = Agent(network=net, participant=participant)
+        source = Source(network=net)
+
+        db_session.add(node)
+        db_session.add(agent)
+        db_session.add(source)
+        db_session.commit()
+
+        classes = get_all_mapped_classes()
+
+        assert classes["Participant"] == {
+            "cls": models.Participant,
+            "table": "participant",
+            "polymorphic_identity": "participant",
+        }
+
+        assert classes["Source"] == {
+            "cls": Source,
+            "table": "node",
+            "polymorphic_identity": "generic_source",
+        }
+
+        assert classes["Agent"] == {
+            "cls": Agent,
+            "table": "node",
+            "polymorphic_identity": "agent",
+        }
+
+        assert classes["Node"] == {
+            "cls": models.Node,
+            "table": "node",
+            "polymorphic_identity": "node",
+        }
+
+    def test_get_polymorphic_mapping(self, db_session):
+        table = Base.metadata.tables["node"]
+        mappers = get_polymorphic_mapping(table)
+
+        assert mappers["generic_source"] == Source
+        assert mappers["agent"] == Agent
+        assert mappers["node"] == models.Node
```

### Comparing `dallinger-9.5.0/tests/test_mturk.py` & `dallinger-9.6.0/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_networks.py` & `dallinger-9.6.0/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_notifications.py` & `dallinger-9.6.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_processes.py` & `dallinger-9.6.0/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_prolific.py` & `dallinger-9.6.0/tests/test_prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_recruiters.py` & `dallinger-9.6.0/tests/test_recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_replay.py` & `dallinger-9.6.0/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_replay_state.py` & `dallinger-9.6.0/tests/test_replay_state.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_sockets.py` & `dallinger-9.6.0/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_sources.py` & `dallinger-9.6.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_transformations.py` & `dallinger-9.6.0/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.5.0/tests/test_utils.py` & `dallinger-9.6.0/tests/test_utils.py`

 * *Files identical despite different names*


# Comparing `tmp/bobocep-0.35.0.tar.gz` & `tmp/bobocep-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bobocep-0.35.0.tar", last modified: Tue Nov 19 14:49:18 2019, max compression
+gzip compressed data, was "bobocep-1.0.1.tar", last modified: Wed Apr 19 14:34:22 2023, max compression
```

## Comparing `bobocep-0.35.0.tar` & `bobocep-1.0.1.tar`

### file list

```diff
@@ -1,137 +1,81 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3627 2019-11-19 14:49:18.000000 bobocep-0.35.0/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2563 2019-11-19 14:47:50.000000 bobocep-0.35.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      126 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/decider/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9406 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/bobo_decider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4136 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/bobo_decider_builder.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/decider/buffers/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/buffers/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4298 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/buffers/match_event.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12527 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/buffers/shared_versioned_match_buffer.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      446 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/decider_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/decider/handlers/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/handlers/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15897 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/handlers/bobo_nfa_handler.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2569 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/handlers/nfa_handler_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/decider/runs/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/runs/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    16499 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/runs/bobo_run.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2974 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/runs/run_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/decider/versions/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/versions/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7296 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/decider/versions/run_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/forwarder/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/forwarder/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/forwarder/action_forwarder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3243 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/forwarder/bobo_forwarder.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      642 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/forwarder/forwarder_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/producer/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/producer/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1164 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/producer/action_producer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4089 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/producer/bobo_producer.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      992 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/producer/producer_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/receiver/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3094 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/bobo_receiver.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/receiver/clocks/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/clocks/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      297 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/clocks/epoch_ns_clock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/receiver/formatters/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/formatters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      556 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/formatters/primitive_event_formatter.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/receiver/generators/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/generators/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/generators/bobo_null_data_generator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/receiver/generators/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/generators/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      297 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/generators/data/bobo_null_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      285 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/generators/data/bobo_null_data_none.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      338 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/generators/data/bobo_null_data_static.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      649 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/receiver_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/receiver/validators/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/validators/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/validators/any_validator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      345 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/validators/bobo_validator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      826 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/validators/str_dict_validator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      563 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/receiver/validators/str_validator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/actions/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      396 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/action_subscriber.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3139 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/bobo_action.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/actions/multi/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/multi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      419 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/multi/multi_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/multi/sequential_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      744 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/no_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/actions/rate_limit_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10920 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/bobo_rule_builder.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/events/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/events/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2433 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/events/action_event.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1049 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/events/bobo_event.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1537 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/events/composite_event.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/events/histories/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/events/histories/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1335 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/events/histories/bobo_history.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1021 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/events/primitive_event.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/nfas/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/nfas/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1954 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/nfas/bobo_nfa.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/nfas/patterns/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/nfas/patterns/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7169 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/nfas/patterns/bobo_pattern.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1427 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/nfas/patterns/bobo_pattern_layer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/predicates/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      927 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/bobo_predicate.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1627 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/bobo_predicate_callable.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      254 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/bobo_predicate_window.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/fixed/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/fixed/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1205 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/fixed/window_fixed.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/sliding/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/sliding/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1262 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/sliding/window_sliding.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/sliding/window_sliding_first.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      722 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/predicates/windows/sliding/window_sliding_last.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/states/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/states/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2207 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/states/bobo_state.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/rules/transitions/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/transitions/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1394 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/rules/transitions/bobo_transition.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/setup/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      887 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/bobo_complex_event.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20196 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/bobo_setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/setup/distributed/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/bobo_dist_constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2548 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/bobo_dist_manager.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/setup/distributed/incoming/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/incoming/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8225 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/incoming/bobo_dist_incoming.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2969 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/incoming/dist_incoming_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/setup/distributed/outgoing/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/outgoing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8816 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/outgoing/bobo_dist_outgoing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      221 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/distributed/outgoing/dist_outgoing_subscriber.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep/setup/task/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/task/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3449 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/task/bobo_task.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1652 2019-11-19 14:47:50.000000 bobocep-0.35.0/bobocep/setup/task/bobo_task_thread.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3627 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4133 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-11-19 14:49:18.000000 bobocep-0.35.0/bobocep.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2019-11-19 14:49:18.000000 bobocep-0.35.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1063 2019-11-19 14:47:50.000000 bobocep-0.35.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.520980 bobocep-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 14:34:13.000000 bobocep-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-19 14:34:22.520980 bobocep-1.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2642 2023-04-19 14:34:13.000000 bobocep-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/bobocep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep/cep/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep/cep/action/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/action/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/action/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep/cep/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep/cep/engine/decider/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/decider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21651 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/decider/decider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/decider/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/decider/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/decider/runserial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep/cep/engine/forwarder/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/forwarder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/forwarder/forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/forwarder/pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep/cep/engine/producer/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/producer/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/producer/pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.516979 bobocep-1.0.1/bobocep/cep/engine/receiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/receiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/receiver/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/receiver/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/receiver/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/engine/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.516979 bobocep-1.0.1/bobocep/cep/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/event/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/event/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/event/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/event/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/event/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.516979 bobocep-1.0.1/bobocep/cep/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/gen/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/gen/event_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/gen/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.516979 bobocep-1.0.1/bobocep/cep/phenom/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/phenom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.516979 bobocep-1.0.1/bobocep/cep/phenom/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/phenom/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/phenom/pattern/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/phenom/pattern/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/phenom/pattern/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/cep/phenom/phenom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.516979 bobocep-1.0.1/bobocep/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.520980 bobocep-1.0.1/bobocep/dist/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/devman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29841 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/dist/tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.520980 bobocep-1.0.1/bobocep/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/setup/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-19 14:34:13.000000 bobocep-1.0.1/bobocep/setup/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:34:22.512979 bobocep-1.0.1/bobocep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-19 14:34:22.000000 bobocep-1.0.1/bobocep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-19 14:34:22.000000 bobocep-1.0.1/bobocep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:34:22.000000 bobocep-1.0.1/bobocep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:34:22.000000 bobocep-1.0.1/bobocep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 14:34:22.000000 bobocep-1.0.1/bobocep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 14:34:22.000000 bobocep-1.0.1/bobocep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 14:34:22.520980 bobocep-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-19 14:34:13.000000 bobocep-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bobocep-0.35.0/README.rst` & `bobocep-1.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,49 @@
-.. image:: https://img.shields.io/travis/r3w0p/bobocep/master.svg
-   :target: https://travis-ci.org/r3w0p/bobocep
-   :alt: Travis CI
-
-.. image:: https://coveralls.io/repos/github/r3w0p/bobocep/badge.svg?branch=master
-   :target: https://coveralls.io/github/r3w0p/bobocep?branch=master
-   :alt: Coveralls
-
-.. image:: https://img.shields.io/lgtm/alerts/g/r3w0p/bobocep.svg?logo=lgtm&logoWidth=18
-   :target: https://lgtm.com/projects/g/r3w0p/bobocep/alerts
-   :alt: LGTM Alerts
-
-.. image:: https://img.shields.io/lgtm/grade/python/github/r3w0p/bobocep
-   :target: https://lgtm.com/projects/g/r3w0p/bobocep/context:python
-   :alt: LGTM Code Quality
-
-.. image:: https://img.shields.io/github/last-commit/r3w0p/bobocep
-   :target: https://github.com/r3w0p/bobocep/graphs/commit-activity
-   :alt: Last Commit
-
-|
-
-.. image:: https://img.shields.io/pypi/v/bobocep
-   :target: https://pypi.org/project/bobocep
-   :alt: PyPI Version
-
-.. image:: https://img.shields.io/pypi/pyversions/bobocep
-   :target: https://pypi.org/project/bobocep
-   :alt: Python Versions
-
-.. image:: https://img.shields.io/github/license/r3w0p/bobocep
-   :target: https://github.com/r3w0p/bobocep/blob/master/LICENSE
-   :alt: License
-
-.. image:: https://img.shields.io/badge/docs-pages-informational
-   :target: https://r3w0p.github.io/bobocep
-   :alt: Documentation
-
-.. image:: https://img.shields.io/badge/code-github-24292e
-   :target: https://github.com/r3w0p/bobocep
-   :alt: GitHub Repository
-
-.. image:: https://img.shields.io/badge/donate-buy%20me%20a%20coffee-orange.svg
-   :target: https://www.buymeacoffee.com/r3w0p
-   :alt: Buy Me A Coffee
-
-.. image:: https://img.shields.io/badge/donate-PayPal-blue.svg
-   :target: https://www.paypal.me/apowpow
-   :alt: PayPal
-
-|
-
-:code:`bobocep` is a `complex event processing <https://en.wikipedia.org/wiki/Complex_event_processing>`_ (CEP) engine
-designed for `edge computing <https://en.wikipedia.org/wiki/Edge_computing>`_ in
-`Internet of Things <https://en.wikipedia.org/wiki/Internet_of_things>`_ (IoT) systems
-to provide inferential reasoning and decision making using stream data.
-It provides `fault tolerance <https://en.wikipedia.org/wiki/Fault_tolerance>`_ (FT) via the
-`active replication <https://en.wikipedia.org/wiki/Replication_(computing)>`_ of
-partially-completed complex events across multiple instances of the software using a
-`message broker <https://en.wikipedia.org/wiki/Message_broker>`_.
+# BoboCEP
 
-This is **experimental** software that is currently being used for research purposes.
-All aspects of the software are subject to change.
+[![CICD](https://github.com/r3w0p/bobocep/actions/workflows/cicd.yml/badge.svg)](
+https://github.com/r3w0p/bobocep/actions/workflows/cicd.yml)
+[![Security](https://github.com/r3w0p/bobocep/actions/workflows/security.yml/badge.svg)](
+https://github.com/r3w0p/bobocep/actions/workflows/security.yml)
+[![Documentation Status](https://readthedocs.org/projects/bobocep/badge/?version=latest)](
+https://bobocep.readthedocs.io/)
+[![License Scan](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fr3w0p%2Fbobocep.svg?type=shield)](
+https://app.fossa.com/projects/git%2Bgithub.com%2Fr3w0p%2Fbobocep?ref=badge_shield)
+[![Donate](https://img.shields.io/badge/donate-ko--fi-red?label=donate)](
+https://ko-fi.com/r3w0p)
+<br/>
+
+[![License](https://img.shields.io/github/license/r3w0p/bobocep?color=blue&label=license)](
+https://github.com/r3w0p/bobocep/blob/main/LICENSE/)
+[![PyPI](https://img.shields.io/pypi/v/bobocep?color=blue&label=pypi)](
+https://pypi.org/project/bobocep/)
+[![Python](https://img.shields.io/pypi/pyversions/bobocep?color=blue&label=python)](
+https://pypi.org/project/bobocep/)
+[![Repo Size](https://img.shields.io/github/repo-size/r3w0p/bobocep?label=repo%20size)](
+https://github.com/r3w0p/bobocep/pulse/)
+<br/>
+
+[![Issues](https://img.shields.io/github/issues/r3w0p/bobocep?label=issues)](
+https://github.com/r3w0p/bobocep/issues/)
+[![Dependencies](https://img.shields.io/librariesio/github/r3w0p/bobocep?label=dependencies)](
+https://libraries.io/pypi/bobocep/)
+[![Coverage](https://img.shields.io/codeclimate/coverage/r3w0p/bobocep?label=coverage)](
+https://codeclimate.com/github/r3w0p/bobocep/)
+[![Maintainability](https://img.shields.io/codeclimate/maintainability/r3w0p/bobocep?label=maintainability)](
+https://codeclimate.com/github/r3w0p/bobocep/)
+
+
+`BoboCEP` is a [Complex Event Processing](https://en.wikipedia.org/wiki/Complex_event_processing) (CEP) engine
+designed for [edge computing](https://en.wikipedia.org/wiki/Edge_computing) in
+[Internet of Things](https://en.wikipedia.org/wiki/Internet_of_things) (IoT) systems
+to facilitate inferential reasoning and decision-making on streaming data.
+It provides [fault tolerance](https://en.wikipedia.org/wiki/Fault_tolerance) (FT) via the
+[active replication](https://en.wikipedia.org/wiki/Replication_(computing)) of
+partially-completed complex events across multiple instances of the software.
+
+
+## License
+
+`BoboCEP` is open source, as per
+[The Open Source Definition](https://opensource.org/osd).
+The code in this repository can be redistributed and/or modified under the terms of the 
+[MIT License](https://github.com/r3w0p/bobocep/blob/main/LICENSE).
```

### Comparing `bobocep-0.35.0/bobocep/decider/bobo_decider.py` & `bobocep-1.0.1/bobocep/cep/engine/decider/run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,279 +1,324 @@
-from queue import Queue
-from typing import List
+# Copyright (c) 2019-2023 r3w0p
+# The following code can be redistributed and/or
+# modified under the terms of the MIT License.
+
+"""
+A run.
+"""
+
+from threading import RLock
+from typing import Dict, Tuple, List
+
+from bobocep import BoboError
+from bobocep.cep.engine.decider.runserial import BoboRunSerial
+from bobocep.cep.event import BoboHistory, BoboEvent
+from bobocep.cep.phenom.pattern.pattern import BoboPattern, \
+    BoboPatternBlock, BoboPredicate
+
+_EXC_RUN_ID_LEN = "run ID must have a length greater than 0"
+_EXC_PHENOM_LEN = "phenomenon name must have a length greater than 0"
+_EXC_INDEX = "block index must be greater than 1"
+_EXC_HISTORY_LEN = "history must have at least 1 event"
 
-from bobocep.decider.decider_subscriber import IDeciderSubscriber
-from bobocep.decider.handlers.bobo_nfa_handler import BoboNFAHandler
-from bobocep.decider.handlers.nfa_handler_subscriber import \
-    INFAHandlerSubscriber
-from bobocep.producer.producer_subscriber import IProducerSubscriber
-from bobocep.receiver.receiver_subscriber import IReceiverSubscriber
-from bobocep.rules.events.action_event import ActionEvent
-from bobocep.rules.events.bobo_event import BoboEvent
-from bobocep.rules.events.composite_event import CompositeEvent
-from bobocep.setup.distributed.incoming.dist_incoming_subscriber import \
-    IDistIncomingSubscriber
-from bobocep.setup.task.bobo_task import BoboTask
-
-
-class BoboDecider(BoboTask,
-                  IReceiverSubscriber,
-                  IProducerSubscriber,
-                  INFAHandlerSubscriber,
-                  IDistIncomingSubscriber):
-    """A :code:`bobocep` data decider.
-
-    :param max_queue_size: The maximum data queue size,
-                           defaults to 0 (infinite).
-    :type max_queue_size: int, optional
-
-    :param active: Whether task should start in an active state,
-                   defaults to True.
-    :type active: bool, optional
+
+class BoboRunError(BoboError):
+    """
+    A run error.
+    """
+
+
+class BoboRun:
+    """
+    A run that tracks the progress of a partially completed complex event.
     """
 
     def __init__(self,
-                 recursive: bool = True,
-                 max_queue_size: int = 0,
-                 active: bool = True) -> None:
-        super().__init__(active=active)
+                 run_id: str,
+                 phenomenon_name: str,
+                 pattern: BoboPattern,
+                 block_index: int,
+                 history: BoboHistory):
+        """
+        :param run_id: An ID for the run.
+        :param phenomenon_name: A phenomenon name associated with the run.
+        :param pattern: A pattern associated with the run.
+        :param block_index: An index which indicates where in the pattern
+            to start the run.
+        :param history: A history of events for the run.
+
+        :raises BoboRunError: Run ID length is equal to 0.
+        :raises BoboRunError: Process name length is equal to 0.
+        :raises BoboRunError: Block index is less than 1.
+        :raises BoboRunError: History does not have enough events in it
+            to cover all blocks up to the block index.
+        """
+        super().__init__()
+        self._lock: RLock = RLock()
 
-        self._recursive = recursive
-        self._event_queue = Queue(maxsize=max_queue_size)
-        self._nfa_handlers = {}
-        self._subs = {}
+        if len(run_id) == 0:
+            raise BoboRunError(_EXC_RUN_ID_LEN)
 
-    def _loop(self) -> None:
-        try:
-            if not self._event_queue.empty():
-                event = self._event_queue.get_nowait()
+        if len(phenomenon_name) == 0:
+            raise BoboRunError(_EXC_PHENOM_LEN)
 
-                if event is not None:
-                    for nfa_handler in self._nfa_handlers.values():
-                        nfa_handler.process(event)
+        if block_index < 1:
+            raise BoboRunError(_EXC_INDEX)
+
+        if history.size() < 1:
+            raise BoboRunError(_EXC_HISTORY_LEN)
+
+        self._run_id: str = run_id
+        self._phenomenon_name: str = phenomenon_name
+        self._pattern: BoboPattern = pattern
+        self._block_index: int = block_index
+        self._history: BoboHistory = history
+        self._halted: bool = self.is_complete()
 
-        except Exception:
-            pass
+    @property
+    def run_id(self) -> str:
+        """
+        :return: The run ID.
+        """
+        return self._run_id
 
-    def add_nfa_handler(self, nfa_handler: BoboNFAHandler) -> None:
+    @property
+    def phenomenon_name(self) -> str:
         """
-        Adds a new NFA handler to the decider.
+        :return: The phenomenon name associated with the run.
+        """
+        return self._phenomenon_name
 
-        :param nfa_handler: The NFA handler to add.
-        :type nfa_handler: BoboNFAHandler
+    @property
+    def pattern(self) -> BoboPattern:
+        """
+        :return: The pattern associated with the run.
+        """
+        return self._pattern
 
-        :raises RuntimeError: NFA handler name already in use.
+    @property
+    def block_index(self) -> int:
         """
+        :return: The current block index of the run.
+        """
+        with self._lock:
+            return self._block_index
+
+    def set_block(self, block_index: int, history: BoboHistory) -> None:
+        """
+        Updates the run's block to a new index and history.
+
+        :param block_index: The new block index.
+        :param history: The new history.
 
+        :raises: BoboRunError: New block index is less than 1.
+        :raises: BoboRunError: New history does not have enough events in it
+            to cover all blocks up to the new block index.
+        """
         with self._lock:
-            if not self._is_cancelled:
-                if nfa_handler.nfa.name not in self._nfa_handlers:
-                    self._nfa_handlers[nfa_handler.nfa.name] = nfa_handler
-                    nfa_handler.subscribe(self)
-                else:
-                    raise RuntimeError("NFA handler name {} already in use."
-                                       .format(nfa_handler.nfa.name))
+            if block_index < 1:
+                raise BoboRunError(_EXC_INDEX.format)
+
+            self._block_index = block_index
+            self._history = history
 
-    def get_all_handlers(self) -> List[BoboNFAHandler]:
+    def history(self) -> BoboHistory:
         """
-        :return: A list of all handlers.
+        :return: The run history.
         """
+        with self._lock:
+            return self._history
 
+    def is_complete(self) -> bool:
+        """
+        :return: True if run is completed; False otherwise.
+        """
         with self._lock:
-            return list(self._nfa_handlers.values())
+            return self._block_index > len(self.pattern.blocks) - 1
 
-    def get_handler(self, name: str) -> BoboNFAHandler:
+    def is_halted(self) -> bool:
+        """
+        :return: True if run has halted; False otherwise.
         """
-        :param name: The handler name.
-        :type name: str
+        with self._lock:
+            return self._halted
 
-        :return: The handler, or None if not found.
+    def serialize(self) -> BoboRunSerial:
+        """
+        :return: A serializable representation of the run.
         """
 
         with self._lock:
-            return self._nfa_handlers.get(name)
+            return BoboRunSerial(
+                run_id=self.run_id,
+                phenomenon_name=self.phenomenon_name,
+                pattern_name=self.pattern.name,
+                block_index=self._block_index,
+                history=self._history)
 
-    def is_recursive(self) -> bool:
-        return self._recursive
+    def halt(self) -> None:
+        """
+        Halts the run.
+        """
+        with self._lock:
+            self._halted = True
 
-    def on_receiver_event(self, event: BoboEvent) -> None:
-        if not self._is_cancelled:
-            self._event_queue.put_nowait(event)
-
-    def on_accepted_producer_event(self, event: CompositeEvent) -> None:
-        if (not self._is_cancelled) and self._recursive:
-            self._event_queue.put_nowait(event)
-
-    def on_producer_action(self, event: ActionEvent):
-        if (not self._is_cancelled) and \
-                self._recursive and \
-                isinstance(event.for_event, CompositeEvent):
-
-            # event added to handler's recent events
-            if event.for_event.name in self._nfa_handlers:
-                self._nfa_handlers[event.for_event.name].add_recent(event)
-
-            # event added to decider queue
-            self._event_queue.put_nowait(event)
-
-    def on_handler_final(self,
-                         nfa_name: str,
-                         run_id: str,
-                         event: CompositeEvent):
-        # notify producer on a new complex event being identified
+    def process(self, event: BoboEvent) -> bool:
+        """
+        :param event: An event for the run to process.
+        :return: `True` if the event caused a state change in the run;
+            `False` otherwise.
+        """
+        # True if state change occurred; False otherwise.
+        # E.g. accepted event, changed block, completed, halted.
         with self._lock:
-            if nfa_name in self._nfa_handlers:
-                if self._recursive:
-                    self._nfa_handlers[nfa_name].add_recent(event)
+            # Do not process if the run has already finished
+            if self._halted:
+                return False
+
+            # Halt if run does not match against all preconditions
+            if len(self.pattern.preconditions) > 0:
+                if not all([precon.evaluate(event, self._history)
+                            for precon in self.pattern.preconditions]):
+                    self._halted = True
+                    return True
+
+            # Halt if run matches against any haltconditions
+            if len(self.pattern.haltconditions) > 0:
+                if any([haltcon.evaluate(event, self._history)
+                        for haltcon in self.pattern.haltconditions]):
+                    self._halted = True
+                    return True
+
+            temp_index = self._block_index
+            block: BoboPatternBlock = self.pattern.blocks[temp_index]
+
+            if block.loop:
+                return self._process_loop(event, block, temp_index)
+            else:
+                return self._process_not_loop(event, block, temp_index)
+
+    def _process_loop(self,
+                      event: BoboEvent,
+                      block: BoboPatternBlock,
+                      temp_index: int) -> bool:
+        """
+        Process a block that loops.
 
-                if nfa_name in self._subs:
-                    for sub in self._subs[nfa_name]:
-                        sub.on_decider_complex_event(event=event)
+        :param event: An event.
+        :param block: The block to process.
+        :param temp_index: Temporary index used during processing.
 
-    def subscribe(self,
-                  nfa_name: str,
-                  subscriber: IDeciderSubscriber) -> None:
+        :return: `True` if halted; `False` otherwise.
         """
-        :param nfa_name: The NFA to subscribe to.
-        :type nfa_name: str
+        match = self._is_match(event, block.predicates)
 
-        :param subscriber: Subscribes to NFA in Decider.
-        :type subscriber: IDeciderSubscriber
+        if match:
+            self._add_event(event, block)
+            return True
+        else:
+            # Looping block can be neither negated nor optional.
+            if block.strict:
+                self._halted = True
+                return True
+            else:
+                # Looping block cannot be the final state.
+                temp_index += 1
+                block = self.pattern.blocks[temp_index]
+                if block.loop:
+                    return self._process_loop(event, block, temp_index)
+                else:
+                    return self._process_not_loop(event, block, temp_index)
 
-        :raises RuntimeError: NFA name not found.
+    def _process_not_loop(self,
+                          event: BoboEvent,
+                          block: BoboPatternBlock,
+                          temp_index: int) -> bool:
         """
+        Process a block that does not loop.
 
-        with self._lock:
-            if not self._is_cancelled:
-                if nfa_name not in self._nfa_handlers:
-                    raise RuntimeError("NFA name {} not found in handlers."
-                                       .format(nfa_name))
-
-                if nfa_name not in self._subs:
-                    self._subs[nfa_name] = []
-
-                if subscriber not in self._subs[nfa_name]:
-                    self._subs[nfa_name].append(subscriber)
-
-    def unsubscribe(self,
-                    nfa_name: str,
-                    unsubscriber: IDeciderSubscriber) -> None:
-        """
-        :param nfa_name: The NFA to unsubscribe from.
-        :type nfa_name: str
+        :param event: An event.
+        :param block: The block to process.
+        :param temp_index: Temporary index used during processing.
 
-        :param unsubscriber: Subscribes to NFA in Decider.
-        :type unsubscriber: IDeciderSubscriber
+        :return: `True` if halted; `False` otherwise.
         """
+        # Non-looping block cannot be both negated and optional.
+        match = self._is_match(event, block.predicates)
 
-        with self._lock:
-            if not self._is_cancelled:
-                if unsubscriber in self._subs[nfa_name]:
-                    self._subs[nfa_name].remove(unsubscriber)
-
-    def on_dist_run_transition(self,
-                               nfa_name: str,
-                               run_id: str,
-                               state_name_from: str,
-                               state_name_to: str,
-                               event: BoboEvent):
-        with self._lock:
-            handler = self._nfa_handlers.get(nfa_name)
-
-            if handler is None:
-                raise RuntimeError(
-                    "Handler not found for NFA {}.".format(nfa_name))
-
-            handler.force_run_transition(
-                run_id=run_id,
-                state_name_from=state_name_from,
-                state_name_to=state_name_to,
-                event=event)
-
-    def on_dist_run_clone(self,
-                          nfa_name: str,
-                          run_id: str,
-                          next_state_name: str,
-                          next_event: BoboEvent):
-        with self._lock:
-            handler = self._nfa_handlers.get(nfa_name)
+        if block.negated:
+            if match:
+                # Negated predicate happened: failure.
+                if block.strict:
+                    self._halted = True
+                    return True
+                return False
+            else:
+                # Negated predicate did not happen: success.
+                self._move_forward(event, block, temp_index)
+                return True
+
+        elif block.optional:
+            # Strict block cannot be optional.
+            if match:
+                # Optional block consumes event.
+                self._move_forward(event, block, temp_index)
+                return True
+            else:
+                # Try event against next block.
+                temp_index += 1
+                block = self.pattern.blocks[temp_index]
+                if block.loop:
+                    return self._process_loop(event, block, temp_index)
+                else:
+                    return self._process_not_loop(event, block, temp_index)
+        else:
+            if match:
+                self._move_forward(event, block, temp_index)
+                return True
+            else:
+                if block.strict:
+                    self._halted = True
+                    return True
+                return False
+
+    def _is_match(self,
+                  event: BoboEvent,
+                  predicates: Tuple[BoboPredicate, ...]) -> bool:
+        """
+        :param event: An event.
+        :param predicates: Predicates to match against.
 
-            if handler is None:
-                raise RuntimeError(
-                    "Handler not found for NFA {}.".format(nfa_name))
-
-            handler.force_run_clone(
-                state_name=next_state_name,
-                event=next_event,
-                parent_run_id=run_id
-            )
-
-    def on_dist_run_halt(self,
-                         nfa_name: str,
-                         run_id: str):
-        with self._lock:
-            handler = self._nfa_handlers.get(nfa_name)
+        :return: `True` if the event matches any predicate;
+            `False` otherwise.
+        """
+        return any(predicate.evaluate(event, self._history)
+                   for predicate in predicates)
 
-            if handler is None:
-                raise RuntimeError(
-                    "Handler not found for NFA {}.".format(nfa_name))
-
-            handler.force_run_halt(
-                run_id=run_id)
-
-    def on_dist_run_final(self,
-                          nfa_name: str,
-                          run_id: str,
-                          event: CompositeEvent) -> None:
-        with self._lock:
-            handler = self._nfa_handlers.get(nfa_name)
+    def _add_event(self, event: BoboEvent, block: BoboPatternBlock) -> None:
+        """
+        :param event: Event to add to history.
+        :param block: Block to determine which group to add event to
+            in the history.
+        """
+        newevents: Dict[str, List[BoboEvent]] = self._history.events
 
-            if handler is None:
-                raise RuntimeError(
-                    "Handler not found for NFA {}.".format(nfa_name))
+        if block.group not in newevents:
+            newevents[block.group] = []
 
-            handler.force_run_final(
-                run_id=run_id,
-                history=event.history)
+        newevents[block.group].append(event)
+        self._history = BoboHistory(events=newevents)
 
-    def on_dist_action(self, event: ActionEvent) -> None:
-        with self._lock:
-            if isinstance(event.for_event, CompositeEvent):
-                handler = self._nfa_handlers.get(event.for_event.name)
+    def _move_forward(self,
+                      event: BoboEvent,
+                      block: BoboPatternBlock,
+                      temp_index: int) -> None:
+        """
+        Move run forward to a new block.
 
-                if handler is None:
-                    raise RuntimeError("Handler not found for NFA {}.".format(
-                        event.for_event.name))
-
-                handler.add_recent(event)
-
-    def _setup(self) -> None:
-        """"""
-
-    def _cancel(self) -> None:
-        """"""
-
-    def on_invalid_data(self, data):
-        """"""
-
-    def on_rejected_producer_event(self, event: CompositeEvent):
-        """"""
-
-    def on_handler_transition(self,
-                              nfa_name: str,
-                              run_id: str,
-                              state_name_from: str,
-                              state_name_to: str,
-                              event: BoboEvent):
-        """"""
-
-    def on_handler_clone(self,
-                         nfa_name: str,
-                         run_id: str,
-                         state_name: str,
-                         event: BoboEvent):
-        """"""
-
-    def on_handler_halt(self,
-                        nfa_name: str,
-                        run_id: str):
-        """"""
+        :param event: An event.
+        :param block: A block.
+        :param temp_index: Temporary index used during processing.
+        """
+        self._add_event(event, block)
+        self._block_index = temp_index + 1
+        self._halted = self.is_complete()
```

### Comparing `bobocep-0.35.0/bobocep/decider/buffers/match_event.py` & `bobocep-1.0.1/bobocep/cep/event/history.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,158 @@
-from typing import Dict, Tuple
+# Copyright (c) 2019-2023 r3w0p
+# The following code can be redistributed and/or
+# modified under the terms of the MIT License.
 
-from bobocep.rules.events.bobo_event import BoboEvent
+"""
+Event history.
+"""
 
+from json import dumps, loads
+from typing import Dict, List, Optional, Tuple
 
-class MatchEvent:
-    """
-    A BoboEvent instance that has been selected as a match for some state
-    criteria by one or more runs.
-
-    :param nfa_name: The name of the BoboNFA instance.
-    :type nfa_name: str
-
-    :param label: The state label with which the event is associated.
-    :type label: str
-
-    :param event: The event selected as being a match for some state.
-    :type event: BoboEvent
+from bobocep.bobocep import BoboJSONable
+from bobocep.cep.event.event import BoboEvent
 
-    :param next_ids: Matches from older states, to which this event links,
-                     defaults to an empty dict.
-    :type next_ids: Dict[str, str], optional
 
-    :param previous_ids: Matches from newer states, to which this event
-                         links, default to an empty dict.
-    :type previous_ids: Dict[str, str], optional
+class BoboHistory(BoboJSONable):
+    """
+    An event history.
     """
 
-    NFA_NAME = "nfa_name"
-    LABEL = "label"
-    EVENT = "event"
-    NEXT_IDS = "next_ids"
-    PREVIOUS_IDS = "previous_ids"
-
-    def __init__(self,
-                 nfa_name: str,
-                 label: str,
-                 event: BoboEvent,
-                 next_ids: Dict[str, Tuple[str, str]] = None,
-                 previous_ids: Dict[str, Tuple[str, str]] = None) -> None:
+    def __init__(self, events: Dict[str, List[BoboEvent]]):
+        """
+        :param events: The history of events.
+            Keys are group names.
+            Values are lists of BoboEvent instances associated with a group.
+        """
         super().__init__()
 
-        self.nfa_name = nfa_name
-        self.label = label
-        self.event = event
-        self.next_ids = {} if next_ids is None else next_ids
-        self.previous_ids = {} if previous_ids is None else previous_ids
+        self._events: Dict[str, List[BoboEvent]] = {}
+        self._first: Optional[BoboEvent] = None
+        self._last: Optional[BoboEvent] = None
 
-    def add_pointer_next(self,
-                         version: str,
-                         label: str = "",
-                         event_id: str = "") -> None:
-        """
-        Points match event to the next match event ID using a run version.
+        if events is not None:
+            for name, event_list in events.items():
+                for event in event_list:
+                    if name not in self._events:
+                        self._events[name] = []
 
-        :param version: The run version.
-        :type version: str
+                    self._events[name].append(event)
 
-        :param label: The state label, defaults to an empty string.
-        :type label: str, optional
+                    if self._first is None or \
+                            event.timestamp < self._first.timestamp:
+                        self._first = event
 
-        :param event_id: The event ID to point to, defaults to an empty string.
-        :type event_id: str, optional
+                    if self._last is None or \
+                            event.timestamp > self._last.timestamp:
+                        self._last = event
 
-        :raises RuntimeError: Label and event ID are the same as those in the
-                              match event i.e. attempt to point match event to
-                              itself.
+    @property
+    def events(self) -> Dict[str, List[BoboEvent]]:
+        """
+        :return: All history events, indexed by group.
         """
+        eventscopy: Dict[str, List[BoboEvent]] = {}
 
-        if label == self.label and event_id == self.event.event_id:
-            raise RuntimeError("Cannot point match event to itself.")
+        for grp in self._events.keys():
+            if grp not in eventscopy:
+                eventscopy[grp] = []
 
-        self.next_ids[version] = (label, event_id)
+            eventscopy[grp] = [eve for eve in self._events[grp]]
 
-    def add_pointer_previous(self,
-                             version: str,
-                             label: str = "",
-                             event_id: str = "") -> None:
+        return eventscopy
+
+    def size(self) -> int:
+        """
+        :return: The total number of history events across all groups.
         """
-        Points match event to the previous match event ID using a run version.
+        count = 0
 
-        :param version: The run version.
-        :type version: str
+        for grp in self._events.keys():
+            count += len(self._events[grp])
 
-        :param label: The state label, defaults to an empty string.
-        :type label: str, optional
+        return count
 
-        :param event_id: The event ID to point to, defaults to an empty string.
-        :type event_id: str, optional
+    def all_groups(self) -> Tuple[str, ...]:
+        """
+        :return: All history groups in a tuple.
+        """
+        return tuple(self._events.keys())
 
-        :raises RuntimeError: Label and event ID are the same as those in the
-                              match event i.e. attempt to point match event to
-                              itself.
+    def all_events(self) -> Tuple[BoboEvent, ...]:
+        """
+        :return: All history events in a tuple.
         """
+        all_events = []
+        for grp in self._events.keys():
+            all_events += self._events[grp]
+        return tuple(all_events)
 
-        if label == self.label and event_id == self.event.event_id:
-            raise RuntimeError("Cannot point match event to itself.")
+    def group(self, group: str) -> Tuple[BoboEvent, ...]:
+        """
+        :param group: A group name.
+        :return: The BoboEvent instances associated with `group`.
+        """
+        if group in self._events:
+            return tuple(self._events[group])
+        else:
+            return tuple()
 
-        self.previous_ids[version] = (label, event_id)
+    def first(self) -> Optional[BoboEvent]:
+        """
+        :return: The BoboEvent with the oldest timestamp,
+            if there is at least one BoboEvent in the history.
+        """
+        return self._first
 
-    def remove_all_pointers(self, version: str) -> None:
+    def last(self) -> Optional[BoboEvent]:
         """
-        Removes all pointers to a match event with a given run version.
+        :return: The BoboEvent with the most recent timestamp,
+            if there is at least one BoboEvent in the history.
+        """
+        return self._last
 
-        :param version: The run version.
-        :type version: str
+    def to_json_dict(self) -> dict:
+        """
+        :return: A JSON `dict` representation of the history.
         """
+        d: Dict[str, List[BoboEvent]] = {}
+
+        for key in self._events:
+            d[key] = [e for e in self._events[key]]
 
-        self.next_ids.pop(version, None)
-        self.previous_ids.pop(version, None)
+        return d
 
-    def has_pointers(self) -> bool:
+    def to_json_str(self) -> str:
         """
-        :return: True if the match event points to any other match events,
-                 False otherwise.
+        :return: A JSON `str` representation of the history.
         """
+        return dumps(self.to_json_dict(), default=lambda o: o.to_json_str())
 
-        return len(self.next_ids) > 0 or len(self.previous_ids) > 0
+    @staticmethod
+    def from_json_str(j: str) -> 'BoboHistory':
+        """
+        :param j: A JSON `str` representation of the history.
+        :return: A new instance of the history.
+        """
+        return BoboHistory.from_json_dict(loads(j))
 
-    def to_dict(self) -> dict:
+    @staticmethod
+    def from_json_dict(d: dict) -> 'BoboHistory':
         """
-        :return: A dict representation of the object.
+        :param d: A JSON `dict` representation of the history.
+        :return: A new instance of the history.
         """
+        from bobocep.cep.event.factory import BoboEventFactory
+
+        events: Dict[str, List[BoboEvent]] = {}
+
+        for key in d:
+            events[key] = [BoboEventFactory.from_json_str(e) for e in d[key]]
 
-        return {
-            self.NFA_NAME: self.nfa_name,
-            self.LABEL: self.label,
-            self.EVENT: self.event.to_dict(),
-            self.NEXT_IDS: self.next_ids,
-            self.PREVIOUS_IDS: self.previous_ids
-        }
+        return BoboHistory(events=events)
+
+    def __str__(self) -> str:
+        """
+        :return: A JSON `str` representation of the history.
+        """
+        return self.to_json_str()
```


# Comparing `tmp/spellbot-8.9.0.tar.gz` & `tmp/spellbot-8.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spellbot-8.9.0.tar", max compression
+gzip compressed data, was "spellbot-8.9.1.tar", max compression
```

## Comparing `spellbot-8.9.0.tar` & `spellbot-8.9.1.tar`

### file list

```diff
@@ -1,94 +1,93 @@
--rw-r--r--   0        0        0     1068 2021-11-26 03:22:03.340065 spellbot-8.9.0/LICENSE.md
--rw-r--r--   0        0        0    10824 2022-12-23 23:53:04.411609 spellbot-8.9.0/README.md
--rw-r--r--   0        0        0     3341 2023-02-03 04:19:42.819986 spellbot-8.9.0/pyproject.toml
--rwxr-xr-x   0        0        0      183 2022-06-28 03:49:01.318112 spellbot-8.9.0/src/spellbot/__init__.py
--rw-r--r--   0        0        0     1801 2022-06-28 03:49:01.318294 spellbot-8.9.0/src/spellbot/_version.py
--rw-r--r--   0        0        0      586 2022-11-29 23:27:22.393332 spellbot-8.9.0/src/spellbot/actions/__init__.py
--rw-r--r--   0        0        0    14123 2022-12-23 22:59:25.745864 spellbot-8.9.0/src/spellbot/actions/admin_action.py
--rw-r--r--   0        0        0     3567 2022-08-10 20:52:44.552188 spellbot-8.9.0/src/spellbot/actions/base_action.py
--rw-r--r--   0        0        0     1491 2022-08-10 20:52:42.516909 spellbot-8.9.0/src/spellbot/actions/block_action.py
--rw-r--r--   0        0        0     1542 2022-11-29 23:27:22.393781 spellbot-8.9.0/src/spellbot/actions/config_action.py
--rw-r--r--   0        0        0     2649 2022-08-10 20:52:44.552422 spellbot-8.9.0/src/spellbot/actions/leave_action.py
--rw-r--r--   0        0        0    17124 2022-11-29 23:27:22.394669 spellbot-8.9.0/src/spellbot/actions/lfg_action.py
--rw-r--r--   0        0        0     3120 2023-02-03 04:19:27.636285 spellbot-8.9.0/src/spellbot/actions/score_action.py
--rw-r--r--   0        0        0     7402 2022-11-17 21:06:36.285619 spellbot-8.9.0/src/spellbot/actions/tasks_action.py
--rw-r--r--   0        0        0      943 2022-08-10 20:52:42.517665 spellbot-8.9.0/src/spellbot/actions/verify_action.py
--rw-r--r--   0        0        0     3860 2022-11-17 21:06:36.285822 spellbot-8.9.0/src/spellbot/actions/watch_action.py
--rw-r--r--   0        0        0     4456 2022-12-23 23:36:10.102494 spellbot-8.9.0/src/spellbot/cli.py
--rw-r--r--   0        0        0     6425 2022-12-25 00:29:43.225050 spellbot-8.9.0/src/spellbot/client.py
--rw-r--r--   0        0        0     2083 2022-11-29 23:27:22.395480 spellbot-8.9.0/src/spellbot/cogs/__init__.py
--rw-r--r--   0        0        0     1971 2022-11-17 21:06:36.286452 spellbot-8.9.0/src/spellbot/cogs/about_cog.py
--rw-r--r--   0        0        0     9846 2022-12-23 22:59:25.746394 spellbot-8.9.0/src/spellbot/cogs/admin_cog.py
--rw-r--r--   0        0        0     1531 2022-11-17 21:06:36.286965 spellbot-8.9.0/src/spellbot/cogs/block_cog.py
--rw-r--r--   0        0        0     1701 2022-11-17 21:06:36.287206 spellbot-8.9.0/src/spellbot/cogs/config_cog.py
--rw-r--r--   0        0        0     1602 2022-11-29 23:27:22.395914 spellbot-8.9.0/src/spellbot/cogs/events_cog.py
--rw-r--r--   0        0        0     1180 2022-11-17 21:06:36.287696 spellbot-8.9.0/src/spellbot/cogs/leave_cog.py
--rw-r--r--   0        0        0     1930 2022-11-25 20:19:37.223026 spellbot-8.9.0/src/spellbot/cogs/lfg_cog.py
--rw-r--r--   0        0        0     3071 2022-12-06 20:24:45.330592 spellbot-8.9.0/src/spellbot/cogs/owner_cog.py
--rw-r--r--   0        0        0     2166 2023-02-03 04:19:27.636784 spellbot-8.9.0/src/spellbot/cogs/score_cog.py
--rw-r--r--   0        0        0     1106 2022-08-10 20:52:42.520436 spellbot-8.9.0/src/spellbot/cogs/sync_cog.py
--rw-r--r--   0        0        0     2224 2022-11-29 23:27:22.396628 spellbot-8.9.0/src/spellbot/cogs/tasks_cog.py
--rw-r--r--   0        0        0     1642 2022-11-17 21:06:36.288671 spellbot-8.9.0/src/spellbot/cogs/verify_cog.py
--rw-r--r--   0        0        0     2559 2022-11-17 21:06:36.289031 spellbot-8.9.0/src/spellbot/cogs/watch_cog.py
--rw-r--r--   0        0        0     4573 2022-08-10 20:52:42.521168 spellbot-8.9.0/src/spellbot/database.py
--rw-r--r--   0        0        0      198 2022-06-28 03:49:01.327183 spellbot-8.9.0/src/spellbot/environment.py
--rw-r--r--   0        0        0     1085 2022-11-17 21:06:36.289303 spellbot-8.9.0/src/spellbot/errors.py
--rw-r--r--   0        0        0      931 2022-06-28 03:49:01.327644 spellbot-8.9.0/src/spellbot/logs.py
--rw-r--r--   0        0        0     4647 2022-12-23 23:36:10.103106 spellbot-8.9.0/src/spellbot/metrics.py
--rw-r--r--   0        0        0      657 2021-09-28 06:28:45.085353 spellbot-8.9.0/src/spellbot/migrations/alembic.ini
--rw-r--r--   0        0        0     1622 2022-12-02 23:54:36.738165 spellbot-8.9.0/src/spellbot/migrations/env.py
--rw-r--r--   0        0        0      493 2021-09-28 06:28:45.085705 spellbot-8.9.0/src/spellbot/migrations/script.py.mako
--rw-r--r--   0        0        0      591 2022-01-25 03:08:39.319503 spellbot-8.9.0/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
--rw-r--r--   0        0        0      645 2021-11-26 04:45:50.803253 spellbot-8.9.0/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
--rw-r--r--   0        0        0      630 2021-12-12 04:33:15.962537 spellbot-8.9.0/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
--rw-r--r--   0        0        0      469 2021-11-26 03:22:03.353698 spellbot-8.9.0/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
--rw-r--r--   0        0        0      641 2021-11-27 01:25:04.571095 spellbot-8.9.0/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
--rw-r--r--   0        0        0      776 2022-11-17 21:06:36.289676 spellbot-8.9.0/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
--rw-r--r--   0        0        0      609 2022-11-17 21:06:36.289852 spellbot-8.9.0/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
--rw-r--r--   0        0        0    10922 2021-11-26 03:22:03.353853 spellbot-8.9.0/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
--rw-r--r--   0        0        0      843 2021-11-26 03:22:03.353978 spellbot-8.9.0/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
--rw-r--r--   0        0        0      474 2021-11-27 17:42:11.654472 spellbot-8.9.0/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
--rw-r--r--   0        0        0      987 2022-11-29 23:27:22.397458 spellbot-8.9.0/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
--rw-r--r--   0        0        0     1261 2022-12-06 19:58:31.890290 spellbot-8.9.0/src/spellbot/models/__init__.py
--rw-r--r--   0        0        0     3172 2022-11-17 21:06:36.290419 spellbot-8.9.0/src/spellbot/models/award.py
--rw-r--r--   0        0        0     2649 2022-08-10 20:52:42.521957 spellbot-8.9.0/src/spellbot/models/base.py
--rw-r--r--   0        0        0      935 2022-08-10 20:52:42.522141 spellbot-8.9.0/src/spellbot/models/block.py
--rw-r--r--   0        0        0     4003 2022-11-29 23:27:22.398216 spellbot-8.9.0/src/spellbot/models/channel.py
--rw-r--r--   0        0        0     1059 2022-08-10 20:52:42.522471 spellbot-8.9.0/src/spellbot/models/config.py
--rw-r--r--   0        0        0    10471 2022-11-29 23:27:22.398981 spellbot-8.9.0/src/spellbot/models/game.py
--rw-r--r--   0        0        0     2468 2022-11-29 23:27:22.399241 spellbot-8.9.0/src/spellbot/models/guild.py
--rw-r--r--   0        0        0      896 2022-06-28 03:49:01.331361 spellbot-8.9.0/src/spellbot/models/play.py
--rw-r--r--   0        0        0     3656 2022-08-10 20:52:42.523010 spellbot-8.9.0/src/spellbot/models/user.py
--rw-r--r--   0        0        0      740 2022-06-28 03:49:01.331841 spellbot-8.9.0/src/spellbot/models/verify.py
--rw-r--r--   0        0        0     1085 2022-08-10 20:52:42.523165 spellbot-8.9.0/src/spellbot/models/watch.py
--rw-r--r--   0        0        0    17221 2022-12-23 23:36:10.103457 spellbot-8.9.0/src/spellbot/operations.py
--rw-r--r--   0        0        0     1051 2022-11-29 23:27:22.400098 spellbot-8.9.0/src/spellbot/services/__init__.py
--rw-r--r--   0        0        0     3199 2022-12-23 23:36:10.103769 spellbot-8.9.0/src/spellbot/services/awards.py
--rw-r--r--   0        0        0     4898 2022-12-23 22:59:25.746946 spellbot-8.9.0/src/spellbot/services/channels.py
--rw-r--r--   0        0        0     1554 2022-08-10 20:52:42.524088 spellbot-8.9.0/src/spellbot/services/configs.py
--rw-r--r--   0        0        0    13240 2022-12-25 00:36:49.288278 spellbot-8.9.0/src/spellbot/services/games.py
--rw-r--r--   0        0        0     4828 2022-11-29 23:27:22.400694 spellbot-8.9.0/src/spellbot/services/guilds.py
--rw-r--r--   0        0        0     7516 2023-02-03 04:19:27.637257 spellbot-8.9.0/src/spellbot/services/plays.py
--rw-r--r--   0        0        0     5369 2022-08-10 20:52:42.524939 spellbot-8.9.0/src/spellbot/services/users.py
--rw-r--r--   0        0        0     1661 2022-06-28 03:49:01.336014 spellbot-8.9.0/src/spellbot/services/verifies.py
--rw-r--r--   0        0        0      502 2022-08-10 20:52:42.525103 spellbot-8.9.0/src/spellbot/services/watches.py
--rw-r--r--   0        0        0     3770 2022-12-23 22:12:57.249464 spellbot-8.9.0/src/spellbot/settings.py
--rw-r--r--   0        0        0     2300 2022-08-10 20:52:42.525443 spellbot-8.9.0/src/spellbot/spelltable.py
--rw-r--r--   0        0        0    10170 2022-12-07 00:03:20.903350 spellbot-8.9.0/src/spellbot/utils.py
--rw-r--r--   0        0        0      251 2022-11-29 23:27:22.401188 spellbot-8.9.0/src/spellbot/views/__init__.py
--rw-r--r--   0        0        0      294 2022-08-10 20:52:42.525931 spellbot-8.9.0/src/spellbot/views/base_view.py
--rw-r--r--   0        0        0     3881 2022-11-25 20:19:40.304992 spellbot-8.9.0/src/spellbot/views/lfg_view.py
--rw-r--r--   0        0        0     2413 2022-11-29 23:27:22.401378 spellbot-8.9.0/src/spellbot/views/setup_view.py
--rw-r--r--   0        0        0      177 2022-06-28 03:49:01.342795 spellbot-8.9.0/src/spellbot/web/__init__.py
--rw-r--r--   0        0        0       35 2022-06-28 03:49:01.342968 spellbot-8.9.0/src/spellbot/web/api/__init__.py
--rw-r--r--   0        0        0      259 2022-06-28 03:49:01.343137 spellbot-8.9.0/src/spellbot/web/api/ping.py
--rw-r--r--   0        0        0     2712 2023-01-01 20:22:31.170296 spellbot-8.9.0/src/spellbot/web/api/record.py
--rw-r--r--   0        0        0     1744 2022-06-28 03:49:01.345054 spellbot-8.9.0/src/spellbot/web/builder.py
--rw-r--r--   0        0        0      647 2022-08-10 20:52:42.526446 spellbot-8.9.0/src/spellbot/web/server.py
--rw-r--r--   0        0        0     1661 2021-11-28 22:40:53.418264 spellbot-8.9.0/src/spellbot/web/templates/channel_record.html.j2
--rw-r--r--   0        0        0     5352 2021-11-26 03:22:03.363431 spellbot-8.9.0/src/spellbot/web/templates/record.css
--rw-r--r--   0        0        0     6365 2022-08-10 20:52:44.555034 spellbot-8.9.0/src/spellbot/web/templates/record_base.html.j2
--rw-r--r--   0        0        0     1978 2021-11-26 03:22:03.363859 spellbot-8.9.0/src/spellbot/web/templates/table2CSV.js
--rw-r--r--   0        0        0     2509 2021-11-28 22:40:53.418856 spellbot-8.9.0/src/spellbot/web/templates/user_record.html.j2
--rw-r--r--   0        0        0    12909 2023-02-03 04:19:44.121804 spellbot-8.9.0/setup.py
--rw-r--r--   0        0        0    12899 2023-02-03 04:19:44.122478 spellbot-8.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-8.9.1/LICENSE.md
+-rw-r--r--   0        0        0    10824 2023-04-18 21:36:17.595924 spellbot-8.9.1/README.md
+-rw-r--r--   0        0        0     3341 2023-04-18 22:54:00.394418 spellbot-8.9.1/pyproject.toml
+-rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-8.9.1/src/spellbot/__init__.py
+-rw-r--r--   0        0        0     1801 2023-04-18 21:36:17.604229 spellbot-8.9.1/src/spellbot/_version.py
+-rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-8.9.1/src/spellbot/actions/__init__.py
+-rw-r--r--   0        0        0    14123 2023-04-18 21:36:17.604426 spellbot-8.9.1/src/spellbot/actions/admin_action.py
+-rw-r--r--   0        0        0     3567 2023-04-18 21:36:17.604506 spellbot-8.9.1/src/spellbot/actions/base_action.py
+-rw-r--r--   0        0        0     1491 2023-04-18 21:36:17.604572 spellbot-8.9.1/src/spellbot/actions/block_action.py
+-rw-r--r--   0        0        0     1542 2023-04-18 21:36:17.604645 spellbot-8.9.1/src/spellbot/actions/config_action.py
+-rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.604693 spellbot-8.9.1/src/spellbot/actions/leave_action.py
+-rw-r--r--   0        0        0    17124 2023-04-18 21:36:17.604820 spellbot-8.9.1/src/spellbot/actions/lfg_action.py
+-rw-r--r--   0        0        0     3120 2023-04-18 21:36:17.604898 spellbot-8.9.1/src/spellbot/actions/score_action.py
+-rw-r--r--   0        0        0     7402 2023-04-18 21:36:17.604981 spellbot-8.9.1/src/spellbot/actions/tasks_action.py
+-rw-r--r--   0        0        0      943 2023-04-18 21:36:17.605035 spellbot-8.9.1/src/spellbot/actions/verify_action.py
+-rw-r--r--   0        0        0     3860 2023-04-18 21:36:17.605103 spellbot-8.9.1/src/spellbot/actions/watch_action.py
+-rw-r--r--   0        0        0     4456 2023-04-18 21:36:17.605183 spellbot-8.9.1/src/spellbot/cli.py
+-rw-r--r--   0        0        0     6425 2023-04-18 21:36:17.605285 spellbot-8.9.1/src/spellbot/client.py
+-rw-r--r--   0        0        0     2083 2023-04-18 21:36:17.605376 spellbot-8.9.1/src/spellbot/cogs/__init__.py
+-rw-r--r--   0        0        0     1971 2023-04-18 22:08:37.549352 spellbot-8.9.1/src/spellbot/cogs/about_cog.py
+-rw-r--r--   0        0        0     9846 2023-04-18 21:36:17.605517 spellbot-8.9.1/src/spellbot/cogs/admin_cog.py
+-rw-r--r--   0        0        0     1531 2023-04-18 21:36:17.605622 spellbot-8.9.1/src/spellbot/cogs/block_cog.py
+-rw-r--r--   0        0        0     1701 2023-04-18 21:36:17.605683 spellbot-8.9.1/src/spellbot/cogs/config_cog.py
+-rw-r--r--   0        0        0     1602 2023-04-18 21:36:17.605748 spellbot-8.9.1/src/spellbot/cogs/events_cog.py
+-rw-r--r--   0        0        0     1180 2023-04-18 21:36:17.605806 spellbot-8.9.1/src/spellbot/cogs/leave_cog.py
+-rw-r--r--   0        0        0     1930 2023-04-18 21:36:17.605872 spellbot-8.9.1/src/spellbot/cogs/lfg_cog.py
+-rw-r--r--   0        0        0     3071 2023-04-18 21:36:17.605938 spellbot-8.9.1/src/spellbot/cogs/owner_cog.py
+-rw-r--r--   0        0        0     2166 2023-04-18 21:36:17.605998 spellbot-8.9.1/src/spellbot/cogs/score_cog.py
+-rw-r--r--   0        0        0     1106 2023-04-18 21:36:17.606052 spellbot-8.9.1/src/spellbot/cogs/sync_cog.py
+-rw-r--r--   0        0        0     2224 2023-04-18 21:36:17.606117 spellbot-8.9.1/src/spellbot/cogs/tasks_cog.py
+-rw-r--r--   0        0        0     1642 2023-04-18 21:36:17.606166 spellbot-8.9.1/src/spellbot/cogs/verify_cog.py
+-rw-r--r--   0        0        0     2559 2023-04-18 21:36:17.606227 spellbot-8.9.1/src/spellbot/cogs/watch_cog.py
+-rw-r--r--   0        0        0     4573 2023-04-18 21:36:17.606307 spellbot-8.9.1/src/spellbot/database.py
+-rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-8.9.1/src/spellbot/environment.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.606418 spellbot-8.9.1/src/spellbot/errors.py
+-rw-r--r--   0        0        0      931 2023-04-18 21:36:17.606470 spellbot-8.9.1/src/spellbot/logs.py
+-rw-r--r--   0        0        0     4647 2023-04-18 21:36:17.606533 spellbot-8.9.1/src/spellbot/metrics.py
+-rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-8.9.1/src/spellbot/migrations/alembic.ini
+-rw-r--r--   0        0        0     1622 2023-04-18 21:36:17.606704 spellbot-8.9.1/src/spellbot/migrations/env.py
+-rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-8.9.1/src/spellbot/migrations/script.py.mako
+-rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-8.9.1/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
+-rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-8.9.1/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
+-rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-8.9.1/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
+-rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-8.9.1/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
+-rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-8.9.1/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
+-rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-8.9.1/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
+-rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-8.9.1/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
+-rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-8.9.1/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
+-rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-8.9.1/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
+-rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-8.9.1/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
+-rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-8.9.1/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
+-rw-r--r--   0        0        0     1261 2023-04-18 21:36:17.607532 spellbot-8.9.1/src/spellbot/models/__init__.py
+-rw-r--r--   0        0        0     3172 2023-04-18 21:36:17.607622 spellbot-8.9.1/src/spellbot/models/award.py
+-rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.607688 spellbot-8.9.1/src/spellbot/models/base.py
+-rw-r--r--   0        0        0      935 2023-04-18 21:36:17.607770 spellbot-8.9.1/src/spellbot/models/block.py
+-rw-r--r--   0        0        0     4003 2023-04-18 21:36:17.607826 spellbot-8.9.1/src/spellbot/models/channel.py
+-rw-r--r--   0        0        0     1059 2023-04-18 21:36:17.607885 spellbot-8.9.1/src/spellbot/models/config.py
+-rw-r--r--   0        0        0    10471 2023-04-18 21:36:17.607972 spellbot-8.9.1/src/spellbot/models/game.py
+-rw-r--r--   0        0        0     2625 2023-04-18 22:53:49.516268 spellbot-8.9.1/src/spellbot/models/guild.py
+-rw-r--r--   0        0        0      896 2023-04-18 21:36:17.608085 spellbot-8.9.1/src/spellbot/models/play.py
+-rw-r--r--   0        0        0     3656 2023-04-18 21:36:17.608138 spellbot-8.9.1/src/spellbot/models/user.py
+-rw-r--r--   0        0        0      740 2023-04-18 21:36:17.608210 spellbot-8.9.1/src/spellbot/models/verify.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-8.9.1/src/spellbot/models/watch.py
+-rw-r--r--   0        0        0    17438 2023-04-18 22:53:49.516511 spellbot-8.9.1/src/spellbot/operations.py
+-rw-r--r--   0        0        0     1051 2023-04-18 21:36:17.608469 spellbot-8.9.1/src/spellbot/services/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-18 21:36:17.608528 spellbot-8.9.1/src/spellbot/services/awards.py
+-rw-r--r--   0        0        0     4898 2023-04-18 21:36:17.608610 spellbot-8.9.1/src/spellbot/services/channels.py
+-rw-r--r--   0        0        0     1554 2023-04-18 21:36:17.608676 spellbot-8.9.1/src/spellbot/services/configs.py
+-rw-r--r--   0        0        0    13240 2023-04-18 21:36:17.608775 spellbot-8.9.1/src/spellbot/services/games.py
+-rw-r--r--   0        0        0     4828 2023-04-18 21:36:17.608845 spellbot-8.9.1/src/spellbot/services/guilds.py
+-rw-r--r--   0        0        0     7516 2023-04-18 21:36:17.608922 spellbot-8.9.1/src/spellbot/services/plays.py
+-rw-r--r--   0        0        0     5369 2023-04-18 21:36:17.608981 spellbot-8.9.1/src/spellbot/services/users.py
+-rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.609034 spellbot-8.9.1/src/spellbot/services/verifies.py
+-rw-r--r--   0        0        0      502 2023-04-18 21:36:17.609093 spellbot-8.9.1/src/spellbot/services/watches.py
+-rw-r--r--   0        0        0     3770 2023-04-18 21:36:17.609161 spellbot-8.9.1/src/spellbot/settings.py
+-rw-r--r--   0        0        0     2300 2023-04-18 21:36:17.609223 spellbot-8.9.1/src/spellbot/spelltable.py
+-rw-r--r--   0        0        0    10441 2023-04-18 22:53:49.516743 spellbot-8.9.1/src/spellbot/utils.py
+-rw-r--r--   0        0        0      251 2023-04-18 21:36:17.609422 spellbot-8.9.1/src/spellbot/views/__init__.py
+-rw-r--r--   0        0        0      294 2023-04-18 21:36:17.609477 spellbot-8.9.1/src/spellbot/views/base_view.py
+-rw-r--r--   0        0        0     3881 2023-04-18 21:36:17.609557 spellbot-8.9.1/src/spellbot/views/lfg_view.py
+-rw-r--r--   0        0        0     2413 2023-04-18 21:36:17.609615 spellbot-8.9.1/src/spellbot/views/setup_view.py
+-rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-8.9.1/src/spellbot/web/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-8.9.1/src/spellbot/web/api/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-8.9.1/src/spellbot/web/api/ping.py
+-rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-8.9.1/src/spellbot/web/api/record.py
+-rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-8.9.1/src/spellbot/web/builder.py
+-rw-r--r--   0        0        0      647 2023-04-18 21:36:17.610025 spellbot-8.9.1/src/spellbot/web/server.py
+-rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-8.9.1/src/spellbot/web/templates/channel_record.html.j2
+-rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-8.9.1/src/spellbot/web/templates/record.css
+-rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-8.9.1/src/spellbot/web/templates/record_base.html.j2
+-rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-8.9.1/src/spellbot/web/templates/table2CSV.js
+-rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-8.9.1/src/spellbot/web/templates/user_record.html.j2
+-rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 spellbot-8.9.1/PKG-INFO
```

### Comparing `spellbot-8.9.0/LICENSE.md` & `spellbot-8.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/README.md` & `spellbot-8.9.1/README.md`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/pyproject.toml` & `spellbot-8.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 license = 'MIT'
 name = 'spellbot'
 packages = [
   {include = "spellbot", from = "src"},
 ]
 readme = 'README.md'
 repository = 'https://github.com/lexicalunit/spellbot'
-version = "8.9.0"
+version = "8.9.1"
 
 [tool.poetry.dependencies]
 Babel = "^2.11.0"
 PyYAML = "^6.0"
 SQLAlchemy = "^1.4.44"
 SQLAlchemy-Utils = "^0.39.0"
 aiohttp = "^3.8.1"
```

### Comparing `spellbot-8.9.0/src/spellbot/_version.py` & `spellbot-8.9.1/src/spellbot/_version.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/__init__.py` & `spellbot-8.9.1/src/spellbot/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/admin_action.py` & `spellbot-8.9.1/src/spellbot/actions/admin_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/base_action.py` & `spellbot-8.9.1/src/spellbot/actions/base_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/block_action.py` & `spellbot-8.9.1/src/spellbot/actions/block_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/config_action.py` & `spellbot-8.9.1/src/spellbot/actions/config_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/leave_action.py` & `spellbot-8.9.1/src/spellbot/actions/leave_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/lfg_action.py` & `spellbot-8.9.1/src/spellbot/actions/lfg_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/score_action.py` & `spellbot-8.9.1/src/spellbot/actions/score_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/tasks_action.py` & `spellbot-8.9.1/src/spellbot/actions/tasks_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/verify_action.py` & `spellbot-8.9.1/src/spellbot/actions/verify_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/actions/watch_action.py` & `spellbot-8.9.1/src/spellbot/actions/watch_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cli.py` & `spellbot-8.9.1/src/spellbot/cli.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/client.py` & `spellbot-8.9.1/src/spellbot/client.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/__init__.py` & `spellbot-8.9.1/src/spellbot/cogs/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/about_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/about_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/admin_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/admin_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/block_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/block_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/config_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/config_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/events_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/events_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/leave_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/leave_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/lfg_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/lfg_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/owner_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/owner_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/score_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/score_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/sync_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/sync_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/tasks_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/tasks_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/verify_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/verify_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/cogs/watch_cog.py` & `spellbot-8.9.1/src/spellbot/cogs/watch_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/database.py` & `spellbot-8.9.1/src/spellbot/database.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/errors.py` & `spellbot-8.9.1/src/spellbot/errors.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/logs.py` & `spellbot-8.9.1/src/spellbot/logs.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/metrics.py` & `spellbot-8.9.1/src/spellbot/metrics.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/alembic.ini` & `spellbot-8.9.1/src/spellbot/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/env.py` & `spellbot-8.9.1/src/spellbot/migrations/env.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py` & `spellbot-8.9.1/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/__init__.py` & `spellbot-8.9.1/src/spellbot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/award.py` & `spellbot-8.9.1/src/spellbot/models/award.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/base.py` & `spellbot-8.9.1/src/spellbot/models/base.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/block.py` & `spellbot-8.9.1/src/spellbot/models/block.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/channel.py` & `spellbot-8.9.1/src/spellbot/models/channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/config.py` & `spellbot-8.9.1/src/spellbot/models/config.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/game.py` & `spellbot-8.9.1/src/spellbot/models/game.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/guild.py` & `spellbot-8.9.1/src/spellbot/models/guild.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,10 +81,16 @@
             "xid": self.xid,
             "created_at": self.created_at,
             "updated_at": self.updated_at,
             "name": self.name,
             "motd": self.motd,
             "show_links": self.show_links,
             "voice_create": self.voice_create,
-            "channels": [channel.to_dict() for channel in self.channels],
-            "awards": [award.to_dict() for award in self.awards],
+            "channels": sorted(
+                [channel.to_dict() for channel in self.channels],
+                key=lambda c: c["xid"],
+            ),
+            "awards": sorted(
+                [award.to_dict() for award in self.awards],
+                key=lambda c: c["id"],
+            ),
         }
```

### Comparing `spellbot-8.9.0/src/spellbot/models/play.py` & `spellbot-8.9.1/src/spellbot/models/play.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/user.py` & `spellbot-8.9.1/src/spellbot/models/user.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/verify.py` & `spellbot-8.9.1/src/spellbot/models/verify.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/models/watch.py` & `spellbot-8.9.1/src/spellbot/models/watch.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/operations.py` & `spellbot-8.9.1/src/spellbot/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -519,44 +519,51 @@
                 user_or_member
                 if hasattr(user_or_member, "roles")
                 else guild.get_member(cast(discord.User, user_or_member).id)
             ),
         )
         if not member or not hasattr(member, "roles"):
             logger.warning(
-                "warning: in guild %s, could not add role %s: could not find member: %s",
+                "warning: in guild %s (%s), could not manage role %s: could not find member: %s",
+                guild.name,
                 guild.id,
                 str(role),
                 str(user_or_member),
             )
             return
         discord_role = discord.utils.find(lambda m: m.name == role, guild.roles)
         if not discord_role:
             logger.warning(
-                "warning: in guild %s, could not add role: could not find role: %s",
+                "warning: in guild %s (%s), could not manage role: could not find role: %s",
+                guild.name,
                 guild.id,
                 str(role),
             )
             return
-        if not bot_can_role(guild):
+        if not bot_can_role(guild, discord_role):
             logger.warning(
-                "warning: in guild %s, could not add role: no permissions to add role: %s",
+                (
+                    "warning: in guild %s (%s), could not manage role:"
+                    " no permissions to manage role: %s"
+                ),
+                guild.name,
                 guild.id,
                 str(role),
             )
             return
         if remove:
             await member.remove_roles(discord_role)
         else:
             await member.add_roles(discord_role)
     except (
         discord.errors.Forbidden,
         discord.errors.HTTPException,
     ) as ex:
         add_span_error(ex)
         logger.exception(
-            "warning: in guild %s, could not add role to member %s: %s",
+            "warning: in guild %s (%s), could not add role to member %s: %s",
+            guild.name,
             guild.id,
             str(user_or_member),
             ex,
             exc_info=True,
         )
```

### Comparing `spellbot-8.9.0/src/spellbot/services/__init__.py` & `spellbot-8.9.1/src/spellbot/services/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/awards.py` & `spellbot-8.9.1/src/spellbot/services/awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/channels.py` & `spellbot-8.9.1/src/spellbot/services/channels.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/configs.py` & `spellbot-8.9.1/src/spellbot/services/configs.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/games.py` & `spellbot-8.9.1/src/spellbot/services/games.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/guilds.py` & `spellbot-8.9.1/src/spellbot/services/guilds.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/plays.py` & `spellbot-8.9.1/src/spellbot/services/plays.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/users.py` & `spellbot-8.9.1/src/spellbot/services/users.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/services/verifies.py` & `spellbot-8.9.1/src/spellbot/services/verifies.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/settings.py` & `spellbot-8.9.1/src/spellbot/settings.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/spelltable.py` & `spellbot-8.9.1/src/spellbot/spelltable.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/utils.py` & `spellbot-8.9.1/src/spellbot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,20 +61,27 @@
     perms = message.channel.permissions_for(message.channel.guild.me)  # type: ignore
     for req in ("send_messages",):
         if not hasattr(perms, req) or not getattr(perms, req):
             return False
     return True
 
 
-def bot_can_role(guild: discord.Guild) -> bool:
+def bot_can_role(guild: discord.Guild, role: Optional[discord.Role] = None) -> bool:
     if not guild.me:
         return False
     perms = guild.me.guild_permissions
-    for req in ("manage_roles",):
-        if not hasattr(perms, req) or not getattr(perms, req):
+    req = "manage_roles"
+    if not hasattr(perms, req) or not getattr(perms, req):
+        return False
+    if role is not None:
+        try:
+            role_hierarchy = list(guild.roles)
+            if role_hierarchy.index(role) > role_hierarchy.index(guild.me.top_role):
+                return False
+        except ValueError:
             return False
     return True
 
 
 def bot_can_read(channel: MessageableChannel) -> bool:
     if not hasattr(channel, "type"):
         return False
```

### Comparing `spellbot-8.9.0/src/spellbot/views/lfg_view.py` & `spellbot-8.9.1/src/spellbot/views/lfg_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/views/setup_view.py` & `spellbot-8.9.1/src/spellbot/views/setup_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/api/record.py` & `spellbot-8.9.1/src/spellbot/web/api/record.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/builder.py` & `spellbot-8.9.1/src/spellbot/web/builder.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/server.py` & `spellbot-8.9.1/src/spellbot/web/server.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/templates/channel_record.html.j2` & `spellbot-8.9.1/src/spellbot/web/templates/channel_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/templates/record.css` & `spellbot-8.9.1/src/spellbot/web/templates/record.css`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/templates/record_base.html.j2` & `spellbot-8.9.1/src/spellbot/web/templates/record_base.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/templates/table2CSV.js` & `spellbot-8.9.1/src/spellbot/web/templates/table2CSV.js`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/src/spellbot/web/templates/user_record.html.j2` & `spellbot-8.9.1/src/spellbot/web/templates/user_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.0/PKG-INFO` & `spellbot-8.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: spellbot
-Version: 8.9.0
+Version: 8.9.1
 Summary: The Discord bot for SpellTable
 Home-page: http://spellbot.io/
 License: MIT
 Keywords: discord,magic,bot,mtg,SpellTable
 Author: Amy Troschinetz
 Author-email: spellbot@lexicalunit.com
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Games/Entertainment :: Board Games
 Requires-Dist: Babel (>=2.11.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: SQLAlchemy (>=1.4.44,<2.0.0)
 Requires-Dist: SQLAlchemy-Utils (>=0.39.0,<0.40.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: spellbot Version: 8.9.0 Summary: The Discord bot
+Metadata-Version: 2.1 Name: spellbot Version: 8.9.1 Summary: The Discord bot
 for SpellTable Home-page: http://spellbot.io/ License: MIT Keywords:
 discord,magic,bot,mtg,SpellTable Author: Amy Troschinetz Author-email:
 spellbot@lexicalunit.com Requires-Python: >=3.10,<4 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Communications :: Chat Classifier: Topic :: Games/
-Entertainment :: Board Games Requires-Dist: Babel (>=2.11.0,<3.0.0) Requires-
-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: SQLAlchemy (>=1.4.44,<2.0.0) Requires-
-Dist: SQLAlchemy-Utils (>=0.39.0,<0.40.0) Requires-Dist: aiohttp
-(>=3.8.1,<4.0.0) Requires-Dist: aiohttp-jinja2 (>=1.5,<2.0) Requires-Dist:
-aiohttp-retry (>=2.8.3,<3.0.0) Requires-Dist: alembic (>=1.8.0,<2.0.0)
-Requires-Dist: asgiref (>=3.5.2,<4.0.0) Requires-Dist: certifi
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Games/Entertainment :: Board Games Requires-Dist: Babel
+(>=2.11.0,<3.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: SQLAlchemy
+(>=1.4.44,<2.0.0) Requires-Dist: SQLAlchemy-Utils (>=0.39.0,<0.40.0) Requires-
+Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: aiohttp-jinja2 (>=1.5,<2.0)
+Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0) Requires-Dist: alembic
+(>=1.8.0,<2.0.0) Requires-Dist: asgiref (>=3.5.2,<4.0.0) Requires-Dist: certifi
 (>=2022.12.7,<2023.0.0) Requires-Dist: charset-normalizer (==2.1.1) Requires-
 Dist: click (>=8.1.3,<9.0.0) Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: datadog (>=0.44.0,<0.45.0) Requires-Dist: ddtrace
 (>=1.6.1,<2.0.0) Requires-Dist: discord.py (>=2.1.0,<3.0.0) Requires-Dist:
 dunamai (>=1.14.1,<2.0.0) Requires-Dist: expiringdict (>=1.2.2,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: humanize
 (>=4.3.0,<5.0.0) Requires-Dist: hupper (>=1.10.3,<2.0.0) Requires-Dist:
```


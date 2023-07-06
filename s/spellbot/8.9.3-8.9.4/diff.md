# Comparing `tmp/spellbot-8.9.3.tar.gz` & `tmp/spellbot-8.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spellbot-8.9.3.tar", max compression
+gzip compressed data, was "spellbot-8.9.4.tar", max compression
```

## Comparing `spellbot-8.9.3.tar` & `spellbot-8.9.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-8.9.3/LICENSE.md
--rw-r--r--   0        0        0    10824 2023-04-18 21:36:17.595924 spellbot-8.9.3/README.md
--rw-r--r--   0        0        0     3274 2023-04-19 22:52:42.224281 spellbot-8.9.3/pyproject.toml
--rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-8.9.3/src/spellbot/__init__.py
--rw-r--r--   0        0        0     1801 2023-04-18 21:36:17.604229 spellbot-8.9.3/src/spellbot/_version.py
--rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-8.9.3/src/spellbot/actions/__init__.py
--rw-r--r--   0        0        0    14123 2023-04-18 21:36:17.604426 spellbot-8.9.3/src/spellbot/actions/admin_action.py
--rw-r--r--   0        0        0     3567 2023-04-18 21:36:17.604506 spellbot-8.9.3/src/spellbot/actions/base_action.py
--rw-r--r--   0        0        0     1491 2023-04-18 21:36:17.604572 spellbot-8.9.3/src/spellbot/actions/block_action.py
--rw-r--r--   0        0        0     1542 2023-04-18 21:36:17.604645 spellbot-8.9.3/src/spellbot/actions/config_action.py
--rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.604693 spellbot-8.9.3/src/spellbot/actions/leave_action.py
--rw-r--r--   0        0        0    17124 2023-04-18 21:36:17.604820 spellbot-8.9.3/src/spellbot/actions/lfg_action.py
--rw-r--r--   0        0        0     3124 2023-04-19 04:04:51.454273 spellbot-8.9.3/src/spellbot/actions/score_action.py
--rw-r--r--   0        0        0     7402 2023-04-18 21:36:17.604981 spellbot-8.9.3/src/spellbot/actions/tasks_action.py
--rw-r--r--   0        0        0      943 2023-04-18 21:36:17.605035 spellbot-8.9.3/src/spellbot/actions/verify_action.py
--rw-r--r--   0        0        0     3860 2023-04-18 21:36:17.605103 spellbot-8.9.3/src/spellbot/actions/watch_action.py
--rw-r--r--   0        0        0     4456 2023-04-18 21:36:17.605183 spellbot-8.9.3/src/spellbot/cli.py
--rw-r--r--   0        0        0     6425 2023-04-18 21:36:17.605285 spellbot-8.9.3/src/spellbot/client.py
--rw-r--r--   0        0        0     2082 2023-04-19 04:04:51.454571 spellbot-8.9.3/src/spellbot/cogs/__init__.py
--rw-r--r--   0        0        0     1971 2023-04-18 22:08:37.549352 spellbot-8.9.3/src/spellbot/cogs/about_cog.py
--rw-r--r--   0        0        0     9846 2023-04-18 21:36:17.605517 spellbot-8.9.3/src/spellbot/cogs/admin_cog.py
--rw-r--r--   0        0        0     1531 2023-04-18 21:36:17.605622 spellbot-8.9.3/src/spellbot/cogs/block_cog.py
--rw-r--r--   0        0        0     1701 2023-04-18 21:36:17.605683 spellbot-8.9.3/src/spellbot/cogs/config_cog.py
--rw-r--r--   0        0        0     1602 2023-04-18 21:36:17.605748 spellbot-8.9.3/src/spellbot/cogs/events_cog.py
--rw-r--r--   0        0        0     1180 2023-04-18 21:36:17.605806 spellbot-8.9.3/src/spellbot/cogs/leave_cog.py
--rw-r--r--   0        0        0     1930 2023-04-18 21:36:17.605872 spellbot-8.9.3/src/spellbot/cogs/lfg_cog.py
--rw-r--r--   0        0        0     3071 2023-04-18 21:36:17.605938 spellbot-8.9.3/src/spellbot/cogs/owner_cog.py
--rw-r--r--   0        0        0     2166 2023-04-18 21:36:17.605998 spellbot-8.9.3/src/spellbot/cogs/score_cog.py
--rw-r--r--   0        0        0     1106 2023-04-18 21:36:17.606052 spellbot-8.9.3/src/spellbot/cogs/sync_cog.py
--rw-r--r--   0        0        0     2224 2023-04-18 21:36:17.606117 spellbot-8.9.3/src/spellbot/cogs/tasks_cog.py
--rw-r--r--   0        0        0     1642 2023-04-18 21:36:17.606166 spellbot-8.9.3/src/spellbot/cogs/verify_cog.py
--rw-r--r--   0        0        0     2559 2023-04-18 21:36:17.606227 spellbot-8.9.3/src/spellbot/cogs/watch_cog.py
--rw-r--r--   0        0        0     4573 2023-04-18 21:36:17.606307 spellbot-8.9.3/src/spellbot/database.py
--rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-8.9.3/src/spellbot/environment.py
--rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.606418 spellbot-8.9.3/src/spellbot/errors.py
--rw-r--r--   0        0        0      931 2023-04-18 21:36:17.606470 spellbot-8.9.3/src/spellbot/logs.py
--rw-r--r--   0        0        0     4647 2023-04-18 21:36:17.606533 spellbot-8.9.3/src/spellbot/metrics.py
--rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-8.9.3/src/spellbot/migrations/alembic.ini
--rw-r--r--   0        0        0     1622 2023-04-18 21:36:17.606704 spellbot-8.9.3/src/spellbot/migrations/env.py
--rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-8.9.3/src/spellbot/migrations/script.py.mako
--rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-8.9.3/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
--rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-8.9.3/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
--rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-8.9.3/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
--rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-8.9.3/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
--rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-8.9.3/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
--rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-8.9.3/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
--rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-8.9.3/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
--rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-8.9.3/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
--rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-8.9.3/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
--rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-8.9.3/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
--rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-8.9.3/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
--rw-r--r--   0        0        0     1261 2023-04-18 21:36:17.607532 spellbot-8.9.3/src/spellbot/models/__init__.py
--rw-r--r--   0        0        0     3172 2023-04-18 21:36:17.607622 spellbot-8.9.3/src/spellbot/models/award.py
--rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.607688 spellbot-8.9.3/src/spellbot/models/base.py
--rw-r--r--   0        0        0      935 2023-04-18 21:36:17.607770 spellbot-8.9.3/src/spellbot/models/block.py
--rw-r--r--   0        0        0     4003 2023-04-18 21:36:17.607826 spellbot-8.9.3/src/spellbot/models/channel.py
--rw-r--r--   0        0        0     1059 2023-04-18 21:36:17.607885 spellbot-8.9.3/src/spellbot/models/config.py
--rw-r--r--   0        0        0    10471 2023-04-18 21:36:17.607972 spellbot-8.9.3/src/spellbot/models/game.py
--rw-r--r--   0        0        0     2625 2023-04-18 22:53:49.516268 spellbot-8.9.3/src/spellbot/models/guild.py
--rw-r--r--   0        0        0      896 2023-04-18 21:36:17.608085 spellbot-8.9.3/src/spellbot/models/play.py
--rw-r--r--   0        0        0     3656 2023-04-18 21:36:17.608138 spellbot-8.9.3/src/spellbot/models/user.py
--rw-r--r--   0        0        0      740 2023-04-18 21:36:17.608210 spellbot-8.9.3/src/spellbot/models/verify.py
--rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-8.9.3/src/spellbot/models/watch.py
--rw-r--r--   0        0        0    17438 2023-04-18 22:53:49.516511 spellbot-8.9.3/src/spellbot/operations.py
--rw-r--r--   0        0        0     1051 2023-04-18 21:36:17.608469 spellbot-8.9.3/src/spellbot/services/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-18 21:36:17.608528 spellbot-8.9.3/src/spellbot/services/awards.py
--rw-r--r--   0        0        0     4900 2023-04-19 04:04:51.454821 spellbot-8.9.3/src/spellbot/services/channels.py
--rw-r--r--   0        0        0     1553 2023-04-19 04:04:51.455067 spellbot-8.9.3/src/spellbot/services/configs.py
--rw-r--r--   0        0        0    13239 2023-04-19 22:44:57.751042 spellbot-8.9.3/src/spellbot/services/games.py
--rw-r--r--   0        0        0     4830 2023-04-19 04:04:51.455764 spellbot-8.9.3/src/spellbot/services/guilds.py
--rw-r--r--   0        0        0     7516 2023-04-18 21:36:17.608922 spellbot-8.9.3/src/spellbot/services/plays.py
--rw-r--r--   0        0        0     5372 2023-04-19 04:04:51.455984 spellbot-8.9.3/src/spellbot/services/users.py
--rw-r--r--   0        0        0     1660 2023-04-19 04:04:51.456240 spellbot-8.9.3/src/spellbot/services/verifies.py
--rw-r--r--   0        0        0      502 2023-04-18 21:36:17.609093 spellbot-8.9.3/src/spellbot/services/watches.py
--rw-r--r--   0        0        0     3770 2023-04-18 21:36:17.609161 spellbot-8.9.3/src/spellbot/settings.py
--rw-r--r--   0        0        0     2300 2023-04-18 21:36:17.609223 spellbot-8.9.3/src/spellbot/spelltable.py
--rw-r--r--   0        0        0    10441 2023-04-18 22:53:49.516743 spellbot-8.9.3/src/spellbot/utils.py
--rw-r--r--   0        0        0      251 2023-04-18 21:36:17.609422 spellbot-8.9.3/src/spellbot/views/__init__.py
--rw-r--r--   0        0        0      294 2023-04-18 21:36:17.609477 spellbot-8.9.3/src/spellbot/views/base_view.py
--rw-r--r--   0        0        0     3881 2023-04-18 21:36:17.609557 spellbot-8.9.3/src/spellbot/views/lfg_view.py
--rw-r--r--   0        0        0     2413 2023-04-18 21:36:17.609615 spellbot-8.9.3/src/spellbot/views/setup_view.py
--rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-8.9.3/src/spellbot/web/__init__.py
--rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-8.9.3/src/spellbot/web/api/__init__.py
--rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-8.9.3/src/spellbot/web/api/ping.py
--rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-8.9.3/src/spellbot/web/api/record.py
--rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-8.9.3/src/spellbot/web/builder.py
--rw-r--r--   0        0        0      647 2023-04-18 21:36:17.610025 spellbot-8.9.3/src/spellbot/web/server.py
--rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-8.9.3/src/spellbot/web/templates/channel_record.html.j2
--rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-8.9.3/src/spellbot/web/templates/record.css
--rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-8.9.3/src/spellbot/web/templates/record_base.html.j2
--rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-8.9.3/src/spellbot/web/templates/table2CSV.js
--rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-8.9.3/src/spellbot/web/templates/user_record.html.j2
--rw-r--r--   0        0        0    12969 1970-01-01 00:00:00.000000 spellbot-8.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-8.9.4/LICENSE.md
+-rw-r--r--   0        0        0    10824 2023-04-18 21:36:17.595924 spellbot-8.9.4/README.md
+-rw-r--r--   0        0        0     3274 2023-04-19 23:38:42.517830 spellbot-8.9.4/pyproject.toml
+-rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-8.9.4/src/spellbot/__init__.py
+-rw-r--r--   0        0        0     1801 2023-04-18 21:36:17.604229 spellbot-8.9.4/src/spellbot/_version.py
+-rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-8.9.4/src/spellbot/actions/__init__.py
+-rw-r--r--   0        0        0    14123 2023-04-18 21:36:17.604426 spellbot-8.9.4/src/spellbot/actions/admin_action.py
+-rw-r--r--   0        0        0     3567 2023-04-18 21:36:17.604506 spellbot-8.9.4/src/spellbot/actions/base_action.py
+-rw-r--r--   0        0        0     1491 2023-04-18 21:36:17.604572 spellbot-8.9.4/src/spellbot/actions/block_action.py
+-rw-r--r--   0        0        0     1542 2023-04-18 21:36:17.604645 spellbot-8.9.4/src/spellbot/actions/config_action.py
+-rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.604693 spellbot-8.9.4/src/spellbot/actions/leave_action.py
+-rw-r--r--   0        0        0    17124 2023-04-18 21:36:17.604820 spellbot-8.9.4/src/spellbot/actions/lfg_action.py
+-rw-r--r--   0        0        0     3124 2023-04-19 04:04:51.454273 spellbot-8.9.4/src/spellbot/actions/score_action.py
+-rw-r--r--   0        0        0     7402 2023-04-18 21:36:17.604981 spellbot-8.9.4/src/spellbot/actions/tasks_action.py
+-rw-r--r--   0        0        0      943 2023-04-18 21:36:17.605035 spellbot-8.9.4/src/spellbot/actions/verify_action.py
+-rw-r--r--   0        0        0     3860 2023-04-18 21:36:17.605103 spellbot-8.9.4/src/spellbot/actions/watch_action.py
+-rw-r--r--   0        0        0     4456 2023-04-18 21:36:17.605183 spellbot-8.9.4/src/spellbot/cli.py
+-rw-r--r--   0        0        0     6425 2023-04-18 21:36:17.605285 spellbot-8.9.4/src/spellbot/client.py
+-rw-r--r--   0        0        0     2082 2023-04-19 04:04:51.454571 spellbot-8.9.4/src/spellbot/cogs/__init__.py
+-rw-r--r--   0        0        0     1971 2023-04-19 23:17:22.400876 spellbot-8.9.4/src/spellbot/cogs/about_cog.py
+-rw-r--r--   0        0        0     9846 2023-04-18 21:36:17.605517 spellbot-8.9.4/src/spellbot/cogs/admin_cog.py
+-rw-r--r--   0        0        0     1531 2023-04-18 21:36:17.605622 spellbot-8.9.4/src/spellbot/cogs/block_cog.py
+-rw-r--r--   0        0        0     1701 2023-04-18 21:36:17.605683 spellbot-8.9.4/src/spellbot/cogs/config_cog.py
+-rw-r--r--   0        0        0     1602 2023-04-18 21:36:17.605748 spellbot-8.9.4/src/spellbot/cogs/events_cog.py
+-rw-r--r--   0        0        0     1180 2023-04-18 21:36:17.605806 spellbot-8.9.4/src/spellbot/cogs/leave_cog.py
+-rw-r--r--   0        0        0     1930 2023-04-18 21:36:17.605872 spellbot-8.9.4/src/spellbot/cogs/lfg_cog.py
+-rw-r--r--   0        0        0     3071 2023-04-18 21:36:17.605938 spellbot-8.9.4/src/spellbot/cogs/owner_cog.py
+-rw-r--r--   0        0        0     2166 2023-04-18 21:36:17.605998 spellbot-8.9.4/src/spellbot/cogs/score_cog.py
+-rw-r--r--   0        0        0     1106 2023-04-18 21:36:17.606052 spellbot-8.9.4/src/spellbot/cogs/sync_cog.py
+-rw-r--r--   0        0        0     2224 2023-04-18 21:36:17.606117 spellbot-8.9.4/src/spellbot/cogs/tasks_cog.py
+-rw-r--r--   0        0        0     1642 2023-04-18 21:36:17.606166 spellbot-8.9.4/src/spellbot/cogs/verify_cog.py
+-rw-r--r--   0        0        0     2559 2023-04-18 21:36:17.606227 spellbot-8.9.4/src/spellbot/cogs/watch_cog.py
+-rw-r--r--   0        0        0     4573 2023-04-18 21:36:17.606307 spellbot-8.9.4/src/spellbot/database.py
+-rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-8.9.4/src/spellbot/environment.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.606418 spellbot-8.9.4/src/spellbot/errors.py
+-rw-r--r--   0        0        0      931 2023-04-18 21:36:17.606470 spellbot-8.9.4/src/spellbot/logs.py
+-rw-r--r--   0        0        0     4647 2023-04-18 21:36:17.606533 spellbot-8.9.4/src/spellbot/metrics.py
+-rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-8.9.4/src/spellbot/migrations/alembic.ini
+-rw-r--r--   0        0        0     1622 2023-04-18 21:36:17.606704 spellbot-8.9.4/src/spellbot/migrations/env.py
+-rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-8.9.4/src/spellbot/migrations/script.py.mako
+-rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-8.9.4/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
+-rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-8.9.4/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
+-rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-8.9.4/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
+-rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-8.9.4/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
+-rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-8.9.4/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
+-rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-8.9.4/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
+-rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-8.9.4/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
+-rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-8.9.4/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
+-rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-8.9.4/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
+-rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-8.9.4/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
+-rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-8.9.4/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
+-rw-r--r--   0        0        0     1261 2023-04-18 21:36:17.607532 spellbot-8.9.4/src/spellbot/models/__init__.py
+-rw-r--r--   0        0        0     3172 2023-04-18 21:36:17.607622 spellbot-8.9.4/src/spellbot/models/award.py
+-rw-r--r--   0        0        0     2649 2023-04-18 21:36:17.607688 spellbot-8.9.4/src/spellbot/models/base.py
+-rw-r--r--   0        0        0      935 2023-04-18 21:36:17.607770 spellbot-8.9.4/src/spellbot/models/block.py
+-rw-r--r--   0        0        0     4003 2023-04-18 21:36:17.607826 spellbot-8.9.4/src/spellbot/models/channel.py
+-rw-r--r--   0        0        0     1059 2023-04-18 21:36:17.607885 spellbot-8.9.4/src/spellbot/models/config.py
+-rw-r--r--   0        0        0    10471 2023-04-18 21:36:17.607972 spellbot-8.9.4/src/spellbot/models/game.py
+-rw-r--r--   0        0        0     2625 2023-04-18 22:53:49.516268 spellbot-8.9.4/src/spellbot/models/guild.py
+-rw-r--r--   0        0        0      896 2023-04-18 21:36:17.608085 spellbot-8.9.4/src/spellbot/models/play.py
+-rw-r--r--   0        0        0     3656 2023-04-18 21:36:17.608138 spellbot-8.9.4/src/spellbot/models/user.py
+-rw-r--r--   0        0        0      740 2023-04-18 21:36:17.608210 spellbot-8.9.4/src/spellbot/models/verify.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-8.9.4/src/spellbot/models/watch.py
+-rw-r--r--   0        0        0    17438 2023-04-18 22:53:49.516511 spellbot-8.9.4/src/spellbot/operations.py
+-rw-r--r--   0        0        0     1051 2023-04-18 21:36:17.608469 spellbot-8.9.4/src/spellbot/services/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-18 21:36:17.608528 spellbot-8.9.4/src/spellbot/services/awards.py
+-rw-r--r--   0        0        0     4900 2023-04-19 04:04:51.454821 spellbot-8.9.4/src/spellbot/services/channels.py
+-rw-r--r--   0        0        0     1553 2023-04-19 04:04:51.455067 spellbot-8.9.4/src/spellbot/services/configs.py
+-rw-r--r--   0        0        0    13239 2023-04-19 22:44:57.751042 spellbot-8.9.4/src/spellbot/services/games.py
+-rw-r--r--   0        0        0     4830 2023-04-19 04:04:51.455764 spellbot-8.9.4/src/spellbot/services/guilds.py
+-rw-r--r--   0        0        0     7516 2023-04-18 21:36:17.608922 spellbot-8.9.4/src/spellbot/services/plays.py
+-rw-r--r--   0        0        0     5372 2023-04-19 04:04:51.455984 spellbot-8.9.4/src/spellbot/services/users.py
+-rw-r--r--   0        0        0     1660 2023-04-19 04:04:51.456240 spellbot-8.9.4/src/spellbot/services/verifies.py
+-rw-r--r--   0        0        0      502 2023-04-18 21:36:17.609093 spellbot-8.9.4/src/spellbot/services/watches.py
+-rw-r--r--   0        0        0     3770 2023-04-18 21:36:17.609161 spellbot-8.9.4/src/spellbot/settings.py
+-rw-r--r--   0        0        0     2300 2023-04-18 21:36:17.609223 spellbot-8.9.4/src/spellbot/spelltable.py
+-rw-r--r--   0        0        0    10265 2023-04-19 23:38:34.319014 spellbot-8.9.4/src/spellbot/utils.py
+-rw-r--r--   0        0        0      251 2023-04-18 21:36:17.609422 spellbot-8.9.4/src/spellbot/views/__init__.py
+-rw-r--r--   0        0        0      294 2023-04-18 21:36:17.609477 spellbot-8.9.4/src/spellbot/views/base_view.py
+-rw-r--r--   0        0        0     3881 2023-04-18 21:36:17.609557 spellbot-8.9.4/src/spellbot/views/lfg_view.py
+-rw-r--r--   0        0        0     2413 2023-04-18 21:36:17.609615 spellbot-8.9.4/src/spellbot/views/setup_view.py
+-rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-8.9.4/src/spellbot/web/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-8.9.4/src/spellbot/web/api/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-8.9.4/src/spellbot/web/api/ping.py
+-rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-8.9.4/src/spellbot/web/api/record.py
+-rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-8.9.4/src/spellbot/web/builder.py
+-rw-r--r--   0        0        0      647 2023-04-18 21:36:17.610025 spellbot-8.9.4/src/spellbot/web/server.py
+-rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-8.9.4/src/spellbot/web/templates/channel_record.html.j2
+-rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-8.9.4/src/spellbot/web/templates/record.css
+-rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-8.9.4/src/spellbot/web/templates/record_base.html.j2
+-rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-8.9.4/src/spellbot/web/templates/table2CSV.js
+-rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-8.9.4/src/spellbot/web/templates/user_record.html.j2
+-rw-r--r--   0        0        0    12969 1970-01-01 00:00:00.000000 spellbot-8.9.4/PKG-INFO
```

### Comparing `spellbot-8.9.3/LICENSE.md` & `spellbot-8.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/README.md` & `spellbot-8.9.4/README.md`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/pyproject.toml` & `spellbot-8.9.4/pyproject.toml`

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
-version = "8.9.3"
+version = "8.9.4"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.4"
 aiohttp-jinja2 = "^1.5.1"
 aiohttp-retry = "^2.8.3"
 alembic = "^1.10.3"
 asgiref = "^3.6.0"
```

### Comparing `spellbot-8.9.3/src/spellbot/_version.py` & `spellbot-8.9.4/src/spellbot/_version.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/__init__.py` & `spellbot-8.9.4/src/spellbot/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/admin_action.py` & `spellbot-8.9.4/src/spellbot/actions/admin_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/base_action.py` & `spellbot-8.9.4/src/spellbot/actions/base_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/block_action.py` & `spellbot-8.9.4/src/spellbot/actions/block_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/config_action.py` & `spellbot-8.9.4/src/spellbot/actions/config_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/leave_action.py` & `spellbot-8.9.4/src/spellbot/actions/leave_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/lfg_action.py` & `spellbot-8.9.4/src/spellbot/actions/lfg_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/score_action.py` & `spellbot-8.9.4/src/spellbot/actions/score_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/tasks_action.py` & `spellbot-8.9.4/src/spellbot/actions/tasks_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/verify_action.py` & `spellbot-8.9.4/src/spellbot/actions/verify_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/actions/watch_action.py` & `spellbot-8.9.4/src/spellbot/actions/watch_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cli.py` & `spellbot-8.9.4/src/spellbot/cli.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/client.py` & `spellbot-8.9.4/src/spellbot/client.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/__init__.py` & `spellbot-8.9.4/src/spellbot/cogs/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/about_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/about_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/admin_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/admin_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/block_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/block_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/config_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/config_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/events_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/events_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/leave_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/leave_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/lfg_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/lfg_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/owner_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/owner_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/score_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/score_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/sync_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/sync_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/tasks_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/tasks_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/verify_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/verify_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/cogs/watch_cog.py` & `spellbot-8.9.4/src/spellbot/cogs/watch_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/database.py` & `spellbot-8.9.4/src/spellbot/database.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/errors.py` & `spellbot-8.9.4/src/spellbot/errors.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/logs.py` & `spellbot-8.9.4/src/spellbot/logs.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/metrics.py` & `spellbot-8.9.4/src/spellbot/metrics.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/alembic.ini` & `spellbot-8.9.4/src/spellbot/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/env.py` & `spellbot-8.9.4/src/spellbot/migrations/env.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py` & `spellbot-8.9.4/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/__init__.py` & `spellbot-8.9.4/src/spellbot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/award.py` & `spellbot-8.9.4/src/spellbot/models/award.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/base.py` & `spellbot-8.9.4/src/spellbot/models/base.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/block.py` & `spellbot-8.9.4/src/spellbot/models/block.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/channel.py` & `spellbot-8.9.4/src/spellbot/models/channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/config.py` & `spellbot-8.9.4/src/spellbot/models/config.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/game.py` & `spellbot-8.9.4/src/spellbot/models/game.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/guild.py` & `spellbot-8.9.4/src/spellbot/models/guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/play.py` & `spellbot-8.9.4/src/spellbot/models/play.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/user.py` & `spellbot-8.9.4/src/spellbot/models/user.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/verify.py` & `spellbot-8.9.4/src/spellbot/models/verify.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/models/watch.py` & `spellbot-8.9.4/src/spellbot/models/watch.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/operations.py` & `spellbot-8.9.4/src/spellbot/operations.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/__init__.py` & `spellbot-8.9.4/src/spellbot/services/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/awards.py` & `spellbot-8.9.4/src/spellbot/services/awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/channels.py` & `spellbot-8.9.4/src/spellbot/services/channels.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/configs.py` & `spellbot-8.9.4/src/spellbot/services/configs.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/games.py` & `spellbot-8.9.4/src/spellbot/services/games.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/guilds.py` & `spellbot-8.9.4/src/spellbot/services/guilds.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/plays.py` & `spellbot-8.9.4/src/spellbot/services/plays.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/users.py` & `spellbot-8.9.4/src/spellbot/services/users.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/services/verifies.py` & `spellbot-8.9.4/src/spellbot/services/verifies.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/settings.py` & `spellbot-8.9.4/src/spellbot/settings.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/spelltable.py` & `spellbot-8.9.4/src/spellbot/spelltable.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/utils.py` & `spellbot-8.9.4/src/spellbot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,16 @@
 def bot_can_role(guild: discord.Guild, role: Optional[discord.Role] = None) -> bool:
     if not guild.me:
         return False
     perms = guild.me.guild_permissions
     req = "manage_roles"
     if not hasattr(perms, req) or not getattr(perms, req):
         return False
-    if role is not None:
-        try:
-            role_hierarchy = list(guild.roles)
-            if role_hierarchy.index(role) > role_hierarchy.index(guild.me.top_role):
-                return False
-        except ValueError:
-            return False
+    if role is not None and role > guild.me.top_role:
+        return False
     return True
 
 
 def bot_can_read(channel: MessageableChannel) -> bool:
     if not hasattr(channel, "type"):
         return False
     channel_type = getattr(channel, "type")
```

### Comparing `spellbot-8.9.3/src/spellbot/views/lfg_view.py` & `spellbot-8.9.4/src/spellbot/views/lfg_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/views/setup_view.py` & `spellbot-8.9.4/src/spellbot/views/setup_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/api/record.py` & `spellbot-8.9.4/src/spellbot/web/api/record.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/builder.py` & `spellbot-8.9.4/src/spellbot/web/builder.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/server.py` & `spellbot-8.9.4/src/spellbot/web/server.py`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/templates/channel_record.html.j2` & `spellbot-8.9.4/src/spellbot/web/templates/channel_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/templates/record.css` & `spellbot-8.9.4/src/spellbot/web/templates/record.css`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/templates/record_base.html.j2` & `spellbot-8.9.4/src/spellbot/web/templates/record_base.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/templates/table2CSV.js` & `spellbot-8.9.4/src/spellbot/web/templates/table2CSV.js`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/src/spellbot/web/templates/user_record.html.j2` & `spellbot-8.9.4/src/spellbot/web/templates/user_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-8.9.3/PKG-INFO` & `spellbot-8.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spellbot
-Version: 8.9.3
+Version: 8.9.4
 Summary: The Discord bot for SpellTable
 Home-page: http://spellbot.io/
 License: MIT
 Keywords: discord,magic,bot,mtg,SpellTable
 Author: Amy Troschinetz
 Author-email: spellbot@lexicalunit.com
 Requires-Python: >=3.10,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spellbot Version: 8.9.3 Summary: The Discord bot
+Metadata-Version: 2.1 Name: spellbot Version: 8.9.4 Summary: The Discord bot
 for SpellTable Home-page: http://spellbot.io/ License: MIT Keywords:
 discord,magic,bot,mtg,SpellTable Author: Amy Troschinetz Author-email:
 spellbot@lexicalunit.com Requires-Python: >=3.10,<4 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```


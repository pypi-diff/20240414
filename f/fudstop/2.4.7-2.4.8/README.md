# Comparing `tmp/fudstop-2.4.7.tar.gz` & `tmp/fudstop-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudstop-2.4.7.tar", last modified: Sat Apr 13 19:49:58 2024, max compression
+gzip compressed data, was "fudstop-2.4.8.tar", last modified: Sat Apr 13 19:57:29 2024, max compression
```

## Comparing `fudstop-2.4.7.tar` & `fudstop-2.4.8.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.549635 fudstop-2.4.7/
--rw-rw-rw-   0        0        0     7618 2024-04-13 19:49:58.549635 fudstop-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2024-01-05 23:27:36.000000 fudstop-2.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.377760 fudstop-2.4.7/app/
--rw-rw-rw-   0        0        0    43348 2024-01-23 23:29:23.000000 fudstop-2.4.7/app/__init__.py
--rw-rw-rw-   0        0        0     4011 2024-01-12 03:32:55.000000 fudstop-2.4.7/app/fetcher.py
--rw-rw-rw-   0        0        0    17884 2024-01-12 06:07:09.000000 fudstop-2.4.7/app/fudstop_info.py
--rw-rw-rw-   0        0        0    38553 2024-01-12 03:47:25.000000 fudstop-2.4.7/app/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.377760 fudstop-2.4.7/fudstop/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.393386 fudstop-2.4.7/fudstop/_markets/
--rw-rw-rw-   0        0        0     1327 2024-01-18 15:18:48.000000 fudstop-2.4.7/fudstop/_markets/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-02-22 04:18:16.000000 fudstop-2.4.7/fudstop/_markets/analyzers.py
--rw-rw-rw-   0        0        0    67237 2024-02-07 15:09:55.000000 fudstop-2.4.7/fudstop/_markets/embeddings.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.393386 fudstop-2.4.7/fudstop/_markets/finished/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:49:02.000000 fudstop-2.4.7/fudstop/_markets/finished/__init__.py
--rw-rw-rw-   0        0        0    25622 2024-01-21 19:47:09.000000 fudstop-2.4.7/fudstop/_markets/finished/db_manager.py
--rw-rw-rw-   0        0        0     2530 2023-10-12 23:34:06.000000 fudstop-2.4.7/fudstop/_markets/finished/economic_data.py
--rw-rw-rw-   0        0        0    53472 2024-02-11 04:30:33.000000 fudstop-2.4.7/fudstop/_markets/finished/master_class.py
--rw-rw-rw-   0        0        0     9940 2024-01-25 21:35:47.000000 fudstop-2.4.7/fudstop/_markets/finished/td9_states.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.393386 fudstop-2.4.7/fudstop/_markets/list_sets/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/list_sets/__init__.py
--rw-rw-rw-   0        0        0    92394 2024-02-22 03:17:43.000000 fudstop-2.4.7/fudstop/_markets/list_sets/dicts.py
--rw-rw-rw-   0        0        0    88831 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/list_sets/saved_tickers.py
--rw-rw-rw-   0        0        0   125429 2024-01-17 16:34:32.000000 fudstop-2.4.7/fudstop/_markets/list_sets/ticker_lists.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.409010 fudstop-2.4.7/fudstop/_markets/market_handlers/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/__init__.py
--rw-rw-rw-   0        0        0     1265 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/cfg.py
--rw-rw-rw-   0        0        0     1491 2024-01-09 04:43:27.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/crypto.py
--rw-rw-rw-   0        0        0    17424 2024-02-12 18:43:10.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/database_.py
--rw-rw-rw-   0        0        0      768 2024-01-09 05:02:23.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/forex.py
--rw-rw-rw-   0        0        0     1770 2024-01-08 17:15:06.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/indices.py
--rw-rw-rw-   0        0        0   762960 2024-01-11 23:53:54.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/list_sets.py
--rw-rw-rw-   0        0        0    13155 2024-01-11 17:06:04.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/options.py
--rw-rw-rw-   0        0        0     3929 2024-01-09 21:38:56.000000 fudstop-2.4.7/fudstop/_markets/market_handlers/stocks.py
--rw-rw-rw-   0        0        0     1166 2024-01-12 17:40:54.000000 fudstop-2.4.7/fudstop/_markets/monitor.py
--rw-rw-rw-   0        0        0    31105 2024-02-12 14:30:27.000000 fudstop-2.4.7/fudstop/_markets/multimarkets.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.409010 fudstop-2.4.7/fudstop/_markets/plotting/
--rw-rw-rw-   0        0        0     1814 2024-01-13 01:48:40.000000 fudstop-2.4.7/fudstop/_markets/plotting/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.409010 fudstop-2.4.7/fudstop/_markets/reference_markets/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/reference_markets/__init__.py
--rw-rw-rw-   0        0        0     1400 2024-01-08 00:31:15.000000 fudstop-2.4.7/fudstop/_markets/reference_markets/conditional_scans.py
--rw-rw-rw-   0        0        0     8389 2024-01-10 04:38:30.000000 fudstop-2.4.7/fudstop/_markets/reference_markets/reference_market.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.409010 fudstop-2.4.7/fudstop/_markets/scripts/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/scripts/__init__.py
--rw-rw-rw-   0        0        0      846 2024-01-20 18:45:32.000000 fudstop-2.4.7/fudstop/_markets/scripts/all_polygon_options.py
--rw-rw-rw-   0        0        0      683 2024-01-07 06:56:40.000000 fudstop-2.4.7/fudstop/_markets/scripts/all_webull_options.py
--rw-rw-rw-   0        0        0     1208 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/scripts/generation.py
--rw-rw-rw-   0        0        0     1351 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/_markets/scripts/million_dollar_trades.py
--rw-rw-rw-   0        0        0     1533 2024-01-18 14:58:07.000000 fudstop-2.4.7/fudstop/_markets/scripts/option_scripts.py
--rw-rw-rw-   0        0        0    20845 2024-01-20 18:50:03.000000 fudstop-2.4.7/fudstop/_markets/scripts/options_market.py
--rw-rw-rw-   0        0        0     2961 2024-01-11 18:09:48.000000 fudstop-2.4.7/fudstop/_markets/scripts/options_volume_analysis.py
--rw-rw-rw-   0        0        0     1942 2024-01-11 18:07:34.000000 fudstop-2.4.7/fudstop/_markets/scripts/rsi_2_4_8.py
--rw-rw-rw-   0        0        0     2172 2024-01-24 23:43:15.000000 fudstop-2.4.7/fudstop/_markets/scripts/rsi_screener.py
--rw-rw-rw-   0        0        0     1197 2024-01-20 05:06:57.000000 fudstop-2.4.7/fudstop/_markets/scripts/ssr_scanner.py
--rw-rw-rw-   0        0        0     7315 2024-01-23 17:20:40.000000 fudstop-2.4.7/fudstop/_markets/scripts/stock_market.py
--rw-rw-rw-   0        0        0     6271 2024-01-12 19:46:21.000000 fudstop-2.4.7/fudstop/_markets/scripts/td9_states.py
--rw-rw-rw-   0        0        0    14287 2024-02-06 18:37:20.000000 fudstop-2.4.7/fudstop/_markets/scripts/universal_snapshot.py
--rw-rw-rw-   0        0        0    13782 2024-01-25 20:46:06.000000 fudstop-2.4.7/fudstop/_markets/stock_market.py
--rw-rw-rw-   0        0        0     1893 2024-01-10 18:26:30.000000 fudstop-2.4.7/fudstop/_markets/webhook_dicts.py
--rw-rw-rw-   0        0        0    14911 2024-01-06 18:40:07.000000 fudstop-2.4.7/fudstop/all_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/_asyncpg/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:59.000000 fudstop-2.4.7/fudstop/apis/_asyncpg/__init__.py
--rw-rw-rw-   0        0        0    15085 2024-03-26 19:05:42.000000 fudstop-2.4.7/fudstop/apis/_asyncpg/asyncpg_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/_datetime/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:52.000000 fudstop-2.4.7/fudstop/apis/_datetime/__init__.py
--rw-rw-rw-   0        0        0      100 2024-02-29 08:36:35.000000 fudstop-2.4.7/fudstop/apis/_datetime/datetime_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/_openai/
--rw-rw-rw-   0        0        0        0 2024-01-07 17:40:15.000000 fudstop-2.4.7/fudstop/apis/_openai/__init__.py
--rw-rw-rw-   0        0        0     4824 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/_openai/agent.py
--rw-rw-rw-   0        0        0     7552 2024-03-07 23:34:16.000000 fudstop-2.4.7/fudstop/apis/_openai/openai_sdk.py
--rw-rw-rw-   0        0        0    27388 2024-02-25 03:36:21.000000 fudstop-2.4.7/fudstop/apis/_openai/tools_shcema.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/_pandas/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:42:25.000000 fudstop-2.4.7/fudstop/apis/_pandas/__init__.py
--rw-rw-rw-   0        0        0      226 2024-02-29 20:44:07.000000 fudstop-2.4.7/fudstop/apis/_pandas/pandas_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/_selenium/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/_selenium/__init__.py
--rw-rw-rw-   0        0        0     1863 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/_selenium/selenium_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/cfr/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/cfr/__init__.py
--rw-rw-rw-   0        0        0     3742 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/cfr/cfr_2.0.py
--rw-rw-rw-   0        0        0       87 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/cfr/cfr_helpers.py
--rw-rw-rw-   0        0        0     7590 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/cfr/cfr_sdk.py
--rw-rw-rw-   0        0        0     2525 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/cfr/title_12.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/datalink/
--rw-rw-rw-   0        0        0        0 2024-03-25 21:17:59.000000 fudstop-2.4.7/fudstop/apis/datalink/__init__.py
--rw-rw-rw-   0        0        0     2661 2024-03-27 07:04:34.000000 fudstop-2.4.7/fudstop/apis/datalink/datalink_sdk.py
--rw-rw-rw-   0        0        0     2609 2024-03-25 21:32:23.000000 fudstop-2.4.7/fudstop/apis/datalink/models.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/discord_/
--rw-rw-rw-   0        0        0     4430 2024-01-08 04:14:36.000000 fudstop-2.4.7/fudstop/apis/discord_/__init__.py
--rw-rw-rw-   0        0        0    12863 2024-02-23 01:28:51.000000 fudstop-2.4.7/fudstop/apis/discord_/discord_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/discord_/models/
--rw-rw-rw-   0        0        0        0 2024-01-18 14:52:13.000000 fudstop-2.4.7/fudstop/apis/discord_/models/__init__.py
--rw-rw-rw-   0        0        0     5431 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/discord_/models/application_commands.py
--rw-rw-rw-   0        0        0     2767 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/discord_/models/search.py
--rw-rw-rw-   0        0        0     1101 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/discord_/models/webhooks.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.424636 fudstop-2.4.7/fudstop/apis/earnings_whisper/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/earnings_whisper/__init__.py
--rw-rw-rw-   0        0        0    12823 2024-03-25 21:47:38.000000 fudstop-2.4.7/fudstop/apis/earnings_whisper/ew_models.py
--rw-rw-rw-   0        0        0     4016 2024-03-25 21:44:18.000000 fudstop-2.4.7/fudstop/apis/earnings_whisper/ew_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/fed_print/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/fed_print/__init__.py
--rw-rw-rw-   0        0        0     2908 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/fed_print/fed_print_sync.py
--rw-rw-rw-   0        0        0     5322 2024-02-24 20:29:40.000000 fudstop-2.4.7/fudstop/apis/fed_print/fedprint_models.py
--rw-rw-rw-   0        0        0     3354 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/fed_print/fedprint_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/federal_register/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/federal_register/__init__.py
--rw-rw-rw-   0        0        0     3075 2024-02-25 17:21:39.000000 fudstop-2.4.7/fudstop/apis/federal_register/fed_register_sdk.py
--rw-rw-rw-   0        0        0     2924 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/federal_register/fed_register_sync.py
--rw-rw-rw-   0        0        0     2904 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/federal_register/register_models.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/gexbot/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/gexbot/__init__.py
--rw-rw-rw-   0        0        0     4095 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/gexbot/gexbot.py
--rw-rw-rw-   0        0        0     4139 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/gexbot/models.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/gpts/
--rw-rw-rw-   0        0        0      231 2024-01-08 03:41:52.000000 fudstop-2.4.7/fudstop/apis/gpts/DiscoAI.py
--rw-rw-rw-   0        0        0        2 2024-01-08 03:38:45.000000 fudstop-2.4.7/fudstop/apis/gpts/__init__.py
--rw-rw-rw-   0        0        0    35379 2024-03-27 01:57:02.000000 fudstop-2.4.7/fudstop/apis/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/master/
--rw-rw-rw-   0        0        0        0 2024-02-25 05:43:46.000000 fudstop-2.4.7/fudstop/apis/master/__init__.py
--rw-rw-rw-   0        0        0     1459 2024-02-25 09:02:57.000000 fudstop-2.4.7/fudstop/apis/master/master_helpers.py
--rw-rw-rw-   0        0        0    29960 2024-02-25 19:23:31.000000 fudstop-2.4.7/fudstop/apis/master/master_sdk.py
--rw-rw-rw-   0        0        0    34633 2024-02-25 09:11:27.000000 fudstop-2.4.7/fudstop/apis/master/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/misc/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/misc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/misc/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/misc/models/__init__.py
--rw-rw-rw-   0        0        0      249 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/misc/models/unsplash_models.py
--rw-rw-rw-   0        0        0     2204 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/misc/models/weather_models.py
--rw-rw-rw-   0        0        0      869 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/misc/unsplash.py
--rw-rw-rw-   0        0        0     1790 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/misc/weather.py
--rw-rw-rw-   0        0        0      294 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/misc/weather_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/nasdaq/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4200 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/nasdaq/nasdaq_lists.py
--rw-rw-rw-   0        0        0    12177 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/nasdaq/nasdaq_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.440260 fudstop-2.4.7/fudstop/apis/newyork_fed/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/newyork_fed/__init__.py
--rw-rw-rw-   0        0        0    14970 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/newyork_fed/models.py
--rw-rw-rw-   0        0        0    22750 2024-03-27 00:32:52.000000 fudstop-2.4.7/fudstop/apis/newyork_fed/newyork_fed_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.455885 fudstop-2.4.7/fudstop/apis/occ/
--rw-rw-rw-   0        0        0        0 2024-01-12 03:42:31.000000 fudstop-2.4.7/fudstop/apis/occ/__init__.py
--rw-rw-rw-   0        0        0    30622 2024-03-27 02:16:15.000000 fudstop-2.4.7/fudstop/apis/occ/occ_models.py
--rw-rw-rw-   0        0        0    14100 2024-03-27 02:05:52.000000 fudstop-2.4.7/fudstop/apis/occ/occ_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.455885 fudstop-2.4.7/fudstop/apis/ofr/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/ofr/__init__.py
--rw-rw-rw-   0        0        0    37577 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/ofr/ofr_list_sets.py
--rw-rw-rw-   0        0        0     5462 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/ofr/ofr_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.455885 fudstop-2.4.7/fudstop/apis/oic/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/oic/__init__.py
--rw-rw-rw-   0        0        0    16116 2024-01-07 16:09:24.000000 fudstop-2.4.7/fudstop/apis/oic/async_oic_sdk.py
--rw-rw-rw-   0        0        0    11292 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/oic/oic_models.py
--rw-rw-rw-   0        0        0     4938 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/oic/oic_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.471510 fudstop-2.4.7/fudstop/apis/polygonio/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/__init__.py
--rw-rw-rw-   0        0        0    30265 2024-04-13 19:49:39.000000 fudstop-2.4.7/fudstop/apis/polygonio/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     2368 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/db_polygon.py
--rw-rw-rw-   0        0        0    47011 2024-01-10 15:38:01.000000 fudstop-2.4.7/fudstop/apis/polygonio/mapping.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.471510 fudstop-2.4.7/fudstop/apis/polygonio/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/__init__.py
--rw-rw-rw-   0        0        0     1330 2024-04-13 19:03:08.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/aggregates.py
--rw-rw-rw-   0        0        0     1319 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/company_info.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.471510 fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/__init__.py
--rw-rw-rw-   0        0        0     5734 2024-01-12 15:43:51.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/option_snapshot.py
--rw-rw-rw-   0        0        0     7043 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/universal_option.py
--rw-rw-rw-   0        0        0    57290 2024-03-07 18:09:56.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/universal_snapshot.py
--rw-rw-rw-   0        0        0     6954 2024-01-10 06:10:49.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/technicals.py
--rw-rw-rw-   0        0        0     2271 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/ticker_news.py
--rw-rw-rw-   0        0        0     3801 2024-01-07 01:51:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/ticker_snapshot.py
--rw-rw-rw-   0        0        0     5787 2024-01-21 19:53:33.000000 fudstop-2.4.7/fudstop/apis/polygonio/models/trades.py
--rw-rw-rw-   0        0        0    13028 2024-02-18 06:32:56.000000 fudstop-2.4.7/fudstop/apis/polygonio/polygon_database.py
--rw-rw-rw-   0        0        0    41160 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/polygon_helpers.py
--rw-rw-rw-   0        0        0    68480 2024-03-07 21:00:57.000000 fudstop-2.4.7/fudstop/apis/polygonio/polygon_options.py
--rw-rw-rw-   0        0        0     3692 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/polygon_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.471510 fudstop-2.4.7/fudstop/apis/polygonio/scripts/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/scripts/__init__.py
--rw-rw-rw-   0        0        0     2267 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/polygonio/scripts/daily_aggregates.py
--rw-rw-rw-   0        0        0     1716 2024-02-04 09:29:32.000000 fudstop-2.4.7/fudstop/apis/polygonio/scripts/rsi.py
--rw-rw-rw-   0        0        0     9164 2024-03-01 01:05:43.000000 fudstop-2.4.7/fudstop/apis/polygonio/technicals.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.471510 fudstop-2.4.7/fudstop/apis/rss/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/rss/__init__.py
--rw-rw-rw-   0        0        0      736 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/rss/rss_helpers.py
--rw-rw-rw-   0        0        0     1497 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/rss/rss_models.py
--rw-rw-rw-   0        0        0    10360 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/apis/rss/rss_sdk.py
--rw-rw-rw-   0        0        0    10203 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/apis/rss/snyc_rss.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.471510 fudstop-2.4.7/fudstop/apis/sec/
--rw-rw-rw-   0        0        0        0 2024-02-29 20:06:34.000000 fudstop-2.4.7/fudstop/apis/sec/__init__.py
--rw-rw-rw-   0        0        0     8441 2024-02-29 22:33:02.000000 fudstop-2.4.7/fudstop/apis/sec/sec_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.471510 fudstop-2.4.7/fudstop/apis/stocksera_/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.487136 fudstop-2.4.7/fudstop/apis/stocksera_/models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/__init__.py
--rw-rw-rw-   0        0        0      487 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/borrowed_shares.py
--rw-rw-rw-   0        0        0      827 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/daily_treasury.py
--rw-rw-rw-   0        0        0      747 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/ftds.py
--rw-rw-rw-   0        0        0      871 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/highest_shorted.py
--rw-rw-rw-   0        0        0      813 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/inflation.py
--rw-rw-rw-   0        0        0     1062 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/insider_trades.py
--rw-rw-rw-   0        0        0      667 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/jim_cramer.py
--rw-rw-rw-   0        0        0      850 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/jobless_claims.py
--rw-rw-rw-   0        0        0     1043 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/low_float.py
--rw-rw-rw-   0        0        0      660 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/market_news.py
--rw-rw-rw-   0        0        0    21824 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/models.py
--rw-rw-rw-   0        0        0      676 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/news_sentiment.py
--rw-rw-rw-   0        0        0      693 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/retail_sales.py
--rw-rw-rw-   0        0        0      708 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/reverse_repo.py
--rw-rw-rw-   0        0        0      777 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/sec_filings.py
--rw-rw-rw-   0        0        0      789 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/models/short_volume.py
--rw-rw-rw-   0        0        0    19676 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/stocksera_/stocksera_.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.487136 fudstop-2.4.7/fudstop/apis/treasury/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/treasury/__init__.py
--rw-rw-rw-   0        0        0    10964 2024-01-20 19:15:58.000000 fudstop-2.4.7/fudstop/apis/treasury/treasury_models.py
--rw-rw-rw-   0        0        0    10281 2024-01-20 19:16:09.000000 fudstop-2.4.7/fudstop/apis/treasury/treasury_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.487136 fudstop-2.4.7/fudstop/apis/webull/
--rw-rw-rw-   0        0        0     4945 2024-01-15 22:06:39.000000 fudstop-2.4.7/fudstop/apis/webull/__init__.py
--rw-rw-rw-   0        0        0    12127 2024-01-23 03:47:19.000000 fudstop-2.4.7/fudstop/apis/webull/database_manager.py
--rw-rw-rw-   0        0        0     2732 2024-01-11 18:10:25.000000 fudstop-2.4.7/fudstop/apis/webull/get_volume_analysis.py
--rw-rw-rw-   0        0        0    10628 2024-01-11 18:10:17.000000 fudstop-2.4.7/fudstop/apis/webull/modal.py
--rw-rw-rw-   0        0        0     5320 2024-01-10 21:10:43.000000 fudstop-2.4.7/fudstop/apis/webull/opt_modal.py
--rw-rw-rw-   0        0        0     9390 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/options.py
--rw-rw-rw-   0        0        0     3357 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/screener_models.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.502760 fudstop-2.4.7/fudstop/apis/webull/trade_models/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-02-18 21:14:42.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/analyst_ratings.py
--rw-rw-rw-   0        0        0    12121 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/capital_flow.py
--rw-rw-rw-   0        0        0     2147 2024-02-24 19:57:32.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/company_brief.py
--rw-rw-rw-   0        0        0     2235 2024-01-23 05:04:58.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/cost_distribution.py
--rw-rw-rw-   0        0        0     1053 2024-02-18 19:14:15.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/etf_holdings.py
--rw-rw-rw-   0        0        0     1727 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/events.py
--rw-rw-rw-   0        0        0    19884 2024-02-18 19:14:03.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/financials.py
--rw-rw-rw-   0        0        0     3780 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/forecast_evaluator.py
--rw-rw-rw-   0        0        0     3500 2024-02-18 18:48:35.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/institutional_holdings.py
--rw-rw-rw-   0        0        0     1335 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/news.py
--rw-rw-rw-   0        0        0     1195 2024-03-01 01:13:55.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/price_streamer.py
--rw-rw-rw-   0        0        0      601 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/short_interest.py
--rw-rw-rw-   0        0        0    11042 2024-03-07 17:43:34.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/ticker_query.py
--rw-rw-rw-   0        0        0     1314 2024-01-13 16:23:06.000000 fudstop-2.4.7/fudstop/apis/webull/trade_models/volume_analysis.py
--rw-rw-rw-   0        0        0    13181 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/webull/webull_helpers.py
--rw-rw-rw-   0        0        0    12274 2024-02-25 06:46:04.000000 fudstop-2.4.7/fudstop/apis/webull/webull_markets.py
--rw-rw-rw-   0        0        0    35666 2024-01-21 19:47:41.000000 fudstop-2.4.7/fudstop/apis/webull/webull_options.py
--rw-rw-rw-   0        0        0     9106 2024-01-18 22:00:22.000000 fudstop-2.4.7/fudstop/apis/webull/webull_parsing.py
--rw-rw-rw-   0        0        0     7131 2024-02-26 02:07:00.000000 fudstop-2.4.7/fudstop/apis/webull/webull_screener.py
--rw-rw-rw-   0        0        0    26318 2024-03-27 00:20:49.000000 fudstop-2.4.7/fudstop/apis/webull/webull_trading.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.502760 fudstop-2.4.7/fudstop/apis/whale/
--rw-rw-rw-   0        0        0        0 2024-03-27 06:54:53.000000 fudstop-2.4.7/fudstop/apis/whale/__init__.py
--rw-rw-rw-   0        0        0    42102 2024-03-27 21:07:42.000000 fudstop-2.4.7/fudstop/apis/whale/whale_models.py
--rw-rw-rw-   0        0        0     7065 2024-03-27 21:07:56.000000 fudstop-2.4.7/fudstop/apis/whale/whale_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.502760 fudstop-2.4.7/fudstop/apis/y_finance/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/apis/y_finance/__init__.py
--rw-rw-rw-   0        0        0     9028 2024-02-18 15:18:29.000000 fudstop-2.4.7/fudstop/apis/y_finance/yf_sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.502760 fudstop-2.4.7/fudstop/database_/
--rw-rw-rw-   0        0        0    66479 2024-02-18 06:41:46.000000 fudstop-2.4.7/fudstop/database_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.502760 fudstop-2.4.7/fudstop/discord_/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/discord_/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-01-11 18:10:55.000000 fudstop-2.4.7/fudstop/discord_/autocomp.py
--rw-rw-rw-   0        0        0    63334 2024-01-15 01:59:11.000000 fudstop-2.4.7/fudstop/discord_/bot.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.518385 fudstop-2.4.7/fudstop/discord_/bot_menus/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/discord_/bot_menus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.518385 fudstop-2.4.7/fudstop/discord_/bot_menus/modals/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/discord_/bot_menus/modals/__init__.py
--rw-rw-rw-   0        0        0     2226 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/discord_/bot_menus/modals/dalle_modal.py
--rw-rw-rw-   0        0        0    13054 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/discord_/bot_menus/modals/options_modal.py
--rw-rw-rw-   0        0        0     3597 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/discord_/bot_menus/pagination.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.518385 fudstop-2.4.7/fudstop/discord_/cogs/
--rw-rw-rw-   0        0        0     4305 2024-01-07 18:05:54.000000 fudstop-2.4.7/fudstop/discord_/cogs/__init__.py
--rw-rw-rw-   0        0        0    20340 2024-01-06 18:32:34.000000 fudstop-2.4.7/fudstop/discord_/cogs/accounting.py
--rw-rw-rw-   0        0        0    11559 2024-01-06 18:29:35.000000 fudstop-2.4.7/fudstop/discord_/cogs/assistant.py
--rw-rw-rw-   0        0        0    11795 2024-02-06 17:49:34.000000 fudstop-2.4.7/fudstop/discord_/cogs/database.py
--rw-rw-rw-   0        0        0    12937 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/discord_/cogs/earnings.py
--rw-rw-rw-   0        0        0     2104 2024-01-06 18:30:08.000000 fudstop-2.4.7/fudstop/discord_/cogs/fed_print.py
--rw-rw-rw-   0        0        0     4463 2024-01-11 18:16:25.000000 fudstop-2.4.7/fudstop/discord_/cogs/filter.py
--rw-rw-rw-   0        0        0    34896 2024-01-11 18:17:51.000000 fudstop-2.4.7/fudstop/discord_/cogs/fiscal_service.py
--rw-rw-rw-   0        0        0     4482 2024-01-07 16:10:05.000000 fudstop-2.4.7/fudstop/discord_/cogs/gex.py
--rw-rw-rw-   0        0        0     6390 2024-02-07 19:46:50.000000 fudstop-2.4.7/fudstop/discord_/cogs/gpt.py
--rw-rw-rw-   0        0        0     3906 2024-02-17 21:04:28.000000 fudstop-2.4.7/fudstop/discord_/cogs/ibrs.py
--rw-rw-rw-   0        0        0     2313 2024-01-06 18:31:02.000000 fudstop-2.4.7/fudstop/discord_/cogs/main_view.py
--rw-rw-rw-   0        0        0    29489 2024-04-06 03:42:15.000000 fudstop-2.4.7/fudstop/discord_/cogs/options.py
--rw-rw-rw-   0        0        0     3827 2024-01-11 18:16:07.000000 fudstop-2.4.7/fudstop/discord_/cogs/plays.py
--rw-rw-rw-   0        0        0     3428 2024-01-06 18:35:15.000000 fudstop-2.4.7/fudstop/discord_/cogs/register.py
--rw-rw-rw-   0        0        0     3800 2024-01-06 18:31:37.000000 fudstop-2.4.7/fudstop/discord_/cogs/spx.py
--rw-rw-rw-   0        0        0     9302 2024-01-11 18:15:53.000000 fudstop-2.4.7/fudstop/discord_/cogs/strategy.py
--rw-rw-rw-   0        0        0     2776 2024-01-06 18:31:52.000000 fudstop-2.4.7/fudstop/discord_/cogs/ta.py
--rw-rw-rw-   0        0        0     3071 2024-01-06 18:32:00.000000 fudstop-2.4.7/fudstop/discord_/cogs/weather.py
--rw-rw-rw-   0        0        0     1346 2024-01-06 18:32:07.000000 fudstop-2.4.7/fudstop/discord_/cogs/webull.py
--rw-rw-rw-   0        0        0    11097 2024-01-06 18:32:21.000000 fudstop-2.4.7/fudstop/discord_/cogs/yfin.py
--rw-rw-rw-   0        0        0     1843 2024-01-14 21:57:53.000000 fudstop-2.4.7/fudstop/discord_/database_getter.py
--rw-rw-rw-   0        0        0     6337 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/discord_/discord_rsi.py
--rw-rw-rw-   0        0        0     3697 2024-01-06 18:23:33.000000 fudstop-2.4.7/fudstop/discord_/embeddings.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.534010 fudstop-2.4.7/fudstop/examples/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/__init__.py
--rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/ecfr_test.py
--rw-rw-rw-   0        0        0      178 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/fed_print_test.py
--rw-rw-rw-   0        0        0      237 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/fed_reg_test.py
--rw-rw-rw-   0        0        0      258 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/nasdaq_test.py
--rw-rw-rw-   0        0        0      181 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/newyork_fed_test.py
--rw-rw-rw-   0        0        0     3793 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/ofr_test.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.534010 fudstop-2.4.7/fudstop/examples/polygonio/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/polygonio/__init__.py
--rw-rw-rw-   0        0        0     1392 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/examples/polygonio/aggregates_second.py
--rw-rw-rw-   0        0        0      709 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/examples/polygonio/company_info.py
--rw-rw-rw-   0        0        0     2345 2024-01-07 23:40:02.000000 fudstop-2.4.7/fudstop/examples/polygonio/get_all_options.py
--rw-rw-rw-   0        0        0      379 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/examples/polygonio/get_all_tickers.py
--rw-rw-rw-   0        0        0      611 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/polygonio/get_near_the_money.py
--rw-rw-rw-   0        0        0     2307 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/polygonio/get_option_aggs.py
--rw-rw-rw-   0        0        0     1190 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/polygonio/get_option_rsi.py
--rw-rw-rw-   0        0        0     3751 2024-01-06 00:03:40.000000 fudstop-2.4.7/fudstop/examples/polygonio/get_option_trades.py
--rw-rw-rw-   0        0        0     2409 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/polygonio/get_ticker_aggs.py
--rw-rw-rw-   0        0        0      683 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/examples/polygonio/market_news.py
--rw-rw-rw-   0        0        0     1305 2024-01-11 18:07:47.000000 fudstop-2.4.7/fudstop/examples/polygonio/polygon_test.py
--rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/scripty.py
--rw-rw-rw-   0        0        0     1871 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/stocksera_test.py
--rw-rw-rw-   0        0        0      776 2024-01-06 17:35:55.000000 fudstop-2.4.7/fudstop/examples/test.py
--rw-rw-rw-   0        0        0     2721 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/test_gex.py
--rw-rw-rw-   0        0        0      284 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/test_insert.py
--rw-rw-rw-   0        0        0     2255 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/test_openai.py
--rw-rw-rw-   0        0        0      698 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/test_opts.py
--rw-rw-rw-   0        0        0      633 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/test_screener.py
--rw-rw-rw-   0        0        0     4324 2024-01-11 18:10:12.000000 fudstop-2.4.7/fudstop/examples/test_sec.py
--rw-rw-rw-   0        0        0     1758 2024-01-11 18:11:03.000000 fudstop-2.4.7/fudstop/examples/test_webull.py
--rw-rw-rw-   0        0        0        0 2024-01-08 17:00:41.000000 fudstop-2.4.7/fudstop/examples/tests_discord.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.534010 fudstop-2.4.7/fudstop/examples/webull/
--rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/webull/__init__.py
--rw-rw-rw-   0        0        0      805 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/webull/markets_example.py
--rw-rw-rw-   0        0        0     2439 2024-01-05 23:27:36.000000 fudstop-2.4.7/fudstop/examples/webull/trade_example.py
--rw-rw-rw-   0        0        0     7753 2024-01-11 18:14:32.000000 fudstop-2.4.7/fudstop/options_filter.py
--rw-rw-rw-   0        0        0    21800 2024-01-11 18:09:07.000000 fudstop-2.4.7/fudstop/plots.py
--rw-rw-rw-   0        0        0    15233 2024-01-11 18:14:18.000000 fudstop-2.4.7/fudstop/schema.py
--rw-rw-rw-   0        0        0      490 2024-02-04 05:36:05.000000 fudstop-2.4.7/fudstop/wet.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:49:58.393386 fudstop-2.4.7/fudstop.egg-info/
--rw-rw-rw-   0        0        0     7618 2024-04-13 19:49:58.000000 fudstop-2.4.7/fudstop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10588 2024-04-13 19:49:58.000000 fudstop-2.4.7/fudstop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 19:49:58.000000 fudstop-2.4.7/fudstop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4028 2024-04-13 19:49:58.000000 fudstop-2.4.7/fudstop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-13 19:49:58.000000 fudstop-2.4.7/fudstop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 19:49:58.549635 fudstop-2.4.7/setup.cfg
--rw-rw-rw-   0        0        0      363 2024-04-13 19:49:54.000000 fudstop-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.651394 fudstop-2.4.8/
+-rw-rw-rw-   0        0        0     7618 2024-04-13 19:57:29.651394 fudstop-2.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2341 2024-01-05 23:27:36.000000 fudstop-2.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.463892 fudstop-2.4.8/app/
+-rw-rw-rw-   0        0        0    43348 2024-01-23 23:29:23.000000 fudstop-2.4.8/app/__init__.py
+-rw-rw-rw-   0        0        0     4011 2024-01-12 03:32:55.000000 fudstop-2.4.8/app/fetcher.py
+-rw-rw-rw-   0        0        0    17884 2024-01-12 06:07:09.000000 fudstop-2.4.8/app/fudstop_info.py
+-rw-rw-rw-   0        0        0    38553 2024-01-12 03:47:25.000000 fudstop-2.4.8/app/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.479518 fudstop-2.4.8/fudstop/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.495144 fudstop-2.4.8/fudstop/_markets/
+-rw-rw-rw-   0        0        0     1327 2024-01-18 15:18:48.000000 fudstop-2.4.8/fudstop/_markets/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-02-22 04:18:16.000000 fudstop-2.4.8/fudstop/_markets/analyzers.py
+-rw-rw-rw-   0        0        0    67237 2024-02-07 15:09:55.000000 fudstop-2.4.8/fudstop/_markets/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.495144 fudstop-2.4.8/fudstop/_markets/finished/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:49:02.000000 fudstop-2.4.8/fudstop/_markets/finished/__init__.py
+-rw-rw-rw-   0        0        0    25622 2024-01-21 19:47:09.000000 fudstop-2.4.8/fudstop/_markets/finished/db_manager.py
+-rw-rw-rw-   0        0        0     2530 2023-10-12 23:34:06.000000 fudstop-2.4.8/fudstop/_markets/finished/economic_data.py
+-rw-rw-rw-   0        0        0    53472 2024-02-11 04:30:33.000000 fudstop-2.4.8/fudstop/_markets/finished/master_class.py
+-rw-rw-rw-   0        0        0     9940 2024-01-25 21:35:47.000000 fudstop-2.4.8/fudstop/_markets/finished/td9_states.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.495144 fudstop-2.4.8/fudstop/_markets/list_sets/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/list_sets/__init__.py
+-rw-rw-rw-   0        0        0    92394 2024-02-22 03:17:43.000000 fudstop-2.4.8/fudstop/_markets/list_sets/dicts.py
+-rw-rw-rw-   0        0        0    88831 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/list_sets/saved_tickers.py
+-rw-rw-rw-   0        0        0   125429 2024-01-17 16:34:32.000000 fudstop-2.4.8/fudstop/_markets/list_sets/ticker_lists.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.495144 fudstop-2.4.8/fudstop/_markets/market_handlers/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/__init__.py
+-rw-rw-rw-   0        0        0     1265 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/cfg.py
+-rw-rw-rw-   0        0        0     1491 2024-01-09 04:43:27.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/crypto.py
+-rw-rw-rw-   0        0        0    17424 2024-02-12 18:43:10.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/database_.py
+-rw-rw-rw-   0        0        0      768 2024-01-09 05:02:23.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/forex.py
+-rw-rw-rw-   0        0        0     1770 2024-01-08 17:15:06.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/indices.py
+-rw-rw-rw-   0        0        0   762960 2024-01-11 23:53:54.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/list_sets.py
+-rw-rw-rw-   0        0        0    13155 2024-01-11 17:06:04.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/options.py
+-rw-rw-rw-   0        0        0     3929 2024-01-09 21:38:56.000000 fudstop-2.4.8/fudstop/_markets/market_handlers/stocks.py
+-rw-rw-rw-   0        0        0     1166 2024-01-12 17:40:54.000000 fudstop-2.4.8/fudstop/_markets/monitor.py
+-rw-rw-rw-   0        0        0    31105 2024-02-12 14:30:27.000000 fudstop-2.4.8/fudstop/_markets/multimarkets.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.495144 fudstop-2.4.8/fudstop/_markets/plotting/
+-rw-rw-rw-   0        0        0     1814 2024-01-13 01:48:40.000000 fudstop-2.4.8/fudstop/_markets/plotting/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.510769 fudstop-2.4.8/fudstop/_markets/reference_markets/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/reference_markets/__init__.py
+-rw-rw-rw-   0        0        0     1400 2024-01-08 00:31:15.000000 fudstop-2.4.8/fudstop/_markets/reference_markets/conditional_scans.py
+-rw-rw-rw-   0        0        0     8389 2024-01-10 04:38:30.000000 fudstop-2.4.8/fudstop/_markets/reference_markets/reference_market.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.510769 fudstop-2.4.8/fudstop/_markets/scripts/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/scripts/__init__.py
+-rw-rw-rw-   0        0        0      846 2024-01-20 18:45:32.000000 fudstop-2.4.8/fudstop/_markets/scripts/all_polygon_options.py
+-rw-rw-rw-   0        0        0      683 2024-01-07 06:56:40.000000 fudstop-2.4.8/fudstop/_markets/scripts/all_webull_options.py
+-rw-rw-rw-   0        0        0     1208 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/scripts/generation.py
+-rw-rw-rw-   0        0        0     1351 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/_markets/scripts/million_dollar_trades.py
+-rw-rw-rw-   0        0        0     1533 2024-01-18 14:58:07.000000 fudstop-2.4.8/fudstop/_markets/scripts/option_scripts.py
+-rw-rw-rw-   0        0        0    20845 2024-01-20 18:50:03.000000 fudstop-2.4.8/fudstop/_markets/scripts/options_market.py
+-rw-rw-rw-   0        0        0     2961 2024-01-11 18:09:48.000000 fudstop-2.4.8/fudstop/_markets/scripts/options_volume_analysis.py
+-rw-rw-rw-   0        0        0     1942 2024-01-11 18:07:34.000000 fudstop-2.4.8/fudstop/_markets/scripts/rsi_2_4_8.py
+-rw-rw-rw-   0        0        0     2172 2024-01-24 23:43:15.000000 fudstop-2.4.8/fudstop/_markets/scripts/rsi_screener.py
+-rw-rw-rw-   0        0        0     1197 2024-01-20 05:06:57.000000 fudstop-2.4.8/fudstop/_markets/scripts/ssr_scanner.py
+-rw-rw-rw-   0        0        0     7315 2024-01-23 17:20:40.000000 fudstop-2.4.8/fudstop/_markets/scripts/stock_market.py
+-rw-rw-rw-   0        0        0     6271 2024-01-12 19:46:21.000000 fudstop-2.4.8/fudstop/_markets/scripts/td9_states.py
+-rw-rw-rw-   0        0        0    14287 2024-02-06 18:37:20.000000 fudstop-2.4.8/fudstop/_markets/scripts/universal_snapshot.py
+-rw-rw-rw-   0        0        0    13782 2024-01-25 20:46:06.000000 fudstop-2.4.8/fudstop/_markets/stock_market.py
+-rw-rw-rw-   0        0        0     1893 2024-01-10 18:26:30.000000 fudstop-2.4.8/fudstop/_markets/webhook_dicts.py
+-rw-rw-rw-   0        0        0    14911 2024-01-06 18:40:07.000000 fudstop-2.4.8/fudstop/all_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.510769 fudstop-2.4.8/fudstop/apis/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.510769 fudstop-2.4.8/fudstop/apis/_asyncpg/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:59.000000 fudstop-2.4.8/fudstop/apis/_asyncpg/__init__.py
+-rw-rw-rw-   0        0        0    15085 2024-03-26 19:05:42.000000 fudstop-2.4.8/fudstop/apis/_asyncpg/asyncpg_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.510769 fudstop-2.4.8/fudstop/apis/_datetime/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:52.000000 fudstop-2.4.8/fudstop/apis/_datetime/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-02-29 08:36:35.000000 fudstop-2.4.8/fudstop/apis/_datetime/datetime_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.510769 fudstop-2.4.8/fudstop/apis/_openai/
+-rw-rw-rw-   0        0        0        0 2024-01-07 17:40:15.000000 fudstop-2.4.8/fudstop/apis/_openai/__init__.py
+-rw-rw-rw-   0        0        0     4824 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/_openai/agent.py
+-rw-rw-rw-   0        0        0     7552 2024-03-07 23:34:16.000000 fudstop-2.4.8/fudstop/apis/_openai/openai_sdk.py
+-rw-rw-rw-   0        0        0    27388 2024-02-25 03:36:21.000000 fudstop-2.4.8/fudstop/apis/_openai/tools_shcema.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.510769 fudstop-2.4.8/fudstop/apis/_pandas/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:42:25.000000 fudstop-2.4.8/fudstop/apis/_pandas/__init__.py
+-rw-rw-rw-   0        0        0      226 2024-02-29 20:44:07.000000 fudstop-2.4.8/fudstop/apis/_pandas/pandas_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/_selenium/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/_selenium/__init__.py
+-rw-rw-rw-   0        0        0     1863 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/_selenium/selenium_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/cfr/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/cfr/__init__.py
+-rw-rw-rw-   0        0        0     3742 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/cfr/cfr_2.0.py
+-rw-rw-rw-   0        0        0       87 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/cfr/cfr_helpers.py
+-rw-rw-rw-   0        0        0     7590 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/cfr/cfr_sdk.py
+-rw-rw-rw-   0        0        0     2525 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/cfr/title_12.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/datalink/
+-rw-rw-rw-   0        0        0        0 2024-03-25 21:17:59.000000 fudstop-2.4.8/fudstop/apis/datalink/__init__.py
+-rw-rw-rw-   0        0        0     2661 2024-03-27 07:04:34.000000 fudstop-2.4.8/fudstop/apis/datalink/datalink_sdk.py
+-rw-rw-rw-   0        0        0     2609 2024-03-25 21:32:23.000000 fudstop-2.4.8/fudstop/apis/datalink/models.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/discord_/
+-rw-rw-rw-   0        0        0     4430 2024-01-08 04:14:36.000000 fudstop-2.4.8/fudstop/apis/discord_/__init__.py
+-rw-rw-rw-   0        0        0    12863 2024-02-23 01:28:51.000000 fudstop-2.4.8/fudstop/apis/discord_/discord_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/discord_/models/
+-rw-rw-rw-   0        0        0        0 2024-01-18 14:52:13.000000 fudstop-2.4.8/fudstop/apis/discord_/models/__init__.py
+-rw-rw-rw-   0        0        0     5431 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/discord_/models/application_commands.py
+-rw-rw-rw-   0        0        0     2767 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/discord_/models/search.py
+-rw-rw-rw-   0        0        0     1101 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/discord_/models/webhooks.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/earnings_whisper/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/earnings_whisper/__init__.py
+-rw-rw-rw-   0        0        0    12823 2024-03-25 21:47:38.000000 fudstop-2.4.8/fudstop/apis/earnings_whisper/ew_models.py
+-rw-rw-rw-   0        0        0     4016 2024-03-25 21:44:18.000000 fudstop-2.4.8/fudstop/apis/earnings_whisper/ew_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/fed_print/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/fed_print/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/fed_print/fed_print_sync.py
+-rw-rw-rw-   0        0        0     5322 2024-02-24 20:29:40.000000 fudstop-2.4.8/fudstop/apis/fed_print/fedprint_models.py
+-rw-rw-rw-   0        0        0     3354 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/fed_print/fedprint_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/federal_register/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/federal_register/__init__.py
+-rw-rw-rw-   0        0        0     3075 2024-02-25 17:21:39.000000 fudstop-2.4.8/fudstop/apis/federal_register/fed_register_sdk.py
+-rw-rw-rw-   0        0        0     2924 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/federal_register/fed_register_sync.py
+-rw-rw-rw-   0        0        0     2904 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/federal_register/register_models.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.526394 fudstop-2.4.8/fudstop/apis/gexbot/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/gexbot/__init__.py
+-rw-rw-rw-   0        0        0     4095 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/gexbot/gexbot.py
+-rw-rw-rw-   0        0        0     4139 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/gexbot/models.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/gpts/
+-rw-rw-rw-   0        0        0      231 2024-01-08 03:41:52.000000 fudstop-2.4.8/fudstop/apis/gpts/DiscoAI.py
+-rw-rw-rw-   0        0        0        2 2024-01-08 03:38:45.000000 fudstop-2.4.8/fudstop/apis/gpts/__init__.py
+-rw-rw-rw-   0        0        0    35379 2024-03-27 01:57:02.000000 fudstop-2.4.8/fudstop/apis/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/master/
+-rw-rw-rw-   0        0        0        0 2024-02-25 05:43:46.000000 fudstop-2.4.8/fudstop/apis/master/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-02-25 09:02:57.000000 fudstop-2.4.8/fudstop/apis/master/master_helpers.py
+-rw-rw-rw-   0        0        0    29960 2024-02-25 19:23:31.000000 fudstop-2.4.8/fudstop/apis/master/master_sdk.py
+-rw-rw-rw-   0        0        0    34633 2024-02-25 09:11:27.000000 fudstop-2.4.8/fudstop/apis/master/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/misc/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/misc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/misc/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/misc/models/__init__.py
+-rw-rw-rw-   0        0        0      249 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/misc/models/unsplash_models.py
+-rw-rw-rw-   0        0        0     2204 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/misc/models/weather_models.py
+-rw-rw-rw-   0        0        0      869 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/misc/unsplash.py
+-rw-rw-rw-   0        0        0     1790 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/misc/weather.py
+-rw-rw-rw-   0        0        0      294 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/misc/weather_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/nasdaq/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4200 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/nasdaq/nasdaq_lists.py
+-rw-rw-rw-   0        0        0    12177 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/nasdaq/nasdaq_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/newyork_fed/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/newyork_fed/__init__.py
+-rw-rw-rw-   0        0        0    14970 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/newyork_fed/models.py
+-rw-rw-rw-   0        0        0    22750 2024-03-27 00:32:52.000000 fudstop-2.4.8/fudstop/apis/newyork_fed/newyork_fed_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/occ/
+-rw-rw-rw-   0        0        0        0 2024-01-12 03:42:31.000000 fudstop-2.4.8/fudstop/apis/occ/__init__.py
+-rw-rw-rw-   0        0        0    30622 2024-03-27 02:16:15.000000 fudstop-2.4.8/fudstop/apis/occ/occ_models.py
+-rw-rw-rw-   0        0        0    14100 2024-03-27 02:05:52.000000 fudstop-2.4.8/fudstop/apis/occ/occ_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/ofr/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/ofr/__init__.py
+-rw-rw-rw-   0        0        0    37577 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/ofr/ofr_list_sets.py
+-rw-rw-rw-   0        0        0     5462 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/ofr/ofr_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.542018 fudstop-2.4.8/fudstop/apis/oic/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/oic/__init__.py
+-rw-rw-rw-   0        0        0    16116 2024-01-07 16:09:24.000000 fudstop-2.4.8/fudstop/apis/oic/async_oic_sdk.py
+-rw-rw-rw-   0        0        0    11292 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/oic/oic_models.py
+-rw-rw-rw-   0        0        0     4938 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/oic/oic_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.557643 fudstop-2.4.8/fudstop/apis/polygonio/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/__init__.py
+-rw-rw-rw-   0        0        0    30140 2024-04-13 19:57:12.000000 fudstop-2.4.8/fudstop/apis/polygonio/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0     2368 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/db_polygon.py
+-rw-rw-rw-   0        0        0    47011 2024-01-10 15:38:01.000000 fudstop-2.4.8/fudstop/apis/polygonio/mapping.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.573268 fudstop-2.4.8/fudstop/apis/polygonio/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/__init__.py
+-rw-rw-rw-   0        0        0     1330 2024-04-13 19:03:08.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/aggregates.py
+-rw-rw-rw-   0        0        0     1319 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/company_info.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.573268 fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/__init__.py
+-rw-rw-rw-   0        0        0     5734 2024-01-12 15:43:51.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/option_snapshot.py
+-rw-rw-rw-   0        0        0     7043 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/universal_option.py
+-rw-rw-rw-   0        0        0    57290 2024-03-07 18:09:56.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/universal_snapshot.py
+-rw-rw-rw-   0        0        0     6954 2024-01-10 06:10:49.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/technicals.py
+-rw-rw-rw-   0        0        0     2271 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/ticker_news.py
+-rw-rw-rw-   0        0        0     3801 2024-01-07 01:51:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/ticker_snapshot.py
+-rw-rw-rw-   0        0        0     5787 2024-01-21 19:53:33.000000 fudstop-2.4.8/fudstop/apis/polygonio/models/trades.py
+-rw-rw-rw-   0        0        0    13028 2024-02-18 06:32:56.000000 fudstop-2.4.8/fudstop/apis/polygonio/polygon_database.py
+-rw-rw-rw-   0        0        0    41160 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/polygon_helpers.py
+-rw-rw-rw-   0        0        0    68480 2024-03-07 21:00:57.000000 fudstop-2.4.8/fudstop/apis/polygonio/polygon_options.py
+-rw-rw-rw-   0        0        0     3692 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/polygon_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.573268 fudstop-2.4.8/fudstop/apis/polygonio/scripts/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2267 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/polygonio/scripts/daily_aggregates.py
+-rw-rw-rw-   0        0        0     1716 2024-02-04 09:29:32.000000 fudstop-2.4.8/fudstop/apis/polygonio/scripts/rsi.py
+-rw-rw-rw-   0        0        0     9164 2024-03-01 01:05:43.000000 fudstop-2.4.8/fudstop/apis/polygonio/technicals.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.573268 fudstop-2.4.8/fudstop/apis/rss/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/rss/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/rss/rss_helpers.py
+-rw-rw-rw-   0        0        0     1497 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/rss/rss_models.py
+-rw-rw-rw-   0        0        0    10360 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/apis/rss/rss_sdk.py
+-rw-rw-rw-   0        0        0    10203 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/apis/rss/snyc_rss.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.573268 fudstop-2.4.8/fudstop/apis/sec/
+-rw-rw-rw-   0        0        0        0 2024-02-29 20:06:34.000000 fudstop-2.4.8/fudstop/apis/sec/__init__.py
+-rw-rw-rw-   0        0        0     8441 2024-02-29 22:33:02.000000 fudstop-2.4.8/fudstop/apis/sec/sec_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.573268 fudstop-2.4.8/fudstop/apis/stocksera_/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.588892 fudstop-2.4.8/fudstop/apis/stocksera_/models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/borrowed_shares.py
+-rw-rw-rw-   0        0        0      827 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/daily_treasury.py
+-rw-rw-rw-   0        0        0      747 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/ftds.py
+-rw-rw-rw-   0        0        0      871 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/highest_shorted.py
+-rw-rw-rw-   0        0        0      813 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/inflation.py
+-rw-rw-rw-   0        0        0     1062 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/insider_trades.py
+-rw-rw-rw-   0        0        0      667 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/jim_cramer.py
+-rw-rw-rw-   0        0        0      850 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/jobless_claims.py
+-rw-rw-rw-   0        0        0     1043 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/low_float.py
+-rw-rw-rw-   0        0        0      660 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/market_news.py
+-rw-rw-rw-   0        0        0    21824 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/models.py
+-rw-rw-rw-   0        0        0      676 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/news_sentiment.py
+-rw-rw-rw-   0        0        0      693 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/retail_sales.py
+-rw-rw-rw-   0        0        0      708 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/reverse_repo.py
+-rw-rw-rw-   0        0        0      777 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/sec_filings.py
+-rw-rw-rw-   0        0        0      789 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/models/short_volume.py
+-rw-rw-rw-   0        0        0    19676 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/stocksera_/stocksera_.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.588892 fudstop-2.4.8/fudstop/apis/treasury/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/treasury/__init__.py
+-rw-rw-rw-   0        0        0    10964 2024-01-20 19:15:58.000000 fudstop-2.4.8/fudstop/apis/treasury/treasury_models.py
+-rw-rw-rw-   0        0        0    10281 2024-01-20 19:16:09.000000 fudstop-2.4.8/fudstop/apis/treasury/treasury_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.588892 fudstop-2.4.8/fudstop/apis/webull/
+-rw-rw-rw-   0        0        0     4945 2024-01-15 22:06:39.000000 fudstop-2.4.8/fudstop/apis/webull/__init__.py
+-rw-rw-rw-   0        0        0    12127 2024-01-23 03:47:19.000000 fudstop-2.4.8/fudstop/apis/webull/database_manager.py
+-rw-rw-rw-   0        0        0     2732 2024-01-11 18:10:25.000000 fudstop-2.4.8/fudstop/apis/webull/get_volume_analysis.py
+-rw-rw-rw-   0        0        0    10628 2024-01-11 18:10:17.000000 fudstop-2.4.8/fudstop/apis/webull/modal.py
+-rw-rw-rw-   0        0        0     5320 2024-01-10 21:10:43.000000 fudstop-2.4.8/fudstop/apis/webull/opt_modal.py
+-rw-rw-rw-   0        0        0     9390 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/options.py
+-rw-rw-rw-   0        0        0     3357 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/screener_models.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.604518 fudstop-2.4.8/fudstop/apis/webull/trade_models/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-02-18 21:14:42.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/analyst_ratings.py
+-rw-rw-rw-   0        0        0    12121 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/capital_flow.py
+-rw-rw-rw-   0        0        0     2147 2024-02-24 19:57:32.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/company_brief.py
+-rw-rw-rw-   0        0        0     2235 2024-01-23 05:04:58.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/cost_distribution.py
+-rw-rw-rw-   0        0        0     1053 2024-02-18 19:14:15.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/etf_holdings.py
+-rw-rw-rw-   0        0        0     1727 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/events.py
+-rw-rw-rw-   0        0        0    19884 2024-02-18 19:14:03.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/financials.py
+-rw-rw-rw-   0        0        0     3780 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/forecast_evaluator.py
+-rw-rw-rw-   0        0        0     3500 2024-02-18 18:48:35.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1335 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/news.py
+-rw-rw-rw-   0        0        0     1195 2024-03-01 01:13:55.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/price_streamer.py
+-rw-rw-rw-   0        0        0      601 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/short_interest.py
+-rw-rw-rw-   0        0        0    11042 2024-03-07 17:43:34.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/ticker_query.py
+-rw-rw-rw-   0        0        0     1314 2024-01-13 16:23:06.000000 fudstop-2.4.8/fudstop/apis/webull/trade_models/volume_analysis.py
+-rw-rw-rw-   0        0        0    13181 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/webull/webull_helpers.py
+-rw-rw-rw-   0        0        0    12274 2024-02-25 06:46:04.000000 fudstop-2.4.8/fudstop/apis/webull/webull_markets.py
+-rw-rw-rw-   0        0        0    35666 2024-01-21 19:47:41.000000 fudstop-2.4.8/fudstop/apis/webull/webull_options.py
+-rw-rw-rw-   0        0        0     9106 2024-01-18 22:00:22.000000 fudstop-2.4.8/fudstop/apis/webull/webull_parsing.py
+-rw-rw-rw-   0        0        0     7131 2024-02-26 02:07:00.000000 fudstop-2.4.8/fudstop/apis/webull/webull_screener.py
+-rw-rw-rw-   0        0        0    26318 2024-03-27 00:20:49.000000 fudstop-2.4.8/fudstop/apis/webull/webull_trading.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.604518 fudstop-2.4.8/fudstop/apis/whale/
+-rw-rw-rw-   0        0        0        0 2024-03-27 06:54:53.000000 fudstop-2.4.8/fudstop/apis/whale/__init__.py
+-rw-rw-rw-   0        0        0    42102 2024-03-27 21:07:42.000000 fudstop-2.4.8/fudstop/apis/whale/whale_models.py
+-rw-rw-rw-   0        0        0     7065 2024-03-27 21:07:56.000000 fudstop-2.4.8/fudstop/apis/whale/whale_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.604518 fudstop-2.4.8/fudstop/apis/y_finance/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/apis/y_finance/__init__.py
+-rw-rw-rw-   0        0        0     9028 2024-02-18 15:18:29.000000 fudstop-2.4.8/fudstop/apis/y_finance/yf_sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.604518 fudstop-2.4.8/fudstop/database_/
+-rw-rw-rw-   0        0        0    66479 2024-02-18 06:41:46.000000 fudstop-2.4.8/fudstop/database_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.604518 fudstop-2.4.8/fudstop/discord_/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/discord_/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-01-11 18:10:55.000000 fudstop-2.4.8/fudstop/discord_/autocomp.py
+-rw-rw-rw-   0        0        0    63334 2024-01-15 01:59:11.000000 fudstop-2.4.8/fudstop/discord_/bot.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.604518 fudstop-2.4.8/fudstop/discord_/bot_menus/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/discord_/bot_menus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.604518 fudstop-2.4.8/fudstop/discord_/bot_menus/modals/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/discord_/bot_menus/modals/__init__.py
+-rw-rw-rw-   0        0        0     2226 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/discord_/bot_menus/modals/dalle_modal.py
+-rw-rw-rw-   0        0        0    13054 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/discord_/bot_menus/modals/options_modal.py
+-rw-rw-rw-   0        0        0     3597 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/discord_/bot_menus/pagination.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.620143 fudstop-2.4.8/fudstop/discord_/cogs/
+-rw-rw-rw-   0        0        0     4305 2024-01-07 18:05:54.000000 fudstop-2.4.8/fudstop/discord_/cogs/__init__.py
+-rw-rw-rw-   0        0        0    20340 2024-01-06 18:32:34.000000 fudstop-2.4.8/fudstop/discord_/cogs/accounting.py
+-rw-rw-rw-   0        0        0    11559 2024-01-06 18:29:35.000000 fudstop-2.4.8/fudstop/discord_/cogs/assistant.py
+-rw-rw-rw-   0        0        0    11795 2024-02-06 17:49:34.000000 fudstop-2.4.8/fudstop/discord_/cogs/database.py
+-rw-rw-rw-   0        0        0    12937 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/discord_/cogs/earnings.py
+-rw-rw-rw-   0        0        0     2104 2024-01-06 18:30:08.000000 fudstop-2.4.8/fudstop/discord_/cogs/fed_print.py
+-rw-rw-rw-   0        0        0     4463 2024-01-11 18:16:25.000000 fudstop-2.4.8/fudstop/discord_/cogs/filter.py
+-rw-rw-rw-   0        0        0    34896 2024-01-11 18:17:51.000000 fudstop-2.4.8/fudstop/discord_/cogs/fiscal_service.py
+-rw-rw-rw-   0        0        0     4482 2024-01-07 16:10:05.000000 fudstop-2.4.8/fudstop/discord_/cogs/gex.py
+-rw-rw-rw-   0        0        0     6390 2024-02-07 19:46:50.000000 fudstop-2.4.8/fudstop/discord_/cogs/gpt.py
+-rw-rw-rw-   0        0        0     3906 2024-02-17 21:04:28.000000 fudstop-2.4.8/fudstop/discord_/cogs/ibrs.py
+-rw-rw-rw-   0        0        0     2313 2024-01-06 18:31:02.000000 fudstop-2.4.8/fudstop/discord_/cogs/main_view.py
+-rw-rw-rw-   0        0        0    29489 2024-04-06 03:42:15.000000 fudstop-2.4.8/fudstop/discord_/cogs/options.py
+-rw-rw-rw-   0        0        0     3827 2024-01-11 18:16:07.000000 fudstop-2.4.8/fudstop/discord_/cogs/plays.py
+-rw-rw-rw-   0        0        0     3428 2024-01-06 18:35:15.000000 fudstop-2.4.8/fudstop/discord_/cogs/register.py
+-rw-rw-rw-   0        0        0     3800 2024-01-06 18:31:37.000000 fudstop-2.4.8/fudstop/discord_/cogs/spx.py
+-rw-rw-rw-   0        0        0     9302 2024-01-11 18:15:53.000000 fudstop-2.4.8/fudstop/discord_/cogs/strategy.py
+-rw-rw-rw-   0        0        0     2776 2024-01-06 18:31:52.000000 fudstop-2.4.8/fudstop/discord_/cogs/ta.py
+-rw-rw-rw-   0        0        0     3071 2024-01-06 18:32:00.000000 fudstop-2.4.8/fudstop/discord_/cogs/weather.py
+-rw-rw-rw-   0        0        0     1346 2024-01-06 18:32:07.000000 fudstop-2.4.8/fudstop/discord_/cogs/webull.py
+-rw-rw-rw-   0        0        0    11097 2024-01-06 18:32:21.000000 fudstop-2.4.8/fudstop/discord_/cogs/yfin.py
+-rw-rw-rw-   0        0        0     1843 2024-01-14 21:57:53.000000 fudstop-2.4.8/fudstop/discord_/database_getter.py
+-rw-rw-rw-   0        0        0     6337 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/discord_/discord_rsi.py
+-rw-rw-rw-   0        0        0     3697 2024-01-06 18:23:33.000000 fudstop-2.4.8/fudstop/discord_/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.635769 fudstop-2.4.8/fudstop/examples/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/__init__.py
+-rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/ecfr_test.py
+-rw-rw-rw-   0        0        0      178 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/fed_print_test.py
+-rw-rw-rw-   0        0        0      237 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/fed_reg_test.py
+-rw-rw-rw-   0        0        0      258 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/nasdaq_test.py
+-rw-rw-rw-   0        0        0      181 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/newyork_fed_test.py
+-rw-rw-rw-   0        0        0     3793 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/ofr_test.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.635769 fudstop-2.4.8/fudstop/examples/polygonio/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/polygonio/__init__.py
+-rw-rw-rw-   0        0        0     1392 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/examples/polygonio/aggregates_second.py
+-rw-rw-rw-   0        0        0      709 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/examples/polygonio/company_info.py
+-rw-rw-rw-   0        0        0     2345 2024-01-07 23:40:02.000000 fudstop-2.4.8/fudstop/examples/polygonio/get_all_options.py
+-rw-rw-rw-   0        0        0      379 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/examples/polygonio/get_all_tickers.py
+-rw-rw-rw-   0        0        0      611 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/polygonio/get_near_the_money.py
+-rw-rw-rw-   0        0        0     2307 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/polygonio/get_option_aggs.py
+-rw-rw-rw-   0        0        0     1190 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/polygonio/get_option_rsi.py
+-rw-rw-rw-   0        0        0     3751 2024-01-06 00:03:40.000000 fudstop-2.4.8/fudstop/examples/polygonio/get_option_trades.py
+-rw-rw-rw-   0        0        0     2409 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/polygonio/get_ticker_aggs.py
+-rw-rw-rw-   0        0        0      683 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/examples/polygonio/market_news.py
+-rw-rw-rw-   0        0        0     1305 2024-01-11 18:07:47.000000 fudstop-2.4.8/fudstop/examples/polygonio/polygon_test.py
+-rw-rw-rw-   0        0        0     1134 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/scripty.py
+-rw-rw-rw-   0        0        0     1871 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/stocksera_test.py
+-rw-rw-rw-   0        0        0      776 2024-01-06 17:35:55.000000 fudstop-2.4.8/fudstop/examples/test.py
+-rw-rw-rw-   0        0        0     2721 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/test_gex.py
+-rw-rw-rw-   0        0        0      284 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/test_insert.py
+-rw-rw-rw-   0        0        0     2255 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/test_openai.py
+-rw-rw-rw-   0        0        0      698 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/test_opts.py
+-rw-rw-rw-   0        0        0      633 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/test_screener.py
+-rw-rw-rw-   0        0        0     4324 2024-01-11 18:10:12.000000 fudstop-2.4.8/fudstop/examples/test_sec.py
+-rw-rw-rw-   0        0        0     1758 2024-01-11 18:11:03.000000 fudstop-2.4.8/fudstop/examples/test_webull.py
+-rw-rw-rw-   0        0        0        0 2024-01-08 17:00:41.000000 fudstop-2.4.8/fudstop/examples/tests_discord.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.635769 fudstop-2.4.8/fudstop/examples/webull/
+-rw-rw-rw-   0        0        0        0 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/webull/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/webull/markets_example.py
+-rw-rw-rw-   0        0        0     2439 2024-01-05 23:27:36.000000 fudstop-2.4.8/fudstop/examples/webull/trade_example.py
+-rw-rw-rw-   0        0        0     7753 2024-01-11 18:14:32.000000 fudstop-2.4.8/fudstop/options_filter.py
+-rw-rw-rw-   0        0        0    21800 2024-01-11 18:09:07.000000 fudstop-2.4.8/fudstop/plots.py
+-rw-rw-rw-   0        0        0    15233 2024-01-11 18:14:18.000000 fudstop-2.4.8/fudstop/schema.py
+-rw-rw-rw-   0        0        0      490 2024-02-04 05:36:05.000000 fudstop-2.4.8/fudstop/wet.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:57:29.479518 fudstop-2.4.8/fudstop.egg-info/
+-rw-rw-rw-   0        0        0     7618 2024-04-13 19:57:29.000000 fudstop-2.4.8/fudstop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10588 2024-04-13 19:57:29.000000 fudstop-2.4.8/fudstop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 19:57:29.000000 fudstop-2.4.8/fudstop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4028 2024-04-13 19:57:29.000000 fudstop-2.4.8/fudstop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 19:57:29.000000 fudstop-2.4.8/fudstop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 19:57:29.651394 fudstop-2.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      363 2024-04-13 19:57:24.000000 fudstop-2.4.8/setup.py
```

### Comparing `fudstop-2.4.7/PKG-INFO` & `fudstop-2.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudstop
-Version: 2.4.7
+Version: 2.4.8
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `fudstop-2.4.7/README.md` & `fudstop-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/app/__init__.py` & `fudstop-2.4.8/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/app/fetcher.py` & `fudstop-2.4.8/app/fetcher.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/app/fudstop_info.py` & `fudstop-2.4.8/app/fudstop_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/app/helpers.py` & `fudstop-2.4.8/app/helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/__init__.py` & `fudstop-2.4.8/fudstop/_markets/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/analyzers.py` & `fudstop-2.4.8/fudstop/_markets/analyzers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/embeddings.py` & `fudstop-2.4.8/fudstop/_markets/embeddings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/finished/db_manager.py` & `fudstop-2.4.8/fudstop/_markets/finished/db_manager.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/finished/economic_data.py` & `fudstop-2.4.8/fudstop/_markets/finished/economic_data.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/finished/master_class.py` & `fudstop-2.4.8/fudstop/_markets/finished/master_class.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/finished/td9_states.py` & `fudstop-2.4.8/fudstop/_markets/finished/td9_states.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/list_sets/dicts.py` & `fudstop-2.4.8/fudstop/_markets/list_sets/dicts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/list_sets/saved_tickers.py` & `fudstop-2.4.8/fudstop/_markets/list_sets/saved_tickers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/list_sets/ticker_lists.py` & `fudstop-2.4.8/fudstop/_markets/list_sets/ticker_lists.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/cfg.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/cfg.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/crypto.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/crypto.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/database_.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/database_.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/forex.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/forex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/indices.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/indices.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/list_sets.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/list_sets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/options.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/market_handlers/stocks.py` & `fudstop-2.4.8/fudstop/_markets/market_handlers/stocks.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/monitor.py` & `fudstop-2.4.8/fudstop/_markets/monitor.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/multimarkets.py` & `fudstop-2.4.8/fudstop/_markets/multimarkets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/plotting/__init__.py` & `fudstop-2.4.8/fudstop/_markets/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/reference_markets/conditional_scans.py` & `fudstop-2.4.8/fudstop/_markets/reference_markets/conditional_scans.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/reference_markets/reference_market.py` & `fudstop-2.4.8/fudstop/_markets/reference_markets/reference_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/all_polygon_options.py` & `fudstop-2.4.8/fudstop/_markets/scripts/all_polygon_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/all_webull_options.py` & `fudstop-2.4.8/fudstop/_markets/scripts/all_webull_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/generation.py` & `fudstop-2.4.8/fudstop/_markets/scripts/generation.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/million_dollar_trades.py` & `fudstop-2.4.8/fudstop/_markets/scripts/million_dollar_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/option_scripts.py` & `fudstop-2.4.8/fudstop/_markets/scripts/option_scripts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/options_market.py` & `fudstop-2.4.8/fudstop/_markets/scripts/options_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/options_volume_analysis.py` & `fudstop-2.4.8/fudstop/_markets/scripts/options_volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/rsi_2_4_8.py` & `fudstop-2.4.8/fudstop/_markets/scripts/rsi_2_4_8.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/rsi_screener.py` & `fudstop-2.4.8/fudstop/_markets/scripts/rsi_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/ssr_scanner.py` & `fudstop-2.4.8/fudstop/_markets/scripts/ssr_scanner.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/stock_market.py` & `fudstop-2.4.8/fudstop/_markets/scripts/stock_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/td9_states.py` & `fudstop-2.4.8/fudstop/_markets/scripts/td9_states.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/scripts/universal_snapshot.py` & `fudstop-2.4.8/fudstop/_markets/scripts/universal_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/stock_market.py` & `fudstop-2.4.8/fudstop/_markets/stock_market.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/_markets/webhook_dicts.py` & `fudstop-2.4.8/fudstop/_markets/webhook_dicts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/all_helpers.py` & `fudstop-2.4.8/fudstop/all_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/_asyncpg/asyncpg_sdk.py` & `fudstop-2.4.8/fudstop/apis/_asyncpg/asyncpg_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/_openai/agent.py` & `fudstop-2.4.8/fudstop/apis/_openai/agent.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/_openai/openai_sdk.py` & `fudstop-2.4.8/fudstop/apis/_openai/openai_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/_openai/tools_shcema.py` & `fudstop-2.4.8/fudstop/apis/_openai/tools_shcema.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/_selenium/selenium_sdk.py` & `fudstop-2.4.8/fudstop/apis/_selenium/selenium_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/cfr/cfr_2.0.py` & `fudstop-2.4.8/fudstop/apis/cfr/cfr_2.0.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/cfr/cfr_sdk.py` & `fudstop-2.4.8/fudstop/apis/cfr/cfr_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/cfr/title_12.py` & `fudstop-2.4.8/fudstop/apis/cfr/title_12.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/datalink/datalink_sdk.py` & `fudstop-2.4.8/fudstop/apis/datalink/datalink_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/datalink/models.py` & `fudstop-2.4.8/fudstop/apis/datalink/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/discord_/__init__.py` & `fudstop-2.4.8/fudstop/apis/discord_/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/discord_/discord_sdk.py` & `fudstop-2.4.8/fudstop/apis/discord_/discord_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/discord_/models/application_commands.py` & `fudstop-2.4.8/fudstop/apis/discord_/models/application_commands.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/discord_/models/search.py` & `fudstop-2.4.8/fudstop/apis/discord_/models/search.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/discord_/models/webhooks.py` & `fudstop-2.4.8/fudstop/apis/discord_/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/earnings_whisper/ew_models.py` & `fudstop-2.4.8/fudstop/apis/earnings_whisper/ew_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/earnings_whisper/ew_sdk.py` & `fudstop-2.4.8/fudstop/apis/earnings_whisper/ew_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/fed_print/fed_print_sync.py` & `fudstop-2.4.8/fudstop/apis/fed_print/fed_print_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/fed_print/fedprint_models.py` & `fudstop-2.4.8/fudstop/apis/fed_print/fedprint_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/fed_print/fedprint_sdk.py` & `fudstop-2.4.8/fudstop/apis/fed_print/fedprint_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/federal_register/fed_register_sdk.py` & `fudstop-2.4.8/fudstop/apis/federal_register/fed_register_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/federal_register/fed_register_sync.py` & `fudstop-2.4.8/fudstop/apis/federal_register/fed_register_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/federal_register/register_models.py` & `fudstop-2.4.8/fudstop/apis/federal_register/register_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/gexbot/gexbot.py` & `fudstop-2.4.8/fudstop/apis/gexbot/gexbot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/gexbot/models.py` & `fudstop-2.4.8/fudstop/apis/gexbot/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/helpers.py` & `fudstop-2.4.8/fudstop/apis/helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/master/master_helpers.py` & `fudstop-2.4.8/fudstop/apis/master/master_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/master/master_sdk.py` & `fudstop-2.4.8/fudstop/apis/master/master_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/master/tools.py` & `fudstop-2.4.8/fudstop/apis/master/tools.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/misc/models/weather_models.py` & `fudstop-2.4.8/fudstop/apis/misc/models/weather_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/misc/unsplash.py` & `fudstop-2.4.8/fudstop/apis/misc/unsplash.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/misc/weather.py` & `fudstop-2.4.8/fudstop/apis/misc/weather.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/nasdaq/nasdaq_lists.py` & `fudstop-2.4.8/fudstop/apis/nasdaq/nasdaq_lists.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/nasdaq/nasdaq_sdk.py` & `fudstop-2.4.8/fudstop/apis/nasdaq/nasdaq_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/newyork_fed/models.py` & `fudstop-2.4.8/fudstop/apis/newyork_fed/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/newyork_fed/newyork_fed_sdk.py` & `fudstop-2.4.8/fudstop/apis/newyork_fed/newyork_fed_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/occ/occ_models.py` & `fudstop-2.4.8/fudstop/apis/occ/occ_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/occ/occ_sdk.py` & `fudstop-2.4.8/fudstop/apis/occ/occ_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/ofr/ofr_list_sets.py` & `fudstop-2.4.8/fudstop/apis/ofr/ofr_list_sets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/ofr/ofr_sdk.py` & `fudstop-2.4.8/fudstop/apis/ofr/ofr_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/oic/async_oic_sdk.py` & `fudstop-2.4.8/fudstop/apis/oic/async_oic_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/oic/oic_models.py` & `fudstop-2.4.8/fudstop/apis/oic/oic_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/oic/oic_sdk.py` & `fudstop-2.4.8/fudstop/apis/oic/oic_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/async_polygon_sdk.py` & `fudstop-2.4.8/fudstop/apis/polygonio/async_polygon_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
             {'Close Price': aggs.close[i], 'Timestamp': aggs.timestamp[i], 'Dollar Cost': cost}
             for i, cost in enumerate(aggs.dollar_cost) 
             if cost > 10000000
         ]
 
         # Create DataFrame from the list of dictionaries
         df_dollar_cost_above_10m = pd.DataFrame(dollar_cost_above_10m_details)
-        df_dollar_cost_above_10m['Timestamp'] = pd.to_datetime(df_dollar_cost_above_10m['Timestamp']).dt.strftime('%H:%M:%S')
+
         # Print the DataFrame to see the result
         df = format_large_numbers_in_dataframe(df_dollar_cost_above_10m)
 
         return df
```

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/db_polygon.py` & `fudstop-2.4.8/fudstop/apis/polygonio/db_polygon.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/mapping.py` & `fudstop-2.4.8/fudstop/apis/polygonio/mapping.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/aggregates.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/aggregates.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/company_info.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/company_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/option_snapshot.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/universal_option.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/universal_option.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/option_models/universal_snapshot.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/option_models/universal_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/technicals.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/technicals.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/ticker_news.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/ticker_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/ticker_snapshot.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/ticker_snapshot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/models/trades.py` & `fudstop-2.4.8/fudstop/apis/polygonio/models/trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/polygon_database.py` & `fudstop-2.4.8/fudstop/apis/polygonio/polygon_database.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/polygon_helpers.py` & `fudstop-2.4.8/fudstop/apis/polygonio/polygon_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/polygon_options.py` & `fudstop-2.4.8/fudstop/apis/polygonio/polygon_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/polygon_sync.py` & `fudstop-2.4.8/fudstop/apis/polygonio/polygon_sync.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/scripts/daily_aggregates.py` & `fudstop-2.4.8/fudstop/apis/polygonio/scripts/daily_aggregates.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/scripts/rsi.py` & `fudstop-2.4.8/fudstop/apis/polygonio/scripts/rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/polygonio/technicals.py` & `fudstop-2.4.8/fudstop/apis/polygonio/technicals.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/rss/rss_helpers.py` & `fudstop-2.4.8/fudstop/apis/rss/rss_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/rss/rss_models.py` & `fudstop-2.4.8/fudstop/apis/rss/rss_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/rss/rss_sdk.py` & `fudstop-2.4.8/fudstop/apis/rss/rss_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/rss/snyc_rss.py` & `fudstop-2.4.8/fudstop/apis/rss/snyc_rss.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/sec/sec_sdk.py` & `fudstop-2.4.8/fudstop/apis/sec/sec_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/daily_treasury.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/daily_treasury.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/ftds.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/ftds.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/highest_shorted.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/highest_shorted.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/inflation.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/inflation.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/insider_trades.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/insider_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/jim_cramer.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/jim_cramer.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/jobless_claims.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/jobless_claims.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/low_float.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/low_float.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/market_news.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/market_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/models.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/news_sentiment.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/news_sentiment.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/retail_sales.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/retail_sales.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/reverse_repo.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/reverse_repo.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/sec_filings.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/sec_filings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/models/short_volume.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/stocksera_/stocksera_.py` & `fudstop-2.4.8/fudstop/apis/stocksera_/stocksera_.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/treasury/treasury_models.py` & `fudstop-2.4.8/fudstop/apis/treasury/treasury_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/treasury/treasury_sdk.py` & `fudstop-2.4.8/fudstop/apis/treasury/treasury_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/__init__.py` & `fudstop-2.4.8/fudstop/apis/webull/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/database_manager.py` & `fudstop-2.4.8/fudstop/apis/webull/database_manager.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/get_volume_analysis.py` & `fudstop-2.4.8/fudstop/apis/webull/get_volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/modal.py` & `fudstop-2.4.8/fudstop/apis/webull/modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/opt_modal.py` & `fudstop-2.4.8/fudstop/apis/webull/opt_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/options.py` & `fudstop-2.4.8/fudstop/apis/webull/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/screener_models.py` & `fudstop-2.4.8/fudstop/apis/webull/screener_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/analyst_ratings.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/capital_flow.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/capital_flow.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/company_brief.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/company_brief.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/cost_distribution.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/etf_holdings.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/events.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/events.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/financials.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/financials.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/forecast_evaluator.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/forecast_evaluator.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/institutional_holdings.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/news.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/price_streamer.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/price_streamer.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/short_interest.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/short_interest.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/ticker_query.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/ticker_query.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/trade_models/volume_analysis.py` & `fudstop-2.4.8/fudstop/apis/webull/trade_models/volume_analysis.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/webull_helpers.py` & `fudstop-2.4.8/fudstop/apis/webull/webull_helpers.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/webull_markets.py` & `fudstop-2.4.8/fudstop/apis/webull/webull_markets.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/webull_options.py` & `fudstop-2.4.8/fudstop/apis/webull/webull_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/webull_parsing.py` & `fudstop-2.4.8/fudstop/apis/webull/webull_parsing.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/webull_screener.py` & `fudstop-2.4.8/fudstop/apis/webull/webull_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/webull/webull_trading.py` & `fudstop-2.4.8/fudstop/apis/webull/webull_trading.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/whale/whale_models.py` & `fudstop-2.4.8/fudstop/apis/whale/whale_models.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/whale/whale_sdk.py` & `fudstop-2.4.8/fudstop/apis/whale/whale_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/apis/y_finance/yf_sdk.py` & `fudstop-2.4.8/fudstop/apis/y_finance/yf_sdk.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/database_/__init__.py` & `fudstop-2.4.8/fudstop/database_/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/autocomp.py` & `fudstop-2.4.8/fudstop/discord_/autocomp.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/bot.py` & `fudstop-2.4.8/fudstop/discord_/bot.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/bot_menus/modals/dalle_modal.py` & `fudstop-2.4.8/fudstop/discord_/bot_menus/modals/dalle_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/bot_menus/modals/options_modal.py` & `fudstop-2.4.8/fudstop/discord_/bot_menus/modals/options_modal.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/bot_menus/pagination.py` & `fudstop-2.4.8/fudstop/discord_/bot_menus/pagination.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/__init__.py` & `fudstop-2.4.8/fudstop/discord_/cogs/__init__.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/accounting.py` & `fudstop-2.4.8/fudstop/discord_/cogs/accounting.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/assistant.py` & `fudstop-2.4.8/fudstop/discord_/cogs/assistant.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/database.py` & `fudstop-2.4.8/fudstop/discord_/cogs/database.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/earnings.py` & `fudstop-2.4.8/fudstop/discord_/cogs/earnings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/fed_print.py` & `fudstop-2.4.8/fudstop/discord_/cogs/fed_print.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/filter.py` & `fudstop-2.4.8/fudstop/discord_/cogs/filter.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/fiscal_service.py` & `fudstop-2.4.8/fudstop/discord_/cogs/fiscal_service.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/gex.py` & `fudstop-2.4.8/fudstop/discord_/cogs/gex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/gpt.py` & `fudstop-2.4.8/fudstop/discord_/cogs/gpt.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/ibrs.py` & `fudstop-2.4.8/fudstop/discord_/cogs/ibrs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/main_view.py` & `fudstop-2.4.8/fudstop/discord_/cogs/main_view.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/options.py` & `fudstop-2.4.8/fudstop/discord_/cogs/options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/plays.py` & `fudstop-2.4.8/fudstop/discord_/cogs/plays.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/register.py` & `fudstop-2.4.8/fudstop/discord_/cogs/register.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/spx.py` & `fudstop-2.4.8/fudstop/discord_/cogs/spx.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/strategy.py` & `fudstop-2.4.8/fudstop/discord_/cogs/strategy.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/ta.py` & `fudstop-2.4.8/fudstop/discord_/cogs/ta.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/weather.py` & `fudstop-2.4.8/fudstop/discord_/cogs/weather.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/webull.py` & `fudstop-2.4.8/fudstop/discord_/cogs/webull.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/cogs/yfin.py` & `fudstop-2.4.8/fudstop/discord_/cogs/yfin.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/database_getter.py` & `fudstop-2.4.8/fudstop/discord_/database_getter.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/discord_rsi.py` & `fudstop-2.4.8/fudstop/discord_/discord_rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/discord_/embeddings.py` & `fudstop-2.4.8/fudstop/discord_/embeddings.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/ecfr_test.py` & `fudstop-2.4.8/fudstop/examples/ecfr_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/ofr_test.py` & `fudstop-2.4.8/fudstop/examples/ofr_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/aggregates_second.py` & `fudstop-2.4.8/fudstop/examples/polygonio/aggregates_second.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/company_info.py` & `fudstop-2.4.8/fudstop/examples/polygonio/company_info.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/get_all_options.py` & `fudstop-2.4.8/fudstop/examples/polygonio/get_all_options.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/get_near_the_money.py` & `fudstop-2.4.8/fudstop/examples/polygonio/get_near_the_money.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/get_option_aggs.py` & `fudstop-2.4.8/fudstop/examples/polygonio/get_option_aggs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/get_option_rsi.py` & `fudstop-2.4.8/fudstop/examples/polygonio/get_option_rsi.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/get_option_trades.py` & `fudstop-2.4.8/fudstop/examples/polygonio/get_option_trades.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/get_ticker_aggs.py` & `fudstop-2.4.8/fudstop/examples/polygonio/get_ticker_aggs.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/market_news.py` & `fudstop-2.4.8/fudstop/examples/polygonio/market_news.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/polygonio/polygon_test.py` & `fudstop-2.4.8/fudstop/examples/polygonio/polygon_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/scripty.py` & `fudstop-2.4.8/fudstop/examples/scripty.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/stocksera_test.py` & `fudstop-2.4.8/fudstop/examples/stocksera_test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/test.py` & `fudstop-2.4.8/fudstop/examples/test.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/test_gex.py` & `fudstop-2.4.8/fudstop/examples/test_gex.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/test_openai.py` & `fudstop-2.4.8/fudstop/examples/test_openai.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/test_opts.py` & `fudstop-2.4.8/fudstop/examples/test_opts.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/test_screener.py` & `fudstop-2.4.8/fudstop/examples/test_screener.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/test_sec.py` & `fudstop-2.4.8/fudstop/examples/test_sec.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/test_webull.py` & `fudstop-2.4.8/fudstop/examples/test_webull.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/webull/markets_example.py` & `fudstop-2.4.8/fudstop/examples/webull/markets_example.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/examples/webull/trade_example.py` & `fudstop-2.4.8/fudstop/examples/webull/trade_example.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/options_filter.py` & `fudstop-2.4.8/fudstop/options_filter.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/plots.py` & `fudstop-2.4.8/fudstop/plots.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop/schema.py` & `fudstop-2.4.8/fudstop/schema.py`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop.egg-info/PKG-INFO` & `fudstop-2.4.8/fudstop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudstop
-Version: 2.4.7
+Version: 2.4.8
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
```

### Comparing `fudstop-2.4.7/fudstop.egg-info/SOURCES.txt` & `fudstop-2.4.8/fudstop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fudstop-2.4.7/fudstop.egg-info/requires.txt` & `fudstop-2.4.8/fudstop.egg-info/requires.txt`

 * *Files identical despite different names*


# Comparing `tmp/ofscraper-3.9.0.dev7.tar.gz` & `tmp/ofscraper-3.9.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.0.dev7.tar", max compression
+gzip compressed data, was "ofscraper-3.9.0.dev9.tar", max compression
```

## Comparing `ofscraper-3.9.0.dev7.tar` & `ofscraper-3.9.0.dev9.tar`

### file list

```diff
@@ -1,164 +1,179 @@
--rw-r--r--   0        0        0     1067 2024-04-02 16:59:06.785275 ofscraper-3.9.0.dev7/LICENSE
--rw-r--r--   0        0        0     4067 2024-04-02 16:59:06.785275 ofscraper-3.9.0.dev7/README.md
--rwxr-xr-x   0        0        0      283 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/__init__.py
--rw-r--r--   0        0        0     6372 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/like.py
--rw-r--r--   0        0        0     9943 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/process.py
--rw-r--r--   0        0        0    23104 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/scraper.py
--rw-r--r--   0        0        0    13937 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/archive.py
--rw-r--r--   0        0        0    21424 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/init.py
--rw-r--r--   0        0        0    13750 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/labels.py
--rw-r--r--   0        0        0     4724 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/me.py
--rw-r--r--   0        0        0    25187 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/messages.py
--rw-r--r--   0        0        0    17245 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8246 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     8913 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3069 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3035 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    14508 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0    11801 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    19969 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1413 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15247 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/media.py
--rw-r--r--   0        0        0     5892 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20730 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     4452 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/posts.py
--rw-r--r--   0        0        0      489 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/semaphoreDelayed.py
--rw-r--r--   0        0        0     8226 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    31963 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/table.py
--rw-r--r--   0        0        0    18318 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/check.py
--rw-r--r--   0        0        0     7479 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/manual.py
--rw-r--r--   0        0        0      430 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3915 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1581 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/config.py
--rw-r--r--   0        0        0      927 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/constants.py
--rw-r--r--   0        0        0       34 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/date.py
--rw-r--r--   0        0        0      184 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/files.py
--rw-r--r--   0        0        0     1231 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/logger.py
--rw-r--r--   0        0        0      775 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1876 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/prompts.py
--rw-r--r--   0        0        0      615 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/req.py
--rw-r--r--   0        0        0   265533 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      212 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/const/time.py
--rw-r--r--   0        0        0     3516 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    44884 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/db/operations.py
--rw-r--r--   0        0        0     8452 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/db/queries.py
--rw-r--r--   0        0        0    14959 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    15034 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     6188 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/common.py
--rw-r--r--   0        0        0     3122 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/globals.py
--rw-r--r--   0        0        0    12589 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/keyhelpers.py
--rw-r--r--   0        0        0     2910 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/log.py
--rw-r--r--   0        0        0      790 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/message.py
--rw-r--r--   0        0        0     5678 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/metadata.py
--rw-r--r--   0        0        0     2092 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/paths.py
--rw-r--r--   0        0        0      453 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/progress.py
--rw-r--r--   0        0        0     1161 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/sem.py
--rw-r--r--   0        0        0     1075 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/text.py
--rw-r--r--   0        0        0     2642 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/download.py
--rw-r--r--   0        0        0    16936 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9046 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    13470 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    14063 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     5481 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0    12337 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     2682 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     2532 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      586 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     6342 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1415 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1122 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3349 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     7043 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    13078 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7310 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6549 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8257 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4621 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27481 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1878 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0    15703 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4134 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7589 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10184 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1290 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1431 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2748 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3806 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1815 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0       12 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     4914 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0    27837 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      383 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      839 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      552 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      253 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2131 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2843 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1756 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6092 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1650 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2893 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1090 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      452 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    23180 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2110 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2111 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4708 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      429 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/console.py
--rw-r--r--   0        0        0      461 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1014 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     2679 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1716 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     8325 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1551 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      584 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      388 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4087 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/menu.py
--rw-r--r--   0        0        0     1732 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3105 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      279 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     5061 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1058 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1606 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0     5615 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4447 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/run.py
--rw-r--r--   0        0        0      255 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1595 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     3752 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3108 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2448 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2075 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2106 2024-04-02 16:59:36.681179 ofscraper-3.9.0.dev7/pyproject.toml
--rw-r--r--   0        0        0     6190 1970-01-01 00:00:00.000000 ofscraper-3.9.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-08 04:31:25.239239 ofscraper-3.9.0.dev9/LICENSE
+-rw-r--r--   0        0        0     4188 2024-04-08 04:31:25.239239 ofscraper-3.9.0.dev9/README.md
+-rwxr-xr-x   0        0        0      283 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/__init__.py
+-rw-r--r--   0        0        0     9230 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/like.py
+-rw-r--r--   0        0        0     9868 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/process.py
+-rw-r--r--   0        0        0    21931 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/scraper.py
+-rw-r--r--   0        0        0    15975 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/archive.py
+-rw-r--r--   0        0        0    19152 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/init.py
+-rw-r--r--   0        0        0    16927 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     4724 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/me.py
+-rw-r--r--   0        0        0    19945 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    17203 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9960 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     8914 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3069 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3036 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    14604 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0    11817 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    16816 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1413 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15247 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     5892 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20470 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5157 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0      489 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/semaphoreDelayed.py
+-rw-r--r--   0        0        0     8226 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    31982 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    21412 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     9739 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0      430 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3915 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1580 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/config.py
+-rw-r--r--   0        0        0      927 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       73 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/date.py
+-rw-r--r--   0        0        0      184 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1231 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/logger.py
+-rw-r--r--   0        0        0      775 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1876 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0      615 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/req.py
+-rw-r--r--   0        0        0   265533 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      212 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3516 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    11310 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      176 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8102 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    15102 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0     7983 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8318 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0     9448 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     5914 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7128 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4597 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    14966 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    15078 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     6173 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/common.py
+-rw-r--r--   0        0        0     2699 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/globals.py
+-rw-r--r--   0        0        0    12589 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/keyhelpers.py
+-rw-r--r--   0        0        0     3451 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/log.py
+-rw-r--r--   0        0        0      790 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/message.py
+-rw-r--r--   0        0        0     5875 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/metadata.py
+-rw-r--r--   0        0        0     2092 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/paths.py
+-rw-r--r--   0        0        0      453 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/progress.py
+-rw-r--r--   0        0        0     1161 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/sem.py
+-rw-r--r--   0        0        0     1075 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/text.py
+-rw-r--r--   0        0        0     3431 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/download.py
+-rw-r--r--   0        0        0    16936 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9047 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    13473 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    14084 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     5480 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0    12331 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     2682 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     2532 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      586 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     6342 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1415 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1122 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3436 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     7125 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    13078 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7310 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6596 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8258 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4622 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27530 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0    16008 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7589 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10184 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1290 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1486 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2748 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0       12 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     6289 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/common_args.py
+-rw-r--r--   0        0        0    20274 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/main_args.py
+-rw-r--r--   0        0        0     1302 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/manual_args.py
+-rw-r--r--   0        0        0     1587 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/message_args.py
+-rw-r--r--   0        0        0     1582 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/paid_args.py
+-rw-r--r--   0        0        0     1956 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/post_args.py
+-rw-r--r--   0        0        0     1635 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/story_args.py
+-rw-r--r--   0        0        0     5623 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     1684 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      863 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      718 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      261 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2131 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1756 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6092 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1650 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2894 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1090 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      452 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    23180 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2110 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2111 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4716 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      405 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      461 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1014 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     2679 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1716 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     8325 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1551 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      616 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      388 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4085 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0     1732 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3105 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      279 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     5061 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1058 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1606 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10457 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4447 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/run.py
+-rw-r--r--   0        0        0      255 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1595 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     3887 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3108 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2448 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2052 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2123 2024-04-08 04:31:49.787098 ofscraper-3.9.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     6349 1970-01-01 00:00:00.000000 ofscraper-3.9.0.dev9/PKG-INFO
```

### Comparing `ofscraper-3.9.0.dev7/LICENSE` & `ofscraper-3.9.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/README.md` & `ofscraper-3.9.0.dev9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 <img src="https://img.shields.io/pypi/v/ofscraper.svg?color=dark_green&label=Stable-Release" alt="drawing" style="height:75px"/>
 </div>
 </a>
 
 ## Dev
 
 <div style="display: inline-block">
-<a href="https://pypi.org/project/ofscraper/3.7.0.dev2/">
-<img src="https://img.shields.io/badge/Pre--Release-v3.70.dev-dark_green.svg" alt="drawing" style="height:75px"/>
+<a href="https://pypi.org/project/ofscraper/3.9.0.dev5/">
+<img src="https://img.shields.io/badge/Pre--Release-v3.90.dev-dark_green.svg" alt="drawing" style="height:75px"/>
 </a>
 </div>
 
 # Table-of-contents
 
 - [Description](#description)
 - [Documentation](#documentation)
@@ -61,14 +61,19 @@
     </li>
 </ol>
 
 # Issues
 
 Open a issue in this repo, or you can mention your issue in the [Discord](#discord)
 
+## Private Reports
+
+A ticket can be created in the ticket channel
+only you and admins have access to ticket discussions
+
 # Feature Requests
 
 [ClearFlask Feedback](https://ofscraper.clearflask.com/feedback) or [Discord](#discord)
 
 # Migrating from DC script
 
 To maintain compatibility with your current folders, make sure to modify the metadata option within the config file. Additionally, configure the save_path, dir_path, and filename settings to generate outputs that align with your existing setup.
```

#### html2text {}

```diff
@@ -28,26 +28,27 @@
       any way. We are not authorized, endorsed, or sponsored by OnlyFans. All
       OnlyFans trademarks remain the property of Fenix International Limited.
    2. This is a theoritical program only and is for educational purposes. If
       you choose to use it then it may or may not work. You solely accept full
       responsability and indemnify the creator, hostors, contributors and all
       other involved persons from any any all responsability.
 # Issues Open a issue in this repo, or you can mention your issue in the
-[Discord](#discord) # Feature Requests [ClearFlask Feedback](https://
-ofscraper.clearflask.com/feedback) or [Discord](#discord) # Migrating from DC
-script To maintain compatibility with your current folders, make sure to modify
-the metadata option within the config file. Additionally, configure the
-save_path, dir_path, and filename settings to generate outputs that align with
-your existing setup. The inherited metadata files from DIGITALCRIMINALS' script
-play a crucial role in preventing redundant downloads by acting as a check for
-duplicates. For comprehensive guidance on making these adjustments, you can
-refer to the provided resources 1. [Migration Guide](https://of-
-scraper.gitbook.io/of-scraper/migrating-from-digitalcriminals-script) 2.
-[Config Options](https://of-scraper.gitbook.io/of-scraper/config-options) 3.
-[Customize Save Path](https://of-scraper.gitbook.io/of-scraper/config-options/
-customizing-save-path) Ask in the discord or open an issue if you need help
-with what to change to accomplish this # Discord [Discord](https://discord.gg/
-wN7uxEVHRK) # Support buymeacoffee.com/datawhores BTC:
-bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87 ETH:
+[Discord](#discord) ## Private Reports A ticket can be created in the ticket
+channel only you and admins have access to ticket discussions # Feature
+Requests [ClearFlask Feedback](https://ofscraper.clearflask.com/feedback) or
+[Discord](#discord) # Migrating from DC script To maintain compatibility with
+your current folders, make sure to modify the metadata option within the config
+file. Additionally, configure the save_path, dir_path, and filename settings to
+generate outputs that align with your existing setup. The inherited metadata
+files from DIGITALCRIMINALS' script play a crucial role in preventing redundant
+downloads by acting as a check for duplicates. For comprehensive guidance on
+making these adjustments, you can refer to the provided resources 1. [Migration
+Guide](https://of-scraper.gitbook.io/of-scraper/migrating-from-
+digitalcriminals-script) 2. [Config Options](https://of-scraper.gitbook.io/of-
+scraper/config-options) 3. [Customize Save Path](https://of-scraper.gitbook.io/
+of-scraper/config-options/customizing-save-path) Ask in the discord or open an
+issue if you need help with what to change to accomplish this # Discord
+[Discord](https://discord.gg/wN7uxEVHRK) # Support buymeacoffee.com/datawhores
+BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87 ETH:
 0x1d427a6E336edF6D95e589C16cb740A1372F6609 [![codecov](https://codecov.io/gh/
 datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://
 codecov.io/gh/datawhores/OF-Scraper)
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/__version__.py` & `ofscraper-3.9.0.dev9/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/__version__.pye` & `ofscraper-3.9.0.dev9/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/actions/like.py` & `ofscraper-3.9.0.dev9/ofscraper/actions/like.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,80 +30,150 @@
     stop_after_attempt,
     wait_random,
 )
 
 import ofscraper.api.archive as archive
 import ofscraper.api.labels as labels_api
 import ofscraper.api.pinned as pinned
+import ofscraper.api.timeline as timeline
 import ofscraper.classes.labels as labels
+import ofscraper.classes.posts as posts_
 import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.utils.args.areas as areas
+import ofscraper.utils.args.read as read_args
 import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
+import ofscraper.utils.progress as progress_utils
+import ofscraper.utils.system.system as system
 from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
-from ..api import timeline
-
 sem = semaphoreDelayed(1)
 log = logging.getLogger("shared")
-import ofscraper.utils.args.read as read_args
 
 
-def get_posts(model_id, username):
-    args = read_args.retriveArgs()
-    pinned_posts = []
-    timeline_posts = []
-    archived_posts = []
-    labelled_posts = []
-    options = args.like_area
-    if "Pinned" in options or "All" in options:
-        pinned_posts = pinned.get_pinned_post(model_id)
-    if "Timeline" in options or "All" in options:
-        timeline_posts = timeline.get_timeline_media_progress(
-            model_id, username, forced_after=0
+@run
+async def get_posts(model_id, username):
+    responses = []
+    final_post_areas = set(areas.get_like_area())
+    tasks = []
+    with progress_utils.setup_api_split_progress_live():
+        async with sessionbuilder.sessionBuilder() as c:
+            while True:
+                max_count = min(
+                    constants.getattr("API_MAX_AREAS"),
+                    system.getcpu_count(),
+                    len(final_post_areas),
+                )
+                if not bool(tasks) and not bool(final_post_areas):
+                    break
+                for _ in range(max_count - len(tasks)):
+                    if "Pinned" in final_post_areas:
+                        tasks.append(
+                            asyncio.create_task(
+                                pinned.get_pinned_posts_progress(model_id, c)
+                            )
+                        )
+                        progress_utils.pinned_layout.visible = True
+                        final_post_areas.remove("Pinned")
+                    elif "Timeline" in final_post_areas:
+                        tasks.append(
+                            asyncio.create_task(
+                                timeline.get_timeline_posts_progress(
+                                    model_id=model_id,
+                                    username=username,
+                                    c=c,
+                                    forced_after=read_args.retriveArgs().after or 0,
+                                )
+                            )
+                        )
+                        progress_utils.timeline_layout.visible = True
+                        final_post_areas.remove("Timeline")
+                    if "Archived" in final_post_areas:
+                        tasks.append(
+                            asyncio.create_task(
+                                archive.get_archived_posts_progress(
+                                    model_id=model_id,
+                                    username=username,
+                                    c=c,
+                                    forced_after=read_args.retriveArgs().after or 0,
+                                )
+                            )
+                        )
+                        progress_utils.archived_layout.visible = True
+                        final_post_areas.remove("Archived")
+
+                    elif "Labels" in final_post_areas:
+                        tasks.append(
+                            asyncio.create_task(
+                                labels_api.get_labels_posts_progress(
+                                    model_id=model_id, c=c
+                                )
+                            )
+                        )
+                        progress_utils.labelled_layout.visible = True
+                        final_post_areas.remove("Labels")
+                if not bool(tasks):
+                    break
+                done, pending = await asyncio.wait(
+                    tasks, return_when=asyncio.FIRST_COMPLETED
+                )
+                await asyncio.sleep(1)
+                tasks = list(pending)
+                for results in done:
+                    try:
+                        data = await results or []
+                        responses.extend(data)
+                        await asyncio.sleep(1)
+                    except Exception as E:
+                        await asyncio.sleep(1)
+                        log.debug(E)
+                        continue
+    return pre_filter(
+        list(
+            map(
+                lambda x: posts_.Post(x, model_id=model_id, username=username),
+                responses,
+            )
         )
-    if "Archived" in options or "All" in options:
-        archived_posts = archive.get_archived_media(model_id, username, forced_after=0)
-    if "Labels" in options or "All" in options:
-        labels_ = labels_api.get_labels(model_id)
-        labelled_posts_ = labels_api.get_labelled_posts(labels_, model_id)
-        labelled_posts_ = list(
-            map(lambda x: labels.Label(x, model_id, username), labelled_posts_)
-        )
-    log.debug(
-        f"[bold]Number of Post Found[/bold] {len(pinned_posts) + len(timeline_posts) + len(archived_posts)}"
     )
-    return pinned_posts + timeline_posts + archived_posts + labelled_posts
 
 
 def get_posts_for_unlike(model_id, username):
     post = get_posts(model_id, username)
     return filter_for_favorited(post)
 
 
 def get_post_for_like(model_id, username):
     post = get_posts(model_id, username)
     return filter_for_unfavorited(post)
 
 
 def filter_for_unfavorited(posts: list) -> list:
-    output = list(filter(lambda x: x.get("isFavorite") == False, posts))
+    output = list(filter(lambda x: x.favorited == False, posts))
     log.debug(f"[bold]Number of unliked post[/bold] {len(output)}")
     return output
 
 
 def filter_for_favorited(posts: list) -> list:
-    output = list(filter(lambda x: x.get("isFavorite") == True, posts))
+    output = list(filter(lambda x: x.favorited == True, posts))
     log.debug(f"[bold]Number of liked post[/bold] {len(output)}")
     return output
 
 
+def pre_filter(posts):
+    valid_post = list(filter(lambda x: x.opened, posts))
+    seen = set()
+    return [
+        post for post in valid_post if post.id not in seen and not seen.add(post.id)
+    ]
+
+
 def get_post_ids(posts: list) -> list:
-    valid_post = list(filter(lambda x: x.get("isOpened") == True, posts))
-    return list(map(lambda x: x.get("id"), valid_post))
+    return list(map(lambda x: x.id, posts))
 
 
 def like(model_id, username, ids: list):
     _like(model_id, username, ids, True)
 
 
 def unlike(model_id, username, ids: list):
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/actions/process.py` & `ofscraper-3.9.0.dev9/ofscraper/actions/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 import ofscraper.utils.actions as actions
 import ofscraper.utils.args.areas as areas
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.exit as exit
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.profiles.tools as profile_tools
-from ofscraper.utils.text import get_text
 
 log = logging.getLogger("shared")
 
 
 @contextmanager
 def scrape_context_manager():
     # reset stream if needed
@@ -72,15 +71,15 @@
     if read_args.retriveArgs().users_first:
         asyncio.run(process_post_user_first())
     else:
         normal_post_process()
 
 
 @exit.exit_wrapper
-async def process_post_user_first():
+def process_post_user_first():
     with scrape_context_manager():
         if not placeholder.check_uniquename():
             log.warning(
                 "[red]Warning: Your generated filenames may not be unique\n \
             https://of-scraper.gitbook.io/of-scraper/config-options/customizing-save-path#warning[/red]      \
             "
             )
@@ -92,15 +91,15 @@
         length = len(userdata)
         output = []
         asyncio.create_task()
 
         # log.info(f"Data retrival progressing on model {count+1}/{length}")
 
 
-async def process_user_first_helper(ele):
+def process_user_first_helper(ele):
     if constants.getattr("SHOW_AVATAR") and ele.avatar:
         log.warning(f"Avatar : {ele.avatar}")
     if bool(areas.get_download_area()):
         log.info(
             f"Getting {','.join(areas.get_download_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
         )
     try:
@@ -112,37 +111,30 @@
     except Exception as e:
         if isinstance(e, KeyboardInterrupt):
             raise e
         log.traceback_(f"failed with exception: {e}")
         log.traceback_(traceback.format_exc())
 
 
-def scrape_paid(user_dict=None):
-    output = []
-    user_dict = user_dict or {}
-    output.extend(OF.process_all_paid())
-    user_dict = user_dict or {}
-    [
-        user_dict.update(
-            {ele.post.model_id: user_dict.get(ele.post.model_id, []) + [ele]}
-        )
-        for ele in output
-    ]
+def scrape_paid_all(user_dict=None):
+    user_dict = OF.process_all_paid()
     oldUsers = selector.get_ALL_SUBS_DICT()
-    for value in user_dict.values():
-        model_id = value[0].post.model_id
-        username = value[0].post.username
+    length = len(list(user_dict.keys()))
+    for count, value in enumerate(user_dict.values()):
+        model_id = value["model_id"]
+        username = value["username"]
+        posts = value["posts"]
+        medias = value["medias"]
+        log.warning(
+            f"Download paid content for {model_id}_{username} number:{count+1}/{length} models "
+        )
         selector.set_ALL_SUBS_DICTVManger(
             {username: models.Model(profile.scrape_profile(model_id))}
         )
-        download.download_process(
-            username,
-            model_id,
-            value,
-        )
+        download.download_process(username, model_id, medias, posts=posts)
     # restore og users
     selector.set_ALL_SUBS_DICT(oldUsers)
 
 
 @exit.exit_wrapper
 def normal_post_process():
     with scrape_context_manager():
@@ -196,15 +188,15 @@
                     log.warning(f"Avatar : {ele.avatar}")
                 log.warning(
                     f"Getting {','.join(areas.get_like_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
                 )
                 model_id = ele.id
                 operations.table_init_create(model_id, ele.name)
                 unfavorited_posts = like.get_post_for_like(model_id, ele.name)
-                unfavorited_posts = filters.media_filter_for_like(
+                unfavorited_posts = filters.post_filter_for_like(
                     unfavorited_posts, like=True
                 )
                 post_ids = like.get_post_ids(unfavorited_posts)
                 like.like(model_id, ele.name, post_ids)
 
 
 @exit.exit_wrapper
@@ -223,15 +215,15 @@
                     log.warning(f"Avatar : {ele.avatar}")
                 log.warning(
                     f"Getting {','.join(areas.get_like_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
                 )
                 model_id = profile.get_id(ele.name)
                 operations.table_init_create(model_id, ele.name)
                 favorited_posts = like.get_posts_for_unlike(model_id, ele.name)
-                favorited_posts = filters.media_filter_for_like(
+                favorited_posts = filters.post_filter_for_like(
                     favorited_posts, like=False
                 )
                 post_ids = like.get_post_ids(favorited_posts)
                 like.unlike(model_id, ele.name, post_ids)
 
 
 def add_selected_areas():
@@ -251,9 +243,9 @@
     elif "like" in action:
         actions.select_areas()
         functs.append(process_like)
     elif "unlike" in action:
         actions.select_areas()
         functs.append(process_unlike)
     if read_args.retriveArgs().scrape_paid:
-        functs.append(scrape_paid)
+        functs.append(scrape_paid_all)
     return functs
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/actions/scraper.py` & `ofscraper-3.9.0.dev9/ofscraper/actions/scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 import asyncio
 import logging
 import platform
 import traceback
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
-from rich.live import Live
-
 import ofscraper.api.archive as archive
 import ofscraper.api.highlights as highlights
 import ofscraper.api.labels as labels_api
 import ofscraper.api.messages as messages
 import ofscraper.api.paid as paid
 import ofscraper.api.pinned as pinned
 import ofscraper.api.profile as profile
@@ -32,54 +30,45 @@
 import ofscraper.classes.posts as posts_
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.db.operations as operations
 import ofscraper.filters.media.main as filters
 import ofscraper.utils.args.areas as areas
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
-import ofscraper.utils.console as console_
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.system.free as free
 import ofscraper.utils.system.system as system
+from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 
 
 @free.space_checker
 async def process_messages(model_id, username, c):
     try:
         with stdout.lowstdout():
             messages_ = await messages.get_messages_progress(model_id, username, c=c)
             messages_ = list(
                 map(lambda x: posts_.Post(x, model_id, username), messages_)
             )
-            [
-                operations.make_messages_table_changes(
-                    messages_,
-                    model_id=model_id,
-                    username=username,
-                )
-            ]
+            await operations.make_messages_table_changes(
+                messages_,
+                model_id=model_id,
+                username=username,
+            )
 
             log.debug(
                 f"[bold]Messages media count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}"
             )
             log.debug("Removing locked messages media")
             output = []
             [output.extend(message.media) for message in messages_]
             log.debug(f"[bold]Messages media count[/bold] {len(output)}")
-
-            await operations.batch_mediainsert(
-                output,
-                model_id=model_id,
-                username=username,
-                downloaded=False,
-            )
             # Update after database
             cache.set(
                 f"{model_id}_scrape_messages",
                 read_args.retriveArgs().after is not None
                 and read_args.retriveArgs().after != 0,
             )
 
@@ -99,20 +88,19 @@
             paid_content = await paid.get_paid_posts_progress(username, model_id, c=c)
             paid_content = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, responsetype="paid"),
                     paid_content,
                 )
             )
-            operations.make_post_table_changes(
+            await operations.make_post_table_changes(
                 paid_content,
                 model_id=model_id,
                 username=username,
             )
-
             output = []
             [output.extend(post.media) for post in paid_content]
             log.debug(f"[bold]Paid media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
@@ -141,15 +129,15 @@
                 map(
                     lambda x: posts_.Post(
                         x, model_id, username, responsetype="stories"
                     ),
                     stories,
                 )
             )
-            operations.make_stories_tables_changes(
+            await operations.make_stories_table_changes(
                 stories,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]Story media count[/bold] {sum(map(lambda x:len(x.post_media), stories))}"
@@ -181,15 +169,15 @@
                 map(
                     lambda x: posts_.Post(
                         x, model_id, username, responsetype="highlights"
                     ),
                     highlights_,
                 )
             )
-            operations.make_stories_tables_changes(
+            await operations.make_stories_table_changes(
                 highlights_,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]highlight media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))}"
@@ -215,78 +203,78 @@
             print(E)
 
 
 @free.space_checker
 async def process_timeline_posts(model_id, username, c):
     try:
         with stdout.lowstdout():
-            timeline_posts = await timeline.get_timeline_media_progress(
+            timeline_posts = await timeline.get_timeline_posts_progress(
                 model_id, username, c=c
             )
+
             timeline_posts = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, "timeline"),
                     timeline_posts,
                 )
             )
-            operations.make_post_table_changes(
-                timeline_posts,
+            timeline_only_posts = list(
+                filter(lambda x: x.regular_timeline, timeline_posts)
+            )
+
+            await operations.make_post_table_changes(
+                timeline_only_posts,
                 model_id=model_id,
                 username=username,
             )
-
             log.debug(
-                f"[bold]Timeline media count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_posts))}"
+                f"[bold]Timeline media count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_only_posts))}"
             )
             log.debug("Removing locked timeline media")
             output = []
-            [output.extend(post.media) for post in timeline_posts]
+            [output.extend(post.media) for post in timeline_only_posts]
             log.debug(f"[bold]Timeline media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
-            await operations.batch_mediainsert(
-                output,
-                model_id=model_id,
-                username=username,
-                downloaded=False,
-            )
             cache.set(
                 f"{model_id}_full_timeline_scrape",
                 read_args.retriveArgs().after is not None,
             )
             return (
                 list(filter(lambda x: isinstance(x, media.Media), output)),
-                timeline_posts,
+                timeline_only_posts,
             )
     except Exception as E:
         try:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         except:
             print(E)
 
 
 @free.space_checker
 async def process_archived_posts(model_id, username, c):
     try:
         with stdout.lowstdout():
-            archived_posts = await archive.get_archived_media(model_id, username, c=c)
+            archived_posts = await archive.get_archived_posts_progress(
+                model_id, username, c=c
+            )
             archived_posts = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, "archived"),
                     archived_posts,
                 )
             )
 
-            operations.make_post_table_changes(
+            await operations.make_post_table_changes(
                 archived_posts,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]Archived media count with locked[/bold] {sum(map(lambda x:len(x.post_media),archived_posts))}"
@@ -318,21 +306,19 @@
             print(E)
 
 
 @free.space_checker
 async def process_pinned_posts(model_id, username, c):
     try:
         with stdout.lowstdout():
-            pinned_posts = await pinned.get_pinned_post(model_id, c=c)
+            pinned_posts = await pinned.get_pinned_posts_progress(model_id, c=c)
             pinned_posts = list(
-                map(
-                    lambda x: posts_.Post(x, model_id, username, "pinned"), pinned_posts
-                )
+                map(lambda x: posts_.Post(x, model_id, username), pinned_posts)
             )
-            operations.make_post_table_changes(
+            await operations.make_post_table_changes(
                 pinned_posts,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]Pinned media count with locked[/bold] {sum(map(lambda x:len(x.post_media),pinned_posts))}"
@@ -344,20 +330,14 @@
 
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
-            await operations.batch_mediainsert(
-                output,
-                model_id=model_id,
-                username=username,
-                downloaded=False,
-            )
 
             return (
                 list(filter(lambda x: isinstance(x, media.Media), output)),
                 pinned_posts,
             )
     except Exception as E:
         try:
@@ -397,116 +377,96 @@
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         except:
             print(E)
 
 
 @free.space_checker
-def process_all_paid():
+@run
+async def process_all_paid():
     with stdout.lowstdout():
-        paid_content = paid.get_all_paid_posts()
+        paid_content = await paid.get_all_paid_posts()
         user_dict = {}
-        post_array = []
-        [
-            user_dict.update(
-                {
-                    (ele.get("fromUser", None) or ele.get("author", None) or {}).get(
-                        "id"
-                    ): user_dict.get(
-                        (
-                            ele.get("fromUser", None) or ele.get("author", None) or {}
-                        ).get("id"),
-                        [],
-                    )
-                    + [ele]
-                }
+        for ele in paid_content:
+            user_id = ele.get("fromUser", {}).get("id") or ele.get("author", {}).get(
+                "id"
             )
-            for ele in paid_content
-        ]
-        output = []
+            user_dict.setdefault(user_id, []).append(ele)
+        output = {}
         for model_id, value in user_dict.items():
             username = profile.scrape_profile(model_id).get("username")
-            if username == "modeldeleted" and operations.check_profile_table_exists(
-                model_id=model_id, username=username
+            if (
+                username == "modeldeleted"
+                and await operations.check_profile_table_exists(
+                    model_id=model_id, username=username
+                )
             ):
                 username = (
-                    operations.get_profile_info(model_id=model_id, username=username)
+                    await operations.get_profile_info(
+                        model_id=model_id, username=username
+                    )
                     or username
                 )
             log.info(f"Processing {username}_{model_id}")
-            operations.table_init_create(model_id=model_id, username=username)
-            log.debug(f"Created table for {username}")
+            await operations.table_init_create(model_id=model_id, username=username)
+            log.debug(f"Created table for {username}_{model_id}")
             all_posts = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, responsetype="paid"),
                     value,
                 )
             )
-            new_dict = {}
-            for ele in all_posts:
-                new_dict[ele.id] = ele
-            new_posts = new_dict.values()
-            operations.make_post_table_changes(
+            seen = set()
+            new_posts = [
+                post
+                for post in all_posts
+                if post.id not in seen and not seen.add(post.id)
+            ]
+            new_medias = [item for post in new_posts for item in post.media]
+            new_medias = filters.filterMedia(new_medias)
+            new_posts = filters.filterPost(new_posts)
+            await operations.make_post_table_changes(
                 new_posts,
                 model_id=model_id,
                 username=username,
             )
-            temp = []
-            [temp.extend(post.media) for post in new_posts]
-            output.extend(temp)
+            await operations.batch_mediainsert(
+                new_medias,
+                model_id=model_id,
+                username=username,
+                downloaded=False,
+            )
+
+            output[model_id] = dict(
+                model_id=model_id, username=username, posts=new_posts, medias=new_medias
+            )
             log.debug(
-                f"[bold]Paid media count {username}_{model_id}[/bold] {len(temp)}"
+                f"[bold]Paid media count {username}_{model_id}[/bold] {len(new_medias)}"
             )
-            log.debug(f"Added Paid {len(temp)} media items from {username}_{model_id}")
-            post_array.extend(new_posts)
 
         log.debug(
-            f"[bold]Paid Media for all models[/bold] {sum(map(lambda x:len(x.media),post_array))}"
+            f"[bold]Paid Media for all models[/bold] {sum(map(lambda x:len(x['medias']),output.values()))}"
         )
-        return filters.filterMedia(output)
+        return output
 
 
 @free.space_checker
 async def process_labels(model_id, username, c):
     try:
         with stdout.lowstdout():
-            labels_ = await labels_api.get_labels(model_id, c=c)
+            labelled_posts_ = await labels_api.get_labels_progress(model_id, c=c)
 
-            labels_ = (
-                labels_
-                if not read_args.retriveArgs().label
-                else list(
-                    filter(
-                        lambda x: x.get("name").lower()
-                        in read_args.retriveArgs().label,
-                        labels_,
-                    )
-                )
-            )
-            labelled_posts_ = await labels_api.get_labelled_posts(
-                labels_, model_id, c=c
-            )
             labelled_posts_ = list(
                 map(lambda x: labels.Label(x, model_id, username), labelled_posts_)
             )
-            curr = set(
-                operations.get_all_labels_ids(model_id=model_id, username=username)
-            )
-            for labelled_post in labelled_posts_:
-                operations.write_labels_table(
-                    labelled_post,
-                    list(
-                        filter(
-                            lambda post: (labelled_post.label_id, post.id) not in curr,
-                            labelled_post.posts,
-                        )
-                    ),
+            await operations.make_label_table_changes(
+                    labelled_posts_,
                     model_id=model_id,
                     username=username,
-                )
+            )
 
             log.debug(
                 f"[bold]Label media count with locked[/bold] {sum(map(lambda x:len(x),[post.post_media for labelled_post in labelled_posts_ for post in labelled_post.posts]))}"
             )
             log.debug("Removing locked messages media")
             output = [
                 post.media
@@ -535,15 +495,15 @@
         else ThreadPoolExecutor()
     )
     try:
         with executor:
             asyncio.get_event_loop().set_default_executor(executor)
             username = ele.name
             output = []
-            with progress_utils.setup_api_progress_live():
+            with progress_utils.setup_api_split_progress_live():
                 medias, posts = await process_task(model_id, username, ele)
                 output.extend(medias)
         return filters.filterMedia(output), filters.filterPost(posts)
     except Exception as E:
         print(E)
         raise E
 
@@ -558,15 +518,15 @@
             max_count = min(
                 constants.getattr("API_MAX_AREAS"),
                 system.getcpu_count(),
                 len(final_post_areas),
             )
             if not bool(tasks) and not bool(final_post_areas):
                 break
-            for i in range(max_count - len(tasks)):
+            for _ in range(max_count - len(tasks)):
                 if "Profile" in final_post_areas:
                     tasks.append(asyncio.create_task(process_profile(username, c)))
                     final_post_areas.remove("Profile")
                 elif "Pinned" in final_post_areas:
                     tasks.append(
                         asyncio.create_task(process_pinned_posts(model_id, username, c))
                     )
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/archive.py` & `ofscraper-3.9.0.dev9/ofscraper/api/timeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,366 +2,441 @@
                                                              
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
+
 import asyncio
 import contextvars
 import logging
 import math
 import traceback
 
 import arrow
 from tenacity import (
     AsyncRetrying,
-    retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
-import ofscraper.utils.config.data as data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
+import ofscraper.utils.sems as sems
+import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
+sem = None
 
 
-sem = None
+@run
+async def get_timeline_posts_progress(model_id, username, forced_after=None, c=None):
+    global sem
+    sem = sems.get_req_sem()
+
+    after = await get_after(model_id, username, forced_after)
+
+    splitArrays = await get_split_array(model_id, username, after)
+    tasks = get_tasks(splitArrays, c, model_id, after)
+    data = await process_tasks(tasks, model_id, after)
+    progress_utils.timeline_layout.visible = False
+    return data
 
 
 @run
-async def get_archived_media(model_id, username, forced_after=None, c=None):
-    tasks = []
-    new_tasks = []
-    min_posts = 50
+async def get_timeline_posts(model_id, username, forced_after=None, c=None):
+    global sem
+    sem = sems.get_req_sem()
+
+    if not read_args.retriveArgs().no_cache:
+        oldtimeline = await operations.get_timeline_postsinfo(
+            model_id=model_id, username=username
+        )
+    else:
+        oldtimeline = []
+    log.trace(
+        "oldtimeline {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"oldtimeline: {str(x)}", oldtimeline))
+            )
+        )
+    )
+    log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
+    oldtimeline = list(filter(lambda x: x != None, oldtimeline))
+    after = await get_after(model_id, username, forced_after)
+
+    with progress_utils.set_up_api_timeline():
+        splitArrays = await get_split_array(model_id, username, after)
+        tasks = get_tasks(splitArrays, c, model_id, after)
+        return await process_tasks(tasks, model_id, after)
+
+
+async def process_tasks(tasks, model_id, after):
     responseArray = []
     page_count = 0
-    job_progress = progress_utils.archived_progress
     overall_progress = progress_utils.overall_progress
 
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
-    oldarchived = (
-        operations.get_archived_postinfo(model_id=model_id, username=username)
-        if not read_args.retriveArgs().no_cache
-        else []
+    page_task = overall_progress.add_task(
+        f" Timeline Content Pages Progress: {page_count}", visible=True
     )
+    while bool(tasks):
+        new_tasks = []
+        try:
+            async with asyncio.timeout(
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
+            ):
+                for task in asyncio.as_completed(tasks):
+                    try:
+                        result, new_tasks_batch = await task
+                        new_tasks.extend(new_tasks_batch)
+                        page_count = page_count + 1
+                        overall_progress.update(
+                            page_task,
+                            description=f"Timeline Content Pages Progress: {page_count}",
+                        )
+                        responseArray.extend(result)
+                    except Exception as E:
+                        log.traceback_(E)
+                        log.traceback_(traceback.format_exc())
+                        continue
+        except TimeoutError as E:
+            cache.set(f"{model_id}_full_timeline_scrape")
+            log.traceback_(E)
+            log.traceback_(traceback.format_exc())
+        tasks = new_tasks
+    overall_progress.remove_task(page_task)
 
+    log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
     log.trace(
-        "oldarchive {posts}".format(
-            posts="\n\n".join(list(map(lambda x: f"oldarchive: {str(x)}", oldarchived)))
+        "post raw duped {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"dupedinfo timeline: {str(x)}", responseArray))
+            )
         )
     )
-    log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
-    oldarchived = list(filter(lambda x: x != None, oldarchived))
-    postedAtArray = sorted(oldarchived, key=lambda x: x[0])
+    seen = set()
+    new_posts = [
+        post
+        for post in responseArray
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
 
-    after = get_after(model_id, username, forced_after)
-    # set check
+    log.trace(f"timeline postids {list(map(lambda x:x.get('id'),new_posts))}")
+    log.trace(
+        "post raw unduped {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"undupedinfo timeline: {str(x)}", new_posts))
+            )
+        )
+    )
+    log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(new_posts)} found")
+    set_check(new_posts, model_id, after)
+    return new_posts
+
+
+async def get_split_array(model_id, username, after):
+    min_posts = 50
+
+    if not read_args.retriveArgs().no_cache:
+        oldtimeline = await operations.get_timeline_postsinfo(
+            model_id=model_id, username=username
+        )
+    else:
+        oldtimeline = []
+    log.trace(
+        "oldtimeline {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"oldtimeline: {str(x)}", oldtimeline))
+            )
+        )
+    )
+    log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
+    oldtimeline = list(filter(lambda x: x is not None, oldtimeline))
+    postsDataArray = sorted(oldtimeline, key=lambda x: x.get("created_at"))
     log.info(
         f"""
-Setting initial archived scan date for {username} to {arrow.get(after).format('YYYY.MM.DD')}
-[yellow]Hint: append ' --after 2000' to command to force scan of all archived posts + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --dupe' to command to force scan of all archived posts + download/re-download of all files[/yellow]
-    """
-    )
-    filteredArray = (
-        list(filter(lambda x: x[0] >= after, postedAtArray))
-        if len(postedAtArray) > 0
-        else []
+Setting initial timeline scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+[yellow]Hint: append ' --after 2000' to command to force scan of all timeline posts + download of new files only[/yellow]
+[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all timeline posts + download/re-download of all files[/yellow]
+
+            """
     )
+    filteredArray = list(filter(lambda x: x.get("created_at") >= after, postsDataArray))
 
-    if len(filteredArray) > min_posts:
-        splitArrays = [
-            filteredArray[i : i + min_posts]
-            for i in range(0, len(filteredArray), min_posts)
-        ]
-        # use the previous split for timesamp
+    splitArrays = [
+        filteredArray[i : i + min_posts]
+        for i in range(0, len(filteredArray), min_posts)
+    ]
+    return splitArrays
+
+
+def get_tasks(splitArrays, c, model_id, after):
+    tasks = []
+    job_progress = progress_utils.timeline_progress
+
+    if len(splitArrays) > 2:
         tasks.append(
             asyncio.create_task(
-                scrape_archived_posts(
+                scrape_timeline_posts(
                     c,
                     model_id,
                     job_progress=job_progress,
-                    required_ids=set(list(map(lambda x: x[0], splitArrays[0]))),
-                    timestamp=read_args.retriveArgs().after.float_timestamp
-                    if read_args.retriveArgs().after
-                    else None,
+                    required_ids=set([ele.get("created_at") for ele in splitArrays[0]]),
+                    timestamp=splitArrays[0][0].get("created_at"),
+                    offset=True,
                 )
             )
         )
         [
             tasks.append(
                 asyncio.create_task(
-                    scrape_archived_posts(
+                    scrape_timeline_posts(
                         c,
                         model_id,
                         job_progress=job_progress,
-                        required_ids=set(list(map(lambda x: x[0], splitArrays[i]))),
-                        timestamp=splitArrays[i - 1][-1][0],
+                        required_ids=set(
+                            [ele.get("created_at") for ele in splitArrays[i]]
+                        ),
+                        timestamp=splitArrays[i - 1][-1].get("created_at"),
+                        offset=False,
                     )
                 )
             )
             for i in range(1, len(splitArrays) - 1)
         ]
         # keeping grabbing until nothing left
         tasks.append(
             asyncio.create_task(
-                scrape_archived_posts(
+                scrape_timeline_posts(
                     c,
                     model_id,
                     job_progress=job_progress,
-                    timestamp=splitArrays[-2][-1][0],
+                    timestamp=splitArrays[-1][0].get("created_at"),
+                    offset=True,
                 )
             )
         )
-    else:
+    # use the first split if less then 3
+    elif len(splitArrays) > 0:
         tasks.append(
             asyncio.create_task(
-                scrape_archived_posts(
-                    c, model_id, job_progress=job_progress, timestamp=after
+                scrape_timeline_posts(
+                    c,
+                    model_id,
+                    job_progress=job_progress,
+                    timestamp=splitArrays[0][0].get("created_at"),
+                    offset=True,
                 )
             )
         )
-
-    page_task = overall_progress.add_task(
-        f"Archived Content Pages Progress: {page_count}", visible=True
-    )
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Archived Content Pages Progress: {page_count}",
-                        )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            cache.set(f"{model_id}_full_archived_scrape")
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-
-        tasks = new_tasks
-    overall_progress.remove_task(page_task)
-    progress_utils.archived_layout.visible = False
-
-    unduped = {}
-    log.debug(f"[bold]Archived Count with Dupes[/bold] {len(responseArray)} found")
-    for post in responseArray:
-        id = post["id"]
-        if unduped.get(id):
-            continue
-        unduped[id] = post
-    log.trace(f"archive dupeset postids {list(unduped.keys())}")
-    log.trace(
-        "archived raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo archive: {str(x)}", unduped))
+    # use after if split is empty i.e no db data
+    else:
+        tasks.append(
+            asyncio.create_task(
+                scrape_timeline_posts(
+                    c, model_id, job_progress=job_progress, timestamp=after, offset=True
+                )
             )
         )
-    )
-    log.debug(f"[bold]Archived Count without Dupes[/bold] {len(unduped)} found")
-    set_check(unduped, model_id, after)
-    return list(unduped.values())
+    return tasks
 
 
 def set_check(unduped, model_id, after):
     if not after:
-        newCheck = {}
-        for post in cache.get(f"archived_check_{model_id}", default=[]) + list(
-            unduped.values()
-        ):
-            newCheck[post["id"]] = post
+        seen = set()
+        all_posts = [
+            post
+            for post in cache.get(f"timeline_check_{model_id}", default=[]) + unduped
+            if post["id"] not in seen and not seen.add(post["id"])
+        ]
         cache.set(
-            f"archived_check_{model_id}",
-            list(newCheck.values()),
+            f"timeline_check_{model_id}",
+            all_posts,
             expire=constants.getattr("DAY_SECONDS"),
         )
         cache.close()
 
 
-def get_after(model_id, username, forced_after=None):
-    if forced_after != None:
+def get_individual_post(id):
+    with sessionbuilder.sessionBuilder(backend="httpx") as c:
+        with c.requests(constants.getattr("INDIVIDUAL_TIMELINE").format(id))() as r:
+            if r.ok:
+                log.trace(f"post raw individual {r.json()}")
+                return r.json()
+            else:
+                log.debug(
+                    f"[bold]individual post response status code:[/bold]{r.status}"
+                )
+                log.debug(f"[bold]individual post response:[/bold] {r.text_()}")
+                log.debug(f"[bold]individual post headers:[/bold] {r.headers}")
+
+
+async def get_after(model_id, username, forced_after=None):
+    if forced_after is not None:
         return forced_after
+    elif not settings.get_after_enabled():
+        return 0
     elif read_args.retriveArgs().after == 0:
         return 0
     elif read_args.retriveArgs().after:
         return read_args.retriveArgs().after.float_timestamp
-
-    elif (
-        cache.get(f"{model_id}_full_archived_scrape")
-        and not read_args.retriveArgs().after
-        and not data.get_disable_after()
-    ):
+    elif cache.get(f"{model_id}_full_timeline_scrape"):
         log.info(
-            "Used --after previously. Scraping all archived posts required to make sure content is not missing"
+            "Used --after previously. Scraping all timeline posts required to make sure content is not missing"
         )
         return 0
-    curr = operations.get_archived_media(model_id=model_id, username=username)
-
+    curr = await operations.get_timeline_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
-    missing_items = list(filter(lambda x: x[10] != 1, curr))
-    missing_items = list(sorted(missing_items, key=lambda x: arrow.get(x[12])))
+    missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
+    missing_items = list(
+        sorted(missing_items, key=lambda x: arrow.get(x.get("posted_at") or 0))
+    )
     if len(missing_items) == 0:
         log.debug("Using last db date because,all downloads in db marked as downloaded")
-        return (
-            operations.get_last_archived_date(model_id=model_id, username=username)
-            - 1000
+        return await operations.get_last_timeline_date(
+            model_id=model_id, username=username
         )
     else:
         log.debug(
             f"Setting date slightly before earliest missing item\nbecause {len(missing_items)} posts in db are marked as undownloaded"
         )
-        return arrow.get(missing_items[0][12]).float_timestamp - 1000
+        return arrow.get(missing_items[0]["posted_at"] or 0).float_timestamp
 
 
-@run
-async def scrape_archived_posts(
-    c, model_id, job_progress=None, timestamp=None, required_ids=None
+async def scrape_timeline_posts(
+    c, model_id, job_progress=None, timestamp=None, required_ids=None, offset=False
 ) -> list:
-    global sem
     posts = None
     attempt.set(0)
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
+    timestamp = float(timestamp) - 1000 if timestamp and offset else timestamp
+
     if timestamp and (
         float(timestamp)
         > (read_args.retriveArgs().before or arrow.now()).float_timestamp
     ):
-        return []
-    if timestamp:
-        ep = constants.getattr("archivedNextEP")
-        url = ep.format(model_id, str(timestamp))
-    else:
-        ep = constants.getattr("archivedEP")
-        url = ep.format(model_id)
+        return [], []
+    url = (
+        constants.getattr("timelineNextEP").format(model_id, str(timestamp))
+        if timestamp
+        else constants.getattr("timelineEP").format(model_id)
+    )
     log.debug(url)
-
     async for _ in AsyncRetrying(
         retry=retry_if_not_exception_type(KeyboardInterrupt),
         stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
         wait=wait_random(
             min=constants.getattr("OF_MIN"),
             max=constants.getattr("OF_MAX"),
         ),
         reraise=True,
     ):
         with _:
-            new_tasks = []
             await sem.acquire()
+            await asyncio.sleep(1)
+            new_tasks = []
             try:
                 attempt.set(attempt.get(0) + 1)
                 task = (
                     job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",
+                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
                         visible=True,
                     )
                     if job_progress
                     else None
                 )
-                async with c.requests(url)() as r:
+
+                async with c.requests(url=url)() as r:
                     if r.ok:
                         posts = (await r.json_())["list"]
-                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
+                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
                         if not posts:
                             posts = []
                         if len(posts) == 0:
-                            log.debug(f" {log_id} -> number of post found 0")
+                            log.debug(f"{log_id} -> number of post found 0")
+
                         elif len(posts) > 0:
-                            log.debug(
-                                f"{log_id} -> number of archived post found {len(posts)}"
-                            )
+                            log.debug(f"{log_id} -> number of post found {len(posts)}")
                             log.debug(
                                 f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
                             )
                             log.debug(
                                 f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
                             )
                             log.debug(
-                                f"{log_id} -> found archived post IDs {list(map(lambda x:x.get('id'),posts))}"
+                                f"{log_id} -> found postids {list(map(lambda x:x.get('id'),posts))}"
                             )
                             log.trace(
-                                "{log_id} -> archive raw {posts}".format(
+                                "{log_id} -> post raw {posts}".format(
                                     log_id=log_id,
                                     posts="\n\n".join(
                                         list(
                                             map(
-                                                lambda x: f"scrapeinfo archive: {str(x)}",
+                                                lambda x: f"scrapeinfo timeline: {str(x)}",
                                                 posts,
                                             )
                                         )
                                     ),
                                 )
                             )
-
-                            if required_ids == None:
+                            if not required_ids:
                                 new_tasks.append(
                                     asyncio.create_task(
-                                        scrape_archived_posts(
+                                        scrape_timeline_posts(
                                             c,
                                             model_id,
                                             job_progress=job_progress,
                                             timestamp=posts[-1]["postedAtPrecise"],
+                                            offset=False,
                                         )
                                     )
                                 )
                             else:
                                 [
                                     required_ids.discard(float(ele["postedAtPrecise"]))
                                     for ele in posts
                                 ]
-
                                 if len(required_ids) > 0 and float(
-                                    timestamp or 0
-                                ) < max(required_ids):
+                                    (timestamp) or 0
+                                ) <= max(required_ids):
                                     new_tasks.append(
                                         asyncio.create_task(
-                                            scrape_archived_posts(
+                                            scrape_timeline_posts(
                                                 c,
                                                 model_id,
                                                 job_progress=job_progress,
                                                 timestamp=posts[-1]["postedAtPrecise"],
                                                 required_ids=required_ids,
+                                                offset=False,
                                             )
                                         )
                                     )
                     else:
                         log.debug(
-                            f"[bold]archived response status code:[/bold]{r.status}"
+                            f"[bold]timeline response status code:[/bold]{r.status}"
                         )
-                        log.debug(f"[bold]archived response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+                        log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
+                        log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
                         r.raise_for_status()
             except Exception as E:
+                await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
+                (
+                    job_progress.remove_task(task)
+                    if job_progress and task != None
+                    else None
+                )
             return posts, new_tasks
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/highlights.py` & `ofscraper-3.9.0.dev9/ofscraper/api/highlights.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import asyncio
 import contextvars
 import logging
 import traceback
 
 from tenacity import (
     AsyncRetrying,
-    retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.utils.constants as constants
@@ -31,126 +30,49 @@
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 sem = None
 attempt = contextvars.ContextVar("attempt")
 
 
+#############################################################################
+#### Stories
+####
+##############################################################################
 @run
 async def get_stories_post_progress(model_id, c=None):
     global sem
     sem = semaphoreDelayed(1)
-    responseArray = []
-    page_count = 0
     tasks = []
     job_progress = progress_utils.stories_progress
-    overall_progress = progress_utils.overall_progress
 
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
     tasks.append(
         asyncio.create_task(scrape_stories(c, model_id, job_progress=job_progress))
     )
-    page_task = overall_progress.add_task(
-        f"Stories Pages Progress: {page_count}", visible=True
-    )
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Stories Content Pages Progress: {page_count}",
-                        )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
 
-    overall_progress.remove_task(page_task)
-    progress_utils.stories_layout.visible = False
+    data = await process_stories_tasks(tasks)
 
-    log.trace(
-        "stories raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo stories: {str(x)}", responseArray))
-            )
-        )
-    )
-    log.debug(f"[bold]stories Count with Dupes[/bold] {len(responseArray)} found")
-    outdict = {}
-    for ele in responseArray:
-        outdict[ele["id"]] = ele
-    log.debug(
-        f"[bold]stories Count with Dupes[/bold] {len(list(outdict.values()))} found"
-    )
-    return list(outdict.values())
+    progress_utils.stories_layout.visible = False
+    return data
 
 
 @run
 async def get_stories_post(model_id, c=None):
     global sem
     sem = semaphoreDelayed(1)
-    responseArray = []
-    page_count = 0
     tasks = []
-
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
-    tasks.append(asyncio.create_task(scrape_stories(c, model_id, None)))
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-
-    log.trace(
-        "stories raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo stories: {str(x)}", responseArray))
+    with progress_utils.set_up_api_stories():
+        tasks.append(
+            asyncio.create_task(
+                scrape_stories(
+                    c, model_id, job_progress=progress_utils.stories_progress
+                )
             )
         )
-    )
-    log.debug(f"[bold]stories Count with Dupes[/bold] {len(responseArray)} found")
-    outdict = {}
-    for ele in responseArray:
-        outdict[ele["id"]] = ele
-    log.debug(
-        f"[bold]stories Count with Dupes[/bold] {len(list(outdict.values()))} found"
-    )
-    return list(outdict.values())
+        return await process_stories_tasks(tasks)
 
 
 async def scrape_stories(c, user_id, job_progress=None) -> list:
     global sem
     global tasks
     stories = None
     attempt.set(0)
@@ -209,236 +131,262 @@
                 await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
+                (
+                    job_progress.remove_task(task)
+                    if job_progress and task != None
+                    else None
+                )
 
             return stories, new_tasks
 
 
-@run
-async def get_highlight_post_progress(model_id, c=None):
-    highlightLists = await get_highlight_list_progress(model_id, c)
-    return await get_highlights_via_list_progress(highlightLists, c)
-
-
-async def get_highlight_list_progress(model_id, c=None):
-    global sem
-    sem = semaphoreDelayed(1)
-
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
-    highlightLists = []
-
+async def process_stories_tasks(tasks):
+    responseArray = []
     page_count = 0
-    tasks = []
-    job_progress = progress_utils.highlights_progress
     overall_progress = progress_utils.overall_progress
-    tasks.append(
-        asyncio.create_task(
-            scrape_highlight_list(c, model_id, job_progress=job_progress)
-        )
-    )
     page_task = overall_progress.add_task(
-        f"Highlights List Pages Progress: {page_count}", visible=True
+        f"Stories Pages Progress: {page_count}", visible=True
     )
+
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         page_count = page_count + 1
                         overall_progress.update(
                             page_task,
-                            description=f"Highlights List Pages Progress: {page_count}",
+                            description=f"Stories Content Pages Progress: {page_count}",
                         )
-                        highlightLists.extend(result)
+                        responseArray.extend(result)
                     except Exception as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
                         continue
         except TimeoutError as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
-
         tasks = new_tasks
-    overall_progress.remove_task(page_task)
-    return highlightLists
 
+    overall_progress.remove_task(page_task)
 
-async def get_highlights_via_list_progress(highlightLists, c=None):
-    job_progress = progress_utils.highlights_progress
-    overall_progress = progress_utils.overall_progress
-    tasks = []
-    [
-        tasks.append(
-            asyncio.create_task(scrape_highlights(c, i, job_progress=job_progress))
+    log.trace(
+        "stories raw duped {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"dupedinfo stories: {str(x)}", responseArray))
+            )
         )
-        for i in highlightLists
+    )
+    log.debug(f"[bold]stories Count with Dupes[/bold] {len(responseArray)} found")
+    seen = set()
+    new_posts = [
+        post
+        for post in responseArray
+        if post["id"] not in seen and not seen.add(post["id"])
     ]
 
-    highlightResponse = []
-    page_count = 0
-    page_task = overall_progress.add_task(
-        f"Highlight Content via List Pages Progress: {page_count}", visible=True
-    )
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Highlight Content via List Pages Progress: {page_count}",
-                        )
-                        highlightResponse.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
+    log.trace(f"stories postids {list(map(lambda x:x.get('id'),new_posts))}")
     log.trace(
-        "highlight raw unduped {posts}".format(
+        "post raw unduped {posts}".format(
             posts="\n\n".join(
-                list(
-                    map(
-                        lambda x: f"undupedinfo heighlight: {str(x)}", highlightResponse
-                    )
-                )
+                list(map(lambda x: f"undupedinfo stories: {str(x)}", new_posts))
             )
         )
     )
-    log.debug(f"[bold]highlight Count with Dupes[/bold] {len(highlightResponse)} found")
-    outdict = {}
-    for ele in highlightResponse:
-        outdict[ele["id"]] = ele
-    log.debug(
-        f"[bold]highlight Count with Dupes[/bold] {len(list(outdict.values()))} found"
+    log.debug(f"[bold]Stories Count without Dupes[/bold] {len(new_posts)} found")
+
+    return new_posts
+
+
+##############################################################################
+#### Highlights
+####
+##############################################################################
+
+
+@run
+async def get_highlight_post_progress(model_id, c=None):
+    highlightLists = await get_highlight_list_progress(model_id, c)
+    return await get_highlights_via_list_progress(highlightLists, c)
+
+
+async def get_highlight_list_progress(model_id, c=None):
+    global sem
+    sem = semaphoreDelayed(1)
+
+    tasks = []
+    tasks.append(
+        asyncio.create_task(
+            scrape_highlight_list(
+                c, model_id, job_progress=progress_utils.highlights_progress
+            )
+        )
     )
-    overall_progress.remove_task(page_task)
-    progress_utils.highlights_layout.visible = False
-    return list(outdict.values())
+    return await process_task_get_highlight_list(tasks)
+
+
+async def get_highlights_via_list_progress(highlightLists, c=None):
+    tasks = []
+    [
+        tasks.append(
+            asyncio.create_task(
+                scrape_highlights(c, i, job_progress=progress_utils.highlights_progress)
+            )
+        )
+        for i in highlightLists
+    ]
+    return await process_task_highlights(tasks)
 
 
 @run
 async def get_highlight_post(model_id, c=None):
     highlightList = await get_highlight_list(model_id, c)
     return await get_highlights_via_list(highlightList, c)
 
 
 async def get_highlight_list(model_id, c=None):
     global sem
     sem = semaphoreDelayed(1)
 
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
+    with progress_utils.set_up_api_highlights_lists():
+        tasks = []
+        tasks.append(
+            asyncio.create_task(
+                scrape_highlight_list(
+                    c, model_id, job_progress=progress_utils.highlights_progress
+                )
+            )
+        )
+        return await process_task_get_highlight_list(tasks)
+
+
+async def get_highlights_via_list(highlightLists, c):
+    tasks = []
+    with progress_utils.set_up_api_highlights():
+
+        [
+            tasks.append(
+                asyncio.create_task(
+                    scrape_highlights(
+                        c, i, job_progress=progress_utils.highlights_progress
+                    )
+                )
+            )
+            for i in highlightLists
+        ]
+        return await process_task_highlights(tasks)
+
+
+async def process_task_get_highlight_list(tasks):
     highlightLists = []
 
     page_count = 0
-    tasks = []
-    tasks.append(
-        asyncio.create_task(scrape_highlight_list(c, model_id, job_progress=None))
+    overall_progress = progress_utils.overall_progress
+
+    page_task = overall_progress.add_task(
+        f"Highlights List Pages Progress: {page_count}", visible=True
     )
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         page_count = page_count + 1
+                        overall_progress.update(
+                            page_task,
+                            description=f"Highlights List Pages Progress: {page_count}",
+                        )
                         highlightLists.extend(result)
                     except Exception as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
                         continue
         except TimeoutError as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
 
         tasks = new_tasks
+    overall_progress.remove_task(page_task)
     return highlightLists
 
 
-async def get_highlights_via_list(highlightLists, c):
-    job_progress = None
-    tasks = []
-    [
-        tasks.append(
-            asyncio.create_task(scrape_highlights(c, i, job_progress=job_progress))
-        )
-        for i in highlightLists
-    ]
-
+async def process_task_highlights(tasks):
     highlightResponse = []
     page_count = 0
+    overall_progress = progress_utils.overall_progress
+    page_task = overall_progress.add_task(
+        f"Highlight Content via List Pages Progress: {page_count}", visible=True
+    )
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         page_count = page_count + 1
+                        overall_progress.update(
+                            page_task,
+                            description=f"Highlight Content via List Pages Progress: {page_count}",
+                        )
                         highlightResponse.extend(result)
                     except Exception as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
                         continue
         except TimeoutError as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         tasks = new_tasks
-
     log.trace(
-        "highlight raw unduped {posts}".format(
+        "highlight raw duped {posts}".format(
             posts="\n\n".join(
                 list(
-                    map(
-                        lambda x: f"undupedinfo heighlight: {str(x)}", highlightResponse
-                    )
+                    map(lambda x: f"dupedinfo heighlight: {str(x)}", highlightResponse)
                 )
             )
         )
     )
     log.debug(f"[bold]highlight Count with Dupes[/bold] {len(highlightResponse)} found")
-    outdict = {}
-    for ele in highlightResponse:
-        outdict[ele["id"]] = ele
-    log.debug(
-        f"[bold]highlight Count with Dupes[/bold] {len(list(outdict.values()))} found"
+    seen = set()
+    new_posts = [
+        post
+        for post in highlightResponse
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
+
+    log.trace(f"highlights postids {list(map(lambda x:x.get('id'),new_posts))}")
+    log.trace(
+        "highlights raw unduped {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"undupedinfo highlights: {str(x)}", new_posts))
+            )
+        )
     )
-    return list(outdict.values())
+    log.debug(f"[bold]Highlights Count without Dupes[/bold] {len(new_posts)} found")
+
+    return new_posts
 
 
 async def scrape_highlight_list(c, user_id, job_progress=None, offset=0) -> list:
     global sem
     attempt.set(0)
     async for _ in AsyncRetrying(
         retry=retry_if_not_exception_type(KeyboardInterrupt),
@@ -488,17 +436,19 @@
                 await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
+                (
+                    job_progress.remove_task(task)
+                    if job_progress and task != None
+                    else None
+                )
 
             return data, new_tasks
 
 
 async def scrape_highlights(c, id, job_progress=None) -> list:
     global sem
     attempt.set(0)
@@ -543,17 +493,19 @@
                 await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
+                (
+                    job_progress.remove_task(task)
+                    if job_progress and task != None
+                    else None
+                )
 
             return resp_data["stories"], new_tasks
 
 
 def get_highlightList(data):
     for ele in list(filter(lambda x: isinstance(x, list), data.values())):
         if (
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/init.py` & `ofscraper-3.9.0.dev9/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/labels.py` & `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/lists.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,370 +1,368 @@
 r"""
-                                                      o       
+                                                             
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import contextvars
 import logging
 import traceback
+from concurrent.futures import ThreadPoolExecutor
 
+from rich.console import Group
+from rich.live import Live
+from rich.panel import Panel
+from rich.progress import Progress, SpinnerColumn, TextColumn
+from rich.style import Style
 from tenacity import (
     AsyncRetrying,
     retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
+import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.utils.args.read as read_args
+import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
-import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.sems as sems
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 sem = None
 
 
 @run
-async def get_labels(model_id, c=None):
-    global sem
-    sem = sems.get_req_sem()
-    responseArray = []
-    tasks = []
-
-    page_count = 0
-    job_progress = progress_utils.labelled_progress
-    overall_progress = progress_utils.overall_progress
-
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
-    tasks.append(
-        asyncio.create_task(scrape_labels(c, model_id, job_progress=job_progress))
+async def get_otherlist():
+    out = []
+    if any(
+        [
+            ele
+            not in [
+                constants.getattr("OFSCRAPER_RESERVED_LIST"),
+                constants.getattr("OFSCRAPER_RESERVED_LIST_ALT"),
+            ]
+            for ele in read_args.retriveArgs().user_list or []
+        ]
+    ):
+        out.extend(await get_lists())
+    out = list(
+        filter(
+            lambda x: x.get("name").lower() in read_args.retriveArgs().user_list or[],
+            out,
+        )
+    )
+    log.debug(
+        f"User lists found on profile {list(map(lambda x:x.get('name').lower(),out))}"
     )
+    return await get_list_users(out)
 
-    page_task = overall_progress.add_task(
-        f"Label Names Pages Progresss: {page_count}", visible=True
+
+@run
+async def get_blacklist():
+    out = []
+    if len(read_args.retriveArgs().black_list or []) >= 1:
+        out.extend(await get_lists())
+    out = list(
+        filter(
+            lambda x: x.get("name").lower() in read_args.retriveArgs().black_list or [],
+            out,
+        )
+    )
+    log.debug(
+        f"Black lists found on profile {list(map(lambda x:x.get('name').lower(),out))}"
     )
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
+    names = list(await get_list_users(out))
+    return set(list(map(lambda x: x["id"], names)))
+
+
+async def get_lists():
+    with ThreadPoolExecutor(
+        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
+    ) as executor:
+        asyncio.get_event_loop().set_default_executor(executor)
+        overall_progress = Progress(
+            SpinnerColumn(style=Style(color="blue")),
+            TextColumn("Getting lists...\n{task.description}"),
+        )
+        job_progress = Progress("{task.description}")
+        progress_group = Group(overall_progress, Panel(Group(job_progress)))
+
+        output = []
+        tasks = []
+        page_count = 0
+        with Live(
+            progress_group, refresh_per_second=5, console=console.get_shared_console()
+        ):
+            async with sessionbuilder.sessionBuilder() as c:
+                tasks.append(asyncio.create_task(scrape_lists(c, job_progress)))
+                page_task = overall_progress.add_task(
+                    f"UserList Pages Progress: {page_count}", visible=True
+                )
+                while bool(tasks):
+                    new_tasks = []
                     try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Label Names Pages Progress: {page_count}",
-                        )
-                        responseArray.extend(result)
-                    except Exception as E:
+                        async with asyncio.timeout(
+                            constants.getattr("API_TIMEOUT_PER_TASKS")
+                            * max(len(tasks), 2)
+                        ):
+                            for task in asyncio.as_completed(tasks):
+                                try:
+                                    result, new_tasks_batch = await task
+                                    new_tasks.extend(new_tasks_batch)
+                                    page_count = page_count + 1
+                                    overall_progress.update(
+                                        page_task,
+                                        description=f"UserList Pages Progress: {page_count}",
+                                    )
+                                    output.extend(result)
+                                except Exception as E:
+                                    log.traceback_(E)
+                                    log.traceback_(traceback.format_exc())
+                                    continue
+                    except TimeoutError as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
-                        continue
-            tasks = new_tasks
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-    overall_progress.remove_task(page_task)
-    progress_utils.labelled_layout.visible = False
-    log.trace(
-        "post label names unduped {posts}".format(
-            posts="\n\n".join(map(lambda x: f" label name unduped:{x}", responseArray))
+                    tasks = new_tasks
+
+        overall_progress.remove_task(page_task)
+        log.trace(
+            "list unduped {posts}".format(
+                posts="\n\n".join(map(lambda x: f" list data raw:{x}", output))
+            )
         )
-    )
-    log.debug(
-        f"[bold]Labels name count without Dupes[/bold] {len(responseArray)} found"
-    )
-    return responseArray
+        log.debug(f"[bold]lists name count without Dupes[/bold] {len(output)} found")
+        return output
 
 
-async def scrape_labels(c, model_id, job_progress=None, offset=0):
+async def scrape_lists(c, job_progress, offset=0):
     global sem
-    labels = None
+    global tasks
+    sem = sems.get_req_sem()
     attempt.set(0)
     async for _ in AsyncRetrying(
         stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
         retry=retry_if_not_exception_type(KeyboardInterrupt),
         wait=wait_random(
             min=constants.getattr("OF_MIN"),
             max=constants.getattr("OF_MAX"),
         ),
         reraise=True,
     ):
         with _:
             new_tasks = []
             await sem.acquire()
-            await asyncio.sleep(1)
             try:
                 attempt.set(attempt.get(0) + 1)
-
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} labels offset -> {offset}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
+                task = job_progress.add_task(
+                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : getting lists offset -> {offset}",
+                    visible=True,
                 )
                 async with c.requests(
-                    url=constants.getattr("labelsEP").format(model_id, offset)
+                    url=constants.getattr("listEP").format(offset)
                 )() as r:
                     if r.ok:
                         data = await r.json_()
-                        labels = list(
-                            filter(lambda x: isinstance(x, list), data.values())
-                        )[0]
+                        out_list = data["list"] or []
+                        log.debug(
+                            f"offset:{offset} -> lists names found {list(map(lambda x:x['name'],out_list))}"
+                        )
                         log.debug(
-                            f"offset:{offset} -> labels names found {len(labels)}"
+                            f"offset:{offset} -> number of lists found {len(out_list)}"
                         )
                         log.debug(
                             f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
                         )
                         log.trace(
                             "offset:{offset} -> label names raw: {posts}".format(
                                 offset=offset, posts=data
                             )
                         )
 
-                        if (
-                            data.get("hasMore")
-                            and len(data.get("list")) > 0
-                            and data.get("nextOffset") != offset
-                        ):
-                            offset = offset + len(data.get("list"))
+                        if data.get("hasMore") and len(out_list) > 0:
+                            offset = offset + len(out_list)
                             new_tasks.append(
                                 asyncio.create_task(
-                                    scrape_labels(
-                                        c,
-                                        model_id,
-                                        job_progress=job_progress,
-                                        offset=offset,
-                                    )
+                                    scrape_lists(c, job_progress, offset=offset)
                                 )
                             )
-                        return data.get("list"), new_tasks
 
                     else:
-                        log.debug(
-                            f"[bold]labels response status code:[/bold]{r.status}"
-                        )
-                        log.debug(f"[bold]labels response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]labels headers:[/bold] {r.headers}")
+                        log.debug(f"[bold]lists response status code:[/bold]{r.status}")
+                        log.debug(f"[bold]lists response:[/bold] {await r.text_()}")
+                        log.debug(f"[bold]lists headers:[/bold] {r.headers}")
                         r.raise_for_status()
             except Exception as E:
-                await asyncio.sleep(1)
-
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
+                job_progress.remove_task(task)
+            return out_list, new_tasks
 
 
-@run
-async def get_labelled_posts(labels, username, c=None):
+async def get_list_users(lists):
     global sem
     sem = sems.get_req_sem()
-    responseDict = get_default_label_dict(labels)
-    tasks = []
-    page_count = 0
-    job_progress = progress_utils.labelled_progress
-    overall_progress = progress_utils.overall_progress
-
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
-    [
-        tasks.append(
-            asyncio.create_task(
-                scrape_labelled_posts(c, label, username, job_progress=job_progress)
-            )
+    with ThreadPoolExecutor(
+        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
+    ) as executor:
+        asyncio.get_event_loop().set_default_executor(executor)
+        overall_progress = Progress(
+            SpinnerColumn(style=Style(color="blue")),
+            TextColumn(
+                "Getting users from lists (this may take awhile)...\n{task.description}"
+            ),
         )
-        for label in labels
-    ]
-
-    page_task = overall_progress.add_task(
-        f" Labels Progress: {page_count}", visible=True
-    )
+        job_progress = Progress("{task.description}")
+        progress_group = Group(overall_progress, Panel(Group(job_progress)))
 
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
+        output = []
+        tasks = []
+        page_count = 0
+        with Live(
+            progress_group, refresh_per_second=5, console=console.get_shared_console()
+        ):
+            async with sessionbuilder.sessionBuilder() as c:
+                [
+                    tasks.append(asyncio.create_task(scrape_list(c, id, job_progress)))
+                    for id in lists
+                ]
+                page_task = overall_progress.add_task(
+                    f"UserList Users Pages Progress: {page_count}", visible=True
+                )
+                while bool(tasks):
+                    new_tasks = []
                     try:
-                        label, new_posts, new_tasks = await task
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task, description=f"Labels Progress: {page_count}"
-                        )
-                        log.debug(
-                            f"[bold]Label {label['name']} new post count with Dupes[/bold] {len(new_posts)} found"
-                        )
-                        new_posts = label_dedupe(new_posts)
-                        log.debug(
-                            f"[bold]Label {label['name']} new post count without Dupes[/bold] {len(new_posts)} found"
-                        )
-                        posts = label_dedupe(
-                            responseDict[label["id"]].get("posts", []) + new_posts
-                        )
-                        responseDict[label["id"]]["posts"] = posts
-                        tasks.extend(new_tasks)
-                    except Exception as E:
+                        async with asyncio.timeout(
+                            constants.getattr("API_TIMEOUT_PER_TASKS")
+                            * max(len(tasks), 2)
+                        ):
+                            for task in asyncio.as_completed(tasks):
+                                try:
+                                    result, new_tasks_batch = await task
+                                    new_tasks.extend(new_tasks_batch)
+                                    page_count = page_count + 1
+                                    overall_progress.update(
+                                        page_task,
+                                        description=f"UserList Users Pages Progress: {page_count}",
+                                    )
+                                    output.extend(result)
+                                except Exception as E:
+                                    log.traceback_(E)
+                                    log.traceback_(traceback.format_exc())
+                                    continue
+                    except TimeoutError as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-    overall_progress.remove_task(page_task)
-    progress_utils.labelled_layout.visible = False
 
+                    tasks = new_tasks
+    overall_progress.remove_task(page_task)
+    outdict = {}
+    for ele in output:
+        outdict[ele["id"]] = ele
     log.trace(
-        "post label joined {posts}".format(
-            posts="\n\n".join(
-                list(
-                    map(
-                        lambda x: f"label post joined: {str(x)}",
-                        list(responseDict.values()),
-                    )
-                )
+        "users found {users}".format(
+            users="\n\n".join(
+                list(map(lambda x: f"user data: {str(x)}", outdict.values()))
             )
         )
     )
-    log.debug(f"[bold]Labels count without Dupes[/bold] {len(responseDict)} found")
-
-    return list(responseDict.values())
+    log.debug(f"[bold]users count without Dupes[/bold] {len(outdict.values())} found")
+    return outdict.values()
 
 
-async def scrape_labelled_posts(c, label, model_id, job_progress=None, offset=0):
+async def scrape_list(c, item, job_progress, offset=0):
     global sem
-    posts = None
+    global tasks
+    users = None
     attempt.set(0)
     async for _ in AsyncRetrying(
         retry=retry_if_not_exception_type(KeyboardInterrupt),
         stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
         wait=wait_random(
             min=constants.getattr("OF_MIN"),
             max=constants.getattr("OF_MAX"),
         ),
         reraise=True,
     ):
         with _:
             new_tasks = []
             await sem.acquire()
-            await asyncio.sleep(1)
             try:
                 attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : getting posts from label -> {label['name']}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
+                task = job_progress.add_task(
+                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : offset -> {offset} + list name -> {item.get('name')}",
+                    visible=True,
                 )
+
                 async with c.requests(
-                    url=constants.getattr("labelledPostsEP").format(
-                        model_id, offset, label["id"]
-                    )
+                    url=constants.getattr("listusersEP").format(item.get("id"), offset)
                 )() as r:
+                    log_id = f"offset:{offset} list:{item.get('name')} =>"
                     if r.ok:
                         data = await r.json_()
-                        posts = list(
-                            filter(lambda x: isinstance(x, list), data.values())
-                        )[0]
+                        users = data.get("list") or []
+                        log.debug(f"{log_id} -> names found {len(users)}")
                         log.debug(
-                            f"offset:{offset} -> labelled posts found {len(posts)}"
+                            f"{log_id}  -> hasMore value in json {data.get('hasMore','undefined') }"
                         )
                         log.debug(
-                            f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
+                            f"usernames {log_id} : usernames retrived -> {list(map(lambda x:x.get('username'),users))}"
                         )
                         log.trace(
-                            "{offset} -> {posts}".format(
+                            "offset: {offset} list: {item} -> {posts}".format(
+                                item=item.get("name"),
                                 offset=offset,
                                 posts="\n\n".join(
                                     list(
                                         map(
-                                            lambda x: f"scrapeinfo label {str(x)}",
-                                            posts,
+                                            lambda x: f"scrapeinfo list {str(x)}", users
                                         )
                                     )
                                 ),
                             )
                         )
-
-                        if data.get("hasMore") and len(posts) > 0:
-                            offset += len(posts)
+                        if (
+                            data.get("hasMore")
+                            and len(users) > 0
+                            and offset != data.get("nextOffset")
+                        ):
+                            offset += len(users)
                             new_tasks.append(
                                 asyncio.create_task(
-                                    scrape_labelled_posts(
-                                        c,
-                                        label,
-                                        model_id,
-                                        job_progress=job_progress,
-                                        offset=offset,
-                                    )
+                                    scrape_list(c, item, job_progress, offset=offset)
                                 )
                             )
 
                     else:
                         log.debug(
                             f"[bold]labelled posts response status code:[/bold]{r.status}"
                         )
                         log.debug(
                             f"[bold]labelled posts response:[/bold] {await r.text_()}"
                         )
                         log.debug(f"[bold]labelled posts headers:[/bold] {r.headers}")
 
                         r.raise_for_status()
             except Exception as E:
-                await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
-
-            return label, posts, new_tasks
-
-
-def label_dedupe(posts):
-    unduped = {}
-    for post in posts:
-        id = post["id"]
-        if unduped.get(id):
-            continue
-        unduped[id] = post
-    return list(unduped.values())
-
-
-def get_default_label_dict(labels):
-    output = {}
-    for label in labels:
-        output[label["id"]] = label
-    return output
+                job_progress.remove_task(task)
+            return users, new_tasks
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/me.py` & `ofscraper-3.9.0.dev9/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/messages.py` & `ofscraper-3.9.0.dev9/ofscraper/api/messages.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,237 +6,143 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import contextvars
 import logging
 import traceback
 
 import arrow
 from tenacity import (
     AsyncRetrying,
-    retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
-import ofscraper.utils.config.data as data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.sems as sems
+import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 sem = None
 
 
 @run
 async def get_messages_progress(model_id, username, forced_after=None, c=None):
     global sem
     sem = sems.get_req_sem()
     global after
 
-    tasks = []
-    responseArray = []
-    page_count = 0
-    # require a min num of posts to be returned
-    min_posts = 40
-    job_progress = progress_utils.messages_progress
-    overall_progress = progress_utils.overall_progress
-
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
     oldmessages = (
-        operations.get_messages_progress_data(model_id=model_id, username=username)
+        await operations.get_messages_post_info(model_id=model_id, username=username)
         if not read_args.retriveArgs().no_cache
         else []
     )
+
     log.trace(
         "oldmessage {posts}".format(
             posts="\n\n".join(
                 list(map(lambda x: f"oldmessages: {str(x)}", oldmessages))
             )
         )
     )
-    oldmessages = list(filter(lambda x: (x.get("date")) != None, oldmessages))
-    log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
-
-    oldmessages = sorted(
-        oldmessages,
-        key=lambda x: arrow.get(x.get("date")).float_timestamp,
-        reverse=True,
-    )
-    oldmessages = [{"date": arrow.now().float_timestamp, "id": None}] + oldmessages
-
     before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
-    after = get_after(model_id, username, forced_after)
+    after = await get_after(model_id, username, forced_after)
 
     log.debug(f"Messages after = {after}")
 
     log.debug(f"Messages before = {before}")
 
-    if after > before:
-        return []
-    if len(oldmessages) <= 2:
-        filteredArray = oldmessages
-    else:
-        i = None
-        j = None
-
-        if before >= oldmessages[1].get("date"):
-            i = 0
-        elif before <= oldmessages[-1].get("date"):
-            i = len(oldmessages) - 2
-        else:
-            i = list(x.get("date") > before for x in oldmessages).index(False) - 1
-
-        if after >= oldmessages[1].get("date"):
-            j = 2
-        elif after < oldmessages[-1].get("date"):
-            j = len(oldmessages)
-        else:
-            temp = list(x.get("date") < after for x in oldmessages)
-            j = temp.index(True) if True in temp else len(oldmessages)
-        j = min(max(i + 2, j), len(oldmessages))
-        i = max(min(j - 2, i), 0)
-        log.debug(f"Messages found i=={i} length=={len(oldmessages)}")
-        log.debug(f"Messages found j=={j} length=={len(oldmessages)}")
-        filteredArray = oldmessages[i:j]
-
     log.info(
         f"""
-Setting initial message scan date for {username} to {arrow.get(after).format('YYYY.MM.DD')}
+Setting initial message scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
 [yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --dupe' to command to force scan of all messages + download/re-download of all files[/yellow]
+[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
 
         """
     )
 
-    IDArray = (
-        list(map(lambda x: x.get("id"), filteredArray))
-        if len(filteredArray) > 0
-        else []
-    )
-    postedAtArray = (
-        list(map(lambda x: x.get("date"), filteredArray))
-        if len(filteredArray) > 0
+    filteredArray = get_filterArray(after, before, oldmessages)
+    splitArrays = get_split_array(filteredArray)
+    tasks = get_tasks(splitArrays, filteredArray, oldmessages, model_id, c)
+    data = await process_tasks(tasks, model_id)
+    progress_utils.messages_layout.visible = False
+    return data
+
+
+@run
+async def get_messages(model_id, username, forced_after=None, c=None):
+    global sem
+    sem = sems.get_req_sem()
+    global after
+
+    oldmessages = (
+        await operations.get_messages_post_info(model_id=model_id, username=username)
+        if not read_args.retriveArgs().no_cache
         else []
     )
-
-    if len(IDArray) <= 2:
-        tasks.append(
-            asyncio.create_task(
-                scrape_messages(c, model_id, job_progress=job_progress, message_id=None)
+    log.trace(
+        "oldmessage {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"oldmessages: {str(x)}", oldmessages))
             )
         )
+    )
 
-    elif len(IDArray) >= min_posts + 1:
-        splitArraysID = [
-            IDArray[i : i + min_posts] for i in range(0, len(IDArray), min_posts)
-        ]
-        splitArraysTime = [
-            postedAtArray[i : i + min_posts]
-            for i in range(0, len(postedAtArray), min_posts)
-        ]
+    before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
+    after = await get_after(model_id, username, forced_after)
 
-        # use the previous split for message_id
-        if i == 0:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_messages(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        message_id=None,
-                        required_ids=set(splitArraysTime[0]),
-                    )
-                )
-            )
-        else:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_messages(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        message_id=splitArraysID[0][0],
-                        required_ids=set(splitArraysTime[0]),
-                    )
-                )
-            )
-        if len(IDArray) >= (min_posts * 2) + 1:
-            [
-                tasks.append(
-                    asyncio.create_task(
-                        scrape_messages(
-                            c,
-                            model_id,
-                            job_progress=job_progress,
-                            required_ids=set(splitArraysTime[i]),
-                            message_id=splitArraysID[i - 1][-1],
-                        )
-                    )
-                )
-                for i in range(1, len(splitArraysID) - 1)
-            ]
-            # keeping grabbing until nothing left
-            tasks.append(
-                asyncio.create_task(
-                    scrape_messages(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        message_id=splitArraysID[-2][-1],
-                    )
-                )
-            )
-        else:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_messages(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        message_id=splitArraysID[-1][-1],
-                    )
-                )
-            )
-    else:
-        tasks.append(
-            asyncio.create_task(
-                scrape_messages(
-                    c,
-                    model_id,
-                    job_progress=job_progress,
-                    message_id=IDArray[0],
-                    required_ids=set(postedAtArray[1:]),
-                )
-            )
-        )
+    log.debug(f"Messages after = {after}")
+
+    log.debug(f"Messages before = {before}")
+
+    log.info(
+        f"""
+Setting initial message scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+[yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
+[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
 
+        """
+    )
+
+    filteredArray = get_filterArray(after, before, oldmessages)
+    splitArrays = get_split_array(filteredArray)
+    with progress_utils.set_up_api_messages():
+        tasks = get_tasks(
+        splitArrays, filteredArray, oldmessages, model_id, c
+    )
+        return await process_tasks(tasks, model_id)
+
+
+async def process_tasks(tasks, model_id):
+    page_count = 0
+    responseArray = []
+    overall_progress = progress_utils.overall_progress
     page_task = overall_progress.add_task(
         f" Message Content Pages Progress: {page_count}", visible=True
     )
 
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         page_count = page_count + 1
                         overall_progress.update(
@@ -250,285 +156,219 @@
                         continue
         except TimeoutError as E:
             cache.set(f"{model_id}_scrape_messages")
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         tasks = new_tasks
     overall_progress.remove_task(page_task)
-    progress_utils.messages_layout.visible = False
 
-    unduped = {}
     log.debug(f"[bold]Messages Count with Dupes[/bold] {len(responseArray)} found")
-
-    for message in responseArray:
-        id = message["id"]
-        if unduped.get(id):
-            continue
-        unduped[id] = message
-
-    log.trace(f"messages dupeset messageids {unduped.keys()}")
     log.trace(
-        "messages raw unduped {posts}".format(
+        "messages raw duped {posts}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo message: {str(x)}", unduped))
+                list(map(lambda x: f"dupedinfo message: {str(x)}", responseArray))
             )
         )
     )
-    set_check(unduped, model_id, after)
-    return list(unduped.values())
+    seen = set()
+    new_posts = [
+        post
+        for post in responseArray
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
 
+    log.debug(f"[bold]Messages Count without Dupes[/bold] {len(responseArray)} found")
 
-@run
-async def get_messages(model_id, username, forced_after=None, c=None):
-    global sem
-    sem = sems.get_req_sem()
-    global after
-    job_progress = None
-    tasks = []
-    responseArray = []
-    # require a min num of posts to be returned
-    min_posts = 40
-
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
-    oldmessages = (
-        operations.get_messages_progress_data(model_id=model_id, username=username)
-        if not read_args.retriveArgs().no_cache
-        else []
-    )
+    log.trace(f"messages messageids {list(map(lambda x:x.get('id'),new_posts))}")
     log.trace(
-        "oldmessage {posts}".format(
+        "messages raw unduped {posts}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"oldmessages: {str(x)}", oldmessages))
+                list(map(lambda x: f"undupedinfo message: {str(x)}", new_posts))
             )
         )
     )
-    oldmessages = list(filter(lambda x: (x.get("date")) != None, oldmessages))
-    log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
+    set_check(new_posts, model_id, after)
+    return new_posts
+
 
+def get_filterArray(after, before, oldmessages):
+    oldmessages = list(filter(lambda x: (x.get("created_at")) != None, oldmessages))
+    log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
     oldmessages = sorted(
         oldmessages,
-        key=lambda x: arrow.get(x.get("date")).float_timestamp,
+        key=lambda x: x.get("created_at"),
         reverse=True,
     )
-    oldmessages = [{"date": arrow.now().float_timestamp, "id": None}] + oldmessages
-
-    before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
-    after = get_after(model_id, username, forced_after)
-
-    log.debug(f"Messages after = {after}")
-
-    log.debug(f"Messages before = {before}")
-
     if after > before:
         return []
-    if len(oldmessages) <= 2:
-        filteredArray = oldmessages
+    elif len(oldmessages) <= 2:
+        return oldmessages
     else:
-        i = None
-        j = None
+        return oldmessages[get_i(oldmessages, before) : get_j(oldmessages, after)]
 
-        if before >= oldmessages[1].get("date"):
-            i = 0
-        elif before <= oldmessages[-1].get("date"):
-            i = len(oldmessages) - 2
-        else:
-            i = list(x.get("date") > before for x in oldmessages).index(False) - 1
-
-        if after >= oldmessages[1].get("date"):
-            j = 2
-        elif after < oldmessages[-1].get("date"):
-            j = len(oldmessages)
-        else:
-            temp = list(x.get("date") < after for x in oldmessages)
-            j = temp.index(True) if True in temp else len(oldmessages)
-        j = min(max(i + 2, j), len(oldmessages))
-        i = max(min(j - 2, i), 0)
-        log.debug(f"Messages found i=={i} length=={len(oldmessages)}")
-        log.debug(f"Messages found j=={j} length=={len(oldmessages)}")
-        filteredArray = oldmessages[i:j]
 
-    log.info(
-        f"""
-Setting initial message scan date for {username} to {arrow.get(after).format('YYYY.MM.DD')}
-[yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --dupe' to command to force scan of all messages + download/re-download of all files[/yellow]
-
-        """
+def get_i(oldmessages, before):
+    """
+    iterate through posts until a date less then or equal
+    to before , set index to -1 this point
+    """
+    if before >= oldmessages[1].get("created_at"):
+        return 0
+    if before <= oldmessages[-1].get("created_at"):
+        return len(oldmessages) - 2
+    # Use a generator expression for efficiency
+    return max(
+        next(
+            index - 1
+            for index, message in enumerate(oldmessages)
+            if message.get("created_at") <= before
+        ),
+        0,
     )
 
-    IDArray = (
-        list(map(lambda x: x.get("id"), filteredArray))
-        if len(filteredArray) > 0
-        else []
-    )
-    postedAtArray = (
-        list(map(lambda x: x.get("date"), filteredArray))
-        if len(filteredArray) > 0
-        else []
+
+def get_j(oldmessages, after):
+    """
+    iterate through posts until a date less then or equal
+    to after , set index to +1 this point
+    """
+    if after >= oldmessages[0].get("created_at"):
+        return 0
+    if after < oldmessages[-1].get("created_at"):
+        return len(oldmessages) - 1
+    return min(
+        next(
+            index + 1
+            for index, message in enumerate(oldmessages)
+            if message.get("created_at") <= after
+        ),
+        len(oldmessages) - 1,
     )
 
-    if len(IDArray) <= 2:
-        tasks.append(
-            asyncio.create_task(
-                scrape_messages(c, model_id, job_progress=job_progress, message_id=None)
-            )
-        )
 
-    elif len(IDArray) >= min_posts + 1:
-        splitArraysID = [
-            IDArray[i : i + min_posts] for i in range(0, len(IDArray), min_posts)
-        ]
-        splitArraysTime = [
-            postedAtArray[i : i + min_posts]
-            for i in range(0, len(postedAtArray), min_posts)
-        ]
+def get_split_array(filteredArray):
+    min_posts = 50
+    return [
+        filteredArray[i : i + min_posts]
+        for i in range(0, len(filteredArray), min_posts)
+    ]
 
-        # use the previous split for message_id
-        if i == 0:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_messages(
-                        c,
-                        model_id,
-                        message_id=None,
-                        required_ids=set(splitArraysTime[0]),
-                    )
+
+def get_tasks(splitArrays, filteredArray, oldmessages, model_id, c):
+    tasks = []
+    job_progress = progress_utils.messages_progress
+
+    if len(splitArrays) > 2:
+        tasks.append(
+            asyncio.create_task(
+                scrape_messages(
+                    c,
+                    model_id,
+                    job_progress=job_progress,
+                    message_id=(
+                        splitArrays[0][0].get("id")
+                        if len(filteredArray) == len(oldmessages)
+                        else None
+                    ),
+                    required_ids=set([ele.get("created_at") for ele in splitArrays[0]]),
                 )
             )
-        else:
+        )
+        [
             tasks.append(
                 asyncio.create_task(
                     scrape_messages(
                         c,
                         model_id,
-                        message_id=splitArraysID[0][0],
-                        required_ids=set(splitArraysTime[0]),
+                        job_progress=job_progress,
+                        message_id=splitArrays[i - 1][-1].get("id"),
+                        required_ids=set(
+                            [ele.get("created_at") for ele in splitArrays[i]]
+                        ),
                     )
                 )
             )
-        if len(IDArray) >= (min_posts * 2) + 1:
-            [
-                tasks.append(
-                    asyncio.create_task(
-                        scrape_messages(
-                            c,
-                            model_id,
-                            required_ids=set(splitArraysTime[i]),
-                            message_id=splitArraysID[i - 1][-1],
-                        )
-                    )
-                )
-                for i in range(1, len(splitArraysID) - 1)
-            ]
-            # keeping grabbing until nothing left
-            tasks.append(
-                asyncio.create_task(
-                    scrape_messages(
-                        c,
-                        model_id,
-                        message_id=splitArraysID[-2][-1],
-                    )
+            for i in range(1, len(splitArrays) - 1)
+        ]
+        # keeping grabbing until nothing left
+        tasks.append(
+            asyncio.create_task(
+                scrape_messages(
+                    c,
+                    model_id,
+                    job_progress=job_progress,
+                    message_id=splitArrays[-2][-1].get("id"),
+                    required_ids=set(
+                        [ele.get("created_at") for ele in splitArrays[-1]]
+                    ),
                 )
             )
-        else:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_messages(
-                        c,
-                        model_id,
-                        message_id=splitArraysID[-1][-1],
-                    )
+        )
+    # use the first split if less then 3
+    elif len(splitArrays) > 0:
+        tasks.append(
+            asyncio.create_task(
+                scrape_messages(
+                    c,
+                    model_id,
+                    job_progress=job_progress,
+                    required_ids=None,
+                    message_id=(
+                        splitArrays[0][0].get("id")
+                        if len(filteredArray) == len(oldmessages)
+                        else None
+                    ),
                 )
             )
+        )
+    # set init message to none
     else:
         tasks.append(
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
-                    message_id=IDArray[0],
-                    required_ids=set(postedAtArray[1:]),
+                    job_progress=job_progress,
+                    message_id=None,
+                    required_ids=None,
                 )
             )
         )
-
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            cache.set(f"{model_id}_scrape_messages")
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-
-    unduped = {}
-    log.debug(f"[bold]Messages Count with Dupes[/bold] {len(responseArray)} found")
-
-    for message in responseArray:
-        id = message["id"]
-        if unduped.get(id):
-            continue
-        unduped[id] = message
-
-    log.trace(f"messages dupeset messageids {unduped.keys()}")
-    log.trace(
-        "messages raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo message: {str(x)}", unduped))
-            )
-        )
-    )
-    set_check(unduped, model_id, after)
-    return list(unduped.values())
+    return tasks
 
 
 def set_check(unduped, model_id, after):
     if not after:
-        newCheck = {}
-        for post in cache.get(f"message_check_{model_id}", default=[]) + list(
-            unduped.values()
-        ):
-            newCheck[post["id"]] = post
+        seen = set()
+        all_posts = [
+            post
+            for post in cache.get(f"message_check_{model_id}", default=[]) + unduped
+            if post["id"] not in seen and not seen.add(post["id"])
+        ]
         cache.set(
             f"message_check_{model_id}",
-            list(newCheck.values()),
+            list(all_posts),
             expire=constants.getattr("DAY_SECONDS"),
         )
         cache.close()
 
 
 async def scrape_messages(
     c, model_id, job_progress=None, message_id=None, required_ids=None
 ) -> list:
     global sem
-    global tasks
     messages = None
     attempt.set(0)
     ep = (
         constants.getattr("messagesNextEP")
         if message_id
         else constants.getattr("messagesEP")
     )
     url = ep.format(model_id, message_id)
-    log.debug(f"{message_id if message_id else 'init'}{url}")
+    log.debug(f"{message_id if message_id else 'init'} {url}")
     async for _ in AsyncRetrying(
         retry=retry_if_not_exception_type(KeyboardInterrupt),
         stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
         wait=wait_random(
             min=constants.getattr("OF_MIN"),
             max=constants.getattr("OF_MAX"),
         ),
@@ -557,18 +397,18 @@
                         if len(messages) == 0:
                             log.debug(f"{log_id} -> number of messages found 0")
                         elif len(messages) > 0:
                             log.debug(
                                 f"{log_id} -> number of messages found {len(messages)}"
                             )
                             log.debug(
-                                f"{log_id} -> first date {messages[-1].get('createdAt') or messages[0].get('postedAt')}"
+                                f"{log_id} -> first date {arrow.get(messages[-1].get('createdAt') or messages[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
                             )
                             log.debug(
-                                f"{log_id} -> last date {messages[-1].get('createdAt') or messages[0].get('postedAt')}"
+                                f"{log_id} -> last date {arrow.get(messages[-1].get('createdAt') or messages[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
                             )
                             log.debug(
                                 f"{log_id} -> found message ids {list(map(lambda x:x.get('id'),messages))}"
                             )
                             log.trace(
                                 "{log_id} -> messages raw {posts}".format(
                                     log_id=log_id,
@@ -636,17 +476,19 @@
             except Exception as E:
                 await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
             finally:
                 sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
+                (
+                    job_progress.remove_task(task)
+                    if job_progress and task != None
+                    else None
+                )
             return messages, new_tasks
 
 
 def get_individual_post(model_id, postid):
     with sessionbuilder.sessionBuilder(
         backend="httpx",
     ) as c:
@@ -660,41 +502,41 @@
                 log.debug(
                     f"[bold]Individual message response status code:[/bold]{r.status}"
                 )
                 log.debug(f"[bold]Individual message  response:[/bold] {r.text_()}")
                 log.debug(f"[bold]Individual message  headers:[/bold] {r.headers}")
 
 
-def get_after(model_id, username, forced_after=None):
+async def get_after(model_id, username, forced_after=None):
     if forced_after != None:
         return forced_after
+    elif not settings.get_after_enabled():
+        return 0
     elif read_args.retriveArgs().after == 0:
         return 0
     elif read_args.retriveArgs().after:
         return read_args.retriveArgs().after.float_timestamp
-    elif (
-        cache.get(f"{model_id}_scrape_messages")
-        and not read_args.retriveArgs().after
-        and not data.get_disable_after()
-    ):
+    elif cache.get(f"{model_id}_scrape_messages"):
         log.debug(
             "Used --after previously. Scraping all messages required to make sure content is not missing"
         )
         return 0
-    curr = operations.get_messages_progress_media(model_id=model_id, username=username)
+    curr = await operations.get_messages_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
-    missing_items = list(filter(lambda x: x[10] != 1, curr))
-    missing_items = list(sorted(missing_items, key=lambda x: arrow.get(x[12])))
+    missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
+    missing_items = list(
+        sorted(missing_items, key=lambda x: arrow.get(x.get("posted_at") or 0))
+    )
     if len(missing_items) == 0:
         log.debug(
             "Using last db date because,all downloads in db are marked as downloaded"
         )
         return arrow.get(
-            operations.get_last_message_date(model_id=model_id, username=username)
+            await operations.get_last_message_date(model_id=model_id, username=username)
         ).float_timestamp
     else:
         log.debug(
             f"Setting date slightly before earliest missing item\nbecause {len(missing_items)} messages in db are marked as undownloaded"
         )
-        return arrow.get(missing_items[0][12]).float_timestamp - 1000
+        return arrow.get(missing_items[0].get("posted_at") or 0).float_timestamp
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/paid.py` & `ofscraper-3.9.0.dev9/ofscraper/api/paid.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,30 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import contextvars
 import logging
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 
 from tenacity import (
     AsyncRetrying,
-    retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.utils.cache as cache
-import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.sems as sems
 from ofscraper.utils.context.run_async import run
 
 paid_content_list_name = "list"
 log = logging.getLogger("shared")
@@ -38,125 +37,109 @@
 sem = None
 
 
 @run
 async def get_paid_posts_progress(username, model_id, c=None):
     global sem
     sem = sems.get_req_sem()
-    responseArray = []
     tasks = []
 
-    page_count = 0
     job_progress = progress_utils.paid_progress
-    overall_progress = progress_utils.overall_progress
     tasks.append(
         asyncio.create_task(scrape_paid(c, username, job_progress=job_progress))
     )
-    page_task = overall_progress.add_task(
-        f"Paid Content Pages Progress: {page_count}", visible=True
-    )
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Paid Content Pages Progress: {page_count}",
-                        )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-    overall_progress.remove_task(page_task)
-    progress_utils.paid_layout.visible = False
+    data = await process_tasks(tasks, model_id)
 
-    outdict = {}
-    for post in responseArray:
-        outdict[post["id"]] = post
-    log.trace(
-        "paid raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo paid: {str(x)}", outdict.values()))
-            )
-        )
-    )
-    set_check(outdict, model_id)
-    return list(outdict.values())
+    progress_utils.paid_layout.visible = False
+    return data
 
 
 @run
 async def get_paid_posts(model_id, username, c=None):
     global sem
     sem = sems.get_req_sem()
-    responseArray = []
     tasks = []
-    job_progress = None
-    page_count = 0
 
     # async with c or sessionbuilder.sessionBuilder(
     #     limit=constants.getattr("API_MAX_CONNECTION")
     # ) as c:
-    tasks.append(
-        asyncio.create_task(scrape_paid(c, username, job_progress=job_progress))
+    with progress_utils.set_up_api_paid():
+        job_progress = progress_utils.paid_progress
+        tasks.append(
+            asyncio.create_task(scrape_paid(c, username, job_progress=job_progress))
+        )
+        return await process_tasks(tasks, model_id)
+
+
+async def process_tasks(tasks, model_id):
+    page_count = 0
+    overall_progress = progress_utils.overall_progress
+    page_task = overall_progress.add_task(
+        f"Paid Content Pages Progress: {page_count}", visible=True
     )
+    responseArray = []
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         page_count = page_count + 1
+                        overall_progress.update(
+                            page_task,
+                            description=f"Paid Content Pages Progress: {page_count}",
+                        )
                         responseArray.extend(result)
                     except Exception as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
                         continue
         except TimeoutError as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         tasks = new_tasks
-    outdict = {}
-    for post in responseArray:
-        outdict[post["id"]] = post
+    overall_progress.remove_task(page_task)
+    log.debug(f"[bold]Paid Count with Dupes[/bold] {len(responseArray)} found")
+
+    seen = set()
+    new_posts = [
+        post
+        for post in responseArray
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
+
+    log.trace(f"paid postids {list(map(lambda x:x.get('id'),new_posts))}")
+
     log.trace(
         "paid raw unduped {posts}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo paid: {str(x)}", outdict.values()))
+                list(map(lambda x: f"undupedinfo paid: {str(x)}", new_posts))
             )
         )
     )
-    set_check(outdict, model_id)
-    return list(outdict.values())
+    log.debug(f"[bold]Paid Count without Dupes[/bold] {len(new_posts)} found")
+
+    set_check(new_posts, model_id)
+    return new_posts
 
 
 def set_check(unduped, model_id):
-    newCheck = {}
-    for post in cache.get(f"purchased_check_{model_id}", default=[]) + list(
-        unduped.values()
-    ):
-        newCheck[post["id"]] = post
+    seen = set()
+    all_posts = [
+        post
+        for post in cache.get(f"purchase_check_{model_id}", default=[]) + unduped
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
     cache.set(
         f"purchased_check_{model_id}",
-        list(newCheck.values()),
+        all_posts,
         expire=constants.getattr("DAY_SECONDS"),
     )
     cache.close()
 
 
 @run
 async def scrape_paid(c, username, job_progress=None, offset=0):
@@ -221,17 +204,19 @@
                             new_tasks.append(
                                 asyncio.create_task(
                                     scrape_paid(
                                         c, username, job_progress, offset=offset
                                     )
                                 )
                             )
-                        job_progress.remove_task(
-                            task
-                        ) if task and job_progress else None
+                        (
+                            job_progress.remove_task(task)
+                            if task and job_progress
+                            else None
+                        )
 
                     else:
                         log.debug(f"[bold]paid response status code:[/bold]{r.status}")
                         log.debug(f"[bold]paid response:[/bold] {await r.text_()}")
                         log.debug(f"[bold]paid headers:[/bold] {r.headers}")
                         job_progress.remove_task(task)
                         r.raise_for_status()
@@ -262,15 +247,15 @@
         tasks = []
         page_count = 0
         with progress_utils.setup_all_paid_live():
             job_progress = progress_utils.all_paid_progress
             overall_progress = progress_utils.overall_progress
 
             async with sessionbuilder.sessionBuilder() as c:
-                allpaid = cache.get(f"purchased_all", default=[])
+                allpaid = cache.get("purchased_all", default=[])
                 log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
 
                 if len(allpaid) > min_posts:
                     splitArrays = [i for i in range(0, len(allpaid), min_posts)]
                     # use the previous split for timesamp
                     tasks.append(
                         asyncio.create_task(
@@ -323,23 +308,41 @@
                             await asyncio.sleep(1)
                         except Exception as E:
                             await asyncio.sleep(1)
                             log.debug(E)
                             continue
 
                 overall_progress.remove_task(page_task)
-        outdict = {}
-        log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
-        for post in output:
-            outdict[post["id"]] = post
 
-        log.debug(f"[bold]Paid Post count[/bold] {len(outdict.values())} found")
+        log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
+        log.trace(
+            "paid raw duped {posts}".format(
+                posts="\n\n".join(
+                    list(map(lambda x: f"dupedinfo all paid: {str(x)}", output))
+                )
+            )
+        )
+        seen = set()
+        new_posts = [
+            post
+            for post in output
+            if post["id"] not in seen and not seen.add(post["id"])
+        ]
+        log.trace(f"all paid postids {list(map(lambda x:x.get('id'),new_posts))}")
+        log.debug(f"[bold]Paid Post count without Dupes[/bold] {len(new_posts)} found")
+        log.trace(
+            "paid raw duped {posts}".format(
+                posts="\n\n".join(
+                    list(map(lambda x: f"undupedinfo all paid: {str(x)}", new_posts))
+                )
+            )
+        )
         cache.set(
-            f"purchased_all",
-            list(map(lambda x: x.get("id"), list(outdict.values()))),
+            "purchased_all",
+            list(map(lambda x: x.get("id"), list())),
             expire=constants.getattr("RESPONSE_EXPIRY"),
         )
         cache.close()
         # filter at user level
         return output
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/pinned.py` & `ofscraper-3.9.0.dev9/ofscraper/api/pinned.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,73 +2,103 @@
                                                              
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
+
 import asyncio
 import contextvars
 import logging
 import math
 import traceback
 
 import arrow
 from tenacity import (
     AsyncRetrying,
-    retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.utils.args.read as read_args
+import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 sem = None
 
 
 @run
-async def get_pinned_post(model_id, c=None):
+async def get_pinned_posts_progress(model_id, c=None):
     tasks = []
-    responseArray = []
-    page_count = 0
     job_progress = progress_utils.pinned_progress
-    overall_progress = progress_utils.overall_progress
 
     # async with sessionbuilder.sessionBuilder(
     #     limit=constants.getattr("API_MAX_CONNECTION")
     # ) as c:
     tasks.append(
         asyncio.create_task(
             scrape_pinned_posts(
                 c,
                 model_id,
                 job_progress=job_progress,
-                timestamp=read_args.retriveArgs().after.float_timestamp
-                if read_args.retriveArgs().after
-                else None,
+                timestamp=(
+                    read_args.retriveArgs().after.float_timestamp
+                    if read_args.retriveArgs().after
+                    else None
+                ),
             )
         )
     )
+    data = await process_tasks(tasks, model_id)
+    progress_utils.pinned_layout.visible = False
+    return data
+
+
+@run
+async def get_pinned_posts(model_id, c=None):
+    tasks = []
+    with progress_utils.set_up_api_pinned():
+
+        tasks.append(
+            asyncio.create_task(
+                scrape_pinned_posts(
+                    c,
+                    model_id,
+                    job_progress=progress_utils.pinned_progress,
+                    timestamp=(
+                        read_args.retriveArgs().after.float_timestamp
+                        if read_args.retriveArgs().after
+                        else None
+                    ),
+                )
+            )
+        )
+    return await process_tasks(tasks, model_id)
+
+
+async def process_tasks(tasks, model_id):
+    responseArray = []
+    page_count = 0
+    overall_progress = progress_utils.overall_progress
 
     page_task = overall_progress.add_task(
         f"Pinned Content Pages Progress: {page_count}", visible=True
     )
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         page_count = page_count + 1
                         overall_progress.update(
@@ -81,29 +111,56 @@
                         log.traceback_(traceback.format_exc())
                         continue
         except TimeoutError as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         tasks = new_tasks
     overall_progress.remove_task(page_task)
-    progress_utils.pinned_layout.visible = False
-    outdict = {}
     log.debug(f"[bold]Pinned Count with Dupes[/bold] {len(responseArray)} found")
-    for post in responseArray:
-        outdict[post["id"]] = post
-    log.trace(f"pinned dupeset postids {outdict.keys()}")
+    log.trace(
+        "pinned raw duped {posts}".format(
+            posts="\n\n".join(
+                list(map(lambda x: f"dupedinfo pinned: {str(x)}", responseArray))
+            )
+        )
+    )
+    seen = set()
+    new_posts = [
+        post
+        for post in responseArray
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
+
+    log.trace(f"pinned postids{list(map(lambda x:x.get('id'),new_posts))}")
     log.trace(
         "pinned raw unduped {posts}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo pinned: {str(x)}", outdict.values()))
+                list(map(lambda x: f"undupedinfo pinned: {str(x)}", new_posts))
             )
         )
     )
-    log.debug(f"[bold]Pinned Count without Dupes[/bold] {len(outdict.values())} found")
-    return list(outdict.values())
+    log.debug(f"[bold]Pinned Count without Dupes[/bold] {len(new_posts)} found")
+    set_check(new_posts, model_id)
+    return new_posts
+
+
+def set_check(unduped, model_id):
+    if not read_args.retriveArgs().after:
+        seen = set()
+        all_posts = [
+            post
+            for post in cache.get(f"pinned_check_{model_id}", default=[]) + unduped
+            if post["id"] not in seen and not seen.add(post["id"])
+        ]
+        cache.set(
+            f"pinned_check_{model_id}",
+            all_posts,
+            expire=constants.getattr("DAY_SECONDS"),
+        )
+        cache.close()
 
 
 async def scrape_pinned_posts(
     c, model_id, job_progress=None, timestamp=None, count=0
 ) -> list:
     global sem
     sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
@@ -129,32 +186,36 @@
     ):
         with _:
             new_tasks = []
             await sem.acquire()
             await asyncio.sleep(1)
             try:
                 attempt.set(attempt.get(0) + 1)
-                task = job_progress.add_task(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",
-                    visible=True,
+                task = (
+                    job_progress.add_task(
+                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
+                        visible=True,
+                    )
+                    if job_progress
+                    else None
                 )
                 async with c.requests(url=url)() as r:
                     if r.ok:
                         posts = (await r.json_())["list"]
                         posts = list(
                             sorted(posts, key=lambda x: float(x["postedAtPrecise"]))
                         )
                         posts = list(
                             filter(
                                 lambda x: float(x["postedAtPrecise"])
                                 > float(timestamp or 0),
                                 posts,
                             )
                         )
-                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
+                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
                         if not posts:
                             posts = []
                         if len(posts) == 0:
                             log.debug(f"{log_id} -> number of pinned post found 0")
                         else:
                             log.debug(
                                 f"{log_id} -> number of pinned post found {len(posts)}"
@@ -189,23 +250,21 @@
                                         job_progress=job_progress,
                                         timestamp=posts[-1]["postedAtPrecise"],
                                         count=count + len(posts),
                                     )
                                 )
                             )
                     else:
-                        log.debug(
-                            f"[bold]timeline response status code:[/bold]{r.status}"
-                        )
-                        log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
+                        log.debug(f"[bold]t response status code:[/bold]{r.status}")
+                        log.debug(f"[bold]pinned response:[/bold] {await r.text_()}")
+                        log.debug(f"[bold]pinned headers:[/bold] {r.headers}")
                         r.raise_for_status()
             except Exception as E:
                 await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(task)
+                job_progress.remove_task(task) if job_progress and task else None
             return posts, new_tasks
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/profile.py` & `ofscraper-3.9.0.dev9/ofscraper/api/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import contextvars
 import logging
 import traceback
 from typing import Union
 
 from rich.console import Console
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/individual.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 log = logging.getLogger("shared")
 
 
 @run
 async def get_subscription(accounts=None):
     global sem
     sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
-    accounts = accounts or read_args.retriveArgs().username
+    accounts = accounts or read_args.retriveArgs().usernames
     if not isinstance(accounts, list) and not isinstance(accounts, set):
         accounts = set([accounts])
     with ThreadPoolExecutor(
         max_workers=constants.getattr("MAX_REQUEST_WORKERS")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.0.dev9/ofscraper/api/labels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,365 +1,471 @@
 r"""
-                                                             
+                                                      o       
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import contextvars
 import logging
 import traceback
-from concurrent.futures import ThreadPoolExecutor
 
-from rich.console import Group
-from rich.live import Live
-from rich.panel import Panel
-from rich.progress import Progress, SpinnerColumn, TextColumn
-from rich.style import Style
 from tenacity import (
     AsyncRetrying,
-    retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
-import ofscraper.utils.args.read as read_args
-import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
+import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.sems as sems
+import ofscraper.utils.args.read as read_args
 from ofscraper.utils.context.run_async import run
+import ofscraper.utils.cache as cache
+
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 sem = None
 
-
 @run
-async def get_otherlist():
-    out = []
-    if any(
-        [
-            ele
-            not in [
-                constants.getattr("OFSCRAPER_RESERVED_LIST"),
-                constants.getattr("OFSCRAPER_RESERVED_LIST_ALT"),
-            ]
-            for ele in read_args.retriveArgs().user_list
-        ]
-    ):
-        out.extend(await get_lists())
-    out = list(
-        filter(
-            lambda x: x.get("name").lower() in read_args.retriveArgs().user_list,
-            out,
+async def get_labels_progress(model_id, c=None):
+    labels_ = await get_labels_data_progress(model_id, c=c)
+    labels_ = (
+        labels_
+        if not read_args.retriveArgs().label
+        else list(
+            filter(
+                lambda x: x.get("name").lower()
+                in read_args.retriveArgs().label,
+                labels_,
+            )
         )
     )
-    log.debug(
-        f"User lists found on profile {list(map(lambda x:x.get('name').lower(),out))}"
+    return await get_posts_for_labels_progress(
+                labels_, model_id, c=c
+     )
+@run
+async def get_labels_data_progress(model_id, c=None):
+    global sem
+    sem = sems.get_req_sem()
+    tasks = []
+    tasks.append(
+        asyncio.create_task(
+            scrape_labels(c, model_id, job_progress=progress_utils.labelled_progress)
+        )
     )
-    return await get_list_users(out)
+    progress_utils.labelled_layout.visible = False
+    return await process_tasks_labels(tasks)
+@run
+async def get_posts_for_labels_progress(labels, model_id, c=None):
+    global sem
+    sem = sems.get_req_sem()
+    tasks = []
+
+    [
+        tasks.append(
+            asyncio.create_task(
+                scrape_posts_labels(c, label, model_id, job_progress= progress_utils.labelled_progress)
+            )
+        )
+        for label in labels
+    ]
+    labels_final=await process_tasks_get_posts_for_labels(tasks,labels,model_id)
+    progress_utils.labelled_layout.visible = False
+    return labels_final
 
 
 @run
-async def get_blacklist():
-    out = []
-    if len(read_args.retriveArgs().black_list) >= 1:
-        out.extend(await get_lists())
-    out = list(
-        filter(
-            lambda x: x.get("name").lower() in read_args.retriveArgs().black_list,
-            out,
+async def get_labels(model_id, c=None):
+    labels_ = await get_labels_data(model_id, c=c)
+    labels_ = (
+        labels_
+        if not read_args.retriveArgs().label
+        else list(
+            filter(
+                lambda x: x.get("name").lower()
+                in read_args.retriveArgs().label,
+                labels_,
+            )
         )
     )
-    log.debug(
-        f"Black lists found on profile {list(map(lambda x:x.get('name').lower(),out))}"
-    )
-    names = list(await get_list_users(out))
-    return set(list(map(lambda x: x["id"], names)))
-
-
-async def get_lists():
-    with ThreadPoolExecutor(
-        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
-    ) as executor:
-        asyncio.get_event_loop().set_default_executor(executor)
-        overall_progress = Progress(
-            SpinnerColumn(style=Style(color="blue")),
-            TextColumn("Getting lists...\n{task.description}"),
+    return await get_posts_for_labels(
+                labels_, model_id, c=c
+     )
+@run
+async def get_labels_data(model_id, c=None):
+    global sem
+    sem = sems.get_req_sem()
+    with progress_utils.set_up_api_labels():
+        tasks = []
+        tasks.append(
+            asyncio.create_task(
+                scrape_labels(c, model_id, job_progress=progress_utils.labelled_progress)
+            )
         )
-        job_progress = Progress("{task.description}")
-        progress_group = Group(overall_progress, Panel(Group(job_progress)))
+        return await process_tasks_labels(tasks)
 
-        output = []
+@run
+async def get_posts_for_labels(labels, model_id, c=None):
+    global sem
+    sem = sems.get_req_sem()
+    with progress_utils.set_up_api_posts_labels():
         tasks = []
-        page_count = 0
-        with Live(
-            progress_group, refresh_per_second=5, console=console.get_shared_console()
-        ):
-            async with sessionbuilder.sessionBuilder() as c:
-                tasks.append(asyncio.create_task(scrape_lists(c, job_progress)))
-                page_task = overall_progress.add_task(
-                    f"UserList Pages Progress: {page_count}", visible=True
+        [
+            tasks.append(
+                asyncio.create_task(
+                    scrape_posts_labels(c, label, model_id, job_progress= progress_utils.labelled_progress)
                 )
-                while bool(tasks):
-                    new_tasks = []
+            )
+            for label in labels
+        ]
+        return await process_tasks_get_posts_for_labels(tasks,labels,model_id)
+
+async def process_tasks_labels(tasks):
+    responseArray = []
+
+    page_count = 0
+    overall_progress = progress_utils.overall_progress
+
+    page_task = overall_progress.add_task(
+        f"Label Names Pages Progress: {page_count}", visible=True
+    )
+    while bool(tasks):
+        new_tasks = []
+        try:
+            async with asyncio.timeout(
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
+            ):
+                for task in asyncio.as_completed(tasks):
                     try:
-                        async with asyncio.timeout(
-                            constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-                        ):
-                            for task in asyncio.as_completed(tasks):
-                                try:
-                                    result, new_tasks_batch = await task
-                                    new_tasks.extend(new_tasks_batch)
-                                    page_count = page_count + 1
-                                    overall_progress.update(
-                                        page_task,
-                                        description=f"UserList Pages Progress: {page_count}",
-                                    )
-                                    output.extend(result)
-                                except Exception as E:
-                                    log.traceback_(E)
-                                    log.traceback_(traceback.format_exc())
-                                    continue
-                    except TimeoutError as E:
+                        result, new_tasks_batch = await task
+                        new_tasks.extend(new_tasks_batch)
+                        page_count = page_count + 1
+                        overall_progress.update(
+                            page_task,
+                            description=f"Label Names Pages Progress: {page_count}",
+                        )
+                        responseArray.extend(result)
+                    except Exception as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
-                    tasks = new_tasks
-
-        overall_progress.remove_task(page_task)
-        log.trace(
-            "list unduped {posts}".format(
-                posts="\n\n".join(map(lambda x: f" list data raw:{x}", output))
-            )
+                        continue
+            tasks = new_tasks
+        except TimeoutError as E:
+            log.traceback_(E)
+            log.traceback_(traceback.format_exc())
+    overall_progress.remove_task(page_task)
+    log.trace(
+        "post label names unduped {posts}".format(
+            posts="\n\n".join(map(lambda x: f" label name unduped:{x}", responseArray))
         )
-        log.debug(f"[bold]lists name count without Dupes[/bold] {len(output)} found")
-        return output
-
+    )
+    log.debug(
+        f"[bold]Labels name count without Dupes[/bold] {len(responseArray)} found"
+    )
+    return responseArray
 
-async def scrape_lists(c, job_progress, offset=0):
+ 
+async def scrape_labels(c, model_id, job_progress=None, offset=0):
     global sem
-    global tasks
-    sem = sems.get_req_sem()
+    labels = None
     attempt.set(0)
     async for _ in AsyncRetrying(
         stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
         retry=retry_if_not_exception_type(KeyboardInterrupt),
         wait=wait_random(
             min=constants.getattr("OF_MIN"),
             max=constants.getattr("OF_MAX"),
         ),
         reraise=True,
     ):
         with _:
             new_tasks = []
             await sem.acquire()
+            await asyncio.sleep(1)
             try:
                 attempt.set(attempt.get(0) + 1)
-                task = job_progress.add_task(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : getting lists offset -> {offset}",
-                    visible=True,
+
+                task = (
+                    job_progress.add_task(
+                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} labels offset -> {offset}",
+                        visible=True,
+                    )
+                    if job_progress
+                    else None
                 )
                 async with c.requests(
-                    url=constants.getattr("listEP").format(offset)
+                    url=constants.getattr("labelsEP").format(model_id, offset)
                 )() as r:
                     if r.ok:
                         data = await r.json_()
-                        out_list = data["list"] or []
+                        labels = list(
+                            filter(lambda x: isinstance(x, list), data.values())
+                        )[0]
                         log.debug(
-                            f"offset:{offset} -> lists names found {list(map(lambda x:x['name'],out_list))}"
-                        )
-                        log.debug(
-                            f"offset:{offset} -> number of lists found {len(out_list)}"
+                            f"offset:{offset} -> labels names found {len(labels)}"
                         )
                         log.debug(
                             f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
                         )
                         log.trace(
                             "offset:{offset} -> label names raw: {posts}".format(
                                 offset=offset, posts=data
                             )
                         )
 
-                        if data.get("hasMore") and len(out_list) > 0:
-                            offset = offset + len(out_list)
+                        if (
+                            data.get("hasMore")
+                            and len(data.get("list")) > 0
+                            and data.get("nextOffset") != offset
+                        ):
+                            offset = offset + len(data.get("list"))
                             new_tasks.append(
                                 asyncio.create_task(
-                                    scrape_lists(c, job_progress, offset=offset)
+                                    scrape_labels(
+                                        c,
+                                        model_id,
+                                        job_progress=job_progress,
+                                        offset=offset,
+                                    )
                                 )
                             )
+                        return data.get("list"), new_tasks
 
                     else:
-                        log.debug(f"[bold]lists response status code:[/bold]{r.status}")
-                        log.debug(f"[bold]lists response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]lists headers:[/bold] {r.headers}")
+                        log.debug(
+                            f"[bold]labels response status code:[/bold]{r.status}"
+                        )
+                        log.debug(f"[bold]labels response:[/bold] {await r.text_()}")
+                        log.debug(f"[bold]labels headers:[/bold] {r.headers}")
                         r.raise_for_status()
             except Exception as E:
+                await asyncio.sleep(1)
+
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(task)
-            return out_list, new_tasks
+                (
+                    job_progress.remove_task(task)
+                    if job_progress and task != None
+                    else None
+                )
 
 
-async def get_list_users(lists):
-    global sem
-    sem = sems.get_req_sem()
-    with ThreadPoolExecutor(
-        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
-    ) as executor:
-        asyncio.get_event_loop().set_default_executor(executor)
-        overall_progress = Progress(
-            SpinnerColumn(style=Style(color="blue")),
-            TextColumn(
-                "Getting users from lists (this may take awhile)...\n{task.description}"
-            ),
-        )
-        job_progress = Progress("{task.description}")
-        progress_group = Group(overall_progress, Panel(Group(job_progress)))
+async def process_tasks_get_posts_for_labels(tasks,labels,model_id):
+    responseDict =get_default_label_dict(labels)
 
-        output = []
-        tasks = []
-        page_count = 0
-        with Live(
-            progress_group, refresh_per_second=5, console=console.get_shared_console()
-        ):
-            async with sessionbuilder.sessionBuilder() as c:
-                [
-                    tasks.append(asyncio.create_task(scrape_list(c, id, job_progress)))
-                    for id in lists
-                ]
-                page_task = overall_progress.add_task(
-                    f"UserList Users Pages Progress: {page_count}", visible=True
-                )
-                while bool(tasks):
-                    new_tasks = []
+    page_count = 0
+    overall_progress = progress_utils.overall_progress
+
+    page_task = overall_progress.add_task(
+        f" Labels Progress: {page_count}", visible=True
+    )
+
+    while bool(tasks):
+
+        new_tasks = []
+        try:
+            async with asyncio.timeout(
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
+            ):
+                for task in asyncio.as_completed(tasks):
                     try:
-                        async with asyncio.timeout(
-                            constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-                        ):
-                            for task in asyncio.as_completed(tasks):
-                                try:
-                                    result, new_tasks_batch = await task
-                                    new_tasks.extend(new_tasks_batch)
-                                    page_count = page_count + 1
-                                    overall_progress.update(
-                                        page_task,
-                                        description=f"UserList Users Pages Progress: {page_count}",
+                        label, new_posts, new_tasks = await task
+                        page_count = page_count + 1
+                        overall_progress.update(
+                            page_task, description=f"Labels Progress: {page_count}"
+                        )
+                        log.debug(
+                            f"[bold]Label {label['name']} new post count with Dupes[/bold] {len(new_posts)} found"
+                        )
+                        new_posts = label_dedupe(new_posts)
+                        log.trace(
+                            f"{label['name']} postids {list(map(lambda x:x.get('id'),new_posts))}"
+                        )
+                        log.trace(
+                            f"{label['name']} post raw unduped {{posts}}".format(
+                                posts="\n\n".join(
+                                    list(
+                                        map(
+                                            lambda x: f"undupedinfo label: {str(x)}",
+                                            new_posts,
+                                        )
                                     )
-                                    output.extend(result)
-                                except Exception as E:
-                                    log.traceback_(E)
-                                    log.traceback_(traceback.format_exc())
-                                    continue
-                    except TimeoutError as E:
+                                )
+                            )
+                        )
+
+                        log.debug(
+                            f"[bold]Label {label['name']} new post count without Dupes[/bold] {len(new_posts)} found"
+                        )
+                        posts = label_dedupe(
+                            responseDict[label["id"]].get("posts", []) + new_posts
+                        )
+                        responseDict[label["id"]]["posts"] = posts
+                        tasks.extend(new_tasks)
+                    except Exception as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
-
-                    tasks = new_tasks
-    overall_progress.remove_task(page_task)
-    outdict = {}
-    for ele in output:
-        outdict[ele["id"]] = ele
+                        continue
+        except TimeoutError as E:
+            log.traceback_(E)
+            log.traceback_(traceback.format_exc())
+        tasks = new_tasks
+    labels=list(responseDict.values())
+    set_check(labels, model_id)
     log.trace(
-        "users found {users}".format(
-            users="\n\n".join(
-                list(map(lambda x: f"user data: {str(x)}", outdict.values()))
+        "post label joined {posts}".format(
+            posts="\n\n".join(
+                list(
+                    map(
+                        lambda x: f"label post joined: {str(x)}",
+                        list(),
+                    )
+                )
             )
         )
     )
-    log.debug(f"[bold]users count without Dupes[/bold] {len(outdict.values())} found")
-    return outdict.values()
-
+    log.debug(f"[bold]Labels count without Dupes[/bold] {len(labels)} found")
+    overall_progress.remove_task(page_task)
+    return labels
 
-async def scrape_list(c, item, job_progress, offset=0):
+async def scrape_posts_labels(c, label, model_id, job_progress=None, offset=0):
     global sem
-    global tasks
-    users = None
+    posts = None
     attempt.set(0)
     async for _ in AsyncRetrying(
         retry=retry_if_not_exception_type(KeyboardInterrupt),
         stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
         wait=wait_random(
             min=constants.getattr("OF_MIN"),
             max=constants.getattr("OF_MAX"),
         ),
         reraise=True,
     ):
         with _:
             new_tasks = []
             await sem.acquire()
+            await asyncio.sleep(1)
             try:
                 attempt.set(attempt.get(0) + 1)
-                task = job_progress.add_task(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : offset -> {offset} + list name -> {item.get('name')}",
-                    visible=True,
+                task = (
+                    job_progress.add_task(
+                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : getting posts from label -> {label['name']}",
+                        visible=True,
+                    )
+                    if job_progress
+                    else None
                 )
-
                 async with c.requests(
-                    url=constants.getattr("listusersEP").format(item.get("id"), offset)
+                    url=constants.getattr("labelledPostsEP").format(
+                        model_id, offset, label["id"]
+                    )
                 )() as r:
-                    log_id = f"offset:{offset} list:{item.get('name')} =>"
                     if r.ok:
                         data = await r.json_()
-                        users = data.get("list") or []
-                        log.debug(f"{log_id} -> names found {len(users)}")
+                        posts = list(
+                            filter(lambda x: isinstance(x, list), data.values())
+                        )[0]
                         log.debug(
-                            f"{log_id}  -> hasMore value in json {data.get('hasMore','undefined') }"
+                            f"offset:{offset} -> labelled posts found {len(posts)}"
                         )
                         log.debug(
-                            f"usernames {log_id} : usernames retrived -> {list(map(lambda x:x.get('username'),users))}"
+                            f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
                         )
                         log.trace(
-                            "offset: {offset} list: {item} -> {posts}".format(
-                                item=item.get("name"),
+                            "{offset} -> {posts}".format(
                                 offset=offset,
                                 posts="\n\n".join(
                                     list(
                                         map(
-                                            lambda x: f"scrapeinfo list {str(x)}", users
+                                            lambda x: f"scrapeinfo label {str(x)}",
+                                            posts,
                                         )
                                     )
                                 ),
                             )
                         )
-                        if (
-                            data.get("hasMore")
-                            and len(users) > 0
-                            and offset != data.get("nextOffset")
-                        ):
-                            offset += len(users)
+
+                        if data.get("hasMore") and len(posts) > 0:
+                            offset += len(posts)
                             new_tasks.append(
                                 asyncio.create_task(
-                                    scrape_list(c, item, job_progress, offset=offset)
+                                    scrape_posts_labels(
+                                        c,
+                                        label,
+                                        model_id,
+                                        job_progress=job_progress,
+                                        offset=offset,
+                                    )
                                 )
                             )
 
                     else:
                         log.debug(
                             f"[bold]labelled posts response status code:[/bold]{r.status}"
                         )
                         log.debug(
                             f"[bold]labelled posts response:[/bold] {await r.text_()}"
                         )
                         log.debug(f"[bold]labelled posts headers:[/bold] {r.headers}")
 
                         r.raise_for_status()
             except Exception as E:
+                await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
 
             finally:
                 sem.release()
-                job_progress.remove_task(task)
-            return users, new_tasks
+                (
+                    job_progress.remove_task(task)
+                    if job_progress and task != None
+                    else None
+                )
+
+            return label, posts, new_tasks
+
+
+def label_dedupe(labelArray):
+    seen = set()
+    new_posts = [
+        post
+        for post in labelArray
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
+    return new_posts
+
+
+def get_default_label_dict(labels):
+    output = {}
+    for label in labels:
+        output[label["id"]] = label
+    return output
+
+def set_check(unduped, model_id):
+    seen = set()
+    new_posts = [post for label in unduped for post in label["posts"]]
+    all_posts = [
+        post
+        for post in cache.get(f"labels_check_{model_id}", default=[]) + new_posts
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
+    cache.set(
+        f"labels_check_{model_id}",
+        all_posts,
+        expire=constants.getattr("DAY_SECONDS"),
+    )
+    cache.close()
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         for offset in range(0, subscribe_count + 1, 10)
     ]
     tasks.extend([asyncio.create_task(funct(c, subscribe_count + 1, recur=True))])
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         output.extend(result)
                     except Exception as E:
@@ -166,15 +166,15 @@
     ]
     tasks.extend([asyncio.create_task(funct(c, subscribe_count + 1, recur=True))])
 
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         output.extend(result)
                     except Exception as E:
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/api/timeline.py` & `ofscraper-3.9.0.dev9/ofscraper/api/archive.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,529 +2,414 @@
                                                              
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
+
 import asyncio
 import contextvars
 import logging
 import math
-import queue
 import traceback
-from multiprocessing import Value
 
 import arrow
 from tenacity import (
     AsyncRetrying,
-    retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random,
 )
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
-import ofscraper.utils.config.data as data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-import ofscraper.utils.sems as sems
+import ofscraper.utils.settings as settings
+from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
-sem = None
 
 
-async def scrape_timeline_posts(
-    c, model_id, job_progress=None, timestamp=None, required_ids=None
-) -> list:
-    posts = None
-    attempt.set(0)
+sem = None
 
-    if timestamp and (
-        float(timestamp)
-        > (read_args.retriveArgs().before or arrow.now()).float_timestamp
-    ):
-        return [], new_tasks
-    if timestamp:
-        log.debug(arrow.get(math.trunc(float(timestamp))))
-        ep = constants.getattr("timelineNextEP")
-        url = ep.format(model_id, str(timestamp))
-    else:
-        ep = constants.getattr("timelineEP")
-        url = ep.format(model_id)
-    log.debug(url)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            await sem.acquire()
-            await asyncio.sleep(1)
-            new_tasks = []
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
-                )
 
-                async with c.requests(url=url)() as r:
-                    if r.ok:
-                        posts = (await r.json_())["list"]
-                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
-                        if not posts:
-                            posts = []
-                        if len(posts) == 0:
-                            log.debug(f"{log_id} -> number of post found 0")
+@run
+async def get_archived_posts_progress(model_id, username, forced_after=None, c=None):
 
-                        elif len(posts) > 0:
-                            log.debug(f"{log_id} -> number of post found {len(posts)}")
-                            log.debug(
-                                f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> found postids {list(map(lambda x:x.get('id'),posts))}"
-                            )
-                            log.trace(
-                                "{log_id} -> post raw {posts}".format(
-                                    log_id=log_id,
-                                    posts="\n\n".join(
-                                        list(
-                                            map(
-                                                lambda x: f"scrapeinfo timeline: {str(x)}",
-                                                posts,
-                                            )
-                                        )
-                                    ),
-                                )
-                            )
-                            if required_ids == None:
-                                new_tasks.append(
-                                    asyncio.create_task(
-                                        scrape_timeline_posts(
-                                            c,
-                                            model_id,
-                                            job_progress=job_progress,
-                                            timestamp=posts[-1]["postedAtPrecise"],
-                                        )
-                                    )
-                                )
-                            else:
-                                [
-                                    required_ids.discard(float(ele["postedAtPrecise"]))
-                                    for ele in posts
-                                ]
-                                if len(required_ids) > 0 and float(
-                                    (timestamp) or 0
-                                ) <= max(required_ids):
-                                    new_tasks.append(
-                                        asyncio.create_task(
-                                            scrape_timeline_posts(
-                                                c,
-                                                model_id,
-                                                job_progress=job_progress,
-                                                timestamp=posts[-1]["postedAtPrecise"],
-                                                required_ids=required_ids,
-                                            )
-                                        )
-                                    )
-                    else:
-                        log.debug(
-                            f"[bold]timeline response status code:[/bold]{r.status}"
-                        )
-                        log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    oldarchived = (
+        await operations.get_archived_postinfo(model_id=model_id, username=username)
+        if not read_args.retriveArgs().no_cache
+        else []
+    )
 
-            finally:
-                sem.release()
-                job_progress.remove_task(
-                    task
-                ) if job_progress and task != None else None
-            return posts, new_tasks
+    log.trace(
+        "oldarchive {posts}".format(
+            posts="\n\n".join(list(map(lambda x: f"oldarchive: {str(x)}", oldarchived)))
+        )
+    )
+
+    log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
+    oldarchived = list(filter(lambda x: x != None, oldarchived))
+    after = await get_after(model_id, username, forced_after)
+    splitArrays = get_split_array(oldarchived, username, after)
+    tasks = get_tasks(splitArrays, c, model_id, after)
+    data = await process_tasks(tasks, model_id, after)
+    progress_utils.archived_layout.visible = False
+    return data
 
 
 @run
-async def get_timeline_media_progress(model_id, username, forced_after=None, c=None):
-    global sem
-    sem = sems.get_req_sem()
-    tasks = []
-    min_posts = 50
-    responseArray = []
-    page_count = 0
-    if not read_args.retriveArgs().no_cache:
-        oldtimeline = operations.get_timeline_postdates(
-            model_id=model_id, username=username
-        )
-    else:
-        oldtimeline = []
+async def get_archived_posts(model_id, username, forced_after=None, c=None):
+    oldarchived = (
+        await operations.get_archived_postinfo(model_id=model_id, username=username)
+        if not read_args.retriveArgs().no_cache
+        else []
+    )
     log.trace(
-        "oldtimeline {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"oldtimeline: {str(x)}", oldtimeline))
-            )
+        "oldarchive {posts}".format(
+            posts="\n\n".join(list(map(lambda x: f"oldarchive: {str(x)}", oldarchived)))
         )
     )
-    log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
-    oldtimeline = list(filter(lambda x: x != None, oldtimeline))
-    postedAtArray = sorted(oldtimeline)
-    after = get_after(model_id, username, forced_after)
-    log.info(
-        f"""
-Setting initial timeline scan date for {username} to {arrow.get(after).format('YYYY.MM.DD')}
-[yellow]Hint: append ' --after 2000' to command to force scan of all timeline posts + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --dupe' to command to force scan of all timeline posts + download/re-download of all files[/yellow]
 
-            """
-    )
-    filteredArray = list(filter(lambda x: x >= after, postedAtArray))
-    filteredArray[1:]
+    log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
+    oldarchived = list(filter(lambda x: x != None, oldarchived))
+    after = await get_after(model_id, username, forced_after)
+    with progress_utils.set_up_api_archived():
+        splitArrays = get_split_array(oldarchived, username, after)
+        tasks = get_tasks(splitArrays, c, model_id, after)
+        return await process_tasks(tasks, model_id, after)
+
 
-    job_progress = progress_utils.timeline_progress
+async def process_tasks(tasks, model_id, after):
+    responseArray = []
+    page_count = 0
     overall_progress = progress_utils.overall_progress
-    # c= c or sessionbuilder.sessionBuilder( limit=constants.getattr("API_MAX_CONNECTION"))
-    if len(filteredArray) >= min_posts + 1:
-        splitArrays = [
-            filteredArray[i : i + min_posts]
-            for i in range(0, len(filteredArray), min_posts)
-        ]
-        # use the previous split for timestamp
-        if len(filteredArray) >= (min_posts * 2) + 1:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_timeline_posts(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        required_ids=set(splitArrays[0]),
-                        timestamp=after,
-                    )
-                )
-            )
-            [
-                tasks.append(
-                    asyncio.create_task(
-                        scrape_timeline_posts(
-                            c,
-                            model_id,
-                            job_progress=job_progress,
-                            required_ids=set(splitArrays[i]),
-                            timestamp=splitArrays[i - 1][-1],
-                        )
-                    )
-                )
-                for i in range(1, len(splitArrays) - 1)
-            ]
-            # keeping grabbing until nothing left
-            tasks.append(
-                asyncio.create_task(
-                    scrape_timeline_posts(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        timestamp=splitArrays[-2][-1],
-                    )
-                )
-            )
-        else:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_timeline_posts(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        timestamp=splitArrays[-1][-1],
-                    )
-                )
-            )
 
-    else:
-        tasks.append(
-            asyncio.create_task(
-                scrape_timeline_posts(
-                    c, model_id, job_progress=job_progress, timestamp=after
-                )
-            )
-        )
     page_task = overall_progress.add_task(
-        f" Timeline Content Pages Progress: {page_count}", visible=True
+        f"Archived Content Pages Progress: {page_count}", visible=True
     )
     while bool(tasks):
         new_tasks = []
         try:
             async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
+                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
             ):
                 for task in asyncio.as_completed(tasks):
                     try:
                         result, new_tasks_batch = await task
                         new_tasks.extend(new_tasks_batch)
                         page_count = page_count + 1
                         overall_progress.update(
                             page_task,
-                            description=f"Timeline Content Pages Progress: {page_count}",
+                            description=f"Archived Content Pages Progress: {page_count}",
                         )
                         responseArray.extend(result)
                     except Exception as E:
                         log.traceback_(E)
                         log.traceback_(traceback.format_exc())
                         continue
         except TimeoutError as E:
-            cache.set(f"{model_id}_full_timeline_scrape")
+            cache.set(f"{model_id}_full_archived_scrape", True)
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
+
         tasks = new_tasks
     overall_progress.remove_task(page_task)
-    progress_utils.timeline_layout.visible = False
+    seen = set()
+    new_posts = [
+        post
+        for post in responseArray
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
 
-    unduped = {}
-    log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
-    for post in responseArray:
-        id = post["id"]
-        if unduped.get(id):
-            continue
-        unduped[id] = post
-
-    log.trace(f"timeline dupeset postids {list(unduped.keys())}")
+    log.trace(f"archive postids {list(map(lambda x:x.get('id'),new_posts))}")
     log.trace(
-        "post raw unduped {posts}".format(
+        "archived raw unduped {posts}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo timeline: {str(x)}", unduped))
+                list(map(lambda x: f"undupedinfo archive: {str(x)}", new_posts))
             )
         )
     )
-    log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
-    set_check(unduped, model_id, after)
-    return list(unduped.values())
-
+    log.debug(f"[bold]Archived Count without Dupes[/bold] {len(new_posts)} found")
+    set_check(new_posts, model_id, after)
+    return new_posts
 
-@run
-async def get_timeline_media(model_id, username, forced_after=None, c=None):
-    global sem
-    job_progress = None
 
-    sem = sems.get_req_sem()
-    tasks = []
+def get_split_array(oldarchived, username, after):
     min_posts = 50
-    responseArray = []
-    page_count = 0
-    if not read_args.retriveArgs().no_cache:
-        oldtimeline = operations.get_timeline_postdates(
-            model_id=model_id, username=username
-        )
-    else:
-        oldtimeline = []
     log.trace(
-        "oldtimeline {posts}".format(
+        "oldarchived {posts}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"oldtimeline: {str(x)}", oldtimeline))
+                list(map(lambda x: f"oldarchived: {str(x)}", oldarchived))
             )
         )
     )
-    log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
-    oldtimeline = list(filter(lambda x: x != None, oldtimeline))
-    postedAtArray = sorted(oldtimeline)
-    after = get_after(model_id, username, forced_after)
+    log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
+    oldarchived = list(filter(lambda x: x != None, oldarchived))
+    postsDataArray = sorted(oldarchived, key=lambda x: x.get("created_at"))
     log.info(
         f"""
-Setting initial timeline scan date for {username} to {arrow.get(after).format('YYYY.MM.DD')}
-[yellow]Hint: append ' --after 2000' to command to force scan of all timeline posts + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --dupe' to command to force scan of all timeline posts + download/re-download of all files[/yellow]
+Setting initial archived scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+[yellow]Hint: append ' --after 2000' to command to force scan of all archived posts + download of new files only[/yellow]
+[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all archived posts + download/re-download of all files[/yellow]
 
             """
     )
-    filteredArray = list(filter(lambda x: x >= after, postedAtArray))
+    filteredArray = list(filter(lambda x: x.get("created_at") >= after, postsDataArray))
 
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
-    if len(filteredArray) >= min_posts + 1:
-        splitArrays = [
-            filteredArray[i : i + min_posts]
-            for i in range(0, len(filteredArray), min_posts)
-        ]
-        # use the previous split for timestamp
-        if len(filteredArray) >= (min_posts * 2) + 1:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_timeline_posts(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        required_ids=set(splitArrays[0]),
-                        timestamp=after,
-                    )
+    # c= c or sessionbuilder.sessionBuilder( limit=constants.getattr("API_MAX_CONNECTION"))
+    splitArrays = [
+        filteredArray[i : i + min_posts]
+        for i in range(0, len(filteredArray), min_posts)
+    ]
+    return splitArrays
+
+
+def get_tasks(splitArrays, c, model_id, after):
+    tasks = []
+    job_progress = progress_utils.archived_progress
+    if len(splitArrays) > 2:
+        tasks.append(
+            asyncio.create_task(
+                scrape_archived_posts(
+                    c,
+                    model_id,
+                    job_progress=job_progress,
+                    required_ids=set([ele.get("created_at") for ele in splitArrays[0]]),
+                    timestamp=splitArrays[0][0].get("created_at"),
+                    offset=True,
                 )
             )
-            [
-                tasks.append(
-                    asyncio.create_task(
-                        scrape_timeline_posts(
-                            c,
-                            model_id,
-                            job_progress=job_progress,
-                            required_ids=set(splitArrays[i]),
-                            timestamp=splitArrays[i - 1][-1],
-                        )
-                    )
-                )
-                for i in range(1, len(splitArrays) - 1)
-            ]
-            # keeping grabbing until nothing left
+        )
+        [
             tasks.append(
                 asyncio.create_task(
-                    scrape_timeline_posts(
+                    scrape_archived_posts(
                         c,
                         model_id,
                         job_progress=job_progress,
-                        timestamp=splitArrays[-2][-1],
+                        required_ids=set(
+                            [ele.get("created_at") for ele in splitArrays[i]]
+                        ),
+                        timestamp=splitArrays[i - 1][-1].get("created_at"),
+                        offset=False,
                     )
                 )
             )
-        else:
-            tasks.append(
-                asyncio.create_task(
-                    scrape_timeline_posts(
-                        c,
-                        model_id,
-                        job_progress=job_progress,
-                        timestamp=splitArrays[-1][-1],
-                    )
+            for i in range(1, len(splitArrays) - 1)
+        ]
+        # keeping grabbing until nothing left
+        tasks.append(
+            asyncio.create_task(
+                scrape_archived_posts(
+                    c,
+                    model_id,
+                    job_progress=job_progress,
+                    timestamp=splitArrays[-1][0].get("created_at"),
+                    offset=True,
                 )
             )
-
-    else:
+        )
+    # use the first split if less then 3
+    elif len(splitArrays) > 0:
         tasks.append(
             asyncio.create_task(
-                scrape_timeline_posts(
-                    c, model_id, job_progress=job_progress, timestamp=after
+                scrape_archived_posts(
+                    c,
+                    model_id,
+                    job_progress=job_progress,
+                    timestamp=splitArrays[0][0].get("created_at"),
+                    offset=True,
                 )
             )
         )
-
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * len(tasks)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            cache.set(f"{model_id}_full_timeline_scrape")
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-
-    unduped = {}
-    log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
-    for post in responseArray:
-        id = post["id"]
-        if unduped.get(id):
-            continue
-        unduped[id] = post
-
-    log.trace(f"timeline dupeset postids {list(unduped.keys())}")
-    log.trace(
-        "post raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo timeline: {str(x)}", unduped))
+    # use after if split is empty i.e no db data
+    else:
+        tasks.append(
+            asyncio.create_task(
+                scrape_archived_posts(
+                    c, model_id, job_progress=job_progress, timestamp=after, offset=True
+                )
             )
         )
-    )
-    log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
-    set_check(unduped, model_id, after)
-    return list(unduped.values())
+    return tasks
 
 
 def set_check(unduped, model_id, after):
     if not after:
-        newCheck = {}
-        for post in cache.get(f"timeline_check_{model_id}", default=[]) + list(
-            unduped.values()
-        ):
-            newCheck[post["id"]] = post
+        seen = set()
+        all_posts = [
+            post
+            for post in cache.get(f"archived_check_{model_id}", default=[]) + unduped
+            if post["id"] not in seen and not seen.add(post["id"])
+        ]
+
         cache.set(
-            f"timeline_check_{model_id}",
-            list(newCheck.values()),
+            f"archived_check_{model_id}",
+            all_posts,
             expire=constants.getattr("DAY_SECONDS"),
         )
         cache.close()
 
 
-def get_individual_post(id):
-    with sessionbuilder.sessionBuilder(backend="httpx") as c:
-        with c.requests(constants.getattr("INDIVIDUAL_TIMELINE").format(id))() as r:
-            if r.ok:
-                log.trace(f"post raw individual {r.json()}")
-                return r.json()
-            else:
-                log.debug(
-                    f"[bold]individual post response status code:[/bold]{r.status}"
-                )
-                log.debug(f"[bold]individual post response:[/bold] {r.text_()}")
-                log.debug(f"[bold]individual post headers:[/bold] {r.headers}")
-
-
-def get_after(model_id, username, forced_after=None):
+async def get_after(model_id, username, forced_after=None):
     if forced_after != None:
         return forced_after
+    elif not settings.get_after_enabled():
+        return 0
     elif read_args.retriveArgs().after == 0:
         return 0
     elif read_args.retriveArgs().after:
         return read_args.retriveArgs().after.float_timestamp
-    elif (
-        cache.get(f"{model_id}_full_timeline_scrape")
-        and not read_args.retriveArgs().after
-        and not data.get_disable_after()
-    ):
+
+    elif cache.get(f"{model_id}_full_archived_scrape"):
         log.info(
-            "Used --after previously. Scraping all timeline posts required to make sure content is not missing"
+            "Used --after previously. Scraping all archived posts required to make sure content is not missing"
         )
         return 0
-    curr = operations.get_timeline_media(model_id=model_id, username=username)
+    curr = await operations.get_archived_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
-    missing_items = list(filter(lambda x: x[10] != 1, curr))
-    missing_items = list(sorted(missing_items, key=lambda x: arrow.get(x[12])))
+    missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
+    missing_items = list(sorted(missing_items, key=lambda x: x.get("posted_at") or 0))
     if len(missing_items) == 0:
         log.debug("Using last db date because,all downloads in db marked as downloaded")
-        return (
-            operations.get_last_timeline_date(model_id=model_id, username=username)
-            - 1000
+        return await operations.get_last_archived_date(
+            model_id=model_id, username=username
         )
     else:
         log.debug(
             f"Setting date slightly before earliest missing item\nbecause {len(missing_items)} posts in db are marked as undownloaded"
         )
-        return arrow.get(missing_items[0][12]).float_timestamp - 1000
+        return missing_items[0].get("posted_at") or 9
+
+
+async def scrape_archived_posts(
+    c, model_id, job_progress=None, timestamp=None, required_ids=None, offset=False
+) -> list:
+    global sem
+    posts = None
+    attempt.set(0)
+    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
+    if timestamp and (
+        float(timestamp)
+        > (read_args.retriveArgs().before or arrow.now()).float_timestamp
+    ):
+        return []
+    timestamp = float(timestamp) - 1000 if timestamp and offset else timestamp
+    url = (
+        constants.getattr("archivedNextEP").format(model_id, str(timestamp))
+        if timestamp
+        else constants.getattr("archivedEP").format(model_id)
+    )
+    log.debug(url)
+
+    async for _ in AsyncRetrying(
+        retry=retry_if_not_exception_type(KeyboardInterrupt),
+        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
+        wait=wait_random(
+            min=constants.getattr("OF_MIN"),
+            max=constants.getattr("OF_MAX"),
+        ),
+        reraise=True,
+    ):
+        with _:
+            new_tasks = []
+            await sem.acquire()
+            try:
+                attempt.set(attempt.get(0) + 1)
+                task = (
+                    job_progress.add_task(
+                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
+                        visible=True,
+                    )
+                    if job_progress
+                    else None
+                )
+                async with c.requests(url)() as r:
+                    if r.ok:
+                        posts = (await r.json_())["list"]
+                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
+                        if not posts or len(posts) == 0:
+                            log.debug(f" {log_id} -> number of post found 0")
+                        elif len(posts) > 0:
+                            log.debug(
+                                f"{log_id} -> number of archived post found {len(posts)}"
+                            )
+                            log.debug(
+                                f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
+                            )
+                            log.debug(
+                                f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
+                            )
+                            log.debug(
+                                f"{log_id} -> found archived post IDs {list(map(lambda x:x.get('id'),posts))}"
+                            )
+                            log.trace(
+                                "{log_id} -> archive raw {posts}".format(
+                                    log_id=log_id,
+                                    posts="\n\n".join(
+                                        list(
+                                            map(
+                                                lambda x: f"scrapeinfo archive: {str(x)}",
+                                                posts,
+                                            )
+                                        )
+                                    ),
+                                )
+                            )
+
+                            if not required_ids:
+                                new_tasks.append(
+                                    asyncio.create_task(
+                                        scrape_archived_posts(
+                                            c,
+                                            model_id,
+                                            job_progress=job_progress,
+                                            timestamp=posts[-1]["postedAtPrecise"],
+                                            offset=False,
+                                        )
+                                    )
+                                )
+                            else:
+                                [
+                                    required_ids.discard(float(ele["postedAtPrecise"]))
+                                    for ele in posts
+                                ]
+
+                                if len(required_ids) > 0 and float(
+                                    timestamp or 0
+                                ) < max(required_ids):
+                                    new_tasks.append(
+                                        asyncio.create_task(
+                                            scrape_archived_posts(
+                                                c,
+                                                model_id,
+                                                job_progress=job_progress,
+                                                timestamp=posts[-1]["postedAtPrecise"],
+                                                required_ids=required_ids,
+                                                offset=False,
+                                            )
+                                        )
+                                    )
+                    else:
+                        log.debug(
+                            f"[bold]archived response status code:[/bold]{r.status}"
+                        )
+                        log.debug(f"[bold]archived response:[/bold] {await r.text_()}")
+                        log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+                        r.raise_for_status()
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                raise E
+
+            finally:
+                sem.release()
+                job_progress.remove_task(task) if job_progress and task else None
+            return posts, new_tasks
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/base.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/base.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/labels.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/media.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/models.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/placeholder.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/placeholder.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         self._placeholder = Placeholders(self._ele, "mp4")
         self._tempname = tempname
 
     async def init(self):
         dir = await self.gettempDir(self._ele)
         file = self._tempname
         self._tempfilepath = paths.truncate(pathlib.Path(dir, file))
+        return self
 
     @basePlaceholder.async_wrapper
     async def gettempDir(self, ele, create=True):
         self._tempdir = await self._placeholder.getmediadir(
             root=(data.get_TempDir(mediatype=ele.mediatype)),
             create=create,
         )
@@ -185,58 +186,51 @@
         self._ele = ele
         self._ext = ext
 
     async def init(self):
         dir = await self.getmediadir()
         file = await self.createfilename()
         self._filepath = paths.truncate(pathlib.Path(dir, file))
+        return self
 
     def add_price_variables(self, username):
         modelObj = selector.get_model_fromParsed(username)
         self._variables.update(
             {
                 "current_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_current_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_current_price == 0 else "Paid"
                 )
             }
         )
         self._variables.update(
             {
                 "regular_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_regular_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_regular_price == 0 else "Paid"
                 )
             }
         )
         self._variables.update(
             {
                 "promo_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_promo_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_promo_price == 0 else "Paid"
                 )
             }
         )
         self._variables.update(
             {
                 "renewal_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_renewal_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_renewal_price == 0 else "Paid"
                 )
             }
         )
 
     async def add_common_variables(self, ele, username, model_id):
         await self.add_main_variables(ele, username, model_id)
         self.add_price_variables(username)
@@ -390,58 +384,51 @@
         self._ele = ele
         self._ext = ext
 
     async def init(self):
         dir = await self.getmediadir()
         file = await self.createfilename()
         self._filepath = paths.truncate(pathlib.Path(dir, file))
+        return self
 
     def add_price_variables(self, username):
         modelObj = selector.get_model_fromParsed(username)
         self._variables.update(
             {
                 "current_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_current_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_current_price == 0 else "Paid"
                 )
             }
         )
         self._variables.update(
             {
                 "regular_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_regular_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_regular_price == 0 else "Paid"
                 )
             }
         )
         self._variables.update(
             {
                 "promo_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_promo_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_promo_price == 0 else "Paid"
                 )
             }
         )
         self._variables.update(
             {
                 "renewal_price": (
                     constants.getattr("MODEL_PRICE_PLACEHOLDER")
                     if not modelObj
-                    else "Free"
-                    if modelObj.final_renewal_price == 0
-                    else "Paid"
+                    else "Free" if modelObj.final_renewal_price == 0 else "Paid"
                 )
             }
         )
 
     async def add_common_variables(self, ele, username, model_id):
         await self.add_main_variables(ele, username, model_id)
         self.add_price_variables(username)
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/posts.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/posts.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class Post(base.base):
     def __init__(self, post, model_id, username, responsetype=None, label=None):
         super().__init__()
         self._post = post
         self._model_id = int(model_id)
         self._username = username
-        self.responsetype = responsetype or post.get("responseType")
+        self._responsetype = responsetype
         self._label = label
 
     # All media return from API dict
     @property
     def post_media(self):
         return self._post.get("media") or []
 
@@ -46,14 +46,32 @@
     @property
     def archived(self):
         if self.post.get("isArchived"):
             return 1
         return 0
 
     @property
+    def pinned(self):
+        if self.post.get("isPinned"):
+            return 1
+        return 0
+
+    @property
+    def favorited(self):
+        return self.post.get("isFavorite")
+
+    @property
+    def opened(self):
+        return self.post.get("isOpened")
+
+    @property
+    def regular_timeline(self):
+        return not self.archived and not self.pinned
+
+    @property
     def db_sanitized_text(self):
         string = self.db_cleanup(self.text)
         return string
 
     @property
     def file_sanitized_text(self):
         string = self.file_cleanup(self.text or self.id)
@@ -69,14 +87,26 @@
         return self.text if not data.get_sanitizeDB() else self.db_sanitized_text
 
     @property
     def title(self):
         return self._post.get("title")
 
     @property
+    def responsetype(self):
+        if self._responsetype:
+            return self._responsetype
+        elif self.pinned:
+            return "pinned"
+        elif self.archived:
+            return "self.archived"
+        elif self.post.get("responseType") == "post":
+            return "timeline"
+        return self.post.get("responseType")
+
+    @property
     def modified_responsetype(self):
         return self.modified_response_helper()
 
     @property
     def id(self):
         return self._post["id"]
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/sessionbuilder.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/classes/table.py` & `ofscraper-3.9.0.dev9/ofscraper/classes/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             return True
         return False
 
     class IntegerInput(Input):
         def __init__(
             self,
             *args,
-            **kwargs
+            **kwargs,
             # ---snip---
         ) -> None:
             super().__init__(
                 # ---snip---
                 *args,
                 **kwargs,
             )
@@ -177,15 +177,15 @@
             return False
         return True
 
     class IntegerInput(Input):
         def __init__(
             self,
             *args,
-            **kwargs
+            **kwargs,
             # ---snip---
         ) -> None:
             super().__init__(
                 # ---snip---
                 *args,
                 **kwargs,
             )
@@ -309,15 +309,15 @@
             return False
         return True
 
     class IntegerInput(Input):
         def __init__(
             self,
             *args,
-            **kwargs
+            **kwargs,
             # ---snip---
         ) -> None:
             super().__init__(
                 # ---snip---
                 *args,
                 **kwargs,
             )
@@ -788,32 +788,32 @@
                     reverse=self.reverse,
                 )
                 self.make_table()
             elif label == "Length":
                 helperNode = self.query_one("#Length")
                 self._filtered_rows = sorted(
                     self._filtered_rows,
-                    key=lambda x: helperNode.convertString(x[index])
-                    if x[index] != "N/A"
-                    else 0,
+                    key=lambda x: (
+                        helperNode.convertString(x[index]) if x[index] != "N/A" else 0
+                    ),
                     reverse=self.reverse,
                 )
                 self.make_table()
             elif label == "Mediatype":
                 self._filtered_rows = sorted(
                     self._filtered_rows, key=lambda x: x[index], reverse=self.reverse
                 )
                 self.make_table()
             elif label == "Post Date":
                 helperNode = self.query_one("#Post_Date")
                 self._filtered_rows = sorted(
                     self._filtered_rows,
-                    key=lambda x: helperNode.convertString(x[index])
-                    if x[index] != "N/A"
-                    else 0,
+                    key=lambda x: (
+                        helperNode.convertString(x[index]) if x[index] != "N/A" else 0
+                    ),
                     reverse=self.reverse,
                 )
                 self.make_table()
             elif label == "Post Media Count":
                 self._filtered_rows = sorted(
                     self._filtered_rows, key=lambda x: x[index], reverse=self.reverse
                 )
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/commands/check.py` & `ofscraper-3.9.0.dev9/ofscraper/commands/check.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 import re
 import threading
 import time
 import traceback
 
 import arrow
 
+import ofscraper.api.archive as archived
 import ofscraper.api.highlights as highlights
 import ofscraper.api.messages as messages_
 import ofscraper.api.paid as paid_
+import ofscraper.api.pinned as pinned
 import ofscraper.api.profile as profile
 import ofscraper.api.timeline as timeline
+import ofscraper.api.labels as labels
 import ofscraper.classes.posts as posts_
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.classes.table as table
 import ofscraper.commands.manual as manual
 import ofscraper.db.operations as operations
 import ofscraper.download.downloadnormal as downloadnormal
 import ofscraper.models.selector as selector
@@ -27,14 +30,16 @@
 import ofscraper.utils.cache as cache
 import ofscraper.utils.console as console_
 import ofscraper.utils.constants as constants
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.network as network
 from ofscraper.download.common.common import textDownloader
 from ofscraper.utils.context.run_async import run
+import ofscraper.utils.args.user as user_helper
+
 
 log = logging.getLogger("shared")
 console = console_.get_shared_console()
 ROW_NAMES = (
     "Number",
     "Download_Cart",
     "UserName",
@@ -49,98 +54,98 @@
     "Price",
     "Post_ID",
     "Media_ID",
     "Text",
 )
 ROWS = []
 app = None
-
-
+prev_names=prev_names=set()
 def process_download_cart():
     while True:
         global app
-        while app and not app.row_queue.empty():
-            if process_download_cart.counter == 0:
-                if not network.check_cdm():
-                    log.info(
-                        "error was raised by cdm checker\ncdm will not be check again\n\n"
-                    )
-                else:
-                    log.info("cdm checker was fine\ncdm will not be check again\n\n")
-                # should be done once before downloads
-                log.info("Getting Models")
-
-            process_download_cart.counter = process_download_cart.counter + 1
-            log.info("Getting items from queue")
-            try:
-                row, key = app.row_queue.get()
-                restype = app.row_names.index("Responsetype")
-                username = app.row_names.index("UserName")
-                post_id = app.row_names.index("Post_ID")
-                media_id = app.row_names.index("Media_ID")
-                url = None
-                if row[restype].plain == "message":
-                    url = constants.getattr("messageTableSPECIFIC").format(
-                        row[username].plain, row[post_id].plain
-                    )
-                elif row[restype].plain == "post":
-                    url = f"{row[post_id]}"
-                elif row[restype].plain == "highlights":
-                    url = constants.getattr("storyEP").format(row[post_id].plain)
-                elif row[restype].plain == "stories":
-                    url = constants.getattr("highlightsWithAStoryEP").format(
-                        row[post_id].plain
-                    )
-                else:
-                    log.info("URL not supported")
-                    continue
-                log.info(f"Added url {url}")
-                log.info("Sending URLs to OF-Scraper")
-                media_dict, post_dict = manual.get_media_from_urls(urls=[url])
-                # None for stories and highlights
-                matchID = int(row[media_id].plain)
-                medialist = list(
-                    filter(
-                        lambda x: x.id == matchID if x.id else None,
-                        list(media_dict.values())[0],
-                    )
+        if not app or app.row_queue.empty():
+            time.sleep(10)
+            continue
+        if process_download_cart.counter == 0:
+            if not network.check_cdm():
+                log.info(
+                    "error was raised by cdm checker\ncdm will not be check again\n\n"
                 )
-                if settings.get_mediatypes() == ["Text"]:
-                    textDownloader(post_dict.values(), username=username)
-                elif len(medialist) > 0 and len(settings.get_mediatypes()) > 1:
-                    media = medialist[0]
-                    model_id = media.post.model_id
-                    username = model_id = media.post.username
-                    args = read_args.retriveArgs()
-                    args.username = set([username])
-                    write_args.setArgs(args)
-                    selector.all_subs_helper()
-                    log.info(
-                        f"Downloading individual media ({media.filename}) to disk for {username}"
-                    )
-                    operations.table_init_create(model_id=model_id, username=username)
-
-                    textDownloader(post_dict.values(), username=username)
+            else:
+                log.info("cdm checker was fine\ncdm will not be check again\n\n")
+            # should be done once before downloads
+            log.info("Getting Models")
+
+        process_download_cart.counter = process_download_cart.counter + 1
+        log.info("Getting items from cart")
+        try:
+            row, key = app.row_queue.get()
+            restype = row[app.row_names.index("Responsetype")].plain
+            username = app.row_names.index("UserName")
+            post_id = app.row_names.index("Post_ID")
+            media_id = app.row_names.index("Media_ID")
+            url = None
+            if restype == "message":
+                url = constants.getattr("messageTableSPECIFIC").format(
+                    row[username].plain, row[post_id].plain
+                )
+            elif restype in {"pinned", "timeline", "archived"}:
+                url = f"{row[post_id]}"
+            elif restype == "highlights":
+                url = constants.getattr("storyEP").format(row[post_id].plain)
+            elif restype == "stories":
+                url = constants.getattr("highlightsWithAStoryEP").format(
+                    row[post_id].plain
+                )
+            else:
+                log.info("URL not supported")
+                continue
+            log.info(f"Added url {url}")
+            log.info("Sending URLs to OF-Scraper")
+            url_dicts= manual.process_urls(urls=[url])
+            set_user_data(url_dicts)
+            # None for stories and highlights
+            matchID = int(row[media_id].plain)
+            medialist = list(
+                filter(
+                    lambda x: x.id == matchID if x.id else None,
+                    [element for inner_list in url_dicts.values() for element in inner_list.get("media_list")],
+                )
+            )
+            postList=[element for inner_list in url_dicts.values() for element in inner_list.get("post_list")]
+            if settings.get_mediatypes() == ["Text"]:
+                textDownloader(postList, username=username)
+            elif len(medialist) > 0 and len(settings.get_mediatypes()) > 1:
+                media = medialist[0]
+                model_id = media.post.model_id
+                username = model_id = media.post.username
+                log.info(
+                    f"Downloading individual media ({media.filename}) to disk for {username}"
+                )
+                operations.table_init_create(model_id=model_id, username=username)
 
-                    values = downloadnormal.process_dicts(username, model_id, [media])
-                    if values == None or values[-1] == 1:
-                        raise Exception("Download is marked as skipped")
-                else:
-                    raise Exception("Issue getting download")
+                textDownloader(postList, username=username)
 
-                log.info("Download Finished")
-                app.update_cell(key, "Download_Cart", "[downloaded]")
-                app.update_cell(key, "Downloaded", True)
-
-            except Exception as E:
-                app.update_downloadcart_cell(key, "[failed]")
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-        time.sleep(10)
+                values = downloadnormal.process_dicts(username, model_id, [media])
+                if values == None or values[-1] == 1:
+                    raise Exception("Download is marked as skipped")
+            else:
+                raise Exception("Issue getting download")
 
+            log.info("Download Finished")
+            app.update_cell(key, "Download_Cart", "[downloaded]")
+            app.update_cell(key, "Downloaded", True)
+
+        except Exception as E:
+            app.update_downloadcart_cell(key, "[failed]")
+            log.traceback_(E)
+            log.traceback_(traceback.format_exc())
+        
+        if app.row_queue.empty():
+            log.info("Download cart is currently empty")
 
 def checker():
     args = read_args.retriveArgs()
     if args.command == "post_check":
         post_checker()
     elif args.command == "msg_check":
         message_checker()
@@ -161,89 +166,119 @@
     links = list(url_helper())
     async with sessionbuilder.sessionBuilder(backend="httpx") as c:
         for ele in links:
             name_match = re.search(
                 f"onlyfans.com/({constants.getattr('USERNAME_REGEX')}+$)", ele
             )
             name_match2 = re.search(f"^{constants.getattr('USERNAME_REGEX')}+$", ele)
+            user_name=None
+            model_id=None
 
             if name_match:
                 user_name = name_match.group(1)
                 log.info(f"Getting Full Timeline for {user_name}")
                 model_id = profile.get_id(user_name)
+                user_dict.setdefault(model_id, {})["model_id"]= model_id
+                user_dict.setdefault(model_id, {})["username"]= user_name
+
             elif name_match2:
                 user_name = name_match2.group(0)
                 model_id = profile.get_id(user_name)
-            else:
-                continue
-            if user_dict.get(user_name):
-                continue
-
-            oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
-            user_dict[user_name] = {}
-            user_dict[user_name] = user_dict[user_name] or []
-            if len(oldtimeline) > 0 and not read_args.retriveArgs().force:
-                user_dict[user_name].extend(oldtimeline)
-            else:
-                user_dict[user_name] = {}
-                user_dict[user_name] = user_dict[user_name] or []
-                data = await timeline.get_timeline_media(
-                    model_id, user_name, forced_after=0, c=c
-                )
-                user_dict[user_name].extend(data)
-                cache.set(
-                    f"timeline_check_{model_id}",
-                    data,
-                    expire=constants.getattr("DAY_SECONDS"),
-                )
+                user_dict.setdefault(model_id, {})["model_id"]= model_id
+                user_dict.setdefault(model_id, {})["username"]= user_name
+            if user_dict.get(model_id) and model_id and user_name:
+                areas = read_args.retriveArgs().check_area
+                await operations.table_init_create(username=user_name, model_id=model_id)
+                if "Timeline" in areas:
+                    oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
+                    if len(oldtimeline) > 0 and not read_args.retriveArgs().force:
+                        data=oldtimeline.get
+                    else:
+                        data = await timeline.get_timeline_posts(
+                            model_id, user_name, forced_after=0, c=c
+                        )
+                    user_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(data)
+                if "Archived" in areas:
+                    oldarchive = cache.get(f"archived_check_{model_id}", default=[])
+                    if len(oldarchive) > 0 and not read_args.retriveArgs().force:
+                        data=oldarchive
+                    else:
+                        data = await archived.get_archived_posts(
+                            model_id, user_name, forced_after=0, c=c
+                        )
+                    user_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(data)
+                if "Pinned" in areas:
+                    oldpinned = cache.get(f"pinned_check_{model_id}", default=[])
+                    if len(oldpinned) > 0 and not read_args.retriveArgs().force:
+                        data=oldpinned
+                    else:
+                        data = await pinned.get_pinned_posts(model_id, c=c)
+                    user_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(data)
+                if "Labels" in areas:
+                    oldlabels = cache.get(f"labels_check_{model_id}", default=[])
+                    if len(oldlabels) > 0 and not read_args.retriveArgs().force:
+                        data=oldlabels
+                    else:
+                        labels_data = await labels.get_labels(model_id, c=c)
+                        await operations.make_label_table_changes(labels_data ,model_id=model_id,username=user_name,posts=False)
+                        data=[post for label in labels_data for post in label["posts"]]
+                    user_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(data)
                 cache.close()
+        # individual links
+        for ele in list(
+            filter(
+                lambda x: re.search(
+                    f"onlyfans.com/{constants.getattr('NUMBER_REGEX')}+/{constants.getattr('USERNAME_REGEX')}+$",
+                    x,
+                ),
+                links,
+            )
+        ):
+            name_match = re.search(
+                f"/({constants.getattr('USERNAME_REGEX')}+$)", ele
+            )
+            num_match = re.search(f"/({constants.getattr('NUMBER_REGEX')}+)", ele)
+            if name_match and num_match:
+                user_name = name_match.group(1)
+                model_id = profile.get_id(user_name)
+                user_dict.setdefault(model_id, {})["model_id"]= model_id
+                user_dict.setdefault(model_id, {})["username"]= user_name
 
-            # individual links
-            for ele in list(
-                filter(
-                    lambda x: re.search(
-                        f"onlyfans.com/{constants.getattr('NUMBER_REGEX')}+/{constants.getattr('USERNAME_REGEX')}+$",
-                        x,
-                    ),
-                    links,
-                )
-            ):
-                name_match = re.search(
-                    f"/({constants.getattr('USERNAME_REGEX')}+$)", ele
-                )
-                num_match = re.search(f"/({constants.getattr('NUMBER_REGEX')}+)", ele)
-                if name_match and num_match:
-                    user_name = name_match.group(1)
-                    post_id = num_match.group(1)
-                    model_id = profile.get_id(user_name)
-                    log.info(f"Getting Invidiual Link for {user_name}")
-                    if not user_dict.get(user_name):
-                        user_dict[name_match.group(1)] = {}
-                    data = timeline.get_individual_post(post_id)
-                    user_dict[user_name] = user_dict[user_name] or []
-                    user_dict[user_name].append(data)
 
+                post_id = num_match.group(1)   
+                log.info(f"Getting individual link for {user_name}")
+                if not user_dict.get(user_name):
+                    user_dict[name_match.group(1)] = {}
+                data = timeline.get_individual_post(post_id)
+                user_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(data)
     ROWS = []
-    for user_name in user_dict.keys():
+    for val in user_dict.values():
+        user_name=val.get("username")
         downloaded = await get_downloaded(user_name, model_id, True)
-        media = get_all_found_media(user_name, user_dict[user_name])
+        posts = list(
+            map(lambda x: posts_.Post(x, model_id, user_name), val.get("post_list", []))
+        )
+        await operations.make_post_table_changes(
+            posts, model_id=model_id, username=user_name
+        )
+        media = await process_post_media(user_name, model_id,posts)
         ROWS.extend(row_gather(media, downloaded, user_name))
     return ROWS
 
 
 def reset_url():
     # clean up args once check modes are ready to launch
     args = read_args.retriveArgs()
     argdict = vars(args)
     if argdict.get("url"):
         read_args.retriveArgs().url = None
     if argdict.get("file"):
         read_args.retriveArgs().file = None
     if argdict.get("username"):
-        read_args.retriveArgs().username = None
+        read_args.retriveArgs().usernames = None
     write_args.setArgs(args)
 
 
 def set_count(ROWS):
     for count, ele in enumerate(ROWS):
         ele[0] = count + 1
 
@@ -272,144 +307,169 @@
             name_match = re.search(f"^{constants.getattr('USERNAME_REGEX')}+$", item)
             if num_match:
                 model_id = num_match.group(1)
                 user_name = profile.scrape_profile(model_id)["username"]
             elif name_match:
                 user_name = name_match.group(0)
                 model_id = profile.get_id(user_name)
-            else:
-                continue
-            log.info(f"Getting Messages/Paid content for {user_name}")
-            # messages
-            messages = None
-            oldmessages = cache.get(f"message_check_{model_id}", default=[])
-            log.debug(f"Number of messages in cache {len(oldmessages)}")
+            if model_id and user_name:
+                log.info(f"Getting Messages/Paid content for {user_name}")
+                await operations.table_init_create(model_id=model_id, username=user_name)
+                # messages
+                messages = None
+                oldmessages = cache.get(f"message_check_{model_id}", default=[])
+                log.debug(f"Number of messages in cache {len(oldmessages)}")
 
-            if len(oldmessages) > 0 and not read_args.retriveArgs().force:
-                messages = oldmessages
-            else:
-                messages = await messages_.get_messages(
-                    model_id, user_name, forced_after=0
+                if len(oldmessages) > 0 and not read_args.retriveArgs().force:
+                    messages = oldmessages
+                else:
+                    messages = await messages_.get_messages(
+                        model_id, user_name, forced_after=0,c=c
+                    )
+                message_posts_array = list(
+                    map(lambda x: posts_.Post(x, model_id, user_name), messages)
                 )
-                cache.set(
-                    f"message_check_{model_id}",
-                    messages,
-                    expire=constants.getattr("DAY_SECONDS"),
+                await operations.make_messages_table_changes(
+                    message_posts_array, model_id=model_id, username=user_name
                 )
-            oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
-            paid = None
-            # paid content
-            if len(oldpaid) > 0 and not read_args.retriveArgs().force:
-                paid = oldpaid
-            else:
-                paid = await paid_.get_paid_posts(model_id, user_name, c=c)
-                cache.set(
-                    f"purchased_check_{model_id}",
-                    paid,
-                    expire=constants.getattr("DAY_SECONDS"),
-                )
-            media = get_all_found_media(user_name, messages + paid)
-            unduped = []
-            id_set = set()
-            for ele in media:
-                if ele.id == None or ele.id not in id_set:
-                    unduped.append(ele)
-                    id_set.add(ele.id)
-            downloaded = await get_downloaded(user_name, model_id, True)
 
-            ROWS.extend(row_gather(unduped, downloaded, user_name))
+                oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
+                paid = None
+                # paid content
+                if len(oldpaid) > 0 and not read_args.retriveArgs().force:
+                    paid = oldpaid
+                else:
+                    paid = await paid_.get_paid_posts(model_id, user_name, c=c)
+                paid_posts_array = list(
+                    map(lambda x: posts_.Post(x, model_id, user_name), paid)
+                )
+                await operations.make_changes_to_content_tables(
+                    paid_posts_array, model_id=model_id, username=user_name
+                )
+
+                media = await process_post_media(
+                    user_name,model_id, paid_posts_array + message_posts_array
+                )
+
+                downloaded = await get_downloaded(user_name, model_id, True)
+
+                ROWS.extend(row_gather(media, downloaded, user_name))
     return ROWS
 
 
 def purchase_checker():
     ROWS = purchase_checker_helper()
     start_helper(ROWS)
 
 
 @run
 async def purchase_checker_helper():
     user_dict = {}
     auth_requests.make_headers()
     ROWS = []
     async with sessionbuilder.sessionBuilder(backend="httpx") as c:
-        for user_name in read_args.retriveArgs().username:
+        for user_name in read_args.retriveArgs().usernames:
             user_name = profile.scrape_profile(user_name)["username"]
             user_dict[user_name] = user_dict.get(user_name, [])
             model_id = profile.get_id(user_name)
+
+            await operations.table_init_create(model_id=model_id, username=user_name)
+
             oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
             paid = None
 
+
             if len(oldpaid) > 0 and not read_args.retriveArgs().force:
                 paid = oldpaid
             else:
                 paid = await paid_.get_paid_posts(model_id, user_name, c=c)
-                cache.set(
-                    f"purchased_check_{model_id}",
-                    paid,
-                    expire=constants.getattr("DAY_SECONDS"),
-                )
+            posts_array = list(map(lambda x: posts_.Post(x, model_id, user_name), paid))
+            await operations.make_changes_to_content_tables(
+                posts_array, model_id=model_id, username=user_name
+            )
             downloaded = await get_downloaded(user_name, model_id)
-            media = get_all_found_media(user_name, paid)
+            media = await process_post_media(user_name, model_id,posts_array)
             ROWS.extend(row_gather(media, downloaded, user_name))
     return ROWS
 
 
 def stories_checker():
     ROWS = stories_checker_helper()
     start_helper(ROWS)
 
 
 @run
 async def stories_checker_helper():
     user_dict = {}
     ROWS = []
     async with sessionbuilder.sessionBuilder(backend="httpx") as c:
-        for user_name in read_args.retriveArgs().username:
+        for user_name in read_args.retriveArgs().usernames:
             user_name = profile.scrape_profile(user_name)["username"]
             user_dict[user_name] = user_dict.get(user_name, [])
             model_id = profile.get_id(user_name)
+            await operations.table_init_create(model_id=model_id, username=user_name)
             stories = await highlights.get_stories_post(model_id, c=c)
             highlights_ = await highlights.get_highlight_post(model_id, c=c)
             highlights_ = list(
                 map(
                     lambda x: posts_.Post(x, model_id, user_name, "highlights"),
                     highlights_,
                 )
             )
             stories = list(
                 map(lambda x: posts_.Post(x, model_id, user_name, "stories"), stories)
             )
 
             downloaded = await get_downloaded(user_name, model_id)
-            media = []
-            [media.extend(ele.all_media) for ele in stories + highlights_]
+            media = await process_post_media(user_name,model_id,stories+highlights_)
             ROWS.extend(row_gather(media, downloaded, user_name))
     return ROWS
 
 
 def url_helper():
     out = []
     out.extend(read_args.retriveArgs().file or [])
     out.extend(read_args.retriveArgs().url or [])
     return map(lambda x: x.strip(), out)
 
 
-def get_all_found_media(user_name, posts):
+@run
+async def set_user_data(url_dicts):
+    global prev_names
+    all_usernames=[nested_dict.get("username") for nested_dict in url_dicts.values()]
+    new_usernames=list(filter(lambda x: x not in prev_names,all_usernames))
+    if len(new_usernames)>0:
+        prev_names.update(new_usernames)
+        user_helper.set_users_arg(new_usernames)
+        await selector.all_subs_helper()
+
+@run
+async def process_post_media(username,model_id,posts_array):
+    seen = set()
+    unduped = [
+    post
+        for post in posts_array
+    if (post.id,post.username) not in seen and not seen.add((post.id,post.username))
+    ]
     temp = []
-    model_id = profile.get_id(user_name)
-    posts_array = list(map(lambda x: posts_.Post(x, model_id, user_name), posts))
-    [temp.extend(ele.all_media) for ele in posts_array]
+    [temp.extend(ele.all_media) for ele in unduped]
+    await operations.batch_mediainsert(
+                temp,
+                model_id=model_id,
+                username=username,
+                downloaded=False,
+    )
     return temp
 
 
 @run
 async def get_downloaded(user_name, model_id, paid=False):
     downloaded = {}
 
-    operations.table_init_create(model_id=model_id, username=user_name)
+    await operations.table_init_create(model_id=model_id, username=user_name)
     paid = await get_paid_ids(model_id, user_name) if paid else []
     [
         downloaded.update({ele: downloaded.get(ele, 0) + 1})
         for ele in operations.get_media_ids_downloaded(
             model_id=model_id, username=user_name
         )
         + paid
@@ -424,20 +484,15 @@
     paid = None
 
     if len(oldpaid) > 0 and not read_args.retriveArgs().force:
         paid = oldpaid
     else:
         async with sessionbuilder.sessionBuilder(backend="httpx") as c:
             paid = await paid_.get_paid_posts(model_id, user_name, c=c)
-            cache.set(
-                f"purchased_check_{model_id}",
-                paid,
-                expire=constants.getattr("DAY_SECONDS"),
-            )
-    media = get_all_found_media(user_name, paid)
+    media = await process_post_media(user_name,model_id, paid)
     media = list(filter(lambda x: x.canview == True, media))
     return list(map(lambda x: x.id, media))
 
 
 def thread_starters(ROWS_):
     worker_thread = threading.Thread(target=process_download_cart, daemon=True)
     worker_thread.start()
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/commands/manual.py` & `ofscraper-3.9.0.dev9/ofscraper/commands/manual.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,131 +12,158 @@
 import ofscraper.db.operations as operations
 import ofscraper.download.download as download
 import ofscraper.models.selector as selector
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.args.write as write_args
 import ofscraper.utils.constants as constants
 import ofscraper.utils.system.network as network
-from ofscraper.download.common.common import textDownloader
+import ofscraper.utils.args.user as user_helper
 from ofscraper.utils.context.run_async import run
 
 
 def manual_download(urls=None):
     log = logging.getLogger("shared")
     network.check_cdm()
     allow_manual_dupes()
-    media_dict, posts_dict = get_media_from_urls(urls)
-    log.debug(f"Number of values from media dict  {len(list(media_dict.values()))}")
-    log.debug(f"Number of values from post dict  {len(list(posts_dict.values()))}")
-
-    get_manual_usernames(media_dict)
-    selector.all_subs_helper()
-    for value in filter(lambda x: len(x) > 0, media_dict.values()):
-        model_id = value[0].post.model_id
-        username = value[0].post.username
+    url_dicts = process_urls(urls)
+    all_media=[item for media_list in url_dicts.values() for item in media_list.get("media_list", [])]
+    all_posts=[item for post_list in url_dicts.values() for item in post_list.get("post_list", [])]
+    log.debug(f"Number of values from media dict  {len(all_media)}")
+    log.debug(f"Number of values from post dict  {len(all_posts)}")
+    if len(all_media)==0 and len(all_posts)==0:
+        return
+    set_user_data(url_dicts)
+    for _,value in url_dicts.items():
+        model_id = value.get("model_id")
+        username = value.get("username")
+        model_id = value.get("model_id")
+        username = value.get("username")
         log.info(f"Downloading individual media for {username}")
         operations.table_init_create(model_id=model_id, username=username)
-        download.download_process(username, model_id, value, posts=None)
-    textDownloader(posts_dict.values(), username=username)
+        operations.make_changes_to_content_tables(value.get("post_list",[]),model_id=model_id,username=username)
+        download.download_process(username, model_id, value.get("media_list",[]), posts=None)
+        operations.batch_mediainsert(value.get("media_list"),username=username,model_id=model_id)
 
 
 def allow_manual_dupes():
     args = read_args.retriveArgs()
-    args.dupe = True
+    args.force_all = True
     write_args.setArgs(args)
 
 
-def get_manual_usernames(media_dict):
-    usernames = []
-    for value in media_dict.values():
-        if len(value) == 0:
-            continue
-        usernames.append(value[0].post.username)
-    args = read_args.retriveArgs()
-    args.username = set(usernames)
-    write_args.setArgs(args)
+def set_user_data(url_dicts):
+    user_helper.set_users_arg([nested_dict.get("username") for nested_dict in url_dicts.values()])
+    selector.all_subs_helper()
 
+def process_urls(urls):
+    out_dict={}
 
-def get_media_from_urls(urls):
-    user_name_dict = {}
-    media_dict = {}
-    post_dict = {}
     for url in url_helper(urls):
         response = get_info(url)
         model = response[0]
         postid = response[1]
         type = response[2]
-        if type == "post":
-            model_id = user_name_dict.get(model) or profile.get_id(model)
+        if type == "post":  
+            user_data=profile.scrape_profile(model)
+            model_id = user_data.get("id")
+            username= user_data.get("username")
+            out_dict.setdefault(model_id, {})["model_id"]= model_id
+            out_dict.setdefault(model_id, {})["username"]= username
+
             value = timeline.get_individual_post(postid)
-            media_dict.update(get_all_media(postid, model_id, value))
-            post_dict.update(get_post_item(model_id, value))
+
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
         elif type == "msg":
-            model_id = model
+            user_data=profile.scrape_profile(model).get("username")
+            model_id = user_data.get("id")
+            username= user_data.get("username")
+            out_dict.setdefault(model_id, {})["model_id"]= model_id
+            out_dict.setdefault(model_id, {})["username"]= username
+            
             value = messages_.get_individual_post(model_id, postid)
-            media_dict.update(get_all_media(postid, model_id, value))
-            post_dict.update(get_post_item(model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
         elif type == "msg2":
-            model_id = user_name_dict.get(model) or profile.get_id(model)
+            user_data=profile.scrape_profile(model)
+            username= user_data.get("username")
+            model_id=user_data.get("id")
+            out_dict.setdefault(model_id, {})["model_id"]= model_id
+            out_dict.setdefault(model_id, {})["username"]= username
+
             value = messages_.get_individual_post(model_id, postid)
-            media_dict.update(get_all_media(postid, model_id, value))
-            post_dict.update(get_post_item(model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
         elif type == "unknown":
             value = unknown_type_helper(postid) or {}
             model_id = value.get("author", {}).get("id")
-            media_dict.update(get_all_media(postid, model_id, value))
-            post_dict.update(get_post_item(model_id, value))
+            if not model_id:
+                continue
+            username=profile.scrape_profile(model_id).get("username")
+            out_dict.setdefault(model_id, {})["model_id"]= model_id
+            out_dict.setdefault(model_id, {})["username"]= username
+
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
         elif type == "highlights":
             value = highlights_.get_individual_highlights(postid) or {}
             model_id = value.get("userId")
-            media_dict.update(get_all_media(postid, model_id, value, "highlights"))
-            post_dict.update(get_post_item(model_id, value, "highlights"))
+            if not model_id:
+                continue
+            username= profile.scrape_profile(model_id).get("username")
+            out_dict.setdefault(model_id, {})["model_id"]= model_id
+            out_dict.setdefault(model_id, {})["username"]= username
+
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value,responsetype="highlights"))
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value,responsetype="highlights"))
             # special case
         elif type == "stories":
             value = highlights_.get_individual_stories(postid) or {}
             model_id = value.get("userId")
-            media_dict.update(get_all_media(postid, model_id, value, "stories"))
-            post_dict.update(get_post_item(model_id, value, "stories"))
+            if not model_id:
+                continue
+            username= profile.scrape_profile(model_id).get("username")
+            out_dict.setdefault(model_id, {})["model_id"]= model_id
+            out_dict.setdefault(model_id, {})["username"]= username
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value,responsetype="stories"))
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value,responsetype="stories"))
             # special case
-    return media_dict, post_dict
+    return out_dict
 
 
 def unknown_type_helper(postid):
     return timeline.get_individual_post(postid)
 
 
-def get_post_item(model_id, value, inputtype=None):
+def get_post_item(model_id, value, responsetype=None):
     if value == None:
         return []
     user_name = profile.scrape_profile(model_id)["username"]
-    post = posts_.Post(value, model_id, user_name, responsetype=inputtype)
-    return {post.id: post}
+    post = posts_.Post(value, model_id, user_name, responsetype=responsetype)
+    return [post]
 
 
-def get_all_media(posts_id, model_id, value, inputtype=None):
-    media_dict = {}
+def get_all_media(posts_id, model_id, value,responsetype=None):
     value = value or {}
     media = []
     if model_id == None:
         return {}
     user_name = profile.scrape_profile(model_id)["username"]
-    post_item = posts_.Post(value, model_id, user_name, responsetype=inputtype)
+    post_item = posts_.Post(value, model_id, user_name, responsetype=responsetype)
     media = post_item.media
     media = list(
         filter(
             lambda x: isinstance(x, media_.Media)
             and (str(x.id) == str(posts_id) or str(x.postid) == str(posts_id)),
             media,
         )
     )
     if len(media) == 0:
         media.extend(paid_failback(posts_id, model_id, user_name))
-    media_dict[model_id] = media
-    return media_dict
-
+    return media
 
 @run
 async def paid_failback(post_id, model_id, username):
     logging.getLogger("shared").debug(
         "Using failback search because query return 0 media"
     )
     post_id = str(post_id)
@@ -197,13 +224,12 @@
         return None, search7.group(0), "unknown"
 
     return None, None, None
 
 
 def url_helper(urls):
     args = read_args.retriveArgs()
-    args = vars(args)
     out = []
     out.extend(args.get("file", []) or [])
     out.extend(args.get("url", []) or [])
     out.extend(urls or [])
     return map(lambda x: x.strip(), out)
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/commands/scraper.py` & `ofscraper-3.9.0.dev9/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/config.py` & `ofscraper-3.9.0.dev9/ofscraper/const/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,9 +49,9 @@
 INFINITE_LOOP_DEFAULT = False
 DISABLE_AFTER_DEFAULT = False
 DEFAULT_USER_LIST = "main"
 DEFAULT_BLACK_LIST = ""
 HASHED_DEFAULT = False
 EMPTY_MEDIA_DEFAULT = {}
 DEFAULT_LOG_LEVEL = "DEBUG"
-INCLUDED_LABELS_ALL = False
+INCLUDE_LABELS_ALL = False
 DISCORD_THREAD_OVERRIDE = False
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/constants.py` & `ofscraper-3.9.0.dev9/ofscraper/const/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/general.py` & `ofscraper-3.9.0.dev9/ofscraper/const/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/other_url.py` & `ofscraper-3.9.0.dev9/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/prompts.py` & `ofscraper-3.9.0.dev9/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/req.py` & `ofscraper-3.9.0.dev9/ofscraper/const/req.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/test_constants.py` & `ofscraper-3.9.0.dev9/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/const/url.py` & `ofscraper-3.9.0.dev9/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/alt_download.py` & `ofscraper-3.9.0.dev9/ofscraper/download/alt_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import pathlib
 import re
 import subprocess
 import traceback
 from functools import partial
 
 import aiofiles
 import arrow
+import psutil
 from tenacity import (
     AsyncRetrying,
     retry_if_not_exception_message,
     stop_after_attempt,
     wait_random,
 )
 
@@ -59,16 +61,15 @@
 )
 
 
 async def alt_download(c, ele, username, model_id, job_progress):
     common_globals.log.debug(
         f"{get_medialog(ele)} Downloading with protected media downloader"
     )
-    sharedPlaceholderObj = placeholder.Placeholders(ele, "mp4")
-    await sharedPlaceholderObj.init()
+    sharedPlaceholderObj = await placeholder.Placeholders(ele, "mp4").init()
     common_globals.log.debug(f"{get_medialog(ele)} download url:  {get_url_log(ele)}")
     if read_args.retriveArgs().metadata != None:
         return await metadata(
             c, ele, username, model_id, placeholderObj=sharedPlaceholderObj
         )
 
     audio, video = await ele.mpd_dict
@@ -84,18 +85,17 @@
 
     return await handle_result(
         sharedPlaceholderObj, ele, audio, video, username, model_id
     )
 
 
 async def handle_result(sharedPlaceholderObj, ele, audio, video, username, model_id):
-    tempPlaceholder = placeholder.tempFilePlaceholder(
+    tempPlaceholder = await placeholder.tempFilePlaceholder(
         ele, f"temp_{ele.id or await ele.final_filename}.mp4"
-    )
-    await tempPlaceholder.init()
+    ).init()
     temp_path = tempPlaceholder.tempfilepath
     temp_path.unlink(missing_ok=True)
     t = subprocess.run(
         [
             settings.get_ffmpeg(),
             "-i",
             str(video["path"]),
@@ -169,16 +169,17 @@
 async def media_item_keys(c, audio, video, ele):
     for item in [audio, video]:
         item = await keyhelpers.un_encrypt(item, c, ele)
 
 
 async def alt_download_downloader(item, c, ele, job_progress):
     downloadspace(mediatype=ele.mediatype)
-    placeholderObj = placeholder.tempFilePlaceholder(ele, f"{item['name']}.part")
-    await placeholderObj.init()
+    placeholderObj = await placeholder.tempFilePlaceholder(
+        ele, f"{item['name']}.part"
+    ).init()
     item["path"] = placeholderObj.tempfilepath
     item["total"] = None
     async for _ in AsyncRetrying(
         stop=stop_after_attempt(constants.getattr("DOWNLOAD_RETRIES")),
         wait=wait_random(
             min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
         ),
@@ -187,17 +188,19 @@
         ),
         reraise=True,
     ):
         with _:
             try:
                 _attempt = common.alt_attempt_get(item)
                 _attempt.set(_attempt.get(0) + 1)
-                pathlib.Path(placeholderObj.tempfilepath).unlink(
-                    missing_ok=True
-                ) if _attempt.get() > 1 else None
+                (
+                    pathlib.Path(placeholderObj.tempfilepath).unlink(missing_ok=True)
+                    if _attempt.get() > 1
+                    else None
+                )
                 data = await asyncio.get_event_loop().run_in_executor(
                     common_globals.cache_thread,
                     partial(cache.get, f"{item['name']}_headers"),
                 )
                 if data:
                     return await main_data_handler(
                         data, item, c, ele, placeholderObj, job_progress
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.0.dev9/ofscraper/download/alt_downloadbatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import ofscraper.download.common.globals as common_globals
 import ofscraper.download.common.keyhelpers as keyhelpers
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.settings as settings
+import ofscraper.utils.system.system as system
 from ofscraper.download.common.common import (
     addLocalDir,
     check_forced_skip,
     downloadspace,
     get_item_total,
     get_medialog,
     get_resume_size,
@@ -51,16 +52,15 @@
 async def alt_download(c, ele, username, model_id):
     common_globals.innerlog.get().debug(
         f"{get_medialog(ele)} Downloading with batch protected media downloader"
     )
     common_globals.innerlog.get().debug(
         f"{get_medialog(ele)} download url:  {get_url_log(ele)}"
     )
-    sharedPlaceholderObj = placeholder.Placeholders(ele, "mp4")
-    await sharedPlaceholderObj.init()
+    sharedPlaceholderObj = await placeholder.Placeholders(ele, "mp4").init()
     if read_args.retriveArgs().metadata != None:
         return await metadata(
             c, ele, username, model_id, placeholderObj=sharedPlaceholderObj
         )
     audio, video = await ele.mpd_dict
     path_to_file_logger(sharedPlaceholderObj, ele, common_globals.innerlog.get())
     audio = await alt_download_downloader(audio, c, ele)
@@ -72,18 +72,17 @@
     await media_item_keys(c, audio, video, ele)
     return await handle_result(
         sharedPlaceholderObj, ele, audio, video, username, model_id
     )
 
 
 async def handle_result(sharedPlaceholderObj, ele, audio, video, username, model_id):
-    tempPlaceholder = placeholder.tempFilePlaceholder(
+    tempPlaceholder = await placeholder.tempFilePlaceholder(
         ele, f"temp_{ele.id or await ele.final_filename}.mp4"
-    )
-    await tempPlaceholder.init()
+    ).init()
     temp_path = tempPlaceholder.tempfilepath
 
     temp_path.unlink(missing_ok=True)
     t = subprocess.run(
         [
             settings.get_ffmpeg(),
             "-i",
@@ -185,17 +184,19 @@
         ),
         reraise=True,
     ):
         with _:
             try:
                 _attempt = common.alt_attempt_get(item)
                 _attempt.set(_attempt.get(0) + 1)
-                pathlib.Path(placeholderObj.tempfilepath).unlink(
-                    missing_ok=True
-                ) if _attempt.get() > 1 else None
+                (
+                    pathlib.Path(placeholderObj.tempfilepath).unlink(missing_ok=True)
+                    if _attempt.get() > 1
+                    else None
+                )
                 data = await asyncio.get_event_loop().run_in_executor(
                     common_globals.cache_thread,
                     partial(cache.get, f"{item['name']}_headers"),
                 )
                 if data:
                     return await main_data_handler(data, item, c, ele, placeholderObj)
                 else:
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/common.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import pathlib
 from functools import partial, singledispatch
 
 from humanfriendly import format_size
 
 import ofscraper.download.common.globals as common_globals
@@ -135,17 +136,15 @@
     return data
 
 
 def get_unknown_content_type(ele):
     return (
         "mp4"
         if ele.mediatype.lower() == "videos"
-        else "jpg"
-        if ele.mediatype.lower() == "images"
-        else None
+        else "jpg" if ele.mediatype.lower() == "images" else None
     )
 
 
 async def batch_total_change_helper(total, new_total):
     if not new_total and not new_total:
         return
     elif not total:
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/globals.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/globals.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,20 +41,14 @@
     skipped = 0
     global forced_skipped
     forced_skipped = 0
     global data
     data = 0
     global total_data
     total_data = 0
-    global desc
-    desc = (
-        "Progress: ({p_count} photos, {v_count} videos, {a_count} audios, {forced_skipped} skipped, {skipped} failed || {sumcount}/{mediacount}||{data}/{total})"
-        if not read_args.retriveArgs().metadata
-        else "Progress: ({p_count} photos, {v_count} videos, {a_count} audios, {forced_skipped} metadata unchanged, {skipped} failed || {sumcount}/{mediacount}||{data}/{total})"
-    )
     global count_lock
     count_lock = aioprocessing.AioLock()
     global chunk_lock
     chunk_lock = aioprocessing.AioLock()
 
     # global
     global thread
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/keyhelpers.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/log.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,21 +53,27 @@
             f"In progress -> {format_size(common_globals.total_bytes )}) ({common_globals.photo_count+common_globals.audio_count+common_globals.video_count} \
 downloads total [{common_globals.video_count} videos, {common_globals.audio_count} audios, {common_globals.photo_count} photos], \
             {common_globals.forced_skipped} skipped, {common_globals.skipped} failed)"
         )
 
 
 def final_log(username, log=None):
-    skipped_word = (
-        "skipped" if not read_args.retriveArgs().metadata else "metadata unchanged"
-    )
+    skipped_word = "skipped"
     (log or common_globals.log).warning(
         f"[bold]{username}[/bold] ({format_size(common_globals.total_bytes )}) ({common_globals.photo_count+common_globals.audio_count+common_globals.video_count}"
         f" downloads total [{common_globals.video_count} videos, {common_globals.audio_count} audios, {common_globals.photo_count} photos], "
         f"{common_globals.forced_skipped} {skipped_word}, {common_globals.skipped} failed)"
     )
+    if read_args.retriveArgs().metadata:
+        skipped_word = "media metadata unchanged"
+        (log or common_globals.log).warning(
+            f"[bold]{username}[/bold] ({format_size(common_globals.total_bytes )}) ({common_globals.photo_count+common_globals.audio_count+common_globals.video_count}"
+            f" downloads total [{common_globals.video_count} videos, {common_globals.audio_count} audios, {common_globals.photo_count} photos], "
+            f"{common_globals.forced_skipped} {skipped_word}, {common_globals.skipped} failed)"
+        )
+        log.info("This only includes updates for the media table")
 
 
 def text_log(username, value=0, fails=0, exists=0, log=None):
     (log or common_globals.log).warning(
         f"[bold]{username}[/bold] {value} text, {exists} skipped, {fails} failed"
     )
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/message.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/metadata.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,38 +26,41 @@
         if placeholderObj:
             if ele.id:
                 await operations.download_media_update(
                     ele,
                     filename=placeholderObj.trunicated_filepath,
                     model_id=model_id,
                     username=username,
-                    downloaded=metadata_downloaded_helper(placeholderObj),
+                    downloaded=await metadata_downloaded_helper(placeholderObj),
                 )
             return (
-                ele.mediatype
-                if metadata_downloaded_helper(placeholderObj)
-                else "forced_skipped",
+                (
+                    ele.mediatype
+                    if await metadata_downloaded_helper(placeholderObj)
+                    else "forced_skipped"
+                ),
                 0,
             )
         elif download_data and download_data.get("content-type"):
             content_type = download_data.get("content-type").split("/")[-1]
-            placeholderObj = placeholder.Placeholders(ele)
-            await placeholderObj.set_trunicated_filepath(ele, content_type)
+            placeholderObj = await placeholder.Placeholders(ele, content_type).init()
             if ele.id:
                 await operations.download_media_update(
                     ele,
                     filename=placeholderObj.trunicated_filepath,
                     model_id=model_id,
                     username=username,
-                    downloaded=metadata_downloaded_helper(placeholderObj),
+                    downloaded=await metadata_downloaded_helper(placeholderObj),
                 )
             return (
-                ele.mediatype
-                if metadata_downloaded_helper(placeholderObj)
-                else "forced_skipped",
+                (
+                    ele.mediatype
+                    if await metadata_downloaded_helper(placeholderObj)
+                    else "forced_skipped"
+                ),
                 0,
             )
         elif _ == 1:
             break
         else:
             try:
                 async for _ in AsyncRetrying(
@@ -80,18 +83,19 @@
                 )
                 common_globals.log.traceback_(
                     f"{get_medialog(ele)} Could not get placeholderObj {traceback.format_exc()}"
                 )
                 common_globals.log.debug(
                     f"{get_medialog(ele)} using a generic placeholderObj"
                 )
-                placeholderObj = await meta_data_placeholder(ele, username, model_id)
+                placeholderObj = await meta_data_placeholder(ele)
 
 
-def metadata_downloaded_helper(placeholderObj):
+async def metadata_downloaded_helper(placeholderObj):
+    placeholderObj = await placeholderObj.init()
     if read_args.retriveArgs().metadata == "none":
         return None
 
     elif read_args.retriveArgs().metadata == "complete":
         return 1
     elif pathlib.Path(placeholderObj.trunicated_filepath).exists():
         return 1
@@ -107,15 +111,15 @@
             "Policy": ele.policy,
             "Key-Pair-Id": ele.keypair,
             "Signature": ele.signature,
         }
         if ele.mpd
         else None
     )
-    common_globals.attempt.set(attempt.get(0) + 1)
+    common_globals.attempt.set(common_globals.attempt.get() + 1)
     common_globals.log.debug(
         f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}]  Getting data for metadata insert"
     )
     async with c.requests(url=url, headers=None, params=params)() as r:
         if r.ok:
             headers = r.headers
             await asyncio.get_event_loop().run_in_executor(
@@ -130,23 +134,25 @@
                 ),
             )
             content_type = headers.get("content-type").split("/")[-1]
             if not content_type and ele.mediatype.lower() == "videos":
                 content_type = "mp4"
             elif not content_type and ele.mediatype.lower() == "images":
                 content_type = "jpg"
-            placeholderObj = placeholderObj or placeholder.Placeholders(ele)
+            placeholderObj = await (
+                placeholderObj or placeholder.Placeholders(ele, ext=content_type)
+            ).init()
             return placeholderObj
 
         else:
             r.raise_for_status()
 
 
-async def meta_data_placeholder(ele, username, model_id):
+async def meta_data_placeholder(ele):
     if ele.mediatype.lower() == "videos":
         content_type = "mp4"
     elif ele.mediatype.lower() == "images":
         content_type = "jpg"
     elif ele.mediatype.lower() == "audios":
         content_type = "mp3"
-    placeholderObj = placeholder.Placeholders()
+    placeholderObj = await placeholder.Placeholders(ele, ext=content_type).init()
     return placeholderObj
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/paths.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/sem.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/sem.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/common/text.py` & `ofscraper-3.9.0.dev9/ofscraper/download/common/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/download.py` & `ofscraper-3.9.0.dev9/ofscraper/download/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,39 +8,53 @@
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.hash as hash
 import ofscraper.utils.separate as seperate
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.system as system
 from ofscraper.download.common.common import textDownloader
+from ofscraper.utils.context.run_async import run
 
 
 def medialist_filter(medialist, model_id, username):
     log = logging.getLogger("shared")
-    if not read_args.retriveArgs().dupe:
+    if read_args.retriveArgs().force_all:
+        log.info(f"forcing all downloads media count {len(medialist)}")
+    elif read_args.retriveArgs().force_model_unique:
+        log.info("Downloading unique for model")
         media_ids = set(
-            operations.get_media_ids_downloaded(model_id=model_id, username=username)
+            operations.get_media_ids_downloaded_model(
+                model_id=model_id, username=username
+            )
         )
         log.debug(
             f"Number of unique media ids in database for {username}: {len(media_ids)}"
         )
         medialist = seperate.separate_by_id(medialist, media_ids)
         log.debug(f"Number of new mediaids with dupe ids removed: {len(medialist)}")
         medialist = seperate.seperate_avatars(medialist)
         log.debug("Removed previously downloaded avatars/headers")
         log.debug(f"Final Number of media to download {len(medialist)}")
-
     else:
-        log.info(f"forcing all downloads media count {len(medialist)}")
+        log.info("Downloading unique across all models")
+        media_ids = set(
+            operations.get_media_ids_downloaded(model_id=model_id, username=username)
+        )
+        log.debug("Number of unique media ids in database for all models")
+        medialist = seperate.separate_by_id(medialist, media_ids)
+        log.debug(f"Number of new mediaids with dupe ids removed: {len(medialist)}")
+        medialist = seperate.seperate_avatars(medialist)
+        log.debug("Removed previously downloaded avatars/headers")
+        log.debug(f"Final Number of media to download {len(medialist)} ")
     return medialist
 
 
 def download_process(username, model_id, medialist, posts=None):
     medialist = medialist_filter(medialist, model_id, username)
-    medialist = helpers.post_count_filter(medialist)
+    medialist = helpers.ele_count_filter(medialist)
     textDownloader(posts, username=username)
     download_picker(username, model_id, medialist)
     remove_downloads_with_hashes(username, model_id)
 
 
 def download_picker(username, model_id, medialist):
     if len(medialist) == 0:
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.0.dev9/ofscraper/download/downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.0.dev9/ofscraper/download/downloadnormal.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import logging
 import traceback
 
 from humanfriendly import format_size
 from rich.live import Live
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/main_download.py` & `ofscraper-3.9.0.dev9/ofscraper/download/main_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import pathlib
 import traceback
 from functools import partial
 
 import aiofiles
 import arrow
@@ -51,15 +52,14 @@
     metadata,
     moveHelper,
     path_to_file_logger,
     sem_wrapper,
     set_profile_cache_helper,
     set_time,
     size_checker,
-    update_total,
 )
 
 
 async def main_download(c, ele, username, model_id, job_progress):
     common_globals.log.debug(f"{get_medialog(ele)} Downloading with normal downloader")
     common_globals.log.debug(f"{get_medialog(ele)} download url:  {get_url_log(ele)}")
     # total may be none if no .part file
@@ -122,35 +122,36 @@
         )
     await set_profile_cache_helper(ele)
     return ele.mediatype, total
 
 
 async def main_download_downloader(c, ele, job_progress):
     downloadspace(mediatype=ele.mediatype)
-    tempholderObj = placeholder.tempFilePlaceholder(
+    tempholderObj = await placeholder.tempFilePlaceholder(
         ele, f"{await ele.final_filename}_{ele.id}.part"
-    )
-    await tempholderObj.init()
+    ).init()
     async for _ in AsyncRetrying(
         stop=stop_after_attempt(constants.getattr("DOWNLOAD_RETRIES")),
         wait=wait_random(
             min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
         ),
         retry=retry_if_not_exception_message(
             constants.getattr("SPACE_DOWNLOAD_MESSAGE")
         ),
         reraise=True,
     ):
         with _:
             try:
                 data = await get_data(ele)
                 common_globals.attempt.set(common_globals.attempt.get(0) + 1)
-                pathlib.Path(tempholderObj.tempfilepath).unlink(
-                    missing_ok=True
-                ) if common_globals.attempt.get() > 1 else None
+                (
+                    pathlib.Path(tempholderObj.tempfilepath).unlink(missing_ok=True)
+                    if common_globals.attempt.get() > 1
+                    else None
+                )
                 if data:
                     return await main_data_handler(
                         data, c, tempholderObj, ele, job_progress
                     )
                 else:
                     return await alt_data_handler(c, tempholderObj, ele, job_progress)
             except OSError as E:
@@ -183,17 +184,16 @@
         raise E
     return result
 
 
 async def main_data_handler(data, c, tempholderObj, ele, job_progress):
     content_type = data.get("content-type").split("/")[-1]
     total = int(data.get("content-length"))
-    placeholderObj = placeholder.Placeholders(ele, content_type)
+    placeholderObj = await placeholder.Placeholders(ele, content_type).init()
     resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
-    await placeholderObj.init()
     # other
     if await check_forced_skip(ele, total) == 0:
         path_to_file_logger(placeholderObj, ele)
         return [0]
     elif total == resume_size:
         path_to_file_logger(placeholderObj, ele)
         return (
@@ -264,16 +264,17 @@
                             },
                         ),
                     )
                     new_total = int(r.headers["content-length"])
                     content_type = r.headers.get("content-type").split("/")[-1]
                     content_type = content_type or get_unknown_content_type(ele)
                     if not placeholderObj:
-                        placeholderObj = placeholder.Placeholders(ele, content_type)
-                        await placeholderObj.init()
+                        placeholderObj = await placeholder.Placeholders(
+                            ele, content_type
+                        ).init()
                     path_to_file_logger(placeholderObj, ele)
                     if await check_forced_skip(ele, new_total):
                         total = 0
                         await common.total_change_helper(old_total, total)
                     elif total == resume_size:
                         None
                     else:
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.0.dev9/ofscraper/download/main_downloadbatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import asyncio
 import pathlib
 import traceback
 from functools import partial
 
 import aiofiles
 import arrow
@@ -119,34 +120,35 @@
         )
     await set_profile_cache_helper(ele)
     return ele.mediatype, total
 
 
 async def main_download_downloader(c, ele):
     downloadspace(mediatype=ele.mediatype)
-    tempholderObj = placeholder.tempFilePlaceholder(
+    tempholderObj = await placeholder.tempFilePlaceholder(
         ele, f"{await ele.final_filename}_{ele.id}.part"
-    )
-    await tempholderObj.init()
+    ).init()
     async for _ in AsyncRetrying(
         stop=stop_after_attempt(constants.getattr("DOWNLOAD_RETRIES")),
         wait=wait_random(
             min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
         ),
         retry=retry_if_not_exception_message(
             constants.getattr("SPACE_DOWNLOAD_MESSAGE")
         ),
         reraise=True,
     ):
         with _:
             try:
                 common_globals.attempt.set(common_globals.attempt.get(0) + 1)
-                pathlib.Path(tempholderObj.tempfilepath).unlink(
-                    missing_ok=True
-                ) if common_globals.attempt.get() > 1 else None
+                (
+                    pathlib.Path(tempholderObj.tempfilepath).unlink(missing_ok=True)
+                    if common_globals.attempt.get() > 1
+                    else None
+                )
                 data = await get_data(ele)
                 if data:
                     return await main_data_handler(data, c, ele, tempholderObj)
                 else:
                     return await alt_data_handler(c, ele, tempholderObj)
 
             except OSError as E:
@@ -180,17 +182,16 @@
         raise E
     return result
 
 
 async def main_data_handler(data, c, ele, tempholderObj):
     content_type = data.get("content-type").split("/")[-1]
     total = int(data.get("content-length"))
-    placeholderObj = placeholder.Placeholders(ele, content_type)
+    placeholderObj = await placeholder.Placeholders(ele, content_type).init()
     resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
-    await placeholderObj.init()
     # other
     if await check_forced_skip(ele, total) == 0:
         path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
         return [0]
     elif total == resume_size:
         path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
         return (
@@ -248,16 +249,17 @@
                         ),
                     )
                     new_total = int(r.headers["content-length"])
                     content_type = r.headers.get("content-type").split("/")[
                         -1
                     ] or get_unknown_content_type(ele)
                     if not placeholderObj:
-                        placeholderObj = placeholder.Placeholders(ele, content_type)
-                        await placeholderObj.init()
+                        placeholderObj = await placeholder.Placeholders(
+                            ele, content_type
+                        ).init()
                     path_to_file_logger(
                         placeholderObj, ele, common_globals.innerlog.get()
                     )
                     if await check_forced_skip(ele, new_total) == 0:
                         total = 0
                         await common.batch_total_change_helper(old_total, total)
                         return (total, tempholderObj.tempfilepath, placeholderObj)
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/media/helpers.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/media/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             )
         )
     out.extend(undated)
     out.extend(dated)
     return out
 
 
-def post_count_filter(media):
+def ele_count_filter(media):
     count = settings.get_max_post_count() or None
     return media[:count]
 
 
 def posts_type_filter(media):
     filtersettings = settings.get_mediatypes()
     if isinstance(filtersettings, str):
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/media/main.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/media/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,17 +433,17 @@
         )
     )
     log.debug(f"filter{count}-> all post final sort count {len(post)}")
 
     return post
 
 
-def media_filter_for_like(media, like=False):
-    media = helpers.timeline_array_filter(media)
+def post_filter_for_like(media, like=False):
+    media = helpers.post_timed_filter(media)
     post_type = "likable" if like else "unlikable"
     log.debug(
         f"[bold]Number of {post_type} posts left after date filter[/bold] {len(media)}"
     )
     media = helpers.final_post_sort(media)
-    media = helpers.post_count_filter(media)
+    media = helpers.ele_count_filter(media)
     log.debug(f"[bold]Final Number of open and {post_type} post[/bold] {len(media)}")
     return media
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/models/date.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/models/flags.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/models/other.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/models/price.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/models/sort.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.0.dev9/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/models/retriver.py` & `ofscraper-3.9.0.dev9/ofscraper/models/retriver.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,65 +6,65 @@
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.console as console
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.me as me_util
 
 
-def get_models() -> list:
+async def get_models() -> list:
     """
     Get user's subscriptions in form of a list.
     """
     with stdout.lowstdout():
         count = get_sub_count()
-        if not bool(read_args.retriveArgs().username):
-            return get_via_list(count)
-        elif "ALL" in read_args.retriveArgs().username:
-            return get_via_list(count)
+        if not bool(read_args.retriveArgs().usernames):
+            return await get_via_list(count)
+        elif "ALL" in read_args.retriveArgs().usernames:
+            return await get_via_list(count)
         elif read_args.retriveArgs().individual:
-            return get_via_individual()
+            return await get_via_individual()
         elif read_args.retriveArgs().list:
             return get_via_list(count)
-        elif (sum(count) // 10) > len(read_args.retriveArgs().username):
-            return get_via_individual()
+        elif (sum(count) // 10) > len(read_args.retriveArgs().usernames):
+            return await get_via_individual()
         else:
-            return get_via_list(count)
+            return await get_via_list(count)
 
 
-def get_via_list(count):
+async def get_via_list(count):
     out = []
-    active_subscriptions = subscriptions.get_subscriptions(count[0])
-    expired_subscriptions = subscriptions.get_subscriptions(count[1], account="expired")
+    active_subscriptions = await subscriptions.get_subscriptions(count[0])
+    expired_subscriptions = await subscriptions.get_subscriptions(count[1], account="expired")
     console.get_shared_console().print(
         "[yellow]Warning: Numbering on OF site can be iffy\nExample Including deactived accounts in expired\nSee: https://of-scraper.gitbook.io/of-scraper/faq#number-of-users-doesnt-match-account-number[/yellow]"
     )
 
     other_subscriptions = lists.get_otherlist()
     out.extend(active_subscriptions)
     out.extend(expired_subscriptions)
     out.extend(other_subscriptions)
     black_list = lists.get_blacklist()
     out = list(filter(lambda x: x.get("id") not in black_list, out))
     models_objects = list(map(lambda x: models.Model(x), out))
     return models_objects
 
 
-def get_main_list(count):
+async def get_main_list(count):
     out = []
-    active_subscriptions = subscriptions.get_subscriptions(count[0], forced=True)
-    expired_subscriptions = subscriptions.get_subscriptions(
+    active_subscriptions = await subscriptions.get_subscriptions(count[0], forced=True)
+    expired_subscriptions = await subscriptions.get_subscriptions(
         count[1], account="expired", forced=True
     )
     out.extend(active_subscriptions)
     out.extend(expired_subscriptions)
     return out
 
 
-def get_via_individual():
-    out = individual.get_subscription()
+async def get_via_individual():
+    out = await individual.get_subscription()
     console.get_shared_console().print(
         "[yellow]Warning: Numbering on OF site can be iffy\nExample Including deactived accounts in expired\nSee: https://of-scraper.gitbook.io/of-scraper/faq#number-of-users-doesnt-match-account-number[/yellow]"
     )
     models_objects = list(map(lambda x: models.Model(x), out))
     if len(models_objects) == 0:
         raise Exception("Provided usernames with did not yield any valid models")
     return models_objects
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/models/selector.py` & `ofscraper-3.9.0.dev9/ofscraper/models/selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.args.user as user_helper
 import ofscraper.utils.args.write as write_args
 import ofscraper.utils.constants as constants
 import ofscraper.utils.manager as manager
 import ofscraper.utils.settings as settings
+from ofscraper.utils.context.run_async import run
 
 ALL_SUBS = None
 PARSED_SUBS = None
 ALL_SUBS_DICT = None
 log = logging.getLogger("shared")
 
 
@@ -51,15 +52,15 @@
 
 def get_ALL_SUBS():
     global ALL_SUBS
     return ALL_SUBS
 
 
 def get_ALL_SUBS_DICTVManger():
-    return manager.get_manager_dict().get("subs")
+    return manager.get_manager_process_dict().get("subs")
 
 
 def getselected_usernames(rescan=False, reset=False):
     # username list will be retrived every time resFet==True
     global ALL_SUBS
     global PARSED_SUBS
     if reset == True and rescan == True:
@@ -80,20 +81,22 @@
         parsed_subscriptions_helper()
     else:
         all_subs_helper(refetch=False)
         parsed_subscriptions_helper()
     return PARSED_SUBS
 
 
-def all_subs_helper(refetch=True, main=False, check=True):
+
+@run
+async def all_subs_helper(refetch=True, main=False, check=True):
     global ALL_SUBS
     if bool(ALL_SUBS) and not refetch:
         return
     while True:
-        ALL_SUBS = retriver.get_models()
+        ALL_SUBS = await retriver.get_models()
         if len(ALL_SUBS) > 0 or not check:
             set_ALL_SUBS_DICTVManger(subsDict=ALL_SUBS)
             break
         elif len(ALL_SUBS) == 0:
             print("No accounts found during scan")
             # give log time to process
             time.sleep(constants.getattr("LOG_DISPLAY_TIMEOUT"))
@@ -102,25 +105,25 @@
 
 
 def parsed_subscriptions_helper(reset=False):
     global ALL_SUBS
     global PARSED_SUBS
     args = read_args.retriveArgs()
     if reset == True:
-        args.username = None
+        args.usernames = None
         write_args.setArgs(args)
-    if not bool(args.username):
+    if not bool(args.usernames):
         selectedusers = retriver.get_selected_model(filterNSort())
-        read_args.retriveArgs().username = list(map(lambda x: x.name, selectedusers))
+        read_args.retriveArgs().usernames = list(map(lambda x: x.name, selectedusers))
         PARSED_SUBS = selectedusers
         write_args.setArgs(args)
-    elif "ALL" in args.username:
+    elif "ALL" in args.usernames:
         PARSED_SUBS = filterNSort()
-    elif args.username:
-        usernameset = set(args.username)
+    elif args.usernames:
+        usernameset = set(args.usernames)
         PARSED_SUBS = list(filter(lambda x: x.name in usernameset, ALL_SUBS))
     return PARSED_SUBS
 
 
 def setfilter(forced=False):
     global args
     while True:
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/area.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 from InquirerPy.base import Choice
 from prompt_toolkit.shortcuts import prompt as prompt
 
 import ofscraper.prompts.prompt_strings as prompt_strings
 import ofscraper.prompts.prompt_validators as prompt_validators
 import ofscraper.prompts.promptConvert as promptClasses
 import ofscraper.utils.args.areas as areas
@@ -22,17 +23,19 @@
 
 def areas_prompt() -> list:
     args = read_args.retriveArgs()
     name = "value"
     message = (
         "Which area(s) would you do you want to download and like"
         if "like" in args.action and len(args.like_area) == 0
-        else "Which area(s) would you want to download and unlike"
-        if "unike" in args.action and len(args.like_area) == 0
-        else "Which area(s) would you like to download"
+        else (
+            "Which area(s) would you want to download and unlike"
+            if "unike" in args.action and len(args.like_area) == 0
+            else "Which area(s) would you like to download"
+        )
     )
     more_instruction = (
         """Hint: Since you have Like or Unlike set
 You must select one or more of Timeline,Pinned,Archived, or Label
 """
         if ("like" or "unlike") in args.action and len(args.like_area) == 0
         else ""
@@ -142,15 +145,15 @@
     answer = promptClasses.batchConverter(
         *[
             {
                 "type": "list",
                 "name": name,
                 "message": "Do you want to reset selected area(s)",
                 "choices": [
-                    Choice("Download", "Download area only"),
+                    Choice("Download", "Download area only + Scrape Paid"),
                     Choice("Like", "Like area only"),
                     "Both",
                     "No",
                 ],
                 "default": "No",
                 "long_instruction": "like area is used for like and unlike\ndownload area is used for download",
             }
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import sys
 
 from InquirerPy.base import Choice
 from InquirerPy.separator import Separator
 from InquirerPy.validator import EmptyInputValidator
 from prompt_toolkit.shortcuts import prompt as prompt
 from rich.console import Console
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import copy
 import json
 import logging
 import os
 import re
 import sys
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import json
 import logging
 import os
 
 from InquirerPy.base import Choice
 from InquirerPy.separator import Separator
 from InquirerPy.validator import EmptyInputValidator, PathValidator
@@ -483,17 +484,19 @@
             },
             # value because of legacy config values
             {
                 "type": "input",
                 "name": "custom",
                 "message": "edit custom value:\n",
                 "option_instruction": "This is a helper value for remapping placeholder values",
-                "default": json.dumps(custom.get_custom())
-                if not isinstance(custom.get_custom(), str)
-                else custom.get_custom() or "",
+                "default": (
+                    json.dumps(custom.get_custom())
+                    if not isinstance(custom.get_custom(), str)
+                    else custom.get_custom() or ""
+                ),
             },
             {
                 "type": "list",
                 "name": "downloadbars",
                 "message": "show download progress bars\nThis can have a negative effect on performance with lower threads",
                 "default": data.get_show_downloadprogress(),
                 "choices": [Choice(True, "Yes"), Choice(False, "No")],
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 from InquirerPy.separator import Separator
 from prompt_toolkit.shortcuts import prompt as prompt
 
 import ofscraper.prompts.promptConvert as promptClasses
 import ofscraper.utils.constants as constants
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import inspect
 
 import arrow
 from InquirerPy.base import Choice
 from InquirerPy.separator import Separator
 from prompt_toolkit.shortcuts import prompt as prompt
 from rich.console import Console
@@ -78,34 +79,34 @@
 
 def modify_subtype_prompt(args):
     answer = promptClasses.batchConverter(
         *[
             {
                 "type": "list",
                 "name": "renewal",
-                "default": True
-                if read_args.retriveArgs().renewal
-                else False
-                if read_args.retriveArgs().renewal == False
-                else None,
+                "default": (
+                    True
+                    if read_args.retriveArgs().renewal
+                    else False if read_args.retriveArgs().renewal == False else None
+                ),
                 "message": "Filter account by whether it has a renewal date",
                 "choices": [
                     Choice(True, "Renewal On"),
                     Choice(False, "Renewal Off"),
                     Choice(None, "Both"),
                 ],
             },
             {
                 "type": "list",
                 "name": "expire",
-                "default": True
-                if read_args.retriveArgs().sub_status
-                else False
-                if read_args.retriveArgs().sub_status == False
-                else None,
+                "default": (
+                    True
+                    if read_args.retriveArgs().sub_status
+                    else False if read_args.retriveArgs().sub_status == False else None
+                ),
                 "message": "Filter accounts based on access to content via a subscription",
                 "choices": [
                     Choice(True, "Active Only"),
                     Choice(False, "Expired Only"),
                     Choice(None, "Both"),
                 ],
             },
@@ -136,33 +137,37 @@
                 "name": "last-seen-after",
                 "message": "Filter accounts by last seen being after the given date",
                 "option_instruction": """enter 0 to disable this filter
                 Otherwise must be in date format
                 """,
                 "validate": prompt_validators.datevalidator(),
                 "filter": lambda x: arrow.get(x or 0),
-                "default": arrow.get(read_args.retriveArgs().last_seen_after).format(
-                    constants.getattr("PROMPT_DATE_FORMAT")
-                )
-                if read_args.retriveArgs().last_seen_after
-                else "",
+                "default": (
+                    arrow.get(read_args.retriveArgs().last_seen_after).format(
+                        constants.getattr("PROMPT_DATE_FORMAT")
+                    )
+                    if read_args.retriveArgs().last_seen_after
+                    else ""
+                ),
             },
             {
                 "type": "input",
                 "name": "last-seen-before",
                 "message": "Filter accounts by last seen being before the given date",
                 "option_instruction": """enter 0 to disable this filter
                 Otherwise must be in date format""",
                 "validate": prompt_validators.datevalidator(),
                 "filter": lambda x: arrow.get(x or 0),
-                "default": arrow.get(read_args.retriveArgs().last_seen_before).format(
-                    constants.getattr("PROMPT_DATE_FORMAT")
-                )
-                if read_args.retriveArgs().last_seen_before
-                else "",
+                "default": (
+                    arrow.get(read_args.retriveArgs().last_seen_before).format(
+                        constants.getattr("PROMPT_DATE_FORMAT")
+                    )
+                    if read_args.retriveArgs().last_seen_before
+                    else ""
+                ),
             },
         ],
         more_instructions="""
         \n
         --last-seen filters by visiblity of 'last seen' value
         in contrast to [--last-seen-after/--last-seen-before]
         which both use a the current time if model hides 'last seen'""",
@@ -196,19 +201,19 @@
         )
 
     free_trail = promptClasses.batchConverter(
         *[
             {
                 "type": "list",
                 "name": "free-trial",
-                "default": True
-                if read_args.retriveArgs().free_trial == True
-                else False
-                if read_args.retriveArgs().free_trial == False
-                else None,
+                "default": (
+                    True
+                    if read_args.retriveArgs().free_trial == True
+                    else False if read_args.retriveArgs().free_trial == False else None
+                ),
                 "message": "Filter Accounts By whether the account is a free trial",
                 "choices": [
                     Choice(True, "Free Trial only"),
                     Choice(False, "Paid and always free accounts"),
                     Choice(None, "Any Account"),
                 ],
             },
@@ -223,19 +228,19 @@
         )
         promo = promptClasses.batchConverter(
             *[
                 {
                     "type": "list",
                     "name": "promo",
                     "message": "Which kind of promo(s) do you want to enable",
-                    "default": True
-                    if read_args.retriveArgs().promo
-                    else False
-                    if read_args.retriveArgs().promo == False
-                    else None,
+                    "default": (
+                        True
+                        if read_args.retriveArgs().promo
+                        else False if read_args.retriveArgs().promo == False else None
+                    ),
                     "choices": [
                         Choice({"all_promo": True, "promo": True}, "Any Promo"),
                         Choice(
                             {"all_promo": None, "promo": True}, "Claimable Promo Only"
                         ),
                     ],
                 },
@@ -264,19 +269,23 @@
         )["promo"]
         promo = promptClasses.batchConverter(
             *[
                 {
                     "type": "list",
                     "name": promo_type,
                     "message": f"Filter accounts presence of {'Any Promotions' if promo_type=='all_promo' else 'Claimable Promotions'}",
-                    "default": True
-                    if vars(read_args.retriveArgs())[promo_type]
-                    else False
-                    if vars(read_args.retriveArgs())[promo_type] == False
-                    else None,
+                    "default": (
+                        True
+                        if vars(read_args.retriveArgs())[promo_type]
+                        else (
+                            False
+                            if vars(read_args.retriveArgs())[promo_type] == False
+                            else None
+                        )
+                    ),
                     "choices": [
                         Choice(True, "Promotions Only"),
                         Choice(False, "No Promotions"),
                         Choice(None, "Both"),
                     ],
                 },
             ]
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 from InquirerPy.separator import Separator
 from InquirerPy.validator import EmptyInputValidator
 from prompt_toolkit.shortcuts import prompt as prompt
 
 import ofscraper.prompts.prompt_validators as prompt_validators
 import ofscraper.prompts.promptConvert as promptClasses
 import ofscraper.utils.constants as constants
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/prompts/prompts.py` & `ofscraper-3.9.0.dev9/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/runner/exit.py` & `ofscraper-3.9.0.dev9/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/runner/load.py` & `ofscraper-3.9.0.dev9/ofscraper/runner/load.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         setdate()
         readConfig()
         setLogger()
         make_folder()
         check()
         run.main()
     except Exception as E:
+        print(E)
+        print(traceback.format_exc())
         try:
             logging.getLogger("shared").debug(traceback.format_exc())
             logging.getLogger("shared").debug(E)
         except Exception as E:
             print(E)
             print(traceback.format_exc())
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/runner/run.py` & `ofscraper-3.9.0.dev9/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/actions.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.args.areas as areas
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.args.write as write_args
 import ofscraper.utils.system.free as free
 
 
@@ -38,28 +39,28 @@
     if "download" in action and reset:
         reset_download()
     elif ("like" or "unlike") in action and reset:
         reset_like()
     write_args.setArgs(args)
     set_post_area(action)
     set_download_area(action)
-    set_scrape_paid(action)
     set_like_area(action)
     remove_post_area()
 
 
 def remove_like_area():
     args = read_args.retriveArgs()
     args.like_area = {}
     write_args.setArgs(args)
 
 
 def remove_download_area():
     args = read_args.retriveArgs()
     args.download_area = {}
+    args.scrape_paid = None
     write_args.setArgs(args)
 
 
 def remove_post_area():
     args = read_args.retriveArgs()
     args.posts = {}
     write_args.setArgs(args)
@@ -110,10 +111,10 @@
 
 def set_scrape_paid(action=None):
     args = read_args.retriveArgs()
     action = action or args.action or {}
     if "download" not in action:
         return
     args.scrape_paid = (
-        prompts.scrape_paid_prompt() if args.scrape_paid != None else args.scrape_paid
+        prompts.scrape_paid_prompt() if not args.scrape_paid else args.scrape_paid
     )
     write_args.setArgs(args)
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/args/areas.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/args/areas.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 def get_like_area():
     post = None
     all_choices = [
         "Archived",
         "Timeline",
         "Pinned",
     ]
-    all_choices.append("Label") if const.getattr("INCLUDED_LABELS_ALL") else None
+    all_choices.append("Label") if const.getattr("INCLUDE_LABELS_ALL") else None
     if len(read_args.retriveArgs().like_area) == 0:
         post = set(read_args.retriveArgs().posts)
     else:
         post = set(read_args.retriveArgs().like_area)
     if "All" in post:
         post.update(set(all_choices))
     elif ("Labels*" or "Labels+") in post:
         post.update(set(all_choices))
         post.update({"Labels"})
         post.discard("Labels*")
-        post.discard("Laabels+")
+        post.discard("Labels+")
     return list(
         filter(
             lambda x: x != "All"
             and x[0] != "-"
             and f"-{x}" not in post
-            and x in all_choices,
+            and x in all_choices + ["Labels"],
             post,
         )
     )
 
 
 def get_download_area():
     post = None
@@ -40,15 +40,15 @@
         "Messages",
         "Timeline",
         "Pinned",
         "Stories",
         "Purchased",
         "Profile",
     ]
-    all_choices.append("Label") if const.getattr("INCLUDED_LABELS_ALL") else None
+    all_choices.append("Label") if const.getattr("INCLUDE_LABELS_ALL") else None
     if len(read_args.retriveArgs().download_area) == 0:
         post = set(read_args.retriveArgs().posts)
     else:
         post = set(read_args.retriveArgs().download_area)
     if "All" in post:
         post.update(set(all_choices))
     elif ("Labels*" or "Labels+") in post:
@@ -57,11 +57,11 @@
         post.discard("Labels*")
         post.discard("Laabels+")
     return list(
         filter(
             lambda x: x != "All"
             and x[0] != "-"
             and f"-{x}" not in post
-            and x in all_choices,
+            and x in all_choices + ["Labels"],
             post,
         )
     )
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/args/read.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/args/read.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import ofscraper.utils.args.globals as global_args
 import ofscraper.utils.args.parse as parse_args
 import ofscraper.utils.manager as manager
 
 
 def retriveArgsVManager():
     try:
-        if not manager.get_manager_dict().get("args"):
-            manager.get_manager_dict()["args"] = parse_args.parse_args()
-        return manager.get_manager_dict().get("args")
+        if not manager.get_manager_process_dict().get("args"):
+            manager.get_manager_process_dict()["args"] = parse_args.parse_args()
+        return manager.get_manager_process_dict().get("args")
     except SystemExit as E:
         if not any(ele in sys.argv[1:] for ele in ["-h", "-v"]):
             print(f"Passed Args {sys.argv[1:]}")
         raise E
 
 
 def retriveArgs():
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/auth/context.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/auth/data.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/auth/file.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/auth/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import json
 import logging
 
 import browser_cookie3
 import requests
 from rich.console import Console
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/auth/make.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/auth/request.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/auth/request.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/binaries.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/cache.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/checkers.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/config/config.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
+
 import logging
 
 from humanfriendly import parse_size
 
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.binaries as binaries
 import ofscraper.utils.config.context as config_context
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/config/context.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/config/data.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/config/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/config/file.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/config/menu.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/config/schema.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/config/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import ofscraper.utils.paths.common as common_paths
 
 
 def get_current_config_schema(config: dict = None) -> dict:
     if isinstance(config, dict) and config.get("config"):
         config = config["config"]
     new_config = {
-        "main_profile"
-        if config == False
-        else constants.getattr("mainProfile"): data.get_main_profile(config=config),
+        (
+            "main_profile" if config == False else constants.getattr("mainProfile")
+        ): data.get_main_profile(config=config),
         "metadata": data.get_metadata(config=config),
         "discord": data.get_discord(config=config),
         "file_options": {
             "save_location": common_paths.get_save_location(config=config),
             "dir_format": data.get_dirformat(config=config),
             "file_format": data.get_fileformat(config=config),
             "textlength": data.get_textlength(config=config),
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/context/exit.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/dates.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/encoding.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/hash.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/hash.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/logs/classes.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/logs/close.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/logs/other.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/menu.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from contextlib import contextmanager
 
 import ofscraper.actions.process as process_actions
 import ofscraper.models.selector as userselector
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.actions as actions
 import ofscraper.utils.auth.file as auth_file
-import ofscraper.utils.checkers as checkers
 import ofscraper.utils.config.menu as config_menu
 import ofscraper.utils.profiles.manage as profiles_manage
 import ofscraper.utils.profiles.tools as profile_tools
 import ofscraper.utils.run as run
 
 log = logging.getLogger("shared")
 count = 0
@@ -35,14 +34,15 @@
             action_result_prompt = prompts.action_prompt()
             if action_result_prompt == "quit":
                 return True
             elif action_result_prompt == "main":
                 continue
             else:
                 count > 0 and reset_menu_helper()
+                actions.set_scrape_paid()
                 functs = process_actions.add_selected_areas()
                 run.run_helper(*functs)
                 count = count + 1
         elif result_main_prompt == "auth":
             # Edit `auth.json` file
             auth_result_prompt = auth_file.edit_auth()
             if auth_result_prompt == "quit":
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/paths/check.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/paths/common.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/paths/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/run.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/separate.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/settings.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,7 +134,13 @@
 
 def get_ffmpeg():
     return (
         config_data.get_ffmpeg()
         or shutil.which(constants.getattr("FFMPEG_DECRYPT"))
         or ""
     )
+
+
+def get_after_enabled():
+    return (
+        read_args.retriveArgs().after is not None or not config_data.get_disable_after()
+    )
```

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/system/network.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/system/system.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev7/ofscraper/utils/text.py` & `ofscraper-3.9.0.dev9/ofscraper/utils/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,15 @@
             return
         elif bool(ele.text) == False:
             return
         # make new text mediatype
         new_ele = copy.deepcopy(ele)
         new_ele.mediatype = "text"
 
-        placeholderObj = placeholder.Textholders(new_ele, "txt")
-        await placeholderObj.init()
+        placeholderObj = await placeholder.Textholders(new_ele, "txt").init()
         if pathlib.Path(placeholderObj.filepath).exists() and not dupe:
             return "exists"
         wrapped_text = textwrap.wrap(
             new_ele.text, width=constants.getattr("MAX_TEXT_LENGTH")
         )
         async with aiofiles.open(placeholderObj.filepath, "w") as p:
             await p.writelines(wrapped_text)
```

### Comparing `ofscraper-3.9.0.dev7/pyproject.toml` & `ofscraper-3.9.0.dev9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.0dev7"
+version = "3.9.0dev9"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
 
@@ -42,14 +42,15 @@
 aiosqlite = "^0.20.0"
 speedtest-cli = "^2.1.3"
 prompt-toolkit = "^3.0.43"
 setproctitle = "^1.3.3"
 lxml = "^5.1.0"
 multiprocess = "^0.70.16"
 dill = "^0.3.8"
+cloup = "^3.0.5"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
```

### Comparing `ofscraper-3.9.0.dev7/PKG-INFO` & `ofscraper-3.9.0.dev9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.0.dev7
+Version: 3.9.0.dev9
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,14 +13,15 @@
 Requires-Dist: aiohttp[speedups] (>=3.8.5,<4.0.0)
 Requires-Dist: aioprocessing (>=2.0.1,<3.0.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: arrow (>=1.3.0,<2.0.0)
 Requires-Dist: browser-cookie3 (==0.19.1)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: certifi (>=2024.2.2,<2025.0.0)
+Requires-Dist: cloup (>=3.0.5,<4.0.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: dunamai (>=1.19.2,<2.0.0)
 Requires-Dist: faust-cchardet (>=2.1.19,<3.0.0)
 Requires-Dist: filelock (>=3.13.1,<4.0.0)
 Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: humanfriendly (>=10.0,<11.0)
@@ -64,16 +65,16 @@
 <img src="https://img.shields.io/pypi/v/ofscraper.svg?color=dark_green&label=Stable-Release" alt="drawing" style="height:75px"/>
 </div>
 </a>
 
 ## Dev
 
 <div style="display: inline-block">
-<a href="https://pypi.org/project/ofscraper/3.7.0.dev2/">
-<img src="https://img.shields.io/badge/Pre--Release-v3.70.dev-dark_green.svg" alt="drawing" style="height:75px"/>
+<a href="https://pypi.org/project/ofscraper/3.9.0.dev5/">
+<img src="https://img.shields.io/badge/Pre--Release-v3.90.dev-dark_green.svg" alt="drawing" style="height:75px"/>
 </a>
 </div>
 
 # Table-of-contents
 
 - [Description](#description)
 - [Documentation](#documentation)
@@ -112,14 +113,19 @@
     </li>
 </ol>
 
 # Issues
 
 Open a issue in this repo, or you can mention your issue in the [Discord](#discord)
 
+## Private Reports
+
+A ticket can be created in the ticket channel
+only you and admins have access to ticket discussions
+
 # Feature Requests
 
 [ClearFlask Feedback](https://ofscraper.clearflask.com/feedback) or [Discord](#discord)
 
 # Migrating from DC script
 
 To maintain compatibility with your current folders, make sure to modify the metadata option within the config file. Additionally, configure the save_path, dir_path, and filename settings to generate outputs that align with your existing setup.
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.0.dev7 Summary:
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.0.dev9 Summary:
 automatically scrape onlyfans Author: datawhores Author-email:
 datawhores@riseup.net Requires-Python: >=3.11,<3.14 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: pyinstaller
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aiohttp[speedups]
 (>=3.8.5,<4.0.0) Requires-Dist: aioprocessing (>=2.0.1,<3.0.0) Requires-Dist:
 aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-
 Dist: browser-cookie3 (==0.19.1) Requires-Dist: bs4 (>=0.0.2,<0.0.3) Requires-
-Dist: certifi (>=2024.2.2,<2025.0.0) Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: diskcache (>=5.6.3,<6.0.0) Requires-Dist: dunamai
-(>=1.19.2,<2.0.0) Requires-Dist: faust-cchardet (>=2.1.19,<3.0.0) Requires-
-Dist: filelock (>=3.13.1,<4.0.0) Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
-Requires-Dist: humanfriendly (>=10.0,<11.0) Requires-Dist: inquirerpy
-(>=0.3.4,<0.4.0) Requires-Dist: lxml (>=5.1.0,<6.0.0) Requires-Dist: more-
-itertools (>=10.2.0,<11.0.0) Requires-Dist: mpegdash (>=0.4.0,<0.5.0) Requires-
-Dist: multiprocess (>=0.70.16,<0.71.0) Requires-Dist: pathvalidate
-(>=3.2.0,<4.0.0) Requires-Dist: poetry-dynamic-versioning (>=1.2.0,<2.0.0)
-Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0) Requires-Dist: psutil
-(>=5.9.8,<6.0.0) Requires-Dist: pycryptodome (>=3.20.0,<4.0.0) Requires-Dist:
-pywidevine (>=1.8.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: schedule (>=1.2.1,<2.0.0)
+Dist: certifi (>=2024.2.2,<2025.0.0) Requires-Dist: cloup (>=3.0.5,<4.0.0)
+Requires-Dist: dill (>=0.3.8,<0.4.0) Requires-Dist: diskcache (>=5.6.3,<6.0.0)
+Requires-Dist: dunamai (>=1.19.2,<2.0.0) Requires-Dist: faust-cchardet
+(>=2.1.19,<3.0.0) Requires-Dist: filelock (>=3.13.1,<4.0.0) Requires-Dist:
+httpx[http2] (>=0.27.0,<0.28.0) Requires-Dist: humanfriendly (>=10.0,<11.0)
+Requires-Dist: inquirerpy (>=0.3.4,<0.4.0) Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: more-itertools (>=10.2.0,<11.0.0) Requires-Dist: mpegdash
+(>=0.4.0,<0.5.0) Requires-Dist: multiprocess (>=0.70.16,<0.71.0) Requires-Dist:
+pathvalidate (>=3.2.0,<4.0.0) Requires-Dist: poetry-dynamic-versioning
+(>=1.2.0,<2.0.0) Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0) Requires-Dist:
+psutil (>=5.9.8,<6.0.0) Requires-Dist: pycryptodome (>=3.20.0,<4.0.0) Requires-
+Dist: pywidevine (>=1.8.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: schedule (>=1.2.1,<2.0.0)
 Requires-Dist: setproctitle (>=1.3.3,<2.0.0) Requires-Dist: setuptools
 (>=69.1.1,<70.0.0) Requires-Dist: speedtest-cli (>=2.1.3,<3.0.0) Requires-Dist:
 tenacity (>=8.2.3,<9.0.0) Requires-Dist: textual (==0.52.1) Requires-Dist:
 uvloop (>=0.19.0,<0.20.0) ; sys_platform == "linux" or sys_platform == "linux2"
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0) Requires-Dist: xxhash
 (>=3.4.1,<4.0.0) Project-URL: Homepage, https://github.com/datawhores/OF-
 Scraper Description-Content-Type: text/markdown # Releases [Releases Page]
@@ -57,26 +57,27 @@
       any way. We are not authorized, endorsed, or sponsored by OnlyFans. All
       OnlyFans trademarks remain the property of Fenix International Limited.
    2. This is a theoritical program only and is for educational purposes. If
       you choose to use it then it may or may not work. You solely accept full
       responsability and indemnify the creator, hostors, contributors and all
       other involved persons from any any all responsability.
 # Issues Open a issue in this repo, or you can mention your issue in the
-[Discord](#discord) # Feature Requests [ClearFlask Feedback](https://
-ofscraper.clearflask.com/feedback) or [Discord](#discord) # Migrating from DC
-script To maintain compatibility with your current folders, make sure to modify
-the metadata option within the config file. Additionally, configure the
-save_path, dir_path, and filename settings to generate outputs that align with
-your existing setup. The inherited metadata files from DIGITALCRIMINALS' script
-play a crucial role in preventing redundant downloads by acting as a check for
-duplicates. For comprehensive guidance on making these adjustments, you can
-refer to the provided resources 1. [Migration Guide](https://of-
-scraper.gitbook.io/of-scraper/migrating-from-digitalcriminals-script) 2.
-[Config Options](https://of-scraper.gitbook.io/of-scraper/config-options) 3.
-[Customize Save Path](https://of-scraper.gitbook.io/of-scraper/config-options/
-customizing-save-path) Ask in the discord or open an issue if you need help
-with what to change to accomplish this # Discord [Discord](https://discord.gg/
-wN7uxEVHRK) # Support buymeacoffee.com/datawhores BTC:
-bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87 ETH:
+[Discord](#discord) ## Private Reports A ticket can be created in the ticket
+channel only you and admins have access to ticket discussions # Feature
+Requests [ClearFlask Feedback](https://ofscraper.clearflask.com/feedback) or
+[Discord](#discord) # Migrating from DC script To maintain compatibility with
+your current folders, make sure to modify the metadata option within the config
+file. Additionally, configure the save_path, dir_path, and filename settings to
+generate outputs that align with your existing setup. The inherited metadata
+files from DIGITALCRIMINALS' script play a crucial role in preventing redundant
+downloads by acting as a check for duplicates. For comprehensive guidance on
+making these adjustments, you can refer to the provided resources 1. [Migration
+Guide](https://of-scraper.gitbook.io/of-scraper/migrating-from-
+digitalcriminals-script) 2. [Config Options](https://of-scraper.gitbook.io/of-
+scraper/config-options) 3. [Customize Save Path](https://of-scraper.gitbook.io/
+of-scraper/config-options/customizing-save-path) Ask in the discord or open an
+issue if you need help with what to change to accomplish this # Discord
+[Discord](https://discord.gg/wN7uxEVHRK) # Support buymeacoffee.com/datawhores
+BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87 ETH:
 0x1d427a6E336edF6D95e589C16cb740A1372F6609 [![codecov](https://codecov.io/gh/
 datawhores/OF-Scraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://
 codecov.io/gh/datawhores/OF-Scraper)
```


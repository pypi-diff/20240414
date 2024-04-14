# Comparing `tmp/xklb-2.6.6.tar.gz` & `tmp/xklb-2.6.7.tar.gz`

## Comparing `xklb-2.6.6.tar` & `xklb-2.6.7.tar`

### file list

```diff
@@ -1,123 +1,124 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.6/.gitattributes
--rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.6/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/__init__.py
--rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/db_playlists.py
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/dl_extract.py
--rw-r--r--   0        0        0    15664 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/fs_extract.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/gdl_extract.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/history.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/hn_extract.py
--rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/lb.py
--rw-r--r--   0        0        0    19486 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/play_actions.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/post_actions.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/readme.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/reddit_extract.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/rss_extract.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/search.py
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/site_extract.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tabs_actions.py
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tabs_extract.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tube_backend.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tube_extract.py
--rw-r--r--   0        0        0   118259 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/__init__.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/av.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/books.py
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/dedupe.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/media_check.py
--rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/media_player.py
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/media_printer.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/subtitle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/add_row.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/big_dirs.py
--rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/block.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/christen.py
--rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/dedupe_czkawka.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/eda.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/export_text.py
--rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/history.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/incremental_diff.py
--rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/links_db.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mcda.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/merge_folders.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/move_list.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/open_links.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/process_ffmpeg.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/process_image.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/rel_mv.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/sample_compare.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/sample_hash.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/search_db.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/extract_text.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/markdown_links.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/substack.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/tildes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/__init__.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    17735 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/consts.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/devices.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/nums.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/objects.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/printing.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/processes.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/strings.py
--rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/web.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.6/.gitignore
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.6/pyproject.toml
--rw-r--r--   0        0        0   158230 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/README.md
--rw-r--r--   0        0        0   161991 2020-02-02 00:00:00.000000 xklb-2.6.6/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.7/.gitattributes
+-rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.7/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/__init__.py
+-rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/db_playlists.py
+-rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/dl_extract.py
+-rw-r--r--   0        0        0    15664 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/fs_extract.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/gdl_extract.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/history.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/hn_extract.py
+-rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/lb.py
+-rw-r--r--   0        0        0    19486 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/play_actions.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/post_actions.py
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/readme.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/reddit_extract.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/rss_extract.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/search.py
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/site_extract.py
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tube_extract.py
+-rw-r--r--   0        0        0   118259 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/__init__.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/av.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/books.py
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/dedupe.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/media_check.py
+-rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/media_player.py
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/media_printer.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/subtitle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/add_row.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/big_dirs.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/christen.py
+-rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/dedupe_czkawka.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/eda.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/export_text.py
+-rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/history.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/incremental_diff.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/links_db.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mcda.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/merge_folders.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/open_links.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/process_ffmpeg.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/process_image.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/rel_mv.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/sample_compare.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/sample_hash.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/search_db.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/extract_text.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/markdown_links.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/substack.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/tildes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    17780 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/processes.py
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22132 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/web.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.7/.gitignore
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.7/pyproject.toml
+-rw-r--r--   0        0        0   158475 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/README.md
+-rw-r--r--   0        0        0   162236 2020-02-02 00:00:00.000000 xklb-2.6.7/PKG-INFO
```

### Comparing `xklb-2.6.6/pdm.lock` & `xklb-2.6.7/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/.github/LICENSE` & `xklb-2.6.7/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/.github/Windows.md` & `xklb-2.6.7/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/.github/examples/extract.svg` & `xklb-2.6.7/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/.github/examples/tubeadd.svg` & `xklb-2.6.7/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/.github/workflows/push.yaml` & `xklb-2.6.7/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/db_media.py` & `xklb-2.6.7/xklb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/db_playlists.py` & `xklb-2.6.7/xklb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/dl_extract.py` & `xklb-2.6.7/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/fs_extract.py` & `xklb-2.6.7/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/gdl_backend.py` & `xklb-2.6.7/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/gdl_extract.py` & `xklb-2.6.7/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/history.py` & `xklb-2.6.7/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/hn_extract.py` & `xklb-2.6.7/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/lb.py` & `xklb-2.6.7/xklb/lb.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,85 +19,89 @@
         "pushshift": "Convert pushshift data to reddit.db format (stdin)",
         "hnadd": "Create / Update a Hacker News database",
         "substack": "Backup substack articles",
         "tildes": "Backup tildes comments and topics",
         "places_import": "Import places of interest (POIs)",
         "add_row": "Add arbitrary data to SQLITE",
     },
-    "Update database subcommands": {
-        "fsupdate": "Update local media",
-        "tubeupdate": "Update online video media",
-        "webupdate": "Update open-directory media",
-        "galleryupdate": "Update online gallery media",
-        "links_update": "Update a link-scraping database",
-        "redditupdate": "Update reddit media",
-    },
-    "Playback subcommands": {
-        "watch": "Watch / Listen",
-        "now": "Show what is currently playing",
-        "next": "Play next file and optionally delete current file",
-        "stop": "Stop all playback",
-        "pause": "Pause all playback",
-        "open_links": "Open links from link dbs",
-        "surf": "Auto-load browser tabs in a streaming way (stdin)",
-    },
-    "Media database subcommands": {
-        "tabs": "Open your tabs for the day",
-        "block": "Block a channel",
-        "playlists": "List stored playlists",
-        "download": "Download media",
-        "download_status": "Show download status",
-        "redownload": "Re-download deleted/lost media",
-        "history": "Show some playback statistics",
-        "search": "Search captions / subtitles",
-    },
     "Text subcommands": {
         "cluster_sort": "Sort text and images by similarity",
         "extract_links": "Extract inner links from lists of web links",
         "extract_text": "Extract human text from lists of web links",
         "markdown_links": "Extract titles from lists of web links",
     },
-    "File subcommands": {
-        "eda": "Exploratory Data Analysis on table-like files",
-        "mcda": "Multi-criteria Ranking for Decision Support",
-        "incremental_diff": "Diff large table-like files in chunks",
-        "media_check": "Check video and audio files for corruption via ffmpeg",
-        "sample_hash": "Calculate a hash based on small file segments",
-        "sample_compare": "Compare files using sample-hash and other shortcuts",
-    },
     "Folder subcommands": {
         "merge_folders": "Merge two or more file trees",
         "relmv": "Move files preserving parent folder hierarchy",
         "mv_list": "Find specific folders to move to different disks",
         "scatter": "Scatter files between folders or disks",
     },
+    "File subcommands": {
+        "sample_hash": "Calculate a hash based on small file segments",
+        "sample_compare": "Compare files using sample-hash and other shortcuts",
+    },
+    "Tabular data subcommands": {
+        "eda": "Exploratory Data Analysis on table-like files",
+        "mcda": "Multi-criteria Ranking for Decision Support",
+        "incremental_diff": "Diff large table-like files in chunks",
+    },
+    "Media File subcommands": {
+        "media_check": "Check video and audio files for corruption via ffmpeg",
+        "process_ffmpeg": "Shrink video/audio to AV1/Opus format (.mkv, .mka)",
+        "process_image": "Shrink images by resizing and AV1 image format (.avif)",
+    },
     "Multi-database subcommands": {
         "merge_dbs": "Merge SQLITE databases",
         "copy_play_counts": "Copy play history",
     },
     "Filesystem Database subcommands": {
         "christen": "Clean filenames",
         "disk_usage": "Show disk usage",
         "mount_stats": "Show some relative mount stats",
         "big_dirs": "Show large folders",
         "search_db": "Search a SQLITE database",
         "optimize": "Re-optimize database",
     },
-    "Single database enrichment subcommands": {
+    "Media Database subcommands": {
+        "tabs": "Open your tabs for the day",
+        "block": "Block a channel",
+        "playlists": "List stored playlists",
+        "download": "Download media",
+        "download_status": "Show download status",
+        "redownload": "Re-download deleted/lost media",
+        "history": "Show some playback statistics",
+        "search": "Search captions / subtitles",
+    },
+    "Playback subcommands": {
+        "watch": "Watch / Listen",
+        "now": "Show what is currently playing",
+        "next": "Play next file and optionally delete current file",
+        "stop": "Stop all playback",
+        "pause": "Pause all playback",
+        "open_links": "Open links from link dbs",
+        "surf": "Auto-load browser tabs in a streaming way (stdin)",
+    },
+    "Database enrichment subcommands": {
         "dedupe_db": "Dedupe SQLITE tables",
         "dedupe_media": "Dedupe similar media",
         "merge_online_local": "Merge online and local data",
         "mpv_watchlater": "Import mpv watchlater files to history",
         "reddit_selftext": "Copy selftext links to media table",
         "tabs_shuffle": "Randomize tabs.db a bit",
     },
+    "Update database subcommands": {
+        "fsupdate": "Update local media",
+        "tubeupdate": "Update online video media",
+        "webupdate": "Update open-directory media",
+        "galleryupdate": "Update online gallery media",
+        "links_update": "Update a link-scraping database",
+        "redditupdate": "Update reddit media",
+    },
     "Misc subcommands": {
         "export_text": "Export HTML files from SQLite databases",
-        "process_ffmpeg": "Shrink video/audio to AV1/Opus format (.mkv, .mka)",
-        "process_image": "Shrink images by resizing and AV1 image format (.avif)",
         "dedupe_czkawka": "Process czkawka diff output",
         "nouns": "Unstructured text -> compound nouns (stdin)",
     },
 }
 
 
 def usage() -> str:
```

### Comparing `xklb-2.6.6/xklb/play_actions.py` & `xklb-2.6.7/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/post_actions.py` & `xklb-2.6.7/xklb/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/readme.py` & `xklb-2.6.7/xklb/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
+<img align="right" width="300" height="600" src="https://raw.githubusercontent.com/chapmanjacobd/library/main/.github/examples/art.avif" />
+
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
 Should also work on Mac OS.
```

### Comparing `xklb-2.6.6/xklb/reddit_extract.py` & `xklb-2.6.7/xklb/reddit_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/rss_extract.py` & `xklb-2.6.7/xklb/rss_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/search.py` & `xklb-2.6.7/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/site_extract.py` & `xklb-2.6.7/xklb/site_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/tabs_actions.py` & `xklb-2.6.7/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/tabs_extract.py` & `xklb-2.6.7/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/tube_backend.py` & `xklb-2.6.7/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/tube_extract.py` & `xklb-2.6.7/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/usage.py` & `xklb-2.6.7/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/data/imagemagick_errors.py` & `xklb-2.6.7/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/data/wordbank.py` & `xklb-2.6.7/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/data/yt_dlp_errors.py` & `xklb-2.6.7/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/media/av.py` & `xklb-2.6.7/xklb/media/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/media/books.py` & `xklb-2.6.7/xklb/media/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/media/dedupe.py` & `xklb-2.6.7/xklb/media/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/media/media_check.py` & `xklb-2.6.7/xklb/media/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/media/media_player.py` & `xklb-2.6.7/xklb/media/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/media/media_printer.py` & `xklb-2.6.7/xklb/media/media_printer.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/media/subtitle.py` & `xklb-2.6.7/xklb/media/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scratch/javguru.py` & `xklb-2.6.7/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scratch/javtiful.py` & `xklb-2.6.7/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scratch/mam_search.py` & `xklb-2.6.7/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scratch/mam_slots.py` & `xklb-2.6.7/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/add_row.py` & `xklb-2.6.7/xklb/scripts/add_row.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/big_dirs.py` & `xklb-2.6.7/xklb/scripts/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/block.py` & `xklb-2.6.7/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/christen.py` & `xklb-2.6.7/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/cluster_sort.py` & `xklb-2.6.7/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/copy_play_counts.py` & `xklb-2.6.7/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/dedupe_czkawka.py` & `xklb-2.6.7/xklb/scripts/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/dedupe_db.py` & `xklb-2.6.7/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/disk_usage.py` & `xklb-2.6.7/xklb/scripts/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/download_status.py` & `xklb-2.6.7/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/eda.py` & `xklb-2.6.7/xklb/scripts/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/export_text.py` & `xklb-2.6.7/xklb/scripts/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/history.py` & `xklb-2.6.7/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/incremental_diff.py` & `xklb-2.6.7/xklb/scripts/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/links_db.py` & `xklb-2.6.7/xklb/scripts/links_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     parser.add_argument("--stop-link")
 
     parser.add_argument("--page-replace")
     parser.add_argument("--page-key", default="page")
     parser.add_argument("--page-step", "--step", "-S", type=int, default=1)
     parser.add_argument("--page-start", "--start-page", "--start", type=int)
 
+    parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
+
     arggroups.filter_links(parser)
 
     arggroups.requests(parser)
     arggroups.selenium(parser)
     arggroups.extractor(parser)
 
     parser.add_argument("--force", action="store_true")
```

### Comparing `xklb-2.6.6/xklb/scripts/mcda.py` & `xklb-2.6.7/xklb/scripts/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/merge_dbs.py` & `xklb-2.6.7/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/merge_folders.py` & `xklb-2.6.7/xklb/scripts/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/merge_online_local.py` & `xklb-2.6.7/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/move_list.py` & `xklb-2.6.7/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/open_links.py` & `xklb-2.6.7/xklb/scripts/open_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/optimize_db.py` & `xklb-2.6.7/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/places_import.py` & `xklb-2.6.7/xklb/scripts/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/playback_control.py` & `xklb-2.6.7/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/playlists.py` & `xklb-2.6.7/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/process_ffmpeg.py` & `xklb-2.6.7/xklb/scripts/process_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/process_image.py` & `xklb-2.6.7/xklb/scripts/process_image.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/redownload.py` & `xklb-2.6.7/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/rel_mv.py` & `xklb-2.6.7/xklb/scripts/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/sample_compare.py` & `xklb-2.6.7/xklb/scripts/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/sample_hash.py` & `xklb-2.6.7/xklb/scripts/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/scatter.py` & `xklb-2.6.7/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/search_db.py` & `xklb-2.6.7/xklb/scripts/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/streaming_tab_loader.py` & `xklb-2.6.7/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/web_add.py` & `xklb-2.6.7/xklb/scripts/web_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/extract_links.py` & `xklb-2.6.7/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/extract_text.py` & `xklb-2.6.7/xklb/scripts/mining/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/markdown_links.py` & `xklb-2.6.7/xklb/scripts/mining/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.6.7/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/nouns.py` & `xklb-2.6.7/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/pushshift.py` & `xklb-2.6.7/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.6.7/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/substack.py` & `xklb-2.6.7/xklb/scripts/mining/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/scripts/mining/tildes.py` & `xklb-2.6.7/xklb/scripts/mining/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/arg_utils.py` & `xklb-2.6.7/xklb/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/arggroups.py` & `xklb-2.6.7/xklb/utils/arggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,16 @@
 def requests(parser):
     parser.add_argument("--cookies", help="path to a Netscape formatted cookies file")
     parser.add_argument("--cookies-from-browser", metavar="BROWSER[+KEYRING][:PROFILE][::CONTAINER]")
     parser.add_argument("--allow-insecure", "--allow-untrusted", "--disable-tls", action="store_true")
 
 
 def selenium(parser):
-    parser.add_argument("--selenium", "--js", "--firefox", action="store_true")
+    parser.add_argument("--selenium", "--js", action="store_true")
+    parser.add_argument("--firefox", action="store_true")
     parser.add_argument("--chrome", action="store_true")
     parser.add_argument("--scroll", action="store_true", help="Scroll down the page; infinite scroll")
     parser.add_argument("--manual", action="store_true", help="Confirm manually in shell before exiting the browser")
     parser.add_argument("--auto-pager", "--autopager", action="store_true")
     parser.add_argument("--poke", action="store_true")
```

### Comparing `xklb-2.6.6/xklb/utils/argparse_utils.py` & `xklb-2.6.7/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/consts.py` & `xklb-2.6.7/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/db_utils.py` & `xklb-2.6.7/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/devices.py` & `xklb-2.6.7/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/file_utils.py` & `xklb-2.6.7/xklb/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/gui.py` & `xklb-2.6.7/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/iterables.py` & `xklb-2.6.7/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/log_utils.py` & `xklb-2.6.7/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/mpv_utils.py` & `xklb-2.6.7/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/nums.py` & `xklb-2.6.7/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/objects.py` & `xklb-2.6.7/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/path_utils.py` & `xklb-2.6.7/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/pd_utils.py` & `xklb-2.6.7/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/printing.py` & `xklb-2.6.7/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/processes.py` & `xklb-2.6.7/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/sql_utils.py` & `xklb-2.6.7/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/strings.py` & `xklb-2.6.7/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/xklb/utils/web.py` & `xklb-2.6.7/xklb/utils/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,27 +230,29 @@
         for logger_name, logger in logging.root.manager.loggerDict.items():
             if logger_name.startswith("selenium"):
                 logging.getLogger(logger_name).setLevel(clamp_index(log_levels, args.verbose - 1))
 
     else:
         from selenium import webdriver
 
-    xvfb = None
+    xvfb = None  # three states
     if args.verbose < consts.LOG_DEBUG and not getattr(args, "manual", False):
         xvfb = False
         try:
             from pyvirtualdisplay.display import Display
 
             args.driver_display = Display(visible=False, size=(1280, 720))
             args.driver_display.start()
             xvfb = True
         except Exception:
             pass
 
-    if which("firefox") and not getattr(args, "chrome", False):
+    if (which("firefox") or which("firefox.exe") or getattr(args, "firefox", False)) and not getattr(
+        args, "chrome", False
+    ):
         from selenium.webdriver.firefox.options import Options
         from selenium.webdriver.firefox.service import Service
 
         service = Service(log_path=tempfile.mktemp(".geckodriver.log"))
         options = Options()
         if Path("selenium").exists():
             options.profile = "selenium"
```

### Comparing `xklb-2.6.6/xklb/assets/kotobago.png` & `xklb-2.6.7/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/.gitignore` & `xklb-2.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/pyproject.toml` & `xklb-2.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.6/.github/README.md` & `xklb-2.6.7/.github/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
+<img align="right" width="300" height="600" src="https://raw.githubusercontent.com/chapmanjacobd/library/main/.github/examples/art.avif" />
+
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
 Should also work on Mac OS.
-<img align="right" width="400" src="https://raw.githubusercontent.com/chapmanjacobd/library/main/.github/examples/tubeadd.svg" />
 
 ### External dependencies
 
 Required: `ffmpeg`
 
 Some features work better with: `mpv`, `firefox`, `fish`
 
@@ -92,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.006)
+    xk media library subcommands (v2.6.007)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -125,102 +126,61 @@
     │ tildes        │ Backup tildes comments and topics                  │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ places-import │ Import places of interest (POIs)                   │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ add-row       │ Add arbitrary data to SQLITE                       │
     ╰───────────────┴────────────────────────────────────────────────────╯
 
-    Update database subcommands:
-    ╭───────────────┬─────────────────────────────────╮
-    │ fsupdate      │ Update local media              │
-    ├───────────────┼─────────────────────────────────┤
-    │ tubeupdate    │ Update online video media       │
-    ├───────────────┼─────────────────────────────────┤
-    │ webupdate     │ Update open-directory media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ galleryupdate │ Update online gallery media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ links-update  │ Update a link-scraping database │
-    ├───────────────┼─────────────────────────────────┤
-    │ redditupdate  │ Update reddit media             │
-    ╰───────────────┴─────────────────────────────────╯
-
-    Playback subcommands:
-    ╭────────────┬───────────────────────────────────────────────────╮
-    │ watch      │ Watch / Listen                                    │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ now        │ Show what is currently playing                    │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ next       │ Play next file and optionally delete current file │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ stop       │ Stop all playback                                 │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ pause      │ Pause all playback                                │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ open-links │ Open links from link dbs                          │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ surf       │ Auto-load browser tabs in a streaming way (stdin) │
-    ╰────────────┴───────────────────────────────────────────────────╯
-
-    Media database subcommands:
-    ╭─────────────────┬────────────────────────────────╮
-    │ tabs            │ Open your tabs for the day     │
-    ├─────────────────┼────────────────────────────────┤
-    │ block           │ Block a channel                │
-    ├─────────────────┼────────────────────────────────┤
-    │ playlists       │ List stored playlists          │
-    ├─────────────────┼────────────────────────────────┤
-    │ download        │ Download media                 │
-    ├─────────────────┼────────────────────────────────┤
-    │ download-status │ Show download status           │
-    ├─────────────────┼────────────────────────────────┤
-    │ redownload      │ Re-download deleted/lost media │
-    ├─────────────────┼────────────────────────────────┤
-    │ history         │ Show some playback statistics  │
-    ├─────────────────┼────────────────────────────────┤
-    │ search          │ Search captions / subtitles    │
-    ╰─────────────────┴────────────────────────────────╯
-
     Text subcommands:
     ╭────────────────┬─────────────────────────────────────────────╮
     │ cluster-sort   │ Sort text and images by similarity          │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-links  │ Extract inner links from lists of web links │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-text   │ Extract human text from lists of web links  │
     ├────────────────┼─────────────────────────────────────────────┤
     │ markdown-links │ Extract titles from lists of web links      │
     ╰────────────────┴─────────────────────────────────────────────╯
 
-    File subcommands:
-    ╭──────────────────┬───────────────────────────────────────────────────────╮
-    │ eda              │ Exploratory Data Analysis on table-like files         │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ mcda             │ Multi-criteria Ranking for Decision Support           │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ incremental-diff │ Diff large table-like files in chunks                 │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ media-check      │ Check video and audio files for corruption via ffmpeg │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ sample-hash      │ Calculate a hash based on small file segments         │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ sample-compare   │ Compare files using sample-hash and other shortcuts   │
-    ╰──────────────────┴───────────────────────────────────────────────────────╯
-
     Folder subcommands:
     ╭───────────────┬──────────────────────────────────────────────────╮
     │ merge-folders │ Merge two or more file trees                     │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ relmv         │ Move files preserving parent folder hierarchy    │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ mv-list       │ Find specific folders to move to different disks │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ scatter       │ Scatter files between folders or disks           │
     ╰───────────────┴──────────────────────────────────────────────────╯
 
+    File subcommands:
+    ╭────────────────┬─────────────────────────────────────────────────────╮
+    │ sample-hash    │ Calculate a hash based on small file segments       │
+    ├────────────────┼─────────────────────────────────────────────────────┤
+    │ sample-compare │ Compare files using sample-hash and other shortcuts │
+    ╰────────────────┴─────────────────────────────────────────────────────╯
+
+    Tabular data subcommands:
+    ╭──────────────────┬───────────────────────────────────────────────╮
+    │ eda              │ Exploratory Data Analysis on table-like files │
+    ├──────────────────┼───────────────────────────────────────────────┤
+    │ mcda             │ Multi-criteria Ranking for Decision Support   │
+    ├──────────────────┼───────────────────────────────────────────────┤
+    │ incremental-diff │ Diff large table-like files in chunks         │
+    ╰──────────────────┴───────────────────────────────────────────────╯
+
+    Media File subcommands:
+    ╭────────────────┬────────────────────────────────────────────────────────╮
+    │ media-check    │ Check video and audio files for corruption via ffmpeg  │
+    ├────────────────┼────────────────────────────────────────────────────────┤
+    │ process-ffmpeg │ Shrink video/audio to AV1/Opus format (.mkv, .mka)     │
+    ├────────────────┼────────────────────────────────────────────────────────┤
+    │ process-image  │ Shrink images by resizing and AV1 image format (.avif) │
+    ╰────────────────┴────────────────────────────────────────────────────────╯
+
     Multi-database subcommands:
     ╭──────────────────┬────────────────────────╮
     │ merge-dbs        │ Merge SQLITE databases │
     ├──────────────────┼────────────────────────┤
     │ copy-play-counts │ Copy play history      │
     ╰──────────────────┴────────────────────────╯
 
@@ -235,41 +195,88 @@
     │ big-dirs    │ Show large folders             │
     ├─────────────┼────────────────────────────────┤
     │ search-db   │ Search a SQLITE database       │
     ├─────────────┼────────────────────────────────┤
     │ optimize    │ Re-optimize database           │
     ╰─────────────┴────────────────────────────────╯
 
-    Single database enrichment subcommands:
+    Media Database subcommands:
+    ╭─────────────────┬────────────────────────────────╮
+    │ tabs            │ Open your tabs for the day     │
+    ├─────────────────┼────────────────────────────────┤
+    │ block           │ Block a channel                │
+    ├─────────────────┼────────────────────────────────┤
+    │ playlists       │ List stored playlists          │
+    ├─────────────────┼────────────────────────────────┤
+    │ download        │ Download media                 │
+    ├─────────────────┼────────────────────────────────┤
+    │ download-status │ Show download status           │
+    ├─────────────────┼────────────────────────────────┤
+    │ redownload      │ Re-download deleted/lost media │
+    ├─────────────────┼────────────────────────────────┤
+    │ history         │ Show some playback statistics  │
+    ├─────────────────┼────────────────────────────────┤
+    │ search          │ Search captions / subtitles    │
+    ╰─────────────────┴────────────────────────────────╯
+
+    Playback subcommands:
+    ╭────────────┬───────────────────────────────────────────────────╮
+    │ watch      │ Watch / Listen                                    │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ now        │ Show what is currently playing                    │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ next       │ Play next file and optionally delete current file │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ stop       │ Stop all playback                                 │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ pause      │ Pause all playback                                │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ open-links │ Open links from link dbs                          │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ surf       │ Auto-load browser tabs in a streaming way (stdin) │
+    ╰────────────┴───────────────────────────────────────────────────╯
+
+    Database enrichment subcommands:
     ╭────────────────────┬────────────────────────────────────────╮
     │ dedupe-db          │ Dedupe SQLITE tables                   │
     ├────────────────────┼────────────────────────────────────────┤
     │ dedupe-media       │ Dedupe similar media                   │
     ├────────────────────┼────────────────────────────────────────┤
     │ merge-online-local │ Merge online and local data            │
     ├────────────────────┼────────────────────────────────────────┤
     │ mpv-watchlater     │ Import mpv watchlater files to history │
     ├────────────────────┼────────────────────────────────────────┤
     │ reddit-selftext    │ Copy selftext links to media table     │
     ├────────────────────┼────────────────────────────────────────┤
     │ tabs-shuffle       │ Randomize tabs.db a bit                │
     ╰────────────────────┴────────────────────────────────────────╯
 
+    Update database subcommands:
+    ╭───────────────┬─────────────────────────────────╮
+    │ fsupdate      │ Update local media              │
+    ├───────────────┼─────────────────────────────────┤
+    │ tubeupdate    │ Update online video media       │
+    ├───────────────┼─────────────────────────────────┤
+    │ webupdate     │ Update open-directory media     │
+    ├───────────────┼─────────────────────────────────┤
+    │ galleryupdate │ Update online gallery media     │
+    ├───────────────┼─────────────────────────────────┤
+    │ links-update  │ Update a link-scraping database │
+    ├───────────────┼─────────────────────────────────┤
+    │ redditupdate  │ Update reddit media             │
+    ╰───────────────┴─────────────────────────────────╯
+
     Misc subcommands:
-    ╭────────────────┬────────────────────────────────────────────────────────╮
-    │ export-text    │ Export HTML files from SQLite databases                │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ process-ffmpeg │ Shrink video/audio to AV1/Opus format (.mkv, .mka)     │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ process-image  │ Shrink images by resizing and AV1 image format (.avif) │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ dedupe-czkawka │ Process czkawka diff output                            │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ nouns          │ Unstructured text -> compound nouns (stdin)            │
-    ╰────────────────┴────────────────────────────────────────────────────────╯
+    ╭────────────────┬─────────────────────────────────────────────╮
+    │ export-text    │ Export HTML files from SQLite databases     │
+    ├────────────────┼─────────────────────────────────────────────┤
+    │ dedupe-czkawka │ Process czkawka diff output                 │
+    ├────────────────┼─────────────────────────────────────────────┤
+    │ nouns          │ Unstructured text -> compound nouns (stdin) │
+    ╰────────────────┴─────────────────────────────────────────────╯
 
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
@@ -945,561 +952,726 @@
         |   test_b |   test_a |
         |----------|----------|
         |        1 |        2 |
 
 
 </details>
 
-### Update database subcommands
+### Text subcommands
 
-###### fsupdate
+###### cluster-sort
 
-<details><summary>Update local media</summary>
+<details><summary>Sort text and images by similarity</summary>
 
-    $ library fsupdate -h
-    usage: library fsupdate DATABASE
+    $ library cluster-sort -h
+    usage: library cluster-sort [input_path | stdin] [output_path | stdout]
 
-    Update each path previously saved:
+    Group lines of text into sorted output
+
+        echo 'red apple
+        broccoli
+        yellow
+        green
+        orange apple
+        red apple' | library cluster-sort
+
+        orange apple
+        red apple
+        red apple
+        broccoli
+        green
+        yellow
+
+    Show the groupings
+
+        echo 'red apple
+        broccoli
+        yellow
+        green
+        orange apple
+        red apple' | library cluster-sort --print-groups
+
+        [
+            {'grouped_paths': ['orange apple', 'red apple', 'red apple']},
+            {'grouped_paths': ['broccoli', 'green', 'yellow']}
+        ]
+
+    Auto-sort images into directories
+
+        echo 'image1.jpg
+        image2.jpg
+        image3.jpg' | library cluster-sort --image --move-groups
+
+    Print similar paths
+
+        library fs 0day.db -pa --cluster --print-groups
 
-        library fsupdate video.db
 
 
 </details>
 
-###### tubeupdate
+###### extract-links
 
-<details><summary>Update online video media</summary>
+<details><summary>Extract inner links from lists of web links</summary>
 
-    $ library tubeupdate -h
-    usage: library tubeupdate [--audio | --video] DATABASE
+    $ library extract-links -h
+    usage: library extract-links PATH ... [--case-sensitive] [--scroll] [--download] [--verbose] [--local-html] [--file FILE] [--path-include ...] [--text-include ...] [--after-include ...] [--before-include ...] [--path-exclude ...] [--text-exclude ...] [--after-exclude ...] [--before-exclude ...]
 
-    Fetch the latest videos for every playlist saved in your database
+    Extract links from within local HTML fragments, files, or remote pages; filtering on link text and nearby plain-text
 
-        library tubeupdate educational.db
+        library links https://en.wikipedia.org/wiki/List_of_bacon_dishes --path-include https://en.wikipedia.org/wiki/ --after-include famous
+        https://en.wikipedia.org/wiki/Omelette
 
-    Fetch extra metadata:
+    Read from local clipboard and filter out links based on nearby plain text:
 
-        By default tubeupdate will quickly add media.
-        You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
+        library links --local-html (cb -t text/html | psub) --after-exclude paranormal spooky horror podcast tech fantasy supernatural lecture sport
+        # note: the equivalent BASH-ism is <(xclip -selection clipboard -t text/html)
 
-        library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
+    Run with `-vv` to see the browser
 
-    Remove duplicate playlists:
 
-        lb dedupe-db video.db playlists --bk extractor_playlist_id
+</details>
+
+###### extract-text
+
+<details><summary>Extract human text from lists of web links</summary>
+
+    $ library extract-text -h
+    usage: library extract-text PATH ... [--skip-links]
+
+    Sorting suggestions
+
+        lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 
 
 </details>
 
-###### webupdate
+### Folder subcommands
 
-<details><summary>Update open-directory media</summary>
+###### merge-folders
 
-    $ library webupdate -h
-    usage: library web-update DATABASE
+<details><summary>Merge two or more file trees</summary>
 
-    Update saved open directories
+    $ library merge-folders -h
+    usage: library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
 
+    Merge multiple folders with the same file tree into a single folder.
+
+    https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
+
+    Trumps are new or replaced files from an earlier source which now conflict with a later source.
+    If you only have one source then the count of trumps will always be zero.
+    The count of conflicts also includes trumps.
 
 
 </details>
 
-###### galleryupdate
+###### relmv
 
-<details><summary>Update online gallery media</summary>
+<details><summary>Move files preserving parent folder hierarchy</summary>
 
-    $ library galleryupdate -h
-    usage: library galleryupdate DATABASE URLS
+    $ library relmv -h
+    usage: library relmv [--simulate] SOURCE ... DEST
 
-    Check previously saved gallery_dl URLs for new content
+    Move files/folders without losing hierarchy metadata
+
+    Move fresh music to your phone every Sunday:
+
+        # move last week music back to their source folders
+        library mv /mnt/d/sync/weekly/ /mnt/d/check/audio/
+
+        # move new music for this week
+        library relmv (
+            library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+        ) /mnt/d/sync/weekly/
 
 
 </details>
 
-###### links-update
+###### mv-list
 
-<details><summary>Update a link-scraping database</summary>
+<details><summary>Find specific folders to move to different disks</summary>
 
-    $ library links-update -h
-    usage: library links-update DATABASE
+    $ library mv-list -h
+    usage: library mv-list [--limit LIMIT] [--lower LOWER] [--upper UPPER] MOUNT_POINT DATABASE
 
-    Fetch new links from each path previously saved
+    Free up space on a specific disk. Find candidates for moving data to a different mount point
 
-        library links-update links.db
+
+    The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
+
+        library fsadd --filesystem d.db ~/d/
+
+    But this should definitely also work with xklb audio and video databases:
+
+        library mv-list /mnt/d/ video.db
+
+    The program will print a table with a sorted list of folders which are good candidates for moving.
+    Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over).
+    The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
+
+        ...
+        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+        │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
+        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+        │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
+        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+        │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
+        ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
+        6702 other folders not shown
+
+        ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
+        ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
+        ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
+        ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
+        ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
+        ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
+
+        Type "done" when finished
+        Type "more" to see more files
+        Paste a folder (and press enter) to toggle selection
+        Type "*" to select all files in the most recently printed table
+
+    Then it will give you a prompt:
+
+        Paste a path:
+
+    Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
+
+        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+        26 selected paths: 162.1 GB ; future free space: 486.9 GB
+
+    You can also press the up arrow or paste it again to remove it from the list:
+
+        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+        25 selected paths: 159.9 GB ; future free space: 484.7 GB
+
+    After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
+
+        Paste a path: done
+
+            Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
+
+                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
 
 
 </details>
 
-###### redditupdate
+###### scatter
 
-<details><summary>Update reddit media</summary>
+<details><summary>Scatter files between folders or disks</summary>
 
-    $ library redditupdate -h
-    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+    $ library scatter -h
+    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
 
-    Fetch the latest posts for every subreddit/redditor saved in your database
+    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
 
-        library redditupdate edu_subreddits.db
+    Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
+
+        library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Reduce number of files per folder (creates more folders)
+
+        library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Multi-device re-bin: balance by size
+
+        library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs.db subfolder/of/mergerfs/mnt
+        Current path distribution:
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+
+        Simulated path distribution:
+        5845 files should be moved
+        20257 files should not be moved
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+        ### Move 1182 files to /mnt/d7 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
+        ### Move 1198 files to /mnt/d6 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
+        ### Move 1146 files to /mnt/d5 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
+        ### Move 1185 files to /mnt/d3 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
+        ### Move 1134 files to /mnt/d4 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+
+    Multi-device re-bin: balance device inodes for specific subfolder
+
+        library scatter -m /mnt/d1:/mnt/d2 fs.db subfolder --group count --sort 'size desc'
+
+    Multi-device re-bin: only consider the most recent 100 files
+
+        library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
+
+    Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
+
+        library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
 
 
 </details>
 
-### Playback subcommands
+### File subcommands
 
-###### watch
+###### sample-hash
 
-<details><summary>Watch / Listen</summary>
+<details><summary>Calculate a hash based on small file segments</summary>
 
-    $ library watch -h
-    usage: library watch DATABASE [optional args]
+    $ library sample-hash -h
+    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
-    Control playback:
-        To stop playback press Ctrl-C in either the terminal or mpv
+    Calculate hashes for large files by reading only small segments of each file
 
-        Create global shortcuts in your desktop environment by sending commands to mpv_socket:
-        echo 'playlist-next force' | socat - /tmp/mpv_socket
+        library sample-hash ./my_file.mkv
 
-    Override the default player (mpv):
-        library does a lot of things to try to automatically use your preferred media player
-        but if it doesn't guess right you can make it explicit:
-        library watch --player "vlc --vlc-opts"
+    The threads flag seems to be faster for rotational media but slower on SSDs
 
-    Cast to chromecast groups:
-        library watch --cast --cast-to "Office pair"
-        library watch -ct "Office pair"  # equivalent
-        If you don't know the exact name of your chromecast group run `catt scan`
 
-    Play media in order (similarly named episodes):
-        library watch --play-in-order
-        library watch -O    # equivalent
+</details>
 
-        The default sort value is 'natural_ps' which means media will be sorted by parent path
-        and then stem in a natural way (using the integer values within the path). But there are many other options:
+###### sample-compare
 
-        Options:
+<details><summary>Compare files using sample-hash and other shortcuts</summary>
 
-            - reverse: reverse the sort order
-            - compat: treat characters like '⑦' as '7'
+    $ library sample-compare -h
+    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
-        Algorithms:
+    Convenience subcommand to compare multiple files using sample-hash
 
-            - natural: parse numbers as integers
-            - os: sort similar to the OS File Explorer sorts. To improve non-alphanumeric sorting on Mac OS X and Linux it is necessary to install pyicu (perhaps via python3-icu -- https://gitlab.pyicu.org/main/pyicu#installing-pyicu)
-            - path: use natsort "path" algorithm (https://natsort.readthedocs.io/en/stable/api.html#the-ns-enum)
-            - human: use system locale
-            - ignorecase: treat all case as equal
-            - lowercase: sort lowercase first
-            - signed: sort with an understanding of negative numbers
-            - python: sort like default python
 
-        Values:
+</details>
 
-            - path
-            - parent
-            - stem
-            - title (or any other column value)
-            - ps: parent, stem
-            - pts: parent, title, stem
+### Tabular data subcommands
 
-        Use this format: algorithm, value, algorithm_value, or option_algorithm_value.
-        For example:
+###### eda
 
-            - library watch -O human
-            - library watch -O title
-            - library watch -O human_title
-            - library watch -O reverse_compat_human_title
+<details><summary>Exploratory Data Analysis on table-like files</summary>
 
-            - library watch -O path       # path algorithm and parent, stem values (path_ps)
-            - library watch -O path_path  # path algorithm and path values
+    $ library eda -h
+    usage: library eda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW] [--repl]
 
-        Also, if you are using --random you need to fetch sibling media to play the media in order:
+    Perform Exploratory Data Analysis (EDA) on one or more files
 
-            - library watch --random --fetch-siblings each -O          # get the first result per directory
-            - library watch --random --fetch-siblings if-audiobook -O  # get the first result per directory if 'audiobook' is in the path
-            - library watch --random --fetch-siblings always -O        # get 2,000 results per directory
+    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
 
-        If searching by a specific subpath it may be preferable to just sort by path instead
-        library watch d/planet.earth.2024/ -u path
 
-        library watch --related  # Similar to -O but uses fts to find similar content
-        library watch -R         # equivalent
-        library watch -RR        # above, plus ignores most filters
+</details>
 
-        library watch --cluster  # cluster-sort to put similar-named paths closer together
-        library watch -C         # equivalent
+###### mcda
 
-        library watch --big-dirs # Recommended to use with --duration or --depth filters; see `lb big-dirs -h` for more info
-        library watch -B         # equivalent
+<details><summary>Multi-criteria Ranking for Decision Support</summary>
 
-        All of these options can be used together but it will be a bit slow and the results might be mid-tier
-        as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
-        library watch -RRCO
+    $ library mcda -h
+    usage: library mcda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW]
 
-        You can even sort the items within each cluster by auto-MCDA ~LOL~
-        library watch -B --sort-groups-by 'mcda median_size,-deleted'
-        library watch -C --sort-groups-by 'mcda median_size,-deleted'
+    Perform Multiple Criteria Decision Analysis (MCDA) on one or more files
 
-    Filter media by file siblings of parent directory:
-        library watch --sibling   # only include files which have more than or equal to one sibling
-        library watch --solo      # only include files which are alone by themselves
+    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
 
-        `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
-        library watch --sibling --solo      # you will always get zero records here
-        library watch --lower 2 --upper 1   # equivalent
+    $ library mcda ~/storage.csv --minimize price --ignore warranty
 
-        You can be more specific via the `--upper` and `--lower` flags
-        library watch --lower 3   # only include files which have three or more siblings
-        library watch --upper 3   # only include files which have fewer than three siblings
-        library watch --lower 3 --upper 3   # only include files which are three siblings inclusive
-        library watch --lower 12 --upper 25 -O  # on my machine this launches My Mister 2018
+        ### Goals
+        #### Maximize
+        - size
+        #### Minimize
+        - price
 
-    Play recent partially-watched videos (requires mpv history):
-        library watch --partial       # play newest first
+        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
+        |----|---------|--------|------------|----------|------------|----------|---------|
+        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
+        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
+        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
 
-        library watch --partial old   # play oldest first
-        library watch -P o            # equivalent
+    $ library mcda ~/storage.csv --ignore warranty
 
-        library watch -P p            # sort by percent remaining
-        library watch -P t            # sort by time remaining
-        library watch -P s            # skip partially watched (only show unseen)
+        ### Goals
+        #### Maximize
+        - price
+        - size
 
-        The default time used is "last-viewed" (ie. the most recent time you closed the video)
-        If you want to use the "first-viewed" time (ie. the very first time you opened the video)
-        library watch -P f            # use watch_later file creation time instead of modified time
+        |    |   price |   size |   warranty |   TOPSIS |     MABAC |   SPOTIS |   BORDA |
+        |----|---------|--------|------------|----------|-----------|----------|---------|
+        |  2 |     519 |     44 |          2 | 1        |  0.536587 | 0        | 7.46341 |
+        |  1 |     453 |     40 |          2 | 0.580079 |  0.103888 | 0.432699 | 7.88333 |
+        |  0 |     359 |     36 |          5 | 0        | -0.463413 | 1        | 8.46341 |
 
-        You can combine most of these options, though some will be overridden by others.
-        library watch -P fo           # this means "show the oldest videos using the time I first opened them"
-        library watch -P pt           # weighted remaining (percent * time remaining)
+    $ library mcda ~/storage.csv --minimize price --ignore warranty
 
-    Print instead of play:
-        library watch --print --limit 10  # print the next 10 files
-        library watch -p -L 10  # print the next 10 files
-        library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
+        ### Goals
+        #### Maximize
+        - size
+        #### Minimize
+        - price
 
-        Printing modes
-        library watch -p    # print as a table
-        library watch -p a  # print an aggregate report
-        library watch -p b  # print a big-dirs report (see library bigdirs -h for more info)
-        library watch -p f  # print fields (defaults to path; use --cols to change)
-                               # -- useful for piping paths to utilities like xargs or GNU Parallel
+        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
+        |----|---------|--------|------------|----------|------------|----------|---------|
+        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
+        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
+        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
 
-        library watch -p d  # mark deleted
-        library watch -p w  # mark watched
+    It also works with HTTP/GCS/S3 URLs:
 
-        Some printing modes can be combined
-        library watch -p df  # print files for piping into another program and mark them as deleted within the db
-        library watch -p bf  # print fields from big-dirs report
+    $ library mcda https://en.wikipedia.org/wiki/List_of_Academy_Award-winning_films --clean --minimize Year
 
-        Check if you have downloaded something before
-        library watch -u duration -p -s 'title'
+        ### Goals
 
-        Print an aggregate report of deleted media
-        library watch -w time_deleted!=0 -p=a
-        ╒═══════════╤══════════════╤═════════╤═════════╕
-        │ path      │ duration     │ size    │   count │
-        ╞═══════════╪══════════════╪═════════╪═════════╡
-        │ Aggregate │ 14 days, 23  │ 50.6 GB │   29058 │
-        │           │ hours and 42 │         │         │
-        │           │ minutes      │         │         │
-        ╘═══════════╧══════════════╧═════════╧═════════╛
-        Total duration: 14 days, 23 hours and 42 minutes
+        #### Maximize
 
-        Print an aggregate report of media that has no duration information (ie. online or corrupt local media)
-        library watch -w 'duration is null' -p=a
+        - Nominations
+        - Awards
 
-        Print a list of filenames which have below 1280px resolution
-        library watch -w 'width<1280' -p=f
+        #### Minimize
 
-        Print media you have partially viewed with mpv
-        library watch --partial -p
-        library watch -P -p  # equivalent
-        library watch -P -p f --cols path,progress,duration  # print CSV of partially watched files
-        library watch --partial -pa  # print an aggregate report of partially watched files
+        - Year
 
-        View how much time you have watched
-        library watch -w play_count'>'0 -p=a
+        |      | Film                                                                    |   Year |   Awards |   Nominations |      TOPSIS |    MABAC |      SPOTIS |   BORDA |
+        |------|-------------------------------------------------------------------------|--------|----------|---------------|-------------|----------|-------------|---------|
+        |  378 | Titanic                                                                 |   1997 |       11 |            14 | 0.999993    | 1.38014  | 4.85378e-06 | 4116.62 |
+        |  868 | Ben-Hur                                                                 |   1959 |       11 |            12 | 0.902148    | 1.30871  | 0.0714303   | 4116.72 |
+        |  296 | The Lord of the Rings: The Return of the King                           |   2003 |       11 |            11 | 0.8558      | 1.27299  | 0.107147    | 4116.76 |
+        | 1341 | West Side Story                                                         |   1961 |       10 |            11 | 0.837716    | 1.22754  | 0.152599    | 4116.78 |
+        |  389 | The English Patient                                                     |   1996 |        9 |            12 | 0.836725    | 1.2178   | 0.162341    | 4116.78 |
+        | 1007 | Gone with the Wind                                                      |   1939 |        8 |            13 | 0.807086    | 1.20806  | 0.172078    | 4116.81 |
+        |  990 | From Here to Eternity                                                   |   1953 |        8 |            13 | 0.807086    | 1.20806  | 0.172079    | 4116.81 |
+        | 1167 | On the Waterfront                                                       |   1954 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        | 1145 | My Fair Lady                                                            |   1964 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        |  591 | Gandhi                                                                  |   1982 |        8 |            11 | 0.755312    | 1.13663  | 0.243509    | 4116.86 |
 
-        See how much video you have
-        library watch video.db -p=a
-        ╒═══════════╤═════════╤═════════╤═════════╕
-        │ path      │   hours │ size    │   count │
-        ╞═══════════╪═════════╪═════════╪═════════╡
-        │ Aggregate │  145769 │ 37.6 TB │  439939 │
-        ╘═══════════╧═════════╧═════════╧═════════╛
-        Total duration: 16 years, 7 months, 19 days, 17 hours and 25 minutes
 
-        View all the columns
-        library watch -p -L 1 --cols '*'
+</details>
 
-        Open ipython with all of your media
-        library watch -vv -p --cols '*'
-        ipdb> len(media)
-        462219
+###### incremental-diff
 
-    Set the play queue size:
-        By default the play queue is 120--long enough that you likely have not noticed
-        but short enough that the program is snappy.
+<details><summary>Diff large table-like files in chunks</summary>
 
-        If you want everything in your play queue you can use the aid of infinity.
-        Pick your poison (these all do effectively the same thing):
-        library watch -L inf
-        library watch -l inf
-        library watch --queue inf
-        library watch -L 999999999999
+    $ library incremental-diff -h
+    usage: library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
 
-        You may also want to restrict the play queue.
-        For example, when you only want 1000 random files:
-        library watch -u random -L 1000
+    See data differences in an incremental way to quickly see how two different files differ.
 
-    Offset the play queue:
-        You can also offset the queue. For example if you want to skip one or ten media:
-        library watch --offset 10      # offset ten from the top of an ordered query
+    Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
 
-    Repeat
-        library watch                  # listen to 120 random songs (DEFAULT_PLAY_QUEUE)
-        library watch --limit 5        # listen to FIVE songs
-        library watch -l inf -u random # listen to random songs indefinitely
-        library watch -s infinite      # listen to songs from the band infinite
+    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared.
+    If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
 
-    Constrain media by search:
-        Audio files have many tags to readily search through so metadata like artist,
-        album, and even mood are included in search.
-        Video files have less consistent metadata and so only paths are included in search.
-        library watch --include happy  # only matches will be included
-        library watch -s happy         # equivalent
-        library watch --exclude sad    # matches will be excluded
-        library watch -E sad           # equivalent
+    To diff everything at once run with `--batch-size inf`
 
-        Search only the path column
-        library watch -O -s 'path : mad max'
-        library watch -O -s 'path : "mad max"' # add "quotes" to be more strict
 
-        Double spaces are parsed as one space
-        library watch -s '  ost'        # will match OST and not ghost
-        library watch -s toy story      # will match '/folder/toy/something/story.mp3'
-        library watch -s 'toy  story'   # will match more strictly '/folder/toy story.mp3'
+</details>
 
-        You can search without -s but it must directly follow the database due to how argparse works
-        library watch ./your.db searching for something
+### Media File subcommands
 
-    Constrain media by arbitrary SQL expressions:
-        library watch --where audio_count = 2  # media which have two audio tracks
-        library watch -w "language = 'eng'"    # media which have an English language tag
-                                                    (this could be audio _or_ subtitle)
-        library watch -w subtitle_count=0      # media that doesn't have subtitles
+###### media-check
 
-    Constrain media to duration (in minutes):
-        library watch --duration 20
-        library watch -d 6  # 6 mins ±10 percent (ie. between 5 and 7 mins)
-        library watch -d-6  # less than 6 mins
-        library watch -d+6  # more than 6 mins
+<details><summary>Check video and audio files for corruption via ffmpeg</summary>
 
-        Duration can be specified multiple times:
-        library watch -d+5 -d-7  # should be similar to -d 6
+    $ library media-check -h
+    usage: library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
 
-        If you want exact time use `where`
-        library watch --where 'duration=6*60'
+    Defaults to decode 0.5 second per 10% of each file
 
-    Constrain media to file size (in megabytes):
-        library watch --size 20
-        library watch -S 6  # 6 MB ±10 percent (ie. between 5 and 7 MB)
-        library watch -S-6  # less than 6 MB
-        library watch -S+6  # more than 6 MB
+        library media-check ./video.mp4
 
-    Constrain media by time_created / time_last_played / time_deleted / time_modified:
-        library watch --created-within '3 days'
-        library watch --created-before '3 years'
+    Decode all the frames of each file to evaluate how corrupt it is
+    (scantime is very slow; about 150 seconds for an hour-long file)
 
-    Constrain media by throughput:
-        Bitrate information is not explicitly saved.
-        You can use file size and duration as a proxy for throughput:
-        library watch -w 'size/duration<50000'
+        library media-check --full-scan ./video.mp4
 
-    Constrain media to portrait orientation video:
-        library watch --portrait
-        library watch -w 'width<height' # equivalent
+    Decode all the packets of each file to evaluate how corrupt it is
+    (scantime is about one second of each file but only accurate for formats where 1 packet == 1 frame)
 
-    Constrain media to duration of videos which match any size constraints:
-        library watch --duration-from-size +700 -u 'duration desc, size desc'
+        library media-check --full-scan --gap 0 ./video.mp4
 
-    Constrain media to online-media or local-media:
-        Not to be confused with only local-media which is not "offline" (ie. one HDD disconnected)
-        library watch --online-media-only
-        library watch --online-media-only -i  # and ignore playback errors (ie. YouTube video deleted)
-        library watch --local-media-only
+    Decode all audio of each file to evaluate how corrupt it is
+    (scantime is about four seconds per file)
 
-    Specify media play order:
-        library watch --sort duration   # play shortest media first
-        library watch -u duration desc  # play longest media first
+        library media-check --full-scan --audio ./video.mp4
 
-        You can use multiple SQL ORDER BY expressions
-        library watch -u 'subtitle_count > 0 desc' # play media that has at least one subtitle first
+    Decode at least one frame at the start and end of each file to evaluate how corrupt it is
+    (scantime is about one second per file)
 
-        Prioritize large-sized media
-        library watch --sort 'ntile(10000) over (order by size/duration) desc'
-        library watch -u 'ntile(100) over (order by size) desc'
+        library media-check --chunk-size 5% --gap 99.9% ./video.mp4
 
-        Sort by count of media with the same-X column (default DESC: most common to least common value)
-        library watch -u same-duration
-        library watch -u same-title
-        library watch -u same-size
-        library watch -u same-width, same-height ASC, same-fps
-        library watch -u same-time_uploaded same-view_count same-upvote_ratio
+    Decode 3s every 5% of a file to evaluate how corrupt it is
+    (scantime is about three seconds per file)
 
-        No media found when using --random
-        In addition to -u/--sort random, there is also the -r/--random flag.
-        If you have a large database it should be faster than -u random but it comes with a caveat:
-        This flag randomizes via rowid at an earlier stage to boost performance.
-        It is possible that you see "No media found" or a smaller amount of media than correct.
-        You can bypass this by setting --limit. For example:
-        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa
-        path         count      size  duration                        avg_duration      avg_size
-        ---------  -------  --------  ------------------------------  --------------  ----------
-        Aggregate    10000  752.5 GB  4 months, 15 days and 10 hours  20 minutes         75.3 MB
-        (17 seconds)
-        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa -l inf
-        path         count     size  duration                                 avg_duration      avg_size
-        ---------  -------  -------  ---------------------------------------  --------------  ----------
-        Aggregate   140868  10.6 TB  5 years, 2 months, 28 days and 14 hours  20 minutes         75.3 MB
-        (30 seconds)
+        library media-check --chunk-size 3 --gap 5% ./video.mp4
 
-    Post-actions -- choose what to do after playing:
-        library watch --post-action keep    # do nothing after playing (default)
-        library watch -k delete             # delete file after playing
-        library watch -k softdelete         # mark deleted after playing
+    Delete the file if 20 percent or more of checks fail
 
-        library watch -k ask_keep           # ask whether to keep after playing
-        library watch -k ask_delete         # ask whether to delete after playing
+        library media-check --delete-corrupt 20% ./video.mp4
 
-        library watch -k move               # move to "keep" dir after playing
-        library watch -k ask_move           # ask whether to move to "keep" folder
-        The default location of the keep folder is ./keep/ (relative to the played media file)
-        You can change this by explicitly setting an *absolute* `keep-dir` path:
-        library watch -k ask_move --keep-dir /home/my/music/keep/
+    To scan a large folder use `fsadd`. I recommend something like this two-stage approach:
 
-        library watch -k ask_move_or_delete # ask after each whether to move to "keep" folder or delete
+        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/
+        library media-check (library fs tmp.db -w 'corruption>15' -pf) --full-scan --delete-corrupt 25%
 
-        You can also bind keys in mpv to different exit codes. For example in input.conf:
-            ; quit 5
+    The above can now be done in one command via `--full-scan-if-corrupt`:
 
-        And if you run something like:
-            library watch --cmd5 ~/bin/process_audio.py
-            library watch --cmd5 echo  # this will effectively do nothing except skip the normal post-actions via mpv shortcut
+        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/ --full-scan-if-corrupt 15% --delete-corrupt 25%
 
-        When semicolon is pressed in mpv (it will exit with error code 5) then the applicable player-exit-code command
-        will start with the media file as the first argument; in this case `~/bin/process_audio.py $path`.
-        The command will be daemonized if library exits before it completes.
+    Corruption stats
 
-        To prevent confusion, normal post-actions will be skipped if the exit-code is greater than 4.
-        Exit-codes 0, 1, 2, 3, and 4: the external post-action will run after normal post-actions. Be careful of conflicting player-exit-code command and post-action behavior when using these!
+        library fs tmp.db -w 'corruption>15' -pa
+        path         count  duration             avg_duration         size    avg_size
+        ---------  -------  -------------------  --------------  ---------  ----------
+        Aggregate      907  15 days and 9 hours  24 minutes      130.6 GiB   147.4 MiB
 
-    Experimental options:
-        Duration to play (in seconds) while changing the channel
-        library watch --interdimensional-cable 40
-        library watch -4dtv 40
-        You can open two terminals to replicate AMV Hell somewhat
-        library watch --volume 0 -4dtv 30
-        library listen -4dtv 30
+    Corruption graph
 
-        Playback multiple files at once
-        library watch --multiple-playback    # one per display; or two if only one display detected
-        library watch --multiple-playback 4  # play four media at once, divide by available screens
-        library watch -m 4 --screen-name eDP # play four media at once on specific screen
-        library watch -m 4 --loop --crop     # play four cropped videos on a loop
-        library watch -m 4 --hstack          # use hstack style
+        sqlite --raw-lines tmp.db 'select corruption from media' | lowcharts hist --min 10 --intervals 10
 
-        When using `--multiple-playback` it may be helpful to set simple window focus rules to prevent keys from accidentally being entered in the wrong mpv window (as new windows are created and capture the cursor focus).
-        You can set and restore your previous mouse focus setting by wrapping the command like this:
+        Samples = 931; Min = 10.0; Max = 100.0
+        Average = 39.1; Variance = 1053.103; STD = 32.452
+        each ∎ represents a count of 6
+        [ 10.0 ..  19.0] [561] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
+        [ 19.0 ..  28.0] [ 69] ∎∎∎∎∎∎∎∎∎∎∎
+        [ 28.0 ..  37.0] [ 33] ∎∎∎∎∎
+        [ 37.0 ..  46.0] [ 18] ∎∎∎
+        [ 46.0 ..  55.0] [ 14] ∎∎
+        [ 55.0 ..  64.0] [ 12] ∎∎
+        [ 64.0 ..  73.0] [ 15] ∎∎
+        [ 73.0 ..  82.0] [ 18] ∎∎∎
+        [ 82.0 ..  91.0] [ 50] ∎∎∎∎∎∎∎∎
+        [ 91.0 .. 100.0] [141] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
 
-            focus-under-mouse
-            library watch ... --multiple-playback 4
-            focus-follows-mouse
 
-        For example in KDE:
+</details>
 
-            function focus-under-mouse
-                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusUnderMouse
-                qdbus-qt5 org.kde.KWin /KWin reconfigure
-            end
+###### process-ffmpeg
 
-            function focus-follows-mouse
-                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusFollowsMouse
-                kwriteconfig5 --file kwinrc --group Windows --key NextFocusPrefersMouse true
-                qdbus-qt5 org.kde.KWin /KWin reconfigure
-            end
+<details><summary>Shrink video/audio to AV1/Opus format (.mkv, .mka)</summary>
 
+    $ library process-ffmpeg -h
+    usage: library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
+
+    Resize videos to max 1440x960px AV1 and/or Opus to save space
+
+    Convert audio to Opus. Optionally split up long tracks into multiple files.
+
+        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process --audio
+
+    Use --always-split to _always_ split files if silence is detected
+
+        library process-audio --always-split audiobook.m4a
+
+    Use --split-longer-than to _only_ detect silence for files in excess of a specific duration
+
+        library process-audio --split-longer-than 36mins audiobook.m4b audiobook2.mp3
 
 
 </details>
 
-###### open-links
+###### process-image
 
-<details><summary>Open links from link dbs</summary>
+<details><summary>Shrink images by resizing and AV1 image format (.avif)</summary>
 
-    $ library open-links -h
-    usage: library open-links DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
+    $ library process-image -h
+    usage: library process-image PATH ...
 
-    Open links from a links db
+    Resize images to max 2400x2400px and format AVIF to save space
 
-        wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
-        library open-links music.korea.ln.db
 
-    Only open links once
+</details>
 
-        library open-links ln.db -w 'time_modified=0'
+### Multi-database subcommands
 
-    Print a preview instead of opening tabs
+###### merge-dbs
 
-        library open-links ln.db -p
-        library open-links ln.db --cols time_modified -p
+<details><summary>Merge SQLITE databases</summary>
 
-    Delete rows
+    $ library merge-dbs -h
+    usage: library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
 
-        Make sure you have the right search query
-        library open-links ln.db "query" -p -L inf
-        library open-links ln.db "query" -pa  # view total
+    Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
+    and there is an existing row with the same PK, the default action is to delete the existing row and insert the new row
+    replacing all existing fields.
 
-        library open-links ln.db "query" -pd  # mark as deleted
+    Upsert mode will update each matching PK row such that if a source row has a NULL field and
+    the destination row has a value then the value will be preserved instead of changed to the source row's NULL value.
 
-    Custom search engine
+    Ignore mode (--only-new-rows) will insert only rows which don't already exist in the destination db
 
-        library open-links ln.db --title --prefix 'https://duckduckgo.com/?q='
+    Test first by using temp databases as the destination db.
+    Try out different modes / flags until you are satisfied with the behavior of the program
 
-    Skip local media
+        library merge-dbs --pk path (mktemp --suffix .db) tv.db movies.db
 
-        library open-links dl.db --online
-        library open-links dl.db -w 'path like "http%"'  # equivalent
+    Merge database data and tables
+
+        library merge-dbs --upsert --pk path video.db tv.db movies.db
+        library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path --skip-column id audio-fts.db audio.db
+
+        library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
+        library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
+
+     To skip copying primary-keys from the source table(s) use --business-keys instead of --primary-keys
+
+     Split DBs using --where
 
+         library merge-dbs --pk path specific-site.db big.db -v --only-new-rows -t media,playlists -w 'path like "https://specific-site%"'
 
 
 </details>
 
-###### surf
+###### copy-play-counts
 
-<details><summary>Auto-load browser tabs in a streaming way (stdin)</summary>
+<details><summary>Copy play history</summary>
 
-    $ library surf -h
-    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
+    $ library copy-play-counts -h
+    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
-    Streaming tab loader: press ctrl+c to stop.
+    Copy play count information between databases
 
-    Open tabs from a line-delimited file:
+        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 
-        cat tabs.txt | library surf -n 5
 
-    You will likely want to use this setting in `about:config`
+</details>
 
-        browser.tabs.loadDivertedInBackground = True
+### Filesystem Database subcommands
 
-    If you prefer GUI, check out https://unli.xyz/tabsender/
+###### christen
+
+<details><summary>Clean filenames</summary>
+
+    $ library christen -h
+    usage: library christen DATABASE [--run]
+
+    Rename files to be somewhat normalized
+
+    Default mode is simulate
+
+        library christen fs.db
+
+    To actually do stuff use the run flag
+
+        library christen audio.db --run
+
+    You can optionally replace all the spaces in your filenames with dots
+
+        library christen --dot-space video.db
+
+
+</details>
+
+###### disk-usage
+
+<details><summary>Show disk usage</summary>
+
+    $ library disk-usage -h
+    usage: library disk-usage DATABASE [--sort-groups-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
+
+    Only include files smaller than 1kib
+
+        library disk-usage du.db --size=-1Ki
+        lb du du.db -S-1Ki
+        | path                                  |      size |   count |
+        |---------------------------------------|-----------|---------|
+        | /home/xk/github/xk/lb/__pycache__/    | 620 Bytes |       1 |
+        | /home/xk/github/xk/lb/.github/        |    1.7 kB |       4 |
+        | /home/xk/github/xk/lb/__pypackages__/ |    1.4 MB |    3519 |
+        | /home/xk/github/xk/lb/xklb/           |    4.4 kB |      12 |
+        | /home/xk/github/xk/lb/tests/          |    3.2 kB |       9 |
+        | /home/xk/github/xk/lb/.git/           |  782.4 kB |    2276 |
+        | /home/xk/github/xk/lb/.pytest_cache/  |    1.5 kB |       5 |
+        | /home/xk/github/xk/lb/.ruff_cache/    |   19.5 kB |     100 |
+        | /home/xk/github/xk/lb/.gitattributes  | 119 Bytes |         |
+        | /home/xk/github/xk/lb/.mypy_cache/    | 280 Bytes |       4 |
+        | /home/xk/github/xk/lb/.pdm-python     |  15 Bytes |         |
+
+    Only include files with a specific depth
+
+        library disk-usage du.db --depth 19
+        lb du du.db -d 19
+        | path                                                                                                                                                                |     size |
+        |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
+
+
+
+</details>
+
+###### big-dirs
+
+<details><summary>Show large folders</summary>
+
+    $ library big-dirs -h
+    usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
+
+    See what folders take up space
+
+        library big-dirs video.db
+        library big-dirs audio.db
+        library big-dirs fs.db
+
+    lb big-dirs video.db --folder-size=+10G --lower 400 --upper 14000
+
+    lb big-dirs video.db --depth 5
+    lb big-dirs video.db --depth 7
+
+    You can even sort by auto-MCDA ~LOL~
+
+    lb big-dirs video.db -u 'mcda median_size,-deleted'
+
+
+</details>
+
+###### search-db
+
+<details><summary>Search a SQLITE database</summary>
+
+    $ library search-db -h
+    usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
+
+    Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
+
+
+</details>
+
+###### optimize
+
+<details><summary>Re-optimize database</summary>
+
+    $ library optimize -h
+    usage: library optimize DATABASE [--force]
+
+    Optimize library databases
+
+    The force flag is usually unnecessary and it can take much longer
 
 
 </details>
 
-### Media database subcommands
+### Media Database subcommands
 
 ###### tabs
 
 <details><summary>Open your tabs for the day</summary>
 
     $ library tabs -h
     usage: library tabs DATABASE
@@ -1968,686 +2140,467 @@
     Search and open file
 
         library search fts.db 'two words' --open
 
 
 </details>
 
-### Text subcommands
-
-###### cluster-sort
-
-<details><summary>Sort text and images by similarity</summary>
-
-    $ library cluster-sort -h
-    usage: library cluster-sort [input_path | stdin] [output_path | stdout]
-
-    Group lines of text into sorted output
-
-        echo 'red apple
-        broccoli
-        yellow
-        green
-        orange apple
-        red apple' | library cluster-sort
-
-        orange apple
-        red apple
-        red apple
-        broccoli
-        green
-        yellow
-
-    Show the groupings
-
-        echo 'red apple
-        broccoli
-        yellow
-        green
-        orange apple
-        red apple' | library cluster-sort --print-groups
-
-        [
-            {'grouped_paths': ['orange apple', 'red apple', 'red apple']},
-            {'grouped_paths': ['broccoli', 'green', 'yellow']}
-        ]
-
-    Auto-sort images into directories
-
-        echo 'image1.jpg
-        image2.jpg
-        image3.jpg' | library cluster-sort --image --move-groups
-
-    Print similar paths
-
-        library fs 0day.db -pa --cluster --print-groups
-
-
-
-</details>
-
-###### extract-links
-
-<details><summary>Extract inner links from lists of web links</summary>
-
-    $ library extract-links -h
-    usage: library extract-links PATH ... [--case-sensitive] [--scroll] [--download] [--verbose] [--local-html] [--file FILE] [--path-include ...] [--text-include ...] [--after-include ...] [--before-include ...] [--path-exclude ...] [--text-exclude ...] [--after-exclude ...] [--before-exclude ...]
-
-    Extract links from within local HTML fragments, files, or remote pages; filtering on link text and nearby plain-text
-
-        library links https://en.wikipedia.org/wiki/List_of_bacon_dishes --path-include https://en.wikipedia.org/wiki/ --after-include famous
-        https://en.wikipedia.org/wiki/Omelette
-
-    Read from local clipboard and filter out links based on nearby plain text:
-
-        library links --local-html (cb -t text/html | psub) --after-exclude paranormal spooky horror podcast tech fantasy supernatural lecture sport
-        # note: the equivalent BASH-ism is <(xclip -selection clipboard -t text/html)
-
-    Run with `-vv` to see the browser
-
-
-</details>
-
-###### extract-text
-
-<details><summary>Extract human text from lists of web links</summary>
-
-    $ library extract-text -h
-    usage: library extract-text PATH ... [--skip-links]
-
-    Sorting suggestions
-
-        lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
-
-
-</details>
-
-### File subcommands
-
-###### eda
-
-<details><summary>Exploratory Data Analysis on table-like files</summary>
-
-    $ library eda -h
-    usage: library eda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW] [--repl]
-
-    Perform Exploratory Data Analysis (EDA) on one or more files
-
-    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
-
-
-</details>
-
-###### mcda
-
-<details><summary>Multi-criteria Ranking for Decision Support</summary>
-
-    $ library mcda -h
-    usage: library mcda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW]
-
-    Perform Multiple Criteria Decision Analysis (MCDA) on one or more files
-
-    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
-
-    $ library mcda ~/storage.csv --minimize price --ignore warranty
-
-        ### Goals
-        #### Maximize
-        - size
-        #### Minimize
-        - price
-
-        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
-        |----|---------|--------|------------|----------|------------|----------|---------|
-        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
-        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
-        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
-
-    $ library mcda ~/storage.csv --ignore warranty
-
-        ### Goals
-        #### Maximize
-        - price
-        - size
-
-        |    |   price |   size |   warranty |   TOPSIS |     MABAC |   SPOTIS |   BORDA |
-        |----|---------|--------|------------|----------|-----------|----------|---------|
-        |  2 |     519 |     44 |          2 | 1        |  0.536587 | 0        | 7.46341 |
-        |  1 |     453 |     40 |          2 | 0.580079 |  0.103888 | 0.432699 | 7.88333 |
-        |  0 |     359 |     36 |          5 | 0        | -0.463413 | 1        | 8.46341 |
-
-    $ library mcda ~/storage.csv --minimize price --ignore warranty
-
-        ### Goals
-        #### Maximize
-        - size
-        #### Minimize
-        - price
-
-        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
-        |----|---------|--------|------------|----------|------------|----------|---------|
-        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
-        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
-        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
-
-    It also works with HTTP/GCS/S3 URLs:
-
-    $ library mcda https://en.wikipedia.org/wiki/List_of_Academy_Award-winning_films --clean --minimize Year
-
-        ### Goals
-
-        #### Maximize
-
-        - Nominations
-        - Awards
-
-        #### Minimize
-
-        - Year
-
-        |      | Film                                                                    |   Year |   Awards |   Nominations |      TOPSIS |    MABAC |      SPOTIS |   BORDA |
-        |------|-------------------------------------------------------------------------|--------|----------|---------------|-------------|----------|-------------|---------|
-        |  378 | Titanic                                                                 |   1997 |       11 |            14 | 0.999993    | 1.38014  | 4.85378e-06 | 4116.62 |
-        |  868 | Ben-Hur                                                                 |   1959 |       11 |            12 | 0.902148    | 1.30871  | 0.0714303   | 4116.72 |
-        |  296 | The Lord of the Rings: The Return of the King                           |   2003 |       11 |            11 | 0.8558      | 1.27299  | 0.107147    | 4116.76 |
-        | 1341 | West Side Story                                                         |   1961 |       10 |            11 | 0.837716    | 1.22754  | 0.152599    | 4116.78 |
-        |  389 | The English Patient                                                     |   1996 |        9 |            12 | 0.836725    | 1.2178   | 0.162341    | 4116.78 |
-        | 1007 | Gone with the Wind                                                      |   1939 |        8 |            13 | 0.807086    | 1.20806  | 0.172078    | 4116.81 |
-        |  990 | From Here to Eternity                                                   |   1953 |        8 |            13 | 0.807086    | 1.20806  | 0.172079    | 4116.81 |
-        | 1167 | On the Waterfront                                                       |   1954 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
-        | 1145 | My Fair Lady                                                            |   1964 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
-        |  591 | Gandhi                                                                  |   1982 |        8 |            11 | 0.755312    | 1.13663  | 0.243509    | 4116.86 |
-
-
-</details>
-
-###### incremental-diff
-
-<details><summary>Diff large table-like files in chunks</summary>
-
-    $ library incremental-diff -h
-    usage: library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
-
-    See data differences in an incremental way to quickly see how two different files differ.
-
-    Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
-
-    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared.
-    If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
-
-    To diff everything at once run with `--batch-size inf`
-
-
-</details>
-
-###### media-check
-
-<details><summary>Check video and audio files for corruption via ffmpeg</summary>
-
-    $ library media-check -h
-    usage: library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
-
-    Defaults to decode 0.5 second per 10% of each file
-
-        library media-check ./video.mp4
-
-    Decode all the frames of each file to evaluate how corrupt it is
-    (scantime is very slow; about 150 seconds for an hour-long file)
-
-        library media-check --full-scan ./video.mp4
-
-    Decode all the packets of each file to evaluate how corrupt it is
-    (scantime is about one second of each file but only accurate for formats where 1 packet == 1 frame)
-
-        library media-check --full-scan --gap 0 ./video.mp4
-
-    Decode all audio of each file to evaluate how corrupt it is
-    (scantime is about four seconds per file)
-
-        library media-check --full-scan --audio ./video.mp4
-
-    Decode at least one frame at the start and end of each file to evaluate how corrupt it is
-    (scantime is about one second per file)
-
-        library media-check --chunk-size 5% --gap 99.9% ./video.mp4
-
-    Decode 3s every 5% of a file to evaluate how corrupt it is
-    (scantime is about three seconds per file)
-
-        library media-check --chunk-size 3 --gap 5% ./video.mp4
-
-    Delete the file if 20 percent or more of checks fail
-
-        library media-check --delete-corrupt 20% ./video.mp4
-
-    To scan a large folder use `fsadd`. I recommend something like this two-stage approach:
-
-        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/
-        library media-check (library fs tmp.db -w 'corruption>15' -pf) --full-scan --delete-corrupt 25%
-
-    The above can now be done in one command via `--full-scan-if-corrupt`:
-
-        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/ --full-scan-if-corrupt 15% --delete-corrupt 25%
-
-    Corruption stats
-
-        library fs tmp.db -w 'corruption>15' -pa
-        path         count  duration             avg_duration         size    avg_size
-        ---------  -------  -------------------  --------------  ---------  ----------
-        Aggregate      907  15 days and 9 hours  24 minutes      130.6 GiB   147.4 MiB
-
-    Corruption graph
-
-        sqlite --raw-lines tmp.db 'select corruption from media' | lowcharts hist --min 10 --intervals 10
-
-        Samples = 931; Min = 10.0; Max = 100.0
-        Average = 39.1; Variance = 1053.103; STD = 32.452
-        each ∎ represents a count of 6
-        [ 10.0 ..  19.0] [561] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-        [ 19.0 ..  28.0] [ 69] ∎∎∎∎∎∎∎∎∎∎∎
-        [ 28.0 ..  37.0] [ 33] ∎∎∎∎∎
-        [ 37.0 ..  46.0] [ 18] ∎∎∎
-        [ 46.0 ..  55.0] [ 14] ∎∎
-        [ 55.0 ..  64.0] [ 12] ∎∎
-        [ 64.0 ..  73.0] [ 15] ∎∎
-        [ 73.0 ..  82.0] [ 18] ∎∎∎
-        [ 82.0 ..  91.0] [ 50] ∎∎∎∎∎∎∎∎
-        [ 91.0 .. 100.0] [141] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-
-
-</details>
-
-###### sample-hash
-
-<details><summary>Calculate a hash based on small file segments</summary>
-
-    $ library sample-hash -h
-    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
-
-    Calculate hashes for large files by reading only small segments of each file
-
-        library sample-hash ./my_file.mkv
-
-    The threads flag seems to be faster for rotational media but slower on SSDs
-
-
-</details>
-
-###### sample-compare
-
-<details><summary>Compare files using sample-hash and other shortcuts</summary>
-
-    $ library sample-compare -h
-    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
-
-    Convenience subcommand to compare multiple files using sample-hash
-
-
-</details>
-
-### Folder subcommands
-
-###### merge-folders
-
-<details><summary>Merge two or more file trees</summary>
-
-    $ library merge-folders -h
-    usage: library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
-
-    Merge multiple folders with the same file tree into a single folder.
-
-    https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
-
-    Trumps are new or replaced files from an earlier source which now conflict with a later source.
-    If you only have one source then the count of trumps will always be zero.
-    The count of conflicts also includes trumps.
-
-
-</details>
-
-###### relmv
+### Playback subcommands
 
-<details><summary>Move files preserving parent folder hierarchy</summary>
+###### watch
 
-    $ library relmv -h
-    usage: library relmv [--simulate] SOURCE ... DEST
+<details><summary>Watch / Listen</summary>
 
-    Move files/folders without losing hierarchy metadata
+    $ library watch -h
+    usage: library watch DATABASE [optional args]
 
-    Move fresh music to your phone every Sunday:
+    Control playback:
+        To stop playback press Ctrl-C in either the terminal or mpv
 
-        # move last week music back to their source folders
-        library mv /mnt/d/sync/weekly/ /mnt/d/check/audio/
+        Create global shortcuts in your desktop environment by sending commands to mpv_socket:
+        echo 'playlist-next force' | socat - /tmp/mpv_socket
 
-        # move new music for this week
-        library relmv (
-            library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
-        ) /mnt/d/sync/weekly/
+    Override the default player (mpv):
+        library does a lot of things to try to automatically use your preferred media player
+        but if it doesn't guess right you can make it explicit:
+        library watch --player "vlc --vlc-opts"
 
+    Cast to chromecast groups:
+        library watch --cast --cast-to "Office pair"
+        library watch -ct "Office pair"  # equivalent
+        If you don't know the exact name of your chromecast group run `catt scan`
 
-</details>
+    Play media in order (similarly named episodes):
+        library watch --play-in-order
+        library watch -O    # equivalent
 
-###### mv-list
+        The default sort value is 'natural_ps' which means media will be sorted by parent path
+        and then stem in a natural way (using the integer values within the path). But there are many other options:
 
-<details><summary>Find specific folders to move to different disks</summary>
+        Options:
 
-    $ library mv-list -h
-    usage: library mv-list [--limit LIMIT] [--lower LOWER] [--upper UPPER] MOUNT_POINT DATABASE
+            - reverse: reverse the sort order
+            - compat: treat characters like '⑦' as '7'
 
-    Free up space on a specific disk. Find candidates for moving data to a different mount point
+        Algorithms:
 
+            - natural: parse numbers as integers
+            - os: sort similar to the OS File Explorer sorts. To improve non-alphanumeric sorting on Mac OS X and Linux it is necessary to install pyicu (perhaps via python3-icu -- https://gitlab.pyicu.org/main/pyicu#installing-pyicu)
+            - path: use natsort "path" algorithm (https://natsort.readthedocs.io/en/stable/api.html#the-ns-enum)
+            - human: use system locale
+            - ignorecase: treat all case as equal
+            - lowercase: sort lowercase first
+            - signed: sort with an understanding of negative numbers
+            - python: sort like default python
 
-    The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
+        Values:
 
-        library fsadd --filesystem d.db ~/d/
+            - path
+            - parent
+            - stem
+            - title (or any other column value)
+            - ps: parent, stem
+            - pts: parent, title, stem
 
-    But this should definitely also work with xklb audio and video databases:
+        Use this format: algorithm, value, algorithm_value, or option_algorithm_value.
+        For example:
 
-        library mv-list /mnt/d/ video.db
+            - library watch -O human
+            - library watch -O title
+            - library watch -O human_title
+            - library watch -O reverse_compat_human_title
 
-    The program will print a table with a sorted list of folders which are good candidates for moving.
-    Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over).
-    The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
+            - library watch -O path       # path algorithm and parent, stem values (path_ps)
+            - library watch -O path_path  # path algorithm and path values
 
-        ...
-        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-        │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
-        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-        │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
-        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-        │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
-        ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
-        6702 other folders not shown
+        Also, if you are using --random you need to fetch sibling media to play the media in order:
 
-        ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
-        ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
-        ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
-        ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
-        ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
-        ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
+            - library watch --random --fetch-siblings each -O          # get the first result per directory
+            - library watch --random --fetch-siblings if-audiobook -O  # get the first result per directory if 'audiobook' is in the path
+            - library watch --random --fetch-siblings always -O        # get 2,000 results per directory
 
-        Type "done" when finished
-        Type "more" to see more files
-        Paste a folder (and press enter) to toggle selection
-        Type "*" to select all files in the most recently printed table
+        If searching by a specific subpath it may be preferable to just sort by path instead
+        library watch d/planet.earth.2024/ -u path
 
-    Then it will give you a prompt:
+        library watch --related  # Similar to -O but uses fts to find similar content
+        library watch -R         # equivalent
+        library watch -RR        # above, plus ignores most filters
 
-        Paste a path:
+        library watch --cluster  # cluster-sort to put similar-named paths closer together
+        library watch -C         # equivalent
 
-    Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
+        library watch --big-dirs # Recommended to use with --duration or --depth filters; see `lb big-dirs -h` for more info
+        library watch -B         # equivalent
 
-        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-        26 selected paths: 162.1 GB ; future free space: 486.9 GB
+        All of these options can be used together but it will be a bit slow and the results might be mid-tier
+        as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
+        library watch -RRCO
 
-    You can also press the up arrow or paste it again to remove it from the list:
+        You can even sort the items within each cluster by auto-MCDA ~LOL~
+        library watch -B --sort-groups-by 'mcda median_size,-deleted'
+        library watch -C --sort-groups-by 'mcda median_size,-deleted'
 
-        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-        25 selected paths: 159.9 GB ; future free space: 484.7 GB
+    Filter media by file siblings of parent directory:
+        library watch --sibling   # only include files which have more than or equal to one sibling
+        library watch --solo      # only include files which are alone by themselves
 
-    After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
+        `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
+        library watch --sibling --solo      # you will always get zero records here
+        library watch --lower 2 --upper 1   # equivalent
 
-        Paste a path: done
+        You can be more specific via the `--upper` and `--lower` flags
+        library watch --lower 3   # only include files which have three or more siblings
+        library watch --upper 3   # only include files which have fewer than three siblings
+        library watch --lower 3 --upper 3   # only include files which are three siblings inclusive
+        library watch --lower 12 --upper 25 -O  # on my machine this launches My Mister 2018
 
-            Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
+    Play recent partially-watched videos (requires mpv history):
+        library watch --partial       # play newest first
 
-                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
+        library watch --partial old   # play oldest first
+        library watch -P o            # equivalent
 
+        library watch -P p            # sort by percent remaining
+        library watch -P t            # sort by time remaining
+        library watch -P s            # skip partially watched (only show unseen)
 
-</details>
+        The default time used is "last-viewed" (ie. the most recent time you closed the video)
+        If you want to use the "first-viewed" time (ie. the very first time you opened the video)
+        library watch -P f            # use watch_later file creation time instead of modified time
 
-###### scatter
+        You can combine most of these options, though some will be overridden by others.
+        library watch -P fo           # this means "show the oldest videos using the time I first opened them"
+        library watch -P pt           # weighted remaining (percent * time remaining)
 
-<details><summary>Scatter files between folders or disks</summary>
+    Print instead of play:
+        library watch --print --limit 10  # print the next 10 files
+        library watch -p -L 10  # print the next 10 files
+        library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
-    $ library scatter -h
-    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
+        Printing modes
+        library watch -p    # print as a table
+        library watch -p a  # print an aggregate report
+        library watch -p b  # print a big-dirs report (see library bigdirs -h for more info)
+        library watch -p f  # print fields (defaults to path; use --cols to change)
+                               # -- useful for piping paths to utilities like xargs or GNU Parallel
 
-    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+        library watch -p d  # mark deleted
+        library watch -p w  # mark watched
 
-    Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
+        Some printing modes can be combined
+        library watch -p df  # print files for piping into another program and mark them as deleted within the db
+        library watch -p bf  # print fields from big-dirs report
 
-        library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+        Check if you have downloaded something before
+        library watch -u duration -p -s 'title'
 
-    Reduce number of files per folder (creates more folders)
+        Print an aggregate report of deleted media
+        library watch -w time_deleted!=0 -p=a
+        ╒═══════════╤══════════════╤═════════╤═════════╕
+        │ path      │ duration     │ size    │   count │
+        ╞═══════════╪══════════════╪═════════╪═════════╡
+        │ Aggregate │ 14 days, 23  │ 50.6 GB │   29058 │
+        │           │ hours and 42 │         │         │
+        │           │ minutes      │         │         │
+        ╘═══════════╧══════════════╧═════════╧═════════╛
+        Total duration: 14 days, 23 hours and 42 minutes
 
-        library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
+        Print an aggregate report of media that has no duration information (ie. online or corrupt local media)
+        library watch -w 'duration is null' -p=a
 
-    Multi-device re-bin: balance by size
+        Print a list of filenames which have below 1280px resolution
+        library watch -w 'width<1280' -p=f
 
-        library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs.db subfolder/of/mergerfs/mnt
-        Current path distribution:
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+        Print media you have partially viewed with mpv
+        library watch --partial -p
+        library watch -P -p  # equivalent
+        library watch -P -p f --cols path,progress,duration  # print CSV of partially watched files
+        library watch --partial -pa  # print an aggregate report of partially watched files
 
-        Simulated path distribution:
-        5845 files should be moved
-        20257 files should not be moved
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
-        ### Move 1182 files to /mnt/d7 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
-        ### Move 1198 files to /mnt/d6 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
-        ### Move 1146 files to /mnt/d5 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
-        ### Move 1185 files to /mnt/d3 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
-        ### Move 1134 files to /mnt/d4 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+        View how much time you have watched
+        library watch -w play_count'>'0 -p=a
 
-    Multi-device re-bin: balance device inodes for specific subfolder
+        See how much video you have
+        library watch video.db -p=a
+        ╒═══════════╤═════════╤═════════╤═════════╕
+        │ path      │   hours │ size    │   count │
+        ╞═══════════╪═════════╪═════════╪═════════╡
+        │ Aggregate │  145769 │ 37.6 TB │  439939 │
+        ╘═══════════╧═════════╧═════════╧═════════╛
+        Total duration: 16 years, 7 months, 19 days, 17 hours and 25 minutes
 
-        library scatter -m /mnt/d1:/mnt/d2 fs.db subfolder --group count --sort 'size desc'
+        View all the columns
+        library watch -p -L 1 --cols '*'
 
-    Multi-device re-bin: only consider the most recent 100 files
+        Open ipython with all of your media
+        library watch -vv -p --cols '*'
+        ipdb> len(media)
+        462219
 
-        library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
+    Set the play queue size:
+        By default the play queue is 120--long enough that you likely have not noticed
+        but short enough that the program is snappy.
 
-    Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
+        If you want everything in your play queue you can use the aid of infinity.
+        Pick your poison (these all do effectively the same thing):
+        library watch -L inf
+        library watch -l inf
+        library watch --queue inf
+        library watch -L 999999999999
 
-        library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
+        You may also want to restrict the play queue.
+        For example, when you only want 1000 random files:
+        library watch -u random -L 1000
 
+    Offset the play queue:
+        You can also offset the queue. For example if you want to skip one or ten media:
+        library watch --offset 10      # offset ten from the top of an ordered query
 
-</details>
+    Repeat
+        library watch                  # listen to 120 random songs (DEFAULT_PLAY_QUEUE)
+        library watch --limit 5        # listen to FIVE songs
+        library watch -l inf -u random # listen to random songs indefinitely
+        library watch -s infinite      # listen to songs from the band infinite
 
-### Multi-database subcommands
+    Constrain media by search:
+        Audio files have many tags to readily search through so metadata like artist,
+        album, and even mood are included in search.
+        Video files have less consistent metadata and so only paths are included in search.
+        library watch --include happy  # only matches will be included
+        library watch -s happy         # equivalent
+        library watch --exclude sad    # matches will be excluded
+        library watch -E sad           # equivalent
 
-###### merge-dbs
+        Search only the path column
+        library watch -O -s 'path : mad max'
+        library watch -O -s 'path : "mad max"' # add "quotes" to be more strict
 
-<details><summary>Merge SQLITE databases</summary>
+        Double spaces are parsed as one space
+        library watch -s '  ost'        # will match OST and not ghost
+        library watch -s toy story      # will match '/folder/toy/something/story.mp3'
+        library watch -s 'toy  story'   # will match more strictly '/folder/toy story.mp3'
 
-    $ library merge-dbs -h
-    usage: library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
+        You can search without -s but it must directly follow the database due to how argparse works
+        library watch ./your.db searching for something
 
-    Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
-    and there is an existing row with the same PK, the default action is to delete the existing row and insert the new row
-    replacing all existing fields.
+    Constrain media by arbitrary SQL expressions:
+        library watch --where audio_count = 2  # media which have two audio tracks
+        library watch -w "language = 'eng'"    # media which have an English language tag
+                                                    (this could be audio _or_ subtitle)
+        library watch -w subtitle_count=0      # media that doesn't have subtitles
 
-    Upsert mode will update each matching PK row such that if a source row has a NULL field and
-    the destination row has a value then the value will be preserved instead of changed to the source row's NULL value.
+    Constrain media to duration (in minutes):
+        library watch --duration 20
+        library watch -d 6  # 6 mins ±10 percent (ie. between 5 and 7 mins)
+        library watch -d-6  # less than 6 mins
+        library watch -d+6  # more than 6 mins
 
-    Ignore mode (--only-new-rows) will insert only rows which don't already exist in the destination db
+        Duration can be specified multiple times:
+        library watch -d+5 -d-7  # should be similar to -d 6
 
-    Test first by using temp databases as the destination db.
-    Try out different modes / flags until you are satisfied with the behavior of the program
+        If you want exact time use `where`
+        library watch --where 'duration=6*60'
 
-        library merge-dbs --pk path (mktemp --suffix .db) tv.db movies.db
+    Constrain media to file size (in megabytes):
+        library watch --size 20
+        library watch -S 6  # 6 MB ±10 percent (ie. between 5 and 7 MB)
+        library watch -S-6  # less than 6 MB
+        library watch -S+6  # more than 6 MB
 
-    Merge database data and tables
+    Constrain media by time_created / time_last_played / time_deleted / time_modified:
+        library watch --created-within '3 days'
+        library watch --created-before '3 years'
 
-        library merge-dbs --upsert --pk path video.db tv.db movies.db
-        library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path --skip-column id audio-fts.db audio.db
+    Constrain media by throughput:
+        Bitrate information is not explicitly saved.
+        You can use file size and duration as a proxy for throughput:
+        library watch -w 'size/duration<50000'
 
-        library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
-        library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
+    Constrain media to portrait orientation video:
+        library watch --portrait
+        library watch -w 'width<height' # equivalent
 
-     To skip copying primary-keys from the source table(s) use --business-keys instead of --primary-keys
+    Constrain media to duration of videos which match any size constraints:
+        library watch --duration-from-size +700 -u 'duration desc, size desc'
 
-     Split DBs using --where
+    Constrain media to online-media or local-media:
+        Not to be confused with only local-media which is not "offline" (ie. one HDD disconnected)
+        library watch --online-media-only
+        library watch --online-media-only -i  # and ignore playback errors (ie. YouTube video deleted)
+        library watch --local-media-only
 
-         library merge-dbs --pk path specific-site.db big.db -v --only-new-rows -t media,playlists -w 'path like "https://specific-site%"'
+    Specify media play order:
+        library watch --sort duration   # play shortest media first
+        library watch -u duration desc  # play longest media first
 
+        You can use multiple SQL ORDER BY expressions
+        library watch -u 'subtitle_count > 0 desc' # play media that has at least one subtitle first
 
-</details>
+        Prioritize large-sized media
+        library watch --sort 'ntile(10000) over (order by size/duration) desc'
+        library watch -u 'ntile(100) over (order by size) desc'
 
-###### copy-play-counts
+        Sort by count of media with the same-X column (default DESC: most common to least common value)
+        library watch -u same-duration
+        library watch -u same-title
+        library watch -u same-size
+        library watch -u same-width, same-height ASC, same-fps
+        library watch -u same-time_uploaded same-view_count same-upvote_ratio
 
-<details><summary>Copy play history</summary>
+        No media found when using --random
+        In addition to -u/--sort random, there is also the -r/--random flag.
+        If you have a large database it should be faster than -u random but it comes with a caveat:
+        This flag randomizes via rowid at an earlier stage to boost performance.
+        It is possible that you see "No media found" or a smaller amount of media than correct.
+        You can bypass this by setting --limit. For example:
+        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa
+        path         count      size  duration                        avg_duration      avg_size
+        ---------  -------  --------  ------------------------------  --------------  ----------
+        Aggregate    10000  752.5 GB  4 months, 15 days and 10 hours  20 minutes         75.3 MB
+        (17 seconds)
+        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa -l inf
+        path         count     size  duration                                 avg_duration      avg_size
+        ---------  -------  -------  ---------------------------------------  --------------  ----------
+        Aggregate   140868  10.6 TB  5 years, 2 months, 28 days and 14 hours  20 minutes         75.3 MB
+        (30 seconds)
 
-    $ library copy-play-counts -h
-    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
+    Post-actions -- choose what to do after playing:
+        library watch --post-action keep    # do nothing after playing (default)
+        library watch -k delete             # delete file after playing
+        library watch -k softdelete         # mark deleted after playing
 
-    Copy play count information between databases
+        library watch -k ask_keep           # ask whether to keep after playing
+        library watch -k ask_delete         # ask whether to delete after playing
 
-        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
+        library watch -k move               # move to "keep" dir after playing
+        library watch -k ask_move           # ask whether to move to "keep" folder
+        The default location of the keep folder is ./keep/ (relative to the played media file)
+        You can change this by explicitly setting an *absolute* `keep-dir` path:
+        library watch -k ask_move --keep-dir /home/my/music/keep/
 
+        library watch -k ask_move_or_delete # ask after each whether to move to "keep" folder or delete
 
-</details>
+        You can also bind keys in mpv to different exit codes. For example in input.conf:
+            ; quit 5
 
-### Filesystem Database subcommands
+        And if you run something like:
+            library watch --cmd5 ~/bin/process_audio.py
+            library watch --cmd5 echo  # this will effectively do nothing except skip the normal post-actions via mpv shortcut
 
-###### christen
+        When semicolon is pressed in mpv (it will exit with error code 5) then the applicable player-exit-code command
+        will start with the media file as the first argument; in this case `~/bin/process_audio.py $path`.
+        The command will be daemonized if library exits before it completes.
 
-<details><summary>Clean filenames</summary>
+        To prevent confusion, normal post-actions will be skipped if the exit-code is greater than 4.
+        Exit-codes 0, 1, 2, 3, and 4: the external post-action will run after normal post-actions. Be careful of conflicting player-exit-code command and post-action behavior when using these!
 
-    $ library christen -h
-    usage: library christen DATABASE [--run]
+    Experimental options:
+        Duration to play (in seconds) while changing the channel
+        library watch --interdimensional-cable 40
+        library watch -4dtv 40
+        You can open two terminals to replicate AMV Hell somewhat
+        library watch --volume 0 -4dtv 30
+        library listen -4dtv 30
 
-    Rename files to be somewhat normalized
+        Playback multiple files at once
+        library watch --multiple-playback    # one per display; or two if only one display detected
+        library watch --multiple-playback 4  # play four media at once, divide by available screens
+        library watch -m 4 --screen-name eDP # play four media at once on specific screen
+        library watch -m 4 --loop --crop     # play four cropped videos on a loop
+        library watch -m 4 --hstack          # use hstack style
 
-    Default mode is simulate
+        When using `--multiple-playback` it may be helpful to set simple window focus rules to prevent keys from accidentally being entered in the wrong mpv window (as new windows are created and capture the cursor focus).
+        You can set and restore your previous mouse focus setting by wrapping the command like this:
 
-        library christen fs.db
+            focus-under-mouse
+            library watch ... --multiple-playback 4
+            focus-follows-mouse
 
-    To actually do stuff use the run flag
+        For example in KDE:
 
-        library christen audio.db --run
+            function focus-under-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusUnderMouse
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
 
-    You can optionally replace all the spaces in your filenames with dots
+            function focus-follows-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusFollowsMouse
+                kwriteconfig5 --file kwinrc --group Windows --key NextFocusPrefersMouse true
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
 
-        library christen --dot-space video.db
 
 
 </details>
 
-###### disk-usage
-
-<details><summary>Show disk usage</summary>
-
-    $ library disk-usage -h
-    usage: library disk-usage DATABASE [--sort-groups-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
+###### open-links
 
-    Only include files smaller than 1kib
+<details><summary>Open links from link dbs</summary>
 
-        library disk-usage du.db --size=-1Ki
-        lb du du.db -S-1Ki
-        | path                                  |      size |   count |
-        |---------------------------------------|-----------|---------|
-        | /home/xk/github/xk/lb/__pycache__/    | 620 Bytes |       1 |
-        | /home/xk/github/xk/lb/.github/        |    1.7 kB |       4 |
-        | /home/xk/github/xk/lb/__pypackages__/ |    1.4 MB |    3519 |
-        | /home/xk/github/xk/lb/xklb/           |    4.4 kB |      12 |
-        | /home/xk/github/xk/lb/tests/          |    3.2 kB |       9 |
-        | /home/xk/github/xk/lb/.git/           |  782.4 kB |    2276 |
-        | /home/xk/github/xk/lb/.pytest_cache/  |    1.5 kB |       5 |
-        | /home/xk/github/xk/lb/.ruff_cache/    |   19.5 kB |     100 |
-        | /home/xk/github/xk/lb/.gitattributes  | 119 Bytes |         |
-        | /home/xk/github/xk/lb/.mypy_cache/    | 280 Bytes |       4 |
-        | /home/xk/github/xk/lb/.pdm-python     |  15 Bytes |         |
+    $ library open-links -h
+    usage: library open-links DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
 
-    Only include files with a specific depth
+    Open links from a links db
 
-        library disk-usage du.db --depth 19
-        lb du du.db -d 19
-        | path                                                                                                                                                                |     size |
-        |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
-        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
-        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
+        wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
+        library open-links music.korea.ln.db
 
+    Only open links once
 
+        library open-links ln.db -w 'time_modified=0'
 
-</details>
+    Print a preview instead of opening tabs
 
-###### big-dirs
+        library open-links ln.db -p
+        library open-links ln.db --cols time_modified -p
 
-<details><summary>Show large folders</summary>
+    Delete rows
 
-    $ library big-dirs -h
-    usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
+        Make sure you have the right search query
+        library open-links ln.db "query" -p -L inf
+        library open-links ln.db "query" -pa  # view total
 
-    See what folders take up space
+        library open-links ln.db "query" -pd  # mark as deleted
 
-        library big-dirs video.db
-        library big-dirs audio.db
-        library big-dirs fs.db
+    Custom search engine
 
-    lb big-dirs video.db --folder-size=+10G --lower 400 --upper 14000
+        library open-links ln.db --title --prefix 'https://duckduckgo.com/?q='
 
-    lb big-dirs video.db --depth 5
-    lb big-dirs video.db --depth 7
+    Skip local media
 
-    You can even sort by auto-MCDA ~LOL~
+        library open-links dl.db --online
+        library open-links dl.db -w 'path like "http%"'  # equivalent
 
-    lb big-dirs video.db -u 'mcda median_size,-deleted'
 
 
 </details>
 
-###### search-db
-
-<details><summary>Search a SQLITE database</summary>
-
-    $ library search-db -h
-    usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
+###### surf
 
-    Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
+<details><summary>Auto-load browser tabs in a streaming way (stdin)</summary>
 
+    $ library surf -h
+    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
 
-</details>
+    Streaming tab loader: press ctrl+c to stop.
 
-###### optimize
+    Open tabs from a line-delimited file:
 
-<details><summary>Re-optimize database</summary>
+        cat tabs.txt | library surf -n 5
 
-    $ library optimize -h
-    usage: library optimize DATABASE [--force]
+    You will likely want to use this setting in `about:config`
 
-    Optimize library databases
+        browser.tabs.loadDivertedInBackground = True
 
-    The force flag is usually unnecessary and it can take much longer
+    If you prefer GUI, check out https://unli.xyz/tabsender/
 
 
 </details>
 
-### Single database enrichment subcommands
+### Database enrichment subcommands
 
 ###### dedupe-db
 
 <details><summary>Dedupe SQLITE tables</summary>
 
     $ library dedupe-db -h
     usage: library dedupe-dbs DATABASE TABLE --bk BUSINESS_KEYS [--pk PRIMARY_KEYS] [--only-columns COLUMNS]
@@ -2745,60 +2698,118 @@
         library tabs-shuffle tabs.db -d  31 -f monthly
         library tabs-shuffle tabs.db -d  90 -f quarterly
         library tabs-shuffle tabs.db -d 365 -f yearly
 
 
 </details>
 
-### Misc subcommands
+### Update database subcommands
 
-###### export-text
+###### fsupdate
 
-<details><summary>Export HTML files from SQLite databases</summary>
+<details><summary>Update local media</summary>
 
-    $ library export-text -h
-    usage: library export-text DATABASE
+    $ library fsupdate -h
+    usage: library fsupdate DATABASE
 
-    Generate HTML files from SQLite databases
+    Update each path previously saved:
+
+        library fsupdate video.db
 
 
 </details>
 
-###### process-ffmpeg
+###### tubeupdate
 
-<details><summary>Shrink video/audio to AV1/Opus format (.mkv, .mka)</summary>
+<details><summary>Update online video media</summary>
 
-    $ library process-ffmpeg -h
-    usage: library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
+    $ library tubeupdate -h
+    usage: library tubeupdate [--audio | --video] DATABASE
 
-    Resize videos to max 1440x960px AV1 and/or Opus to save space
+    Fetch the latest videos for every playlist saved in your database
 
-    Convert audio to Opus. Optionally split up long tracks into multiple files.
+        library tubeupdate educational.db
 
-        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process --audio
+    Fetch extra metadata:
 
-    Use --always-split to _always_ split files if silence is detected
+        By default tubeupdate will quickly add media.
+        You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
 
-        library process-audio --always-split audiobook.m4a
+        library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 
-    Use --split-longer-than to _only_ detect silence for files in excess of a specific duration
+    Remove duplicate playlists:
 
-        library process-audio --split-longer-than 36mins audiobook.m4b audiobook2.mp3
+        lb dedupe-db video.db playlists --bk extractor_playlist_id
 
 
 </details>
 
-###### process-image
+###### webupdate
 
-<details><summary>Shrink images by resizing and AV1 image format (.avif)</summary>
+<details><summary>Update open-directory media</summary>
 
-    $ library process-image -h
-    usage: library process-image PATH ...
+    $ library webupdate -h
+    usage: library web-update DATABASE
 
-    Resize images to max 2400x2400px and format AVIF to save space
+    Update saved open directories
+
+
+
+</details>
+
+###### galleryupdate
+
+<details><summary>Update online gallery media</summary>
+
+    $ library galleryupdate -h
+    usage: library galleryupdate DATABASE URLS
+
+    Check previously saved gallery_dl URLs for new content
+
+
+</details>
+
+###### links-update
+
+<details><summary>Update a link-scraping database</summary>
+
+    $ library links-update -h
+    usage: library links-update DATABASE
+
+    Fetch new links from each path previously saved
+
+        library links-update links.db
+
+
+</details>
+
+###### redditupdate
+
+<details><summary>Update reddit media</summary>
+
+    $ library redditupdate -h
+    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+
+    Fetch the latest posts for every subreddit/redditor saved in your database
+
+        library redditupdate edu_subreddits.db
+
+
+</details>
+
+### Misc subcommands
+
+###### export-text
+
+<details><summary>Export HTML files from SQLite databases</summary>
+
+    $ library export-text -h
+    usage: library export-text DATABASE
+
+    Generate HTML files from SQLite databases
 
 
 </details>
 
 
 <details><summary>Chicken mode</summary>
```

### Comparing `xklb-2.6.6/PKG-INFO` & `xklb-2.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.6.6
+Version: 2.6.7
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -90,22 +90,23 @@
 
 A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
+<img align="right" width="300" height="600" src="https://raw.githubusercontent.com/chapmanjacobd/library/main/.github/examples/art.avif" />
+
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
 Should also work on Mac OS.
-<img align="right" width="400" src="https://raw.githubusercontent.com/chapmanjacobd/library/main/.github/examples/tubeadd.svg" />
 
 ### External dependencies
 
 Required: `ffmpeg`
 
 Some features work better with: `mpv`, `firefox`, `fish`
 
@@ -180,15 +181,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.006)
+    xk media library subcommands (v2.6.007)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -213,102 +214,61 @@
     │ tildes        │ Backup tildes comments and topics                  │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ places-import │ Import places of interest (POIs)                   │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ add-row       │ Add arbitrary data to SQLITE                       │
     ╰───────────────┴────────────────────────────────────────────────────╯
 
-    Update database subcommands:
-    ╭───────────────┬─────────────────────────────────╮
-    │ fsupdate      │ Update local media              │
-    ├───────────────┼─────────────────────────────────┤
-    │ tubeupdate    │ Update online video media       │
-    ├───────────────┼─────────────────────────────────┤
-    │ webupdate     │ Update open-directory media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ galleryupdate │ Update online gallery media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ links-update  │ Update a link-scraping database │
-    ├───────────────┼─────────────────────────────────┤
-    │ redditupdate  │ Update reddit media             │
-    ╰───────────────┴─────────────────────────────────╯
-
-    Playback subcommands:
-    ╭────────────┬───────────────────────────────────────────────────╮
-    │ watch      │ Watch / Listen                                    │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ now        │ Show what is currently playing                    │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ next       │ Play next file and optionally delete current file │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ stop       │ Stop all playback                                 │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ pause      │ Pause all playback                                │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ open-links │ Open links from link dbs                          │
-    ├────────────┼───────────────────────────────────────────────────┤
-    │ surf       │ Auto-load browser tabs in a streaming way (stdin) │
-    ╰────────────┴───────────────────────────────────────────────────╯
-
-    Media database subcommands:
-    ╭─────────────────┬────────────────────────────────╮
-    │ tabs            │ Open your tabs for the day     │
-    ├─────────────────┼────────────────────────────────┤
-    │ block           │ Block a channel                │
-    ├─────────────────┼────────────────────────────────┤
-    │ playlists       │ List stored playlists          │
-    ├─────────────────┼────────────────────────────────┤
-    │ download        │ Download media                 │
-    ├─────────────────┼────────────────────────────────┤
-    │ download-status │ Show download status           │
-    ├─────────────────┼────────────────────────────────┤
-    │ redownload      │ Re-download deleted/lost media │
-    ├─────────────────┼────────────────────────────────┤
-    │ history         │ Show some playback statistics  │
-    ├─────────────────┼────────────────────────────────┤
-    │ search          │ Search captions / subtitles    │
-    ╰─────────────────┴────────────────────────────────╯
-
     Text subcommands:
     ╭────────────────┬─────────────────────────────────────────────╮
     │ cluster-sort   │ Sort text and images by similarity          │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-links  │ Extract inner links from lists of web links │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-text   │ Extract human text from lists of web links  │
     ├────────────────┼─────────────────────────────────────────────┤
     │ markdown-links │ Extract titles from lists of web links      │
     ╰────────────────┴─────────────────────────────────────────────╯
 
-    File subcommands:
-    ╭──────────────────┬───────────────────────────────────────────────────────╮
-    │ eda              │ Exploratory Data Analysis on table-like files         │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ mcda             │ Multi-criteria Ranking for Decision Support           │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ incremental-diff │ Diff large table-like files in chunks                 │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ media-check      │ Check video and audio files for corruption via ffmpeg │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ sample-hash      │ Calculate a hash based on small file segments         │
-    ├──────────────────┼───────────────────────────────────────────────────────┤
-    │ sample-compare   │ Compare files using sample-hash and other shortcuts   │
-    ╰──────────────────┴───────────────────────────────────────────────────────╯
-
     Folder subcommands:
     ╭───────────────┬──────────────────────────────────────────────────╮
     │ merge-folders │ Merge two or more file trees                     │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ relmv         │ Move files preserving parent folder hierarchy    │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ mv-list       │ Find specific folders to move to different disks │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ scatter       │ Scatter files between folders or disks           │
     ╰───────────────┴──────────────────────────────────────────────────╯
 
+    File subcommands:
+    ╭────────────────┬─────────────────────────────────────────────────────╮
+    │ sample-hash    │ Calculate a hash based on small file segments       │
+    ├────────────────┼─────────────────────────────────────────────────────┤
+    │ sample-compare │ Compare files using sample-hash and other shortcuts │
+    ╰────────────────┴─────────────────────────────────────────────────────╯
+
+    Tabular data subcommands:
+    ╭──────────────────┬───────────────────────────────────────────────╮
+    │ eda              │ Exploratory Data Analysis on table-like files │
+    ├──────────────────┼───────────────────────────────────────────────┤
+    │ mcda             │ Multi-criteria Ranking for Decision Support   │
+    ├──────────────────┼───────────────────────────────────────────────┤
+    │ incremental-diff │ Diff large table-like files in chunks         │
+    ╰──────────────────┴───────────────────────────────────────────────╯
+
+    Media File subcommands:
+    ╭────────────────┬────────────────────────────────────────────────────────╮
+    │ media-check    │ Check video and audio files for corruption via ffmpeg  │
+    ├────────────────┼────────────────────────────────────────────────────────┤
+    │ process-ffmpeg │ Shrink video/audio to AV1/Opus format (.mkv, .mka)     │
+    ├────────────────┼────────────────────────────────────────────────────────┤
+    │ process-image  │ Shrink images by resizing and AV1 image format (.avif) │
+    ╰────────────────┴────────────────────────────────────────────────────────╯
+
     Multi-database subcommands:
     ╭──────────────────┬────────────────────────╮
     │ merge-dbs        │ Merge SQLITE databases │
     ├──────────────────┼────────────────────────┤
     │ copy-play-counts │ Copy play history      │
     ╰──────────────────┴────────────────────────╯
 
@@ -323,41 +283,88 @@
     │ big-dirs    │ Show large folders             │
     ├─────────────┼────────────────────────────────┤
     │ search-db   │ Search a SQLITE database       │
     ├─────────────┼────────────────────────────────┤
     │ optimize    │ Re-optimize database           │
     ╰─────────────┴────────────────────────────────╯
 
-    Single database enrichment subcommands:
+    Media Database subcommands:
+    ╭─────────────────┬────────────────────────────────╮
+    │ tabs            │ Open your tabs for the day     │
+    ├─────────────────┼────────────────────────────────┤
+    │ block           │ Block a channel                │
+    ├─────────────────┼────────────────────────────────┤
+    │ playlists       │ List stored playlists          │
+    ├─────────────────┼────────────────────────────────┤
+    │ download        │ Download media                 │
+    ├─────────────────┼────────────────────────────────┤
+    │ download-status │ Show download status           │
+    ├─────────────────┼────────────────────────────────┤
+    │ redownload      │ Re-download deleted/lost media │
+    ├─────────────────┼────────────────────────────────┤
+    │ history         │ Show some playback statistics  │
+    ├─────────────────┼────────────────────────────────┤
+    │ search          │ Search captions / subtitles    │
+    ╰─────────────────┴────────────────────────────────╯
+
+    Playback subcommands:
+    ╭────────────┬───────────────────────────────────────────────────╮
+    │ watch      │ Watch / Listen                                    │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ now        │ Show what is currently playing                    │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ next       │ Play next file and optionally delete current file │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ stop       │ Stop all playback                                 │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ pause      │ Pause all playback                                │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ open-links │ Open links from link dbs                          │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ surf       │ Auto-load browser tabs in a streaming way (stdin) │
+    ╰────────────┴───────────────────────────────────────────────────╯
+
+    Database enrichment subcommands:
     ╭────────────────────┬────────────────────────────────────────╮
     │ dedupe-db          │ Dedupe SQLITE tables                   │
     ├────────────────────┼────────────────────────────────────────┤
     │ dedupe-media       │ Dedupe similar media                   │
     ├────────────────────┼────────────────────────────────────────┤
     │ merge-online-local │ Merge online and local data            │
     ├────────────────────┼────────────────────────────────────────┤
     │ mpv-watchlater     │ Import mpv watchlater files to history │
     ├────────────────────┼────────────────────────────────────────┤
     │ reddit-selftext    │ Copy selftext links to media table     │
     ├────────────────────┼────────────────────────────────────────┤
     │ tabs-shuffle       │ Randomize tabs.db a bit                │
     ╰────────────────────┴────────────────────────────────────────╯
 
+    Update database subcommands:
+    ╭───────────────┬─────────────────────────────────╮
+    │ fsupdate      │ Update local media              │
+    ├───────────────┼─────────────────────────────────┤
+    │ tubeupdate    │ Update online video media       │
+    ├───────────────┼─────────────────────────────────┤
+    │ webupdate     │ Update open-directory media     │
+    ├───────────────┼─────────────────────────────────┤
+    │ galleryupdate │ Update online gallery media     │
+    ├───────────────┼─────────────────────────────────┤
+    │ links-update  │ Update a link-scraping database │
+    ├───────────────┼─────────────────────────────────┤
+    │ redditupdate  │ Update reddit media             │
+    ╰───────────────┴─────────────────────────────────╯
+
     Misc subcommands:
-    ╭────────────────┬────────────────────────────────────────────────────────╮
-    │ export-text    │ Export HTML files from SQLite databases                │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ process-ffmpeg │ Shrink video/audio to AV1/Opus format (.mkv, .mka)     │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ process-image  │ Shrink images by resizing and AV1 image format (.avif) │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ dedupe-czkawka │ Process czkawka diff output                            │
-    ├────────────────┼────────────────────────────────────────────────────────┤
-    │ nouns          │ Unstructured text -> compound nouns (stdin)            │
-    ╰────────────────┴────────────────────────────────────────────────────────╯
+    ╭────────────────┬─────────────────────────────────────────────╮
+    │ export-text    │ Export HTML files from SQLite databases     │
+    ├────────────────┼─────────────────────────────────────────────┤
+    │ dedupe-czkawka │ Process czkawka diff output                 │
+    ├────────────────┼─────────────────────────────────────────────┤
+    │ nouns          │ Unstructured text -> compound nouns (stdin) │
+    ╰────────────────┴─────────────────────────────────────────────╯
 
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
@@ -1033,561 +1040,726 @@
         |   test_b |   test_a |
         |----------|----------|
         |        1 |        2 |
 
 
 </details>
 
-### Update database subcommands
+### Text subcommands
 
-###### fsupdate
+###### cluster-sort
 
-<details><summary>Update local media</summary>
+<details><summary>Sort text and images by similarity</summary>
 
-    $ library fsupdate -h
-    usage: library fsupdate DATABASE
+    $ library cluster-sort -h
+    usage: library cluster-sort [input_path | stdin] [output_path | stdout]
 
-    Update each path previously saved:
+    Group lines of text into sorted output
+
+        echo 'red apple
+        broccoli
+        yellow
+        green
+        orange apple
+        red apple' | library cluster-sort
+
+        orange apple
+        red apple
+        red apple
+        broccoli
+        green
+        yellow
+
+    Show the groupings
+
+        echo 'red apple
+        broccoli
+        yellow
+        green
+        orange apple
+        red apple' | library cluster-sort --print-groups
+
+        [
+            {'grouped_paths': ['orange apple', 'red apple', 'red apple']},
+            {'grouped_paths': ['broccoli', 'green', 'yellow']}
+        ]
+
+    Auto-sort images into directories
+
+        echo 'image1.jpg
+        image2.jpg
+        image3.jpg' | library cluster-sort --image --move-groups
+
+    Print similar paths
+
+        library fs 0day.db -pa --cluster --print-groups
 
-        library fsupdate video.db
 
 
 </details>
 
-###### tubeupdate
+###### extract-links
 
-<details><summary>Update online video media</summary>
+<details><summary>Extract inner links from lists of web links</summary>
 
-    $ library tubeupdate -h
-    usage: library tubeupdate [--audio | --video] DATABASE
+    $ library extract-links -h
+    usage: library extract-links PATH ... [--case-sensitive] [--scroll] [--download] [--verbose] [--local-html] [--file FILE] [--path-include ...] [--text-include ...] [--after-include ...] [--before-include ...] [--path-exclude ...] [--text-exclude ...] [--after-exclude ...] [--before-exclude ...]
 
-    Fetch the latest videos for every playlist saved in your database
+    Extract links from within local HTML fragments, files, or remote pages; filtering on link text and nearby plain-text
 
-        library tubeupdate educational.db
+        library links https://en.wikipedia.org/wiki/List_of_bacon_dishes --path-include https://en.wikipedia.org/wiki/ --after-include famous
+        https://en.wikipedia.org/wiki/Omelette
 
-    Fetch extra metadata:
+    Read from local clipboard and filter out links based on nearby plain text:
 
-        By default tubeupdate will quickly add media.
-        You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
+        library links --local-html (cb -t text/html | psub) --after-exclude paranormal spooky horror podcast tech fantasy supernatural lecture sport
+        # note: the equivalent BASH-ism is <(xclip -selection clipboard -t text/html)
 
-        library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
+    Run with `-vv` to see the browser
 
-    Remove duplicate playlists:
 
-        lb dedupe-db video.db playlists --bk extractor_playlist_id
+</details>
+
+###### extract-text
+
+<details><summary>Extract human text from lists of web links</summary>
+
+    $ library extract-text -h
+    usage: library extract-text PATH ... [--skip-links]
+
+    Sorting suggestions
+
+        lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 
 
 </details>
 
-###### webupdate
+### Folder subcommands
 
-<details><summary>Update open-directory media</summary>
+###### merge-folders
 
-    $ library webupdate -h
-    usage: library web-update DATABASE
+<details><summary>Merge two or more file trees</summary>
 
-    Update saved open directories
+    $ library merge-folders -h
+    usage: library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
 
+    Merge multiple folders with the same file tree into a single folder.
+
+    https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
+
+    Trumps are new or replaced files from an earlier source which now conflict with a later source.
+    If you only have one source then the count of trumps will always be zero.
+    The count of conflicts also includes trumps.
 
 
 </details>
 
-###### galleryupdate
+###### relmv
 
-<details><summary>Update online gallery media</summary>
+<details><summary>Move files preserving parent folder hierarchy</summary>
 
-    $ library galleryupdate -h
-    usage: library galleryupdate DATABASE URLS
+    $ library relmv -h
+    usage: library relmv [--simulate] SOURCE ... DEST
 
-    Check previously saved gallery_dl URLs for new content
+    Move files/folders without losing hierarchy metadata
+
+    Move fresh music to your phone every Sunday:
+
+        # move last week music back to their source folders
+        library mv /mnt/d/sync/weekly/ /mnt/d/check/audio/
+
+        # move new music for this week
+        library relmv (
+            library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+        ) /mnt/d/sync/weekly/
 
 
 </details>
 
-###### links-update
+###### mv-list
 
-<details><summary>Update a link-scraping database</summary>
+<details><summary>Find specific folders to move to different disks</summary>
 
-    $ library links-update -h
-    usage: library links-update DATABASE
+    $ library mv-list -h
+    usage: library mv-list [--limit LIMIT] [--lower LOWER] [--upper UPPER] MOUNT_POINT DATABASE
 
-    Fetch new links from each path previously saved
+    Free up space on a specific disk. Find candidates for moving data to a different mount point
 
-        library links-update links.db
+
+    The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
+
+        library fsadd --filesystem d.db ~/d/
+
+    But this should definitely also work with xklb audio and video databases:
+
+        library mv-list /mnt/d/ video.db
+
+    The program will print a table with a sorted list of folders which are good candidates for moving.
+    Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over).
+    The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
+
+        ...
+        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+        │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
+        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+        │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
+        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+        │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
+        ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
+        6702 other folders not shown
+
+        ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
+        ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
+        ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
+        ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
+        ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
+        ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
+
+        Type "done" when finished
+        Type "more" to see more files
+        Paste a folder (and press enter) to toggle selection
+        Type "*" to select all files in the most recently printed table
+
+    Then it will give you a prompt:
+
+        Paste a path:
+
+    Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
+
+        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+        26 selected paths: 162.1 GB ; future free space: 486.9 GB
+
+    You can also press the up arrow or paste it again to remove it from the list:
+
+        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+        25 selected paths: 159.9 GB ; future free space: 484.7 GB
+
+    After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
+
+        Paste a path: done
+
+            Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
+
+                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
 
 
 </details>
 
-###### redditupdate
+###### scatter
 
-<details><summary>Update reddit media</summary>
+<details><summary>Scatter files between folders or disks</summary>
 
-    $ library redditupdate -h
-    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+    $ library scatter -h
+    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
 
-    Fetch the latest posts for every subreddit/redditor saved in your database
+    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
 
-        library redditupdate edu_subreddits.db
+    Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
+
+        library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Reduce number of files per folder (creates more folders)
+
+        library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Multi-device re-bin: balance by size
+
+        library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs.db subfolder/of/mergerfs/mnt
+        Current path distribution:
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+
+        Simulated path distribution:
+        5845 files should be moved
+        20257 files should not be moved
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+        ### Move 1182 files to /mnt/d7 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
+        ### Move 1198 files to /mnt/d6 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
+        ### Move 1146 files to /mnt/d5 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
+        ### Move 1185 files to /mnt/d3 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
+        ### Move 1134 files to /mnt/d4 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+
+    Multi-device re-bin: balance device inodes for specific subfolder
+
+        library scatter -m /mnt/d1:/mnt/d2 fs.db subfolder --group count --sort 'size desc'
+
+    Multi-device re-bin: only consider the most recent 100 files
+
+        library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
+
+    Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
+
+        library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
 
 
 </details>
 
-### Playback subcommands
+### File subcommands
 
-###### watch
+###### sample-hash
 
-<details><summary>Watch / Listen</summary>
+<details><summary>Calculate a hash based on small file segments</summary>
 
-    $ library watch -h
-    usage: library watch DATABASE [optional args]
+    $ library sample-hash -h
+    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
-    Control playback:
-        To stop playback press Ctrl-C in either the terminal or mpv
+    Calculate hashes for large files by reading only small segments of each file
 
-        Create global shortcuts in your desktop environment by sending commands to mpv_socket:
-        echo 'playlist-next force' | socat - /tmp/mpv_socket
+        library sample-hash ./my_file.mkv
 
-    Override the default player (mpv):
-        library does a lot of things to try to automatically use your preferred media player
-        but if it doesn't guess right you can make it explicit:
-        library watch --player "vlc --vlc-opts"
+    The threads flag seems to be faster for rotational media but slower on SSDs
 
-    Cast to chromecast groups:
-        library watch --cast --cast-to "Office pair"
-        library watch -ct "Office pair"  # equivalent
-        If you don't know the exact name of your chromecast group run `catt scan`
 
-    Play media in order (similarly named episodes):
-        library watch --play-in-order
-        library watch -O    # equivalent
+</details>
 
-        The default sort value is 'natural_ps' which means media will be sorted by parent path
-        and then stem in a natural way (using the integer values within the path). But there are many other options:
+###### sample-compare
 
-        Options:
+<details><summary>Compare files using sample-hash and other shortcuts</summary>
 
-            - reverse: reverse the sort order
-            - compat: treat characters like '⑦' as '7'
+    $ library sample-compare -h
+    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
-        Algorithms:
+    Convenience subcommand to compare multiple files using sample-hash
 
-            - natural: parse numbers as integers
-            - os: sort similar to the OS File Explorer sorts. To improve non-alphanumeric sorting on Mac OS X and Linux it is necessary to install pyicu (perhaps via python3-icu -- https://gitlab.pyicu.org/main/pyicu#installing-pyicu)
-            - path: use natsort "path" algorithm (https://natsort.readthedocs.io/en/stable/api.html#the-ns-enum)
-            - human: use system locale
-            - ignorecase: treat all case as equal
-            - lowercase: sort lowercase first
-            - signed: sort with an understanding of negative numbers
-            - python: sort like default python
 
-        Values:
+</details>
 
-            - path
-            - parent
-            - stem
-            - title (or any other column value)
-            - ps: parent, stem
-            - pts: parent, title, stem
+### Tabular data subcommands
 
-        Use this format: algorithm, value, algorithm_value, or option_algorithm_value.
-        For example:
+###### eda
 
-            - library watch -O human
-            - library watch -O title
-            - library watch -O human_title
-            - library watch -O reverse_compat_human_title
+<details><summary>Exploratory Data Analysis on table-like files</summary>
 
-            - library watch -O path       # path algorithm and parent, stem values (path_ps)
-            - library watch -O path_path  # path algorithm and path values
+    $ library eda -h
+    usage: library eda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW] [--repl]
 
-        Also, if you are using --random you need to fetch sibling media to play the media in order:
+    Perform Exploratory Data Analysis (EDA) on one or more files
 
-            - library watch --random --fetch-siblings each -O          # get the first result per directory
-            - library watch --random --fetch-siblings if-audiobook -O  # get the first result per directory if 'audiobook' is in the path
-            - library watch --random --fetch-siblings always -O        # get 2,000 results per directory
+    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
 
-        If searching by a specific subpath it may be preferable to just sort by path instead
-        library watch d/planet.earth.2024/ -u path
 
-        library watch --related  # Similar to -O but uses fts to find similar content
-        library watch -R         # equivalent
-        library watch -RR        # above, plus ignores most filters
+</details>
 
-        library watch --cluster  # cluster-sort to put similar-named paths closer together
-        library watch -C         # equivalent
+###### mcda
 
-        library watch --big-dirs # Recommended to use with --duration or --depth filters; see `lb big-dirs -h` for more info
-        library watch -B         # equivalent
+<details><summary>Multi-criteria Ranking for Decision Support</summary>
 
-        All of these options can be used together but it will be a bit slow and the results might be mid-tier
-        as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
-        library watch -RRCO
+    $ library mcda -h
+    usage: library mcda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW]
 
-        You can even sort the items within each cluster by auto-MCDA ~LOL~
-        library watch -B --sort-groups-by 'mcda median_size,-deleted'
-        library watch -C --sort-groups-by 'mcda median_size,-deleted'
+    Perform Multiple Criteria Decision Analysis (MCDA) on one or more files
 
-    Filter media by file siblings of parent directory:
-        library watch --sibling   # only include files which have more than or equal to one sibling
-        library watch --solo      # only include files which are alone by themselves
+    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
 
-        `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
-        library watch --sibling --solo      # you will always get zero records here
-        library watch --lower 2 --upper 1   # equivalent
+    $ library mcda ~/storage.csv --minimize price --ignore warranty
 
-        You can be more specific via the `--upper` and `--lower` flags
-        library watch --lower 3   # only include files which have three or more siblings
-        library watch --upper 3   # only include files which have fewer than three siblings
-        library watch --lower 3 --upper 3   # only include files which are three siblings inclusive
-        library watch --lower 12 --upper 25 -O  # on my machine this launches My Mister 2018
+        ### Goals
+        #### Maximize
+        - size
+        #### Minimize
+        - price
 
-    Play recent partially-watched videos (requires mpv history):
-        library watch --partial       # play newest first
+        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
+        |----|---------|--------|------------|----------|------------|----------|---------|
+        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
+        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
+        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
 
-        library watch --partial old   # play oldest first
-        library watch -P o            # equivalent
+    $ library mcda ~/storage.csv --ignore warranty
 
-        library watch -P p            # sort by percent remaining
-        library watch -P t            # sort by time remaining
-        library watch -P s            # skip partially watched (only show unseen)
+        ### Goals
+        #### Maximize
+        - price
+        - size
 
-        The default time used is "last-viewed" (ie. the most recent time you closed the video)
-        If you want to use the "first-viewed" time (ie. the very first time you opened the video)
-        library watch -P f            # use watch_later file creation time instead of modified time
+        |    |   price |   size |   warranty |   TOPSIS |     MABAC |   SPOTIS |   BORDA |
+        |----|---------|--------|------------|----------|-----------|----------|---------|
+        |  2 |     519 |     44 |          2 | 1        |  0.536587 | 0        | 7.46341 |
+        |  1 |     453 |     40 |          2 | 0.580079 |  0.103888 | 0.432699 | 7.88333 |
+        |  0 |     359 |     36 |          5 | 0        | -0.463413 | 1        | 8.46341 |
 
-        You can combine most of these options, though some will be overridden by others.
-        library watch -P fo           # this means "show the oldest videos using the time I first opened them"
-        library watch -P pt           # weighted remaining (percent * time remaining)
+    $ library mcda ~/storage.csv --minimize price --ignore warranty
 
-    Print instead of play:
-        library watch --print --limit 10  # print the next 10 files
-        library watch -p -L 10  # print the next 10 files
-        library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
+        ### Goals
+        #### Maximize
+        - size
+        #### Minimize
+        - price
 
-        Printing modes
-        library watch -p    # print as a table
-        library watch -p a  # print an aggregate report
-        library watch -p b  # print a big-dirs report (see library bigdirs -h for more info)
-        library watch -p f  # print fields (defaults to path; use --cols to change)
-                               # -- useful for piping paths to utilities like xargs or GNU Parallel
+        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
+        |----|---------|--------|------------|----------|------------|----------|---------|
+        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
+        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
+        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
 
-        library watch -p d  # mark deleted
-        library watch -p w  # mark watched
+    It also works with HTTP/GCS/S3 URLs:
 
-        Some printing modes can be combined
-        library watch -p df  # print files for piping into another program and mark them as deleted within the db
-        library watch -p bf  # print fields from big-dirs report
+    $ library mcda https://en.wikipedia.org/wiki/List_of_Academy_Award-winning_films --clean --minimize Year
 
-        Check if you have downloaded something before
-        library watch -u duration -p -s 'title'
+        ### Goals
 
-        Print an aggregate report of deleted media
-        library watch -w time_deleted!=0 -p=a
-        ╒═══════════╤══════════════╤═════════╤═════════╕
-        │ path      │ duration     │ size    │   count │
-        ╞═══════════╪══════════════╪═════════╪═════════╡
-        │ Aggregate │ 14 days, 23  │ 50.6 GB │   29058 │
-        │           │ hours and 42 │         │         │
-        │           │ minutes      │         │         │
-        ╘═══════════╧══════════════╧═════════╧═════════╛
-        Total duration: 14 days, 23 hours and 42 minutes
+        #### Maximize
 
-        Print an aggregate report of media that has no duration information (ie. online or corrupt local media)
-        library watch -w 'duration is null' -p=a
+        - Nominations
+        - Awards
 
-        Print a list of filenames which have below 1280px resolution
-        library watch -w 'width<1280' -p=f
+        #### Minimize
 
-        Print media you have partially viewed with mpv
-        library watch --partial -p
-        library watch -P -p  # equivalent
-        library watch -P -p f --cols path,progress,duration  # print CSV of partially watched files
-        library watch --partial -pa  # print an aggregate report of partially watched files
+        - Year
 
-        View how much time you have watched
-        library watch -w play_count'>'0 -p=a
+        |      | Film                                                                    |   Year |   Awards |   Nominations |      TOPSIS |    MABAC |      SPOTIS |   BORDA |
+        |------|-------------------------------------------------------------------------|--------|----------|---------------|-------------|----------|-------------|---------|
+        |  378 | Titanic                                                                 |   1997 |       11 |            14 | 0.999993    | 1.38014  | 4.85378e-06 | 4116.62 |
+        |  868 | Ben-Hur                                                                 |   1959 |       11 |            12 | 0.902148    | 1.30871  | 0.0714303   | 4116.72 |
+        |  296 | The Lord of the Rings: The Return of the King                           |   2003 |       11 |            11 | 0.8558      | 1.27299  | 0.107147    | 4116.76 |
+        | 1341 | West Side Story                                                         |   1961 |       10 |            11 | 0.837716    | 1.22754  | 0.152599    | 4116.78 |
+        |  389 | The English Patient                                                     |   1996 |        9 |            12 | 0.836725    | 1.2178   | 0.162341    | 4116.78 |
+        | 1007 | Gone with the Wind                                                      |   1939 |        8 |            13 | 0.807086    | 1.20806  | 0.172078    | 4116.81 |
+        |  990 | From Here to Eternity                                                   |   1953 |        8 |            13 | 0.807086    | 1.20806  | 0.172079    | 4116.81 |
+        | 1167 | On the Waterfront                                                       |   1954 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        | 1145 | My Fair Lady                                                            |   1964 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        |  591 | Gandhi                                                                  |   1982 |        8 |            11 | 0.755312    | 1.13663  | 0.243509    | 4116.86 |
 
-        See how much video you have
-        library watch video.db -p=a
-        ╒═══════════╤═════════╤═════════╤═════════╕
-        │ path      │   hours │ size    │   count │
-        ╞═══════════╪═════════╪═════════╪═════════╡
-        │ Aggregate │  145769 │ 37.6 TB │  439939 │
-        ╘═══════════╧═════════╧═════════╧═════════╛
-        Total duration: 16 years, 7 months, 19 days, 17 hours and 25 minutes
 
-        View all the columns
-        library watch -p -L 1 --cols '*'
+</details>
 
-        Open ipython with all of your media
-        library watch -vv -p --cols '*'
-        ipdb> len(media)
-        462219
+###### incremental-diff
 
-    Set the play queue size:
-        By default the play queue is 120--long enough that you likely have not noticed
-        but short enough that the program is snappy.
+<details><summary>Diff large table-like files in chunks</summary>
 
-        If you want everything in your play queue you can use the aid of infinity.
-        Pick your poison (these all do effectively the same thing):
-        library watch -L inf
-        library watch -l inf
-        library watch --queue inf
-        library watch -L 999999999999
+    $ library incremental-diff -h
+    usage: library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
 
-        You may also want to restrict the play queue.
-        For example, when you only want 1000 random files:
-        library watch -u random -L 1000
+    See data differences in an incremental way to quickly see how two different files differ.
 
-    Offset the play queue:
-        You can also offset the queue. For example if you want to skip one or ten media:
-        library watch --offset 10      # offset ten from the top of an ordered query
+    Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
 
-    Repeat
-        library watch                  # listen to 120 random songs (DEFAULT_PLAY_QUEUE)
-        library watch --limit 5        # listen to FIVE songs
-        library watch -l inf -u random # listen to random songs indefinitely
-        library watch -s infinite      # listen to songs from the band infinite
+    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared.
+    If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
 
-    Constrain media by search:
-        Audio files have many tags to readily search through so metadata like artist,
-        album, and even mood are included in search.
-        Video files have less consistent metadata and so only paths are included in search.
-        library watch --include happy  # only matches will be included
-        library watch -s happy         # equivalent
-        library watch --exclude sad    # matches will be excluded
-        library watch -E sad           # equivalent
+    To diff everything at once run with `--batch-size inf`
 
-        Search only the path column
-        library watch -O -s 'path : mad max'
-        library watch -O -s 'path : "mad max"' # add "quotes" to be more strict
 
-        Double spaces are parsed as one space
-        library watch -s '  ost'        # will match OST and not ghost
-        library watch -s toy story      # will match '/folder/toy/something/story.mp3'
-        library watch -s 'toy  story'   # will match more strictly '/folder/toy story.mp3'
+</details>
 
-        You can search without -s but it must directly follow the database due to how argparse works
-        library watch ./your.db searching for something
+### Media File subcommands
 
-    Constrain media by arbitrary SQL expressions:
-        library watch --where audio_count = 2  # media which have two audio tracks
-        library watch -w "language = 'eng'"    # media which have an English language tag
-                                                    (this could be audio _or_ subtitle)
-        library watch -w subtitle_count=0      # media that doesn't have subtitles
+###### media-check
 
-    Constrain media to duration (in minutes):
-        library watch --duration 20
-        library watch -d 6  # 6 mins ±10 percent (ie. between 5 and 7 mins)
-        library watch -d-6  # less than 6 mins
-        library watch -d+6  # more than 6 mins
+<details><summary>Check video and audio files for corruption via ffmpeg</summary>
 
-        Duration can be specified multiple times:
-        library watch -d+5 -d-7  # should be similar to -d 6
+    $ library media-check -h
+    usage: library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
 
-        If you want exact time use `where`
-        library watch --where 'duration=6*60'
+    Defaults to decode 0.5 second per 10% of each file
 
-    Constrain media to file size (in megabytes):
-        library watch --size 20
-        library watch -S 6  # 6 MB ±10 percent (ie. between 5 and 7 MB)
-        library watch -S-6  # less than 6 MB
-        library watch -S+6  # more than 6 MB
+        library media-check ./video.mp4
 
-    Constrain media by time_created / time_last_played / time_deleted / time_modified:
-        library watch --created-within '3 days'
-        library watch --created-before '3 years'
+    Decode all the frames of each file to evaluate how corrupt it is
+    (scantime is very slow; about 150 seconds for an hour-long file)
 
-    Constrain media by throughput:
-        Bitrate information is not explicitly saved.
-        You can use file size and duration as a proxy for throughput:
-        library watch -w 'size/duration<50000'
+        library media-check --full-scan ./video.mp4
 
-    Constrain media to portrait orientation video:
-        library watch --portrait
-        library watch -w 'width<height' # equivalent
+    Decode all the packets of each file to evaluate how corrupt it is
+    (scantime is about one second of each file but only accurate for formats where 1 packet == 1 frame)
 
-    Constrain media to duration of videos which match any size constraints:
-        library watch --duration-from-size +700 -u 'duration desc, size desc'
+        library media-check --full-scan --gap 0 ./video.mp4
 
-    Constrain media to online-media or local-media:
-        Not to be confused with only local-media which is not "offline" (ie. one HDD disconnected)
-        library watch --online-media-only
-        library watch --online-media-only -i  # and ignore playback errors (ie. YouTube video deleted)
-        library watch --local-media-only
+    Decode all audio of each file to evaluate how corrupt it is
+    (scantime is about four seconds per file)
 
-    Specify media play order:
-        library watch --sort duration   # play shortest media first
-        library watch -u duration desc  # play longest media first
+        library media-check --full-scan --audio ./video.mp4
 
-        You can use multiple SQL ORDER BY expressions
-        library watch -u 'subtitle_count > 0 desc' # play media that has at least one subtitle first
+    Decode at least one frame at the start and end of each file to evaluate how corrupt it is
+    (scantime is about one second per file)
 
-        Prioritize large-sized media
-        library watch --sort 'ntile(10000) over (order by size/duration) desc'
-        library watch -u 'ntile(100) over (order by size) desc'
+        library media-check --chunk-size 5% --gap 99.9% ./video.mp4
 
-        Sort by count of media with the same-X column (default DESC: most common to least common value)
-        library watch -u same-duration
-        library watch -u same-title
-        library watch -u same-size
-        library watch -u same-width, same-height ASC, same-fps
-        library watch -u same-time_uploaded same-view_count same-upvote_ratio
+    Decode 3s every 5% of a file to evaluate how corrupt it is
+    (scantime is about three seconds per file)
 
-        No media found when using --random
-        In addition to -u/--sort random, there is also the -r/--random flag.
-        If you have a large database it should be faster than -u random but it comes with a caveat:
-        This flag randomizes via rowid at an earlier stage to boost performance.
-        It is possible that you see "No media found" or a smaller amount of media than correct.
-        You can bypass this by setting --limit. For example:
-        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa
-        path         count      size  duration                        avg_duration      avg_size
-        ---------  -------  --------  ------------------------------  --------------  ----------
-        Aggregate    10000  752.5 GB  4 months, 15 days and 10 hours  20 minutes         75.3 MB
-        (17 seconds)
-        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa -l inf
-        path         count     size  duration                                 avg_duration      avg_size
-        ---------  -------  -------  ---------------------------------------  --------------  ----------
-        Aggregate   140868  10.6 TB  5 years, 2 months, 28 days and 14 hours  20 minutes         75.3 MB
-        (30 seconds)
+        library media-check --chunk-size 3 --gap 5% ./video.mp4
 
-    Post-actions -- choose what to do after playing:
-        library watch --post-action keep    # do nothing after playing (default)
-        library watch -k delete             # delete file after playing
-        library watch -k softdelete         # mark deleted after playing
+    Delete the file if 20 percent or more of checks fail
 
-        library watch -k ask_keep           # ask whether to keep after playing
-        library watch -k ask_delete         # ask whether to delete after playing
+        library media-check --delete-corrupt 20% ./video.mp4
 
-        library watch -k move               # move to "keep" dir after playing
-        library watch -k ask_move           # ask whether to move to "keep" folder
-        The default location of the keep folder is ./keep/ (relative to the played media file)
-        You can change this by explicitly setting an *absolute* `keep-dir` path:
-        library watch -k ask_move --keep-dir /home/my/music/keep/
+    To scan a large folder use `fsadd`. I recommend something like this two-stage approach:
 
-        library watch -k ask_move_or_delete # ask after each whether to move to "keep" folder or delete
+        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/
+        library media-check (library fs tmp.db -w 'corruption>15' -pf) --full-scan --delete-corrupt 25%
 
-        You can also bind keys in mpv to different exit codes. For example in input.conf:
-            ; quit 5
+    The above can now be done in one command via `--full-scan-if-corrupt`:
 
-        And if you run something like:
-            library watch --cmd5 ~/bin/process_audio.py
-            library watch --cmd5 echo  # this will effectively do nothing except skip the normal post-actions via mpv shortcut
+        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/ --full-scan-if-corrupt 15% --delete-corrupt 25%
 
-        When semicolon is pressed in mpv (it will exit with error code 5) then the applicable player-exit-code command
-        will start with the media file as the first argument; in this case `~/bin/process_audio.py $path`.
-        The command will be daemonized if library exits before it completes.
+    Corruption stats
 
-        To prevent confusion, normal post-actions will be skipped if the exit-code is greater than 4.
-        Exit-codes 0, 1, 2, 3, and 4: the external post-action will run after normal post-actions. Be careful of conflicting player-exit-code command and post-action behavior when using these!
+        library fs tmp.db -w 'corruption>15' -pa
+        path         count  duration             avg_duration         size    avg_size
+        ---------  -------  -------------------  --------------  ---------  ----------
+        Aggregate      907  15 days and 9 hours  24 minutes      130.6 GiB   147.4 MiB
 
-    Experimental options:
-        Duration to play (in seconds) while changing the channel
-        library watch --interdimensional-cable 40
-        library watch -4dtv 40
-        You can open two terminals to replicate AMV Hell somewhat
-        library watch --volume 0 -4dtv 30
-        library listen -4dtv 30
+    Corruption graph
 
-        Playback multiple files at once
-        library watch --multiple-playback    # one per display; or two if only one display detected
-        library watch --multiple-playback 4  # play four media at once, divide by available screens
-        library watch -m 4 --screen-name eDP # play four media at once on specific screen
-        library watch -m 4 --loop --crop     # play four cropped videos on a loop
-        library watch -m 4 --hstack          # use hstack style
+        sqlite --raw-lines tmp.db 'select corruption from media' | lowcharts hist --min 10 --intervals 10
 
-        When using `--multiple-playback` it may be helpful to set simple window focus rules to prevent keys from accidentally being entered in the wrong mpv window (as new windows are created and capture the cursor focus).
-        You can set and restore your previous mouse focus setting by wrapping the command like this:
+        Samples = 931; Min = 10.0; Max = 100.0
+        Average = 39.1; Variance = 1053.103; STD = 32.452
+        each ∎ represents a count of 6
+        [ 10.0 ..  19.0] [561] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
+        [ 19.0 ..  28.0] [ 69] ∎∎∎∎∎∎∎∎∎∎∎
+        [ 28.0 ..  37.0] [ 33] ∎∎∎∎∎
+        [ 37.0 ..  46.0] [ 18] ∎∎∎
+        [ 46.0 ..  55.0] [ 14] ∎∎
+        [ 55.0 ..  64.0] [ 12] ∎∎
+        [ 64.0 ..  73.0] [ 15] ∎∎
+        [ 73.0 ..  82.0] [ 18] ∎∎∎
+        [ 82.0 ..  91.0] [ 50] ∎∎∎∎∎∎∎∎
+        [ 91.0 .. 100.0] [141] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
 
-            focus-under-mouse
-            library watch ... --multiple-playback 4
-            focus-follows-mouse
 
-        For example in KDE:
+</details>
 
-            function focus-under-mouse
-                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusUnderMouse
-                qdbus-qt5 org.kde.KWin /KWin reconfigure
-            end
+###### process-ffmpeg
 
-            function focus-follows-mouse
-                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusFollowsMouse
-                kwriteconfig5 --file kwinrc --group Windows --key NextFocusPrefersMouse true
-                qdbus-qt5 org.kde.KWin /KWin reconfigure
-            end
+<details><summary>Shrink video/audio to AV1/Opus format (.mkv, .mka)</summary>
 
+    $ library process-ffmpeg -h
+    usage: library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
+
+    Resize videos to max 1440x960px AV1 and/or Opus to save space
+
+    Convert audio to Opus. Optionally split up long tracks into multiple files.
+
+        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process --audio
+
+    Use --always-split to _always_ split files if silence is detected
+
+        library process-audio --always-split audiobook.m4a
+
+    Use --split-longer-than to _only_ detect silence for files in excess of a specific duration
+
+        library process-audio --split-longer-than 36mins audiobook.m4b audiobook2.mp3
 
 
 </details>
 
-###### open-links
+###### process-image
 
-<details><summary>Open links from link dbs</summary>
+<details><summary>Shrink images by resizing and AV1 image format (.avif)</summary>
 
-    $ library open-links -h
-    usage: library open-links DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
+    $ library process-image -h
+    usage: library process-image PATH ...
 
-    Open links from a links db
+    Resize images to max 2400x2400px and format AVIF to save space
 
-        wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
-        library open-links music.korea.ln.db
 
-    Only open links once
+</details>
 
-        library open-links ln.db -w 'time_modified=0'
+### Multi-database subcommands
 
-    Print a preview instead of opening tabs
+###### merge-dbs
 
-        library open-links ln.db -p
-        library open-links ln.db --cols time_modified -p
+<details><summary>Merge SQLITE databases</summary>
 
-    Delete rows
+    $ library merge-dbs -h
+    usage: library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
 
-        Make sure you have the right search query
-        library open-links ln.db "query" -p -L inf
-        library open-links ln.db "query" -pa  # view total
+    Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
+    and there is an existing row with the same PK, the default action is to delete the existing row and insert the new row
+    replacing all existing fields.
 
-        library open-links ln.db "query" -pd  # mark as deleted
+    Upsert mode will update each matching PK row such that if a source row has a NULL field and
+    the destination row has a value then the value will be preserved instead of changed to the source row's NULL value.
 
-    Custom search engine
+    Ignore mode (--only-new-rows) will insert only rows which don't already exist in the destination db
 
-        library open-links ln.db --title --prefix 'https://duckduckgo.com/?q='
+    Test first by using temp databases as the destination db.
+    Try out different modes / flags until you are satisfied with the behavior of the program
 
-    Skip local media
+        library merge-dbs --pk path (mktemp --suffix .db) tv.db movies.db
 
-        library open-links dl.db --online
-        library open-links dl.db -w 'path like "http%"'  # equivalent
+    Merge database data and tables
+
+        library merge-dbs --upsert --pk path video.db tv.db movies.db
+        library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path --skip-column id audio-fts.db audio.db
+
+        library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
+        library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
+
+     To skip copying primary-keys from the source table(s) use --business-keys instead of --primary-keys
+
+     Split DBs using --where
 
+         library merge-dbs --pk path specific-site.db big.db -v --only-new-rows -t media,playlists -w 'path like "https://specific-site%"'
 
 
 </details>
 
-###### surf
+###### copy-play-counts
 
-<details><summary>Auto-load browser tabs in a streaming way (stdin)</summary>
+<details><summary>Copy play history</summary>
 
-    $ library surf -h
-    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
+    $ library copy-play-counts -h
+    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
-    Streaming tab loader: press ctrl+c to stop.
+    Copy play count information between databases
 
-    Open tabs from a line-delimited file:
+        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 
-        cat tabs.txt | library surf -n 5
 
-    You will likely want to use this setting in `about:config`
+</details>
 
-        browser.tabs.loadDivertedInBackground = True
+### Filesystem Database subcommands
 
-    If you prefer GUI, check out https://unli.xyz/tabsender/
+###### christen
+
+<details><summary>Clean filenames</summary>
+
+    $ library christen -h
+    usage: library christen DATABASE [--run]
+
+    Rename files to be somewhat normalized
+
+    Default mode is simulate
+
+        library christen fs.db
+
+    To actually do stuff use the run flag
+
+        library christen audio.db --run
+
+    You can optionally replace all the spaces in your filenames with dots
+
+        library christen --dot-space video.db
+
+
+</details>
+
+###### disk-usage
+
+<details><summary>Show disk usage</summary>
+
+    $ library disk-usage -h
+    usage: library disk-usage DATABASE [--sort-groups-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
+
+    Only include files smaller than 1kib
+
+        library disk-usage du.db --size=-1Ki
+        lb du du.db -S-1Ki
+        | path                                  |      size |   count |
+        |---------------------------------------|-----------|---------|
+        | /home/xk/github/xk/lb/__pycache__/    | 620 Bytes |       1 |
+        | /home/xk/github/xk/lb/.github/        |    1.7 kB |       4 |
+        | /home/xk/github/xk/lb/__pypackages__/ |    1.4 MB |    3519 |
+        | /home/xk/github/xk/lb/xklb/           |    4.4 kB |      12 |
+        | /home/xk/github/xk/lb/tests/          |    3.2 kB |       9 |
+        | /home/xk/github/xk/lb/.git/           |  782.4 kB |    2276 |
+        | /home/xk/github/xk/lb/.pytest_cache/  |    1.5 kB |       5 |
+        | /home/xk/github/xk/lb/.ruff_cache/    |   19.5 kB |     100 |
+        | /home/xk/github/xk/lb/.gitattributes  | 119 Bytes |         |
+        | /home/xk/github/xk/lb/.mypy_cache/    | 280 Bytes |       4 |
+        | /home/xk/github/xk/lb/.pdm-python     |  15 Bytes |         |
+
+    Only include files with a specific depth
+
+        library disk-usage du.db --depth 19
+        lb du du.db -d 19
+        | path                                                                                                                                                                |     size |
+        |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
+
+
+
+</details>
+
+###### big-dirs
+
+<details><summary>Show large folders</summary>
+
+    $ library big-dirs -h
+    usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
+
+    See what folders take up space
+
+        library big-dirs video.db
+        library big-dirs audio.db
+        library big-dirs fs.db
+
+    lb big-dirs video.db --folder-size=+10G --lower 400 --upper 14000
+
+    lb big-dirs video.db --depth 5
+    lb big-dirs video.db --depth 7
+
+    You can even sort by auto-MCDA ~LOL~
+
+    lb big-dirs video.db -u 'mcda median_size,-deleted'
+
+
+</details>
+
+###### search-db
+
+<details><summary>Search a SQLITE database</summary>
+
+    $ library search-db -h
+    usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
+
+    Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
+
+
+</details>
+
+###### optimize
+
+<details><summary>Re-optimize database</summary>
+
+    $ library optimize -h
+    usage: library optimize DATABASE [--force]
+
+    Optimize library databases
+
+    The force flag is usually unnecessary and it can take much longer
 
 
 </details>
 
-### Media database subcommands
+### Media Database subcommands
 
 ###### tabs
 
 <details><summary>Open your tabs for the day</summary>
 
     $ library tabs -h
     usage: library tabs DATABASE
@@ -2056,686 +2228,467 @@
     Search and open file
 
         library search fts.db 'two words' --open
 
 
 </details>
 
-### Text subcommands
-
-###### cluster-sort
-
-<details><summary>Sort text and images by similarity</summary>
-
-    $ library cluster-sort -h
-    usage: library cluster-sort [input_path | stdin] [output_path | stdout]
-
-    Group lines of text into sorted output
-
-        echo 'red apple
-        broccoli
-        yellow
-        green
-        orange apple
-        red apple' | library cluster-sort
-
-        orange apple
-        red apple
-        red apple
-        broccoli
-        green
-        yellow
-
-    Show the groupings
-
-        echo 'red apple
-        broccoli
-        yellow
-        green
-        orange apple
-        red apple' | library cluster-sort --print-groups
-
-        [
-            {'grouped_paths': ['orange apple', 'red apple', 'red apple']},
-            {'grouped_paths': ['broccoli', 'green', 'yellow']}
-        ]
-
-    Auto-sort images into directories
-
-        echo 'image1.jpg
-        image2.jpg
-        image3.jpg' | library cluster-sort --image --move-groups
-
-    Print similar paths
-
-        library fs 0day.db -pa --cluster --print-groups
-
-
-
-</details>
-
-###### extract-links
-
-<details><summary>Extract inner links from lists of web links</summary>
-
-    $ library extract-links -h
-    usage: library extract-links PATH ... [--case-sensitive] [--scroll] [--download] [--verbose] [--local-html] [--file FILE] [--path-include ...] [--text-include ...] [--after-include ...] [--before-include ...] [--path-exclude ...] [--text-exclude ...] [--after-exclude ...] [--before-exclude ...]
-
-    Extract links from within local HTML fragments, files, or remote pages; filtering on link text and nearby plain-text
-
-        library links https://en.wikipedia.org/wiki/List_of_bacon_dishes --path-include https://en.wikipedia.org/wiki/ --after-include famous
-        https://en.wikipedia.org/wiki/Omelette
-
-    Read from local clipboard and filter out links based on nearby plain text:
-
-        library links --local-html (cb -t text/html | psub) --after-exclude paranormal spooky horror podcast tech fantasy supernatural lecture sport
-        # note: the equivalent BASH-ism is <(xclip -selection clipboard -t text/html)
-
-    Run with `-vv` to see the browser
-
-
-</details>
-
-###### extract-text
-
-<details><summary>Extract human text from lists of web links</summary>
-
-    $ library extract-text -h
-    usage: library extract-text PATH ... [--skip-links]
-
-    Sorting suggestions
-
-        lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
-
-
-</details>
-
-### File subcommands
-
-###### eda
-
-<details><summary>Exploratory Data Analysis on table-like files</summary>
-
-    $ library eda -h
-    usage: library eda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW] [--repl]
-
-    Perform Exploratory Data Analysis (EDA) on one or more files
-
-    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
-
-
-</details>
-
-###### mcda
-
-<details><summary>Multi-criteria Ranking for Decision Support</summary>
-
-    $ library mcda -h
-    usage: library mcda PATH ... [--table TABLE] [--start-row START_ROW] [--end-row END_ROW]
-
-    Perform Multiple Criteria Decision Analysis (MCDA) on one or more files
-
-    Only 20,000 rows per file are loaded for performance purposes. Set `--end-row inf` to read all the rows and/or run out of RAM.
-
-    $ library mcda ~/storage.csv --minimize price --ignore warranty
-
-        ### Goals
-        #### Maximize
-        - size
-        #### Minimize
-        - price
-
-        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
-        |----|---------|--------|------------|----------|------------|----------|---------|
-        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
-        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
-        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
-
-    $ library mcda ~/storage.csv --ignore warranty
-
-        ### Goals
-        #### Maximize
-        - price
-        - size
-
-        |    |   price |   size |   warranty |   TOPSIS |     MABAC |   SPOTIS |   BORDA |
-        |----|---------|--------|------------|----------|-----------|----------|---------|
-        |  2 |     519 |     44 |          2 | 1        |  0.536587 | 0        | 7.46341 |
-        |  1 |     453 |     40 |          2 | 0.580079 |  0.103888 | 0.432699 | 7.88333 |
-        |  0 |     359 |     36 |          5 | 0        | -0.463413 | 1        | 8.46341 |
-
-    $ library mcda ~/storage.csv --minimize price --ignore warranty
-
-        ### Goals
-        #### Maximize
-        - size
-        #### Minimize
-        - price
-
-        |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
-        |----|---------|--------|------------|----------|------------|----------|---------|
-        |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
-        |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
-        |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
-
-    It also works with HTTP/GCS/S3 URLs:
-
-    $ library mcda https://en.wikipedia.org/wiki/List_of_Academy_Award-winning_films --clean --minimize Year
-
-        ### Goals
-
-        #### Maximize
-
-        - Nominations
-        - Awards
-
-        #### Minimize
-
-        - Year
-
-        |      | Film                                                                    |   Year |   Awards |   Nominations |      TOPSIS |    MABAC |      SPOTIS |   BORDA |
-        |------|-------------------------------------------------------------------------|--------|----------|---------------|-------------|----------|-------------|---------|
-        |  378 | Titanic                                                                 |   1997 |       11 |            14 | 0.999993    | 1.38014  | 4.85378e-06 | 4116.62 |
-        |  868 | Ben-Hur                                                                 |   1959 |       11 |            12 | 0.902148    | 1.30871  | 0.0714303   | 4116.72 |
-        |  296 | The Lord of the Rings: The Return of the King                           |   2003 |       11 |            11 | 0.8558      | 1.27299  | 0.107147    | 4116.76 |
-        | 1341 | West Side Story                                                         |   1961 |       10 |            11 | 0.837716    | 1.22754  | 0.152599    | 4116.78 |
-        |  389 | The English Patient                                                     |   1996 |        9 |            12 | 0.836725    | 1.2178   | 0.162341    | 4116.78 |
-        | 1007 | Gone with the Wind                                                      |   1939 |        8 |            13 | 0.807086    | 1.20806  | 0.172078    | 4116.81 |
-        |  990 | From Here to Eternity                                                   |   1953 |        8 |            13 | 0.807086    | 1.20806  | 0.172079    | 4116.81 |
-        | 1167 | On the Waterfront                                                       |   1954 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
-        | 1145 | My Fair Lady                                                            |   1964 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
-        |  591 | Gandhi                                                                  |   1982 |        8 |            11 | 0.755312    | 1.13663  | 0.243509    | 4116.86 |
-
-
-</details>
-
-###### incremental-diff
-
-<details><summary>Diff large table-like files in chunks</summary>
-
-    $ library incremental-diff -h
-    usage: library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
-
-    See data differences in an incremental way to quickly see how two different files differ.
-
-    Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
-
-    If files are unsorted you may need to use `--join-keys id,name` to specify ID columns. Rows that have the same ID will then be compared.
-    If you are comparing SQLITE files you may be able to use `--sort id,name` to achieve the same effect.
-
-    To diff everything at once run with `--batch-size inf`
-
-
-</details>
-
-###### media-check
-
-<details><summary>Check video and audio files for corruption via ffmpeg</summary>
-
-    $ library media-check -h
-    usage: library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
-
-    Defaults to decode 0.5 second per 10% of each file
-
-        library media-check ./video.mp4
-
-    Decode all the frames of each file to evaluate how corrupt it is
-    (scantime is very slow; about 150 seconds for an hour-long file)
-
-        library media-check --full-scan ./video.mp4
-
-    Decode all the packets of each file to evaluate how corrupt it is
-    (scantime is about one second of each file but only accurate for formats where 1 packet == 1 frame)
-
-        library media-check --full-scan --gap 0 ./video.mp4
-
-    Decode all audio of each file to evaluate how corrupt it is
-    (scantime is about four seconds per file)
-
-        library media-check --full-scan --audio ./video.mp4
-
-    Decode at least one frame at the start and end of each file to evaluate how corrupt it is
-    (scantime is about one second per file)
-
-        library media-check --chunk-size 5% --gap 99.9% ./video.mp4
-
-    Decode 3s every 5% of a file to evaluate how corrupt it is
-    (scantime is about three seconds per file)
-
-        library media-check --chunk-size 3 --gap 5% ./video.mp4
-
-    Delete the file if 20 percent or more of checks fail
-
-        library media-check --delete-corrupt 20% ./video.mp4
-
-    To scan a large folder use `fsadd`. I recommend something like this two-stage approach:
-
-        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/
-        library media-check (library fs tmp.db -w 'corruption>15' -pf) --full-scan --delete-corrupt 25%
-
-    The above can now be done in one command via `--full-scan-if-corrupt`:
-
-        library fsadd --delete-unplayable --check-corrupt --chunk-size 5% tmp.db ./video/ ./folders/ --full-scan-if-corrupt 15% --delete-corrupt 25%
-
-    Corruption stats
-
-        library fs tmp.db -w 'corruption>15' -pa
-        path         count  duration             avg_duration         size    avg_size
-        ---------  -------  -------------------  --------------  ---------  ----------
-        Aggregate      907  15 days and 9 hours  24 minutes      130.6 GiB   147.4 MiB
-
-    Corruption graph
-
-        sqlite --raw-lines tmp.db 'select corruption from media' | lowcharts hist --min 10 --intervals 10
-
-        Samples = 931; Min = 10.0; Max = 100.0
-        Average = 39.1; Variance = 1053.103; STD = 32.452
-        each ∎ represents a count of 6
-        [ 10.0 ..  19.0] [561] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-        [ 19.0 ..  28.0] [ 69] ∎∎∎∎∎∎∎∎∎∎∎
-        [ 28.0 ..  37.0] [ 33] ∎∎∎∎∎
-        [ 37.0 ..  46.0] [ 18] ∎∎∎
-        [ 46.0 ..  55.0] [ 14] ∎∎
-        [ 55.0 ..  64.0] [ 12] ∎∎
-        [ 64.0 ..  73.0] [ 15] ∎∎
-        [ 73.0 ..  82.0] [ 18] ∎∎∎
-        [ 82.0 ..  91.0] [ 50] ∎∎∎∎∎∎∎∎
-        [ 91.0 .. 100.0] [141] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-
-
-</details>
-
-###### sample-hash
-
-<details><summary>Calculate a hash based on small file segments</summary>
-
-    $ library sample-hash -h
-    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
-
-    Calculate hashes for large files by reading only small segments of each file
-
-        library sample-hash ./my_file.mkv
-
-    The threads flag seems to be faster for rotational media but slower on SSDs
-
-
-</details>
-
-###### sample-compare
-
-<details><summary>Compare files using sample-hash and other shortcuts</summary>
-
-    $ library sample-compare -h
-    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
-
-    Convenience subcommand to compare multiple files using sample-hash
-
-
-</details>
-
-### Folder subcommands
-
-###### merge-folders
-
-<details><summary>Merge two or more file trees</summary>
-
-    $ library merge-folders -h
-    usage: library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
-
-    Merge multiple folders with the same file tree into a single folder.
-
-    https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
-
-    Trumps are new or replaced files from an earlier source which now conflict with a later source.
-    If you only have one source then the count of trumps will always be zero.
-    The count of conflicts also includes trumps.
-
-
-</details>
-
-###### relmv
+### Playback subcommands
 
-<details><summary>Move files preserving parent folder hierarchy</summary>
+###### watch
 
-    $ library relmv -h
-    usage: library relmv [--simulate] SOURCE ... DEST
+<details><summary>Watch / Listen</summary>
 
-    Move files/folders without losing hierarchy metadata
+    $ library watch -h
+    usage: library watch DATABASE [optional args]
 
-    Move fresh music to your phone every Sunday:
+    Control playback:
+        To stop playback press Ctrl-C in either the terminal or mpv
 
-        # move last week music back to their source folders
-        library mv /mnt/d/sync/weekly/ /mnt/d/check/audio/
+        Create global shortcuts in your desktop environment by sending commands to mpv_socket:
+        echo 'playlist-next force' | socat - /tmp/mpv_socket
 
-        # move new music for this week
-        library relmv (
-            library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
-        ) /mnt/d/sync/weekly/
+    Override the default player (mpv):
+        library does a lot of things to try to automatically use your preferred media player
+        but if it doesn't guess right you can make it explicit:
+        library watch --player "vlc --vlc-opts"
 
+    Cast to chromecast groups:
+        library watch --cast --cast-to "Office pair"
+        library watch -ct "Office pair"  # equivalent
+        If you don't know the exact name of your chromecast group run `catt scan`
 
-</details>
+    Play media in order (similarly named episodes):
+        library watch --play-in-order
+        library watch -O    # equivalent
 
-###### mv-list
+        The default sort value is 'natural_ps' which means media will be sorted by parent path
+        and then stem in a natural way (using the integer values within the path). But there are many other options:
 
-<details><summary>Find specific folders to move to different disks</summary>
+        Options:
 
-    $ library mv-list -h
-    usage: library mv-list [--limit LIMIT] [--lower LOWER] [--upper UPPER] MOUNT_POINT DATABASE
+            - reverse: reverse the sort order
+            - compat: treat characters like '⑦' as '7'
 
-    Free up space on a specific disk. Find candidates for moving data to a different mount point
+        Algorithms:
 
+            - natural: parse numbers as integers
+            - os: sort similar to the OS File Explorer sorts. To improve non-alphanumeric sorting on Mac OS X and Linux it is necessary to install pyicu (perhaps via python3-icu -- https://gitlab.pyicu.org/main/pyicu#installing-pyicu)
+            - path: use natsort "path" algorithm (https://natsort.readthedocs.io/en/stable/api.html#the-ns-enum)
+            - human: use system locale
+            - ignorecase: treat all case as equal
+            - lowercase: sort lowercase first
+            - signed: sort with an understanding of negative numbers
+            - python: sort like default python
 
-    The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
+        Values:
 
-        library fsadd --filesystem d.db ~/d/
+            - path
+            - parent
+            - stem
+            - title (or any other column value)
+            - ps: parent, stem
+            - pts: parent, title, stem
 
-    But this should definitely also work with xklb audio and video databases:
+        Use this format: algorithm, value, algorithm_value, or option_algorithm_value.
+        For example:
 
-        library mv-list /mnt/d/ video.db
+            - library watch -O human
+            - library watch -O title
+            - library watch -O human_title
+            - library watch -O reverse_compat_human_title
 
-    The program will print a table with a sorted list of folders which are good candidates for moving.
-    Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over).
-    The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
+            - library watch -O path       # path algorithm and parent, stem values (path_ps)
+            - library watch -O path_path  # path algorithm and path values
 
-        ...
-        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-        │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
-        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-        │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
-        ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-        │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
-        ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
-        6702 other folders not shown
+        Also, if you are using --random you need to fetch sibling media to play the media in order:
 
-        ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
-        ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
-        ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
-        ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
-        ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
-        ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
+            - library watch --random --fetch-siblings each -O          # get the first result per directory
+            - library watch --random --fetch-siblings if-audiobook -O  # get the first result per directory if 'audiobook' is in the path
+            - library watch --random --fetch-siblings always -O        # get 2,000 results per directory
 
-        Type "done" when finished
-        Type "more" to see more files
-        Paste a folder (and press enter) to toggle selection
-        Type "*" to select all files in the most recently printed table
+        If searching by a specific subpath it may be preferable to just sort by path instead
+        library watch d/planet.earth.2024/ -u path
 
-    Then it will give you a prompt:
+        library watch --related  # Similar to -O but uses fts to find similar content
+        library watch -R         # equivalent
+        library watch -RR        # above, plus ignores most filters
 
-        Paste a path:
+        library watch --cluster  # cluster-sort to put similar-named paths closer together
+        library watch -C         # equivalent
 
-    Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
+        library watch --big-dirs # Recommended to use with --duration or --depth filters; see `lb big-dirs -h` for more info
+        library watch -B         # equivalent
 
-        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-        26 selected paths: 162.1 GB ; future free space: 486.9 GB
+        All of these options can be used together but it will be a bit slow and the results might be mid-tier
+        as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
+        library watch -RRCO
 
-    You can also press the up arrow or paste it again to remove it from the list:
+        You can even sort the items within each cluster by auto-MCDA ~LOL~
+        library watch -B --sort-groups-by 'mcda median_size,-deleted'
+        library watch -C --sort-groups-by 'mcda median_size,-deleted'
 
-        Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-        25 selected paths: 159.9 GB ; future free space: 484.7 GB
+    Filter media by file siblings of parent directory:
+        library watch --sibling   # only include files which have more than or equal to one sibling
+        library watch --solo      # only include files which are alone by themselves
 
-    After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
+        `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
+        library watch --sibling --solo      # you will always get zero records here
+        library watch --lower 2 --upper 1   # equivalent
 
-        Paste a path: done
+        You can be more specific via the `--upper` and `--lower` flags
+        library watch --lower 3   # only include files which have three or more siblings
+        library watch --upper 3   # only include files which have fewer than three siblings
+        library watch --lower 3 --upper 3   # only include files which are three siblings inclusive
+        library watch --lower 12 --upper 25 -O  # on my machine this launches My Mister 2018
 
-            Folder list saved to /tmp/tmp7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
+    Play recent partially-watched videos (requires mpv history):
+        library watch --partial       # play newest first
 
-                rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmp7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
+        library watch --partial old   # play oldest first
+        library watch -P o            # equivalent
 
+        library watch -P p            # sort by percent remaining
+        library watch -P t            # sort by time remaining
+        library watch -P s            # skip partially watched (only show unseen)
 
-</details>
+        The default time used is "last-viewed" (ie. the most recent time you closed the video)
+        If you want to use the "first-viewed" time (ie. the very first time you opened the video)
+        library watch -P f            # use watch_later file creation time instead of modified time
 
-###### scatter
+        You can combine most of these options, though some will be overridden by others.
+        library watch -P fo           # this means "show the oldest videos using the time I first opened them"
+        library watch -P pt           # weighted remaining (percent * time remaining)
 
-<details><summary>Scatter files between folders or disks</summary>
+    Print instead of play:
+        library watch --print --limit 10  # print the next 10 files
+        library watch -p -L 10  # print the next 10 files
+        library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
-    $ library scatter -h
-    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --targets TARGETS DATABASE RELATIVE_PATH ...
+        Printing modes
+        library watch -p    # print as a table
+        library watch -p a  # print an aggregate report
+        library watch -p b  # print a big-dirs report (see library bigdirs -h for more info)
+        library watch -p f  # print fields (defaults to path; use --cols to change)
+                               # -- useful for piping paths to utilities like xargs or GNU Parallel
 
-    Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+        library watch -p d  # mark deleted
+        library watch -p w  # mark watched
 
-    Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
+        Some printing modes can be combined
+        library watch -p df  # print files for piping into another program and mark them as deleted within the db
+        library watch -p bf  # print fields from big-dirs report
 
-        library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+        Check if you have downloaded something before
+        library watch -u duration -p -s 'title'
 
-    Reduce number of files per folder (creates more folders)
+        Print an aggregate report of deleted media
+        library watch -w time_deleted!=0 -p=a
+        ╒═══════════╤══════════════╤═════════╤═════════╕
+        │ path      │ duration     │ size    │   count │
+        ╞═══════════╪══════════════╪═════════╪═════════╡
+        │ Aggregate │ 14 days, 23  │ 50.6 GB │   29058 │
+        │           │ hours and 42 │         │         │
+        │           │ minutes      │         │         │
+        ╘═══════════╧══════════════╧═════════╧═════════╛
+        Total duration: 14 days, 23 hours and 42 minutes
 
-        library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
+        Print an aggregate report of media that has no duration information (ie. online or corrupt local media)
+        library watch -w 'duration is null' -p=a
 
-    Multi-device re-bin: balance by size
+        Print a list of filenames which have below 1280px resolution
+        library watch -w 'width<1280' -p=f
 
-        library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs.db subfolder/of/mergerfs/mnt
-        Current path distribution:
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+        Print media you have partially viewed with mpv
+        library watch --partial -p
+        library watch -P -p  # equivalent
+        library watch -P -p f --cols path,progress,duration  # print CSV of partially watched files
+        library watch --partial -pa  # print an aggregate report of partially watched files
 
-        Simulated path distribution:
-        5845 files should be moved
-        20257 files should not be moved
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_downloaded│
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
-        ### Move 1182 files to /mnt/d7 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
-        ### Move 1198 files to /mnt/d6 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
-        ### Move 1146 files to /mnt/d5 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
-        ### Move 1185 files to /mnt/d3 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
-        ### Move 1134 files to /mnt/d4 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+        View how much time you have watched
+        library watch -w play_count'>'0 -p=a
 
-    Multi-device re-bin: balance device inodes for specific subfolder
+        See how much video you have
+        library watch video.db -p=a
+        ╒═══════════╤═════════╤═════════╤═════════╕
+        │ path      │   hours │ size    │   count │
+        ╞═══════════╪═════════╪═════════╪═════════╡
+        │ Aggregate │  145769 │ 37.6 TB │  439939 │
+        ╘═══════════╧═════════╧═════════╧═════════╛
+        Total duration: 16 years, 7 months, 19 days, 17 hours and 25 minutes
 
-        library scatter -m /mnt/d1:/mnt/d2 fs.db subfolder --group count --sort 'size desc'
+        View all the columns
+        library watch -p -L 1 --cols '*'
 
-    Multi-device re-bin: only consider the most recent 100 files
+        Open ipython with all of your media
+        library watch -vv -p --cols '*'
+        ipdb> len(media)
+        462219
 
-        library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
+    Set the play queue size:
+        By default the play queue is 120--long enough that you likely have not noticed
+        but short enough that the program is snappy.
 
-    Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
+        If you want everything in your play queue you can use the aid of infinity.
+        Pick your poison (these all do effectively the same thing):
+        library watch -L inf
+        library watch -l inf
+        library watch --queue inf
+        library watch -L 999999999999
 
-        library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
+        You may also want to restrict the play queue.
+        For example, when you only want 1000 random files:
+        library watch -u random -L 1000
 
+    Offset the play queue:
+        You can also offset the queue. For example if you want to skip one or ten media:
+        library watch --offset 10      # offset ten from the top of an ordered query
 
-</details>
+    Repeat
+        library watch                  # listen to 120 random songs (DEFAULT_PLAY_QUEUE)
+        library watch --limit 5        # listen to FIVE songs
+        library watch -l inf -u random # listen to random songs indefinitely
+        library watch -s infinite      # listen to songs from the band infinite
 
-### Multi-database subcommands
+    Constrain media by search:
+        Audio files have many tags to readily search through so metadata like artist,
+        album, and even mood are included in search.
+        Video files have less consistent metadata and so only paths are included in search.
+        library watch --include happy  # only matches will be included
+        library watch -s happy         # equivalent
+        library watch --exclude sad    # matches will be excluded
+        library watch -E sad           # equivalent
 
-###### merge-dbs
+        Search only the path column
+        library watch -O -s 'path : mad max'
+        library watch -O -s 'path : "mad max"' # add "quotes" to be more strict
 
-<details><summary>Merge SQLITE databases</summary>
+        Double spaces are parsed as one space
+        library watch -s '  ost'        # will match OST and not ghost
+        library watch -s toy story      # will match '/folder/toy/something/story.mp3'
+        library watch -s 'toy  story'   # will match more strictly '/folder/toy story.mp3'
 
-    $ library merge-dbs -h
-    usage: library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
+        You can search without -s but it must directly follow the database due to how argparse works
+        library watch ./your.db searching for something
 
-    Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
-    and there is an existing row with the same PK, the default action is to delete the existing row and insert the new row
-    replacing all existing fields.
+    Constrain media by arbitrary SQL expressions:
+        library watch --where audio_count = 2  # media which have two audio tracks
+        library watch -w "language = 'eng'"    # media which have an English language tag
+                                                    (this could be audio _or_ subtitle)
+        library watch -w subtitle_count=0      # media that doesn't have subtitles
 
-    Upsert mode will update each matching PK row such that if a source row has a NULL field and
-    the destination row has a value then the value will be preserved instead of changed to the source row's NULL value.
+    Constrain media to duration (in minutes):
+        library watch --duration 20
+        library watch -d 6  # 6 mins ±10 percent (ie. between 5 and 7 mins)
+        library watch -d-6  # less than 6 mins
+        library watch -d+6  # more than 6 mins
 
-    Ignore mode (--only-new-rows) will insert only rows which don't already exist in the destination db
+        Duration can be specified multiple times:
+        library watch -d+5 -d-7  # should be similar to -d 6
 
-    Test first by using temp databases as the destination db.
-    Try out different modes / flags until you are satisfied with the behavior of the program
+        If you want exact time use `where`
+        library watch --where 'duration=6*60'
 
-        library merge-dbs --pk path (mktemp --suffix .db) tv.db movies.db
+    Constrain media to file size (in megabytes):
+        library watch --size 20
+        library watch -S 6  # 6 MB ±10 percent (ie. between 5 and 7 MB)
+        library watch -S-6  # less than 6 MB
+        library watch -S+6  # more than 6 MB
 
-    Merge database data and tables
+    Constrain media by time_created / time_last_played / time_deleted / time_modified:
+        library watch --created-within '3 days'
+        library watch --created-before '3 years'
 
-        library merge-dbs --upsert --pk path video.db tv.db movies.db
-        library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path --skip-column id audio-fts.db audio.db
+    Constrain media by throughput:
+        Bitrate information is not explicitly saved.
+        You can use file size and duration as a proxy for throughput:
+        library watch -w 'size/duration<50000'
 
-        library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
-        library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
+    Constrain media to portrait orientation video:
+        library watch --portrait
+        library watch -w 'width<height' # equivalent
 
-     To skip copying primary-keys from the source table(s) use --business-keys instead of --primary-keys
+    Constrain media to duration of videos which match any size constraints:
+        library watch --duration-from-size +700 -u 'duration desc, size desc'
 
-     Split DBs using --where
+    Constrain media to online-media or local-media:
+        Not to be confused with only local-media which is not "offline" (ie. one HDD disconnected)
+        library watch --online-media-only
+        library watch --online-media-only -i  # and ignore playback errors (ie. YouTube video deleted)
+        library watch --local-media-only
 
-         library merge-dbs --pk path specific-site.db big.db -v --only-new-rows -t media,playlists -w 'path like "https://specific-site%"'
+    Specify media play order:
+        library watch --sort duration   # play shortest media first
+        library watch -u duration desc  # play longest media first
 
+        You can use multiple SQL ORDER BY expressions
+        library watch -u 'subtitle_count > 0 desc' # play media that has at least one subtitle first
 
-</details>
+        Prioritize large-sized media
+        library watch --sort 'ntile(10000) over (order by size/duration) desc'
+        library watch -u 'ntile(100) over (order by size) desc'
 
-###### copy-play-counts
+        Sort by count of media with the same-X column (default DESC: most common to least common value)
+        library watch -u same-duration
+        library watch -u same-title
+        library watch -u same-size
+        library watch -u same-width, same-height ASC, same-fps
+        library watch -u same-time_uploaded same-view_count same-upvote_ratio
 
-<details><summary>Copy play history</summary>
+        No media found when using --random
+        In addition to -u/--sort random, there is also the -r/--random flag.
+        If you have a large database it should be faster than -u random but it comes with a caveat:
+        This flag randomizes via rowid at an earlier stage to boost performance.
+        It is possible that you see "No media found" or a smaller amount of media than correct.
+        You can bypass this by setting --limit. For example:
+        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa
+        path         count      size  duration                        avg_duration      avg_size
+        ---------  -------  --------  ------------------------------  --------------  ----------
+        Aggregate    10000  752.5 GB  4 months, 15 days and 10 hours  20 minutes         75.3 MB
+        (17 seconds)
+        library watch -B --folder-size=+12GiB --folder-size=-100GiB -r -pa -l inf
+        path         count     size  duration                                 avg_duration      avg_size
+        ---------  -------  -------  ---------------------------------------  --------------  ----------
+        Aggregate   140868  10.6 TB  5 years, 2 months, 28 days and 14 hours  20 minutes         75.3 MB
+        (30 seconds)
 
-    $ library copy-play-counts -h
-    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
+    Post-actions -- choose what to do after playing:
+        library watch --post-action keep    # do nothing after playing (default)
+        library watch -k delete             # delete file after playing
+        library watch -k softdelete         # mark deleted after playing
 
-    Copy play count information between databases
+        library watch -k ask_keep           # ask whether to keep after playing
+        library watch -k ask_delete         # ask whether to delete after playing
 
-        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
+        library watch -k move               # move to "keep" dir after playing
+        library watch -k ask_move           # ask whether to move to "keep" folder
+        The default location of the keep folder is ./keep/ (relative to the played media file)
+        You can change this by explicitly setting an *absolute* `keep-dir` path:
+        library watch -k ask_move --keep-dir /home/my/music/keep/
 
+        library watch -k ask_move_or_delete # ask after each whether to move to "keep" folder or delete
 
-</details>
+        You can also bind keys in mpv to different exit codes. For example in input.conf:
+            ; quit 5
 
-### Filesystem Database subcommands
+        And if you run something like:
+            library watch --cmd5 ~/bin/process_audio.py
+            library watch --cmd5 echo  # this will effectively do nothing except skip the normal post-actions via mpv shortcut
 
-###### christen
+        When semicolon is pressed in mpv (it will exit with error code 5) then the applicable player-exit-code command
+        will start with the media file as the first argument; in this case `~/bin/process_audio.py $path`.
+        The command will be daemonized if library exits before it completes.
 
-<details><summary>Clean filenames</summary>
+        To prevent confusion, normal post-actions will be skipped if the exit-code is greater than 4.
+        Exit-codes 0, 1, 2, 3, and 4: the external post-action will run after normal post-actions. Be careful of conflicting player-exit-code command and post-action behavior when using these!
 
-    $ library christen -h
-    usage: library christen DATABASE [--run]
+    Experimental options:
+        Duration to play (in seconds) while changing the channel
+        library watch --interdimensional-cable 40
+        library watch -4dtv 40
+        You can open two terminals to replicate AMV Hell somewhat
+        library watch --volume 0 -4dtv 30
+        library listen -4dtv 30
 
-    Rename files to be somewhat normalized
+        Playback multiple files at once
+        library watch --multiple-playback    # one per display; or two if only one display detected
+        library watch --multiple-playback 4  # play four media at once, divide by available screens
+        library watch -m 4 --screen-name eDP # play four media at once on specific screen
+        library watch -m 4 --loop --crop     # play four cropped videos on a loop
+        library watch -m 4 --hstack          # use hstack style
 
-    Default mode is simulate
+        When using `--multiple-playback` it may be helpful to set simple window focus rules to prevent keys from accidentally being entered in the wrong mpv window (as new windows are created and capture the cursor focus).
+        You can set and restore your previous mouse focus setting by wrapping the command like this:
 
-        library christen fs.db
+            focus-under-mouse
+            library watch ... --multiple-playback 4
+            focus-follows-mouse
 
-    To actually do stuff use the run flag
+        For example in KDE:
 
-        library christen audio.db --run
+            function focus-under-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusUnderMouse
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
 
-    You can optionally replace all the spaces in your filenames with dots
+            function focus-follows-mouse
+                kwriteconfig5 --file kwinrc --group Windows --key FocusPolicy FocusFollowsMouse
+                kwriteconfig5 --file kwinrc --group Windows --key NextFocusPrefersMouse true
+                qdbus-qt5 org.kde.KWin /KWin reconfigure
+            end
 
-        library christen --dot-space video.db
 
 
 </details>
 
-###### disk-usage
-
-<details><summary>Show disk usage</summary>
-
-    $ library disk-usage -h
-    usage: library disk-usage DATABASE [--sort-groups-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
+###### open-links
 
-    Only include files smaller than 1kib
+<details><summary>Open links from link dbs</summary>
 
-        library disk-usage du.db --size=-1Ki
-        lb du du.db -S-1Ki
-        | path                                  |      size |   count |
-        |---------------------------------------|-----------|---------|
-        | /home/xk/github/xk/lb/__pycache__/    | 620 Bytes |       1 |
-        | /home/xk/github/xk/lb/.github/        |    1.7 kB |       4 |
-        | /home/xk/github/xk/lb/__pypackages__/ |    1.4 MB |    3519 |
-        | /home/xk/github/xk/lb/xklb/           |    4.4 kB |      12 |
-        | /home/xk/github/xk/lb/tests/          |    3.2 kB |       9 |
-        | /home/xk/github/xk/lb/.git/           |  782.4 kB |    2276 |
-        | /home/xk/github/xk/lb/.pytest_cache/  |    1.5 kB |       5 |
-        | /home/xk/github/xk/lb/.ruff_cache/    |   19.5 kB |     100 |
-        | /home/xk/github/xk/lb/.gitattributes  | 119 Bytes |         |
-        | /home/xk/github/xk/lb/.mypy_cache/    | 280 Bytes |       4 |
-        | /home/xk/github/xk/lb/.pdm-python     |  15 Bytes |         |
+    $ library open-links -h
+    usage: library open-links DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
 
-    Only include files with a specific depth
+    Open links from a links db
 
-        library disk-usage du.db --depth 19
-        lb du du.db -d 19
-        | path                                                                                                                                                                |     size |
-        |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
-        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
-        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
+        wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
+        library open-links music.korea.ln.db
 
+    Only open links once
 
+        library open-links ln.db -w 'time_modified=0'
 
-</details>
+    Print a preview instead of opening tabs
 
-###### big-dirs
+        library open-links ln.db -p
+        library open-links ln.db --cols time_modified -p
 
-<details><summary>Show large folders</summary>
+    Delete rows
 
-    $ library big-dirs -h
-    usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
+        Make sure you have the right search query
+        library open-links ln.db "query" -p -L inf
+        library open-links ln.db "query" -pa  # view total
 
-    See what folders take up space
+        library open-links ln.db "query" -pd  # mark as deleted
 
-        library big-dirs video.db
-        library big-dirs audio.db
-        library big-dirs fs.db
+    Custom search engine
 
-    lb big-dirs video.db --folder-size=+10G --lower 400 --upper 14000
+        library open-links ln.db --title --prefix 'https://duckduckgo.com/?q='
 
-    lb big-dirs video.db --depth 5
-    lb big-dirs video.db --depth 7
+    Skip local media
 
-    You can even sort by auto-MCDA ~LOL~
+        library open-links dl.db --online
+        library open-links dl.db -w 'path like "http%"'  # equivalent
 
-    lb big-dirs video.db -u 'mcda median_size,-deleted'
 
 
 </details>
 
-###### search-db
-
-<details><summary>Search a SQLITE database</summary>
-
-    $ library search-db -h
-    usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
+###### surf
 
-    Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
+<details><summary>Auto-load browser tabs in a streaming way (stdin)</summary>
 
+    $ library surf -h
+    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
 
-</details>
+    Streaming tab loader: press ctrl+c to stop.
 
-###### optimize
+    Open tabs from a line-delimited file:
 
-<details><summary>Re-optimize database</summary>
+        cat tabs.txt | library surf -n 5
 
-    $ library optimize -h
-    usage: library optimize DATABASE [--force]
+    You will likely want to use this setting in `about:config`
 
-    Optimize library databases
+        browser.tabs.loadDivertedInBackground = True
 
-    The force flag is usually unnecessary and it can take much longer
+    If you prefer GUI, check out https://unli.xyz/tabsender/
 
 
 </details>
 
-### Single database enrichment subcommands
+### Database enrichment subcommands
 
 ###### dedupe-db
 
 <details><summary>Dedupe SQLITE tables</summary>
 
     $ library dedupe-db -h
     usage: library dedupe-dbs DATABASE TABLE --bk BUSINESS_KEYS [--pk PRIMARY_KEYS] [--only-columns COLUMNS]
@@ -2833,60 +2786,118 @@
         library tabs-shuffle tabs.db -d  31 -f monthly
         library tabs-shuffle tabs.db -d  90 -f quarterly
         library tabs-shuffle tabs.db -d 365 -f yearly
 
 
 </details>
 
-### Misc subcommands
+### Update database subcommands
 
-###### export-text
+###### fsupdate
 
-<details><summary>Export HTML files from SQLite databases</summary>
+<details><summary>Update local media</summary>
 
-    $ library export-text -h
-    usage: library export-text DATABASE
+    $ library fsupdate -h
+    usage: library fsupdate DATABASE
 
-    Generate HTML files from SQLite databases
+    Update each path previously saved:
+
+        library fsupdate video.db
 
 
 </details>
 
-###### process-ffmpeg
+###### tubeupdate
 
-<details><summary>Shrink video/audio to AV1/Opus format (.mkv, .mka)</summary>
+<details><summary>Update online video media</summary>
 
-    $ library process-ffmpeg -h
-    usage: library process-ffmpeg PATH ... [--always-split] [--split-longer-than DURATION] [--min-split-segment SECONDS] [--simulate]
+    $ library tubeupdate -h
+    usage: library tubeupdate [--audio | --video] DATABASE
 
-    Resize videos to max 1440x960px AV1 and/or Opus to save space
+    Fetch the latest videos for every playlist saved in your database
 
-    Convert audio to Opus. Optionally split up long tracks into multiple files.
+        library tubeupdate educational.db
 
-        fd -tf -eDTS -eAAC -eWAV -eAIF -eAIFF -eFLAC -eAIFF -eM4A -eMP3 -eOGG -eMP4 -eWMA -j4 -x library process --audio
+    Fetch extra metadata:
 
-    Use --always-split to _always_ split files if silence is detected
+        By default tubeupdate will quickly add media.
+        You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
 
-        library process-audio --always-split audiobook.m4a
+        library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 
-    Use --split-longer-than to _only_ detect silence for files in excess of a specific duration
+    Remove duplicate playlists:
 
-        library process-audio --split-longer-than 36mins audiobook.m4b audiobook2.mp3
+        lb dedupe-db video.db playlists --bk extractor_playlist_id
 
 
 </details>
 
-###### process-image
+###### webupdate
 
-<details><summary>Shrink images by resizing and AV1 image format (.avif)</summary>
+<details><summary>Update open-directory media</summary>
 
-    $ library process-image -h
-    usage: library process-image PATH ...
+    $ library webupdate -h
+    usage: library web-update DATABASE
 
-    Resize images to max 2400x2400px and format AVIF to save space
+    Update saved open directories
+
+
+
+</details>
+
+###### galleryupdate
+
+<details><summary>Update online gallery media</summary>
+
+    $ library galleryupdate -h
+    usage: library galleryupdate DATABASE URLS
+
+    Check previously saved gallery_dl URLs for new content
+
+
+</details>
+
+###### links-update
+
+<details><summary>Update a link-scraping database</summary>
+
+    $ library links-update -h
+    usage: library links-update DATABASE
+
+    Fetch new links from each path previously saved
+
+        library links-update links.db
+
+
+</details>
+
+###### redditupdate
+
+<details><summary>Update reddit media</summary>
+
+    $ library redditupdate -h
+    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+
+    Fetch the latest posts for every subreddit/redditor saved in your database
+
+        library redditupdate edu_subreddits.db
+
+
+</details>
+
+### Misc subcommands
+
+###### export-text
+
+<details><summary>Export HTML files from SQLite databases</summary>
+
+    $ library export-text -h
+    usage: library export-text DATABASE
+
+    Generate HTML files from SQLite databases
 
 
 </details>
 
 
 <details><summary>Chicken mode</summary>
```


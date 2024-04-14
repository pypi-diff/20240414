# Comparing `tmp/xklb-2.6.5.tar.gz` & `tmp/xklb-2.6.6.tar.gz`

## Comparing `xklb-2.6.5.tar` & `xklb-2.6.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.5/.gitattributes
--rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.5/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/__init__.py
--rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/db_playlists.py
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/dl_extract.py
--rw-r--r--   0        0        0    15664 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/fs_extract.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/gdl_extract.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/history.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/hn_extract.py
--rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/lb.py
--rw-r--r--   0        0        0    19486 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/play_actions.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/post_actions.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/readme.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/reddit_extract.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/rss_extract.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/search.py
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/site_extract.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tabs_actions.py
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tabs_extract.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tube_backend.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tube_extract.py
--rw-r--r--   0        0        0   118259 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/__init__.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/av.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/books.py
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/dedupe.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/media_check.py
--rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/media_player.py
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/media_printer.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/subtitle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/add_row.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/big_dirs.py
--rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/block.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/christen.py
--rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/dedupe_czkawka.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/eda.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/export_text.py
--rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/history.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/incremental_diff.py
--rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/links_db.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mcda.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/merge_folders.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/move_list.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/open_links.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/process_ffmpeg.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/process_image.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/rel_mv.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/sample_compare.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/sample_hash.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/search_db.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0     9863 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/extract_text.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/markdown_links.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/substack.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/tildes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/__init__.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    17735 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/consts.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/devices.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/nums.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/objects.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/printing.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/processes.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/strings.py
--rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/web.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.5/.gitignore
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.5/pyproject.toml
--rw-r--r--   0        0        0   158100 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/README.md
--rw-r--r--   0        0        0   161861 2020-02-02 00:00:00.000000 xklb-2.6.5/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.6/.gitattributes
+-rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.6/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/__init__.py
+-rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/db_playlists.py
+-rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/dl_extract.py
+-rw-r--r--   0        0        0    15664 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/fs_extract.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/gdl_extract.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/history.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/hn_extract.py
+-rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/lb.py
+-rw-r--r--   0        0        0    19486 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/play_actions.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/post_actions.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/readme.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/reddit_extract.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/rss_extract.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/search.py
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/site_extract.py
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/tube_extract.py
+-rw-r--r--   0        0        0   118259 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/__init__.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/av.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/books.py
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/dedupe.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/media_check.py
+-rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/media_player.py
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/media_printer.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/media/subtitle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/add_row.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/big_dirs.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/christen.py
+-rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/dedupe_czkawka.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/eda.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/export_text.py
+-rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/history.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/incremental_diff.py
+-rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/links_db.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mcda.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/merge_folders.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/open_links.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/process_ffmpeg.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/process_image.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/rel_mv.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/sample_compare.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/sample_hash.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/search_db.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/extract_text.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/markdown_links.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/substack.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/scripts/mining/tildes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    17735 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/processes.py
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/utils/web.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.6/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.6/.gitignore
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.6/pyproject.toml
+-rw-r--r--   0        0        0   158230 2020-02-02 00:00:00.000000 xklb-2.6.6/.github/README.md
+-rw-r--r--   0        0        0   161991 2020-02-02 00:00:00.000000 xklb-2.6.6/PKG-INFO
```

### Comparing `xklb-2.6.5/pdm.lock` & `xklb-2.6.6/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/.github/LICENSE` & `xklb-2.6.6/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/.github/Windows.md` & `xklb-2.6.6/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/.github/examples/extract.svg` & `xklb-2.6.6/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/.github/examples/tubeadd.svg` & `xklb-2.6.6/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/.github/workflows/push.yaml` & `xklb-2.6.6/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/db_media.py` & `xklb-2.6.6/xklb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/db_playlists.py` & `xklb-2.6.6/xklb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/dl_extract.py` & `xklb-2.6.6/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/fs_extract.py` & `xklb-2.6.6/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/gdl_backend.py` & `xklb-2.6.6/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/gdl_extract.py` & `xklb-2.6.6/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/history.py` & `xklb-2.6.6/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/hn_extract.py` & `xklb-2.6.6/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/lb.py` & `xklb-2.6.6/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/play_actions.py` & `xklb-2.6.6/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/post_actions.py` & `xklb-2.6.6/xklb/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/readme.py` & `xklb-2.6.6/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/reddit_extract.py` & `xklb-2.6.6/xklb/reddit_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/rss_extract.py` & `xklb-2.6.6/xklb/rss_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/search.py` & `xklb-2.6.6/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/site_extract.py` & `xklb-2.6.6/xklb/site_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/tabs_actions.py` & `xklb-2.6.6/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/tabs_extract.py` & `xklb-2.6.6/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/tube_backend.py` & `xklb-2.6.6/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/tube_extract.py` & `xklb-2.6.6/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/usage.py` & `xklb-2.6.6/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/data/imagemagick_errors.py` & `xklb-2.6.6/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/data/wordbank.py` & `xklb-2.6.6/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/data/yt_dlp_errors.py` & `xklb-2.6.6/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/media/av.py` & `xklb-2.6.6/xklb/media/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/media/books.py` & `xklb-2.6.6/xklb/media/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/media/dedupe.py` & `xklb-2.6.6/xklb/media/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/media/media_check.py` & `xklb-2.6.6/xklb/media/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/media/media_player.py` & `xklb-2.6.6/xklb/media/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/media/media_printer.py` & `xklb-2.6.6/xklb/media/media_printer.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/media/subtitle.py` & `xklb-2.6.6/xklb/media/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scratch/javguru.py` & `xklb-2.6.6/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scratch/javtiful.py` & `xklb-2.6.6/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scratch/mam_search.py` & `xklb-2.6.6/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scratch/mam_slots.py` & `xklb-2.6.6/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/add_row.py` & `xklb-2.6.6/xklb/scripts/add_row.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/big_dirs.py` & `xklb-2.6.6/xklb/scripts/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/block.py` & `xklb-2.6.6/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/christen.py` & `xklb-2.6.6/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/cluster_sort.py` & `xklb-2.6.6/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/copy_play_counts.py` & `xklb-2.6.6/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/dedupe_czkawka.py` & `xklb-2.6.6/xklb/scripts/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/dedupe_db.py` & `xklb-2.6.6/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/disk_usage.py` & `xklb-2.6.6/xklb/scripts/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/download_status.py` & `xklb-2.6.6/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/eda.py` & `xklb-2.6.6/xklb/scripts/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/export_text.py` & `xklb-2.6.6/xklb/scripts/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/history.py` & `xklb-2.6.6/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/incremental_diff.py` & `xklb-2.6.6/xklb/scripts/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/links_db.py` & `xklb-2.6.6/xklb/scripts/links_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     parser.add_argument("--page-step", "--step", "-S", type=int, default=1)
     parser.add_argument("--page-start", "--start-page", "--start", type=int)
 
     arggroups.filter_links(parser)
 
     arggroups.requests(parser)
     arggroups.selenium(parser)
+    arggroups.extractor(parser)
 
     parser.add_argument("--force", action="store_true")
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     if "add" in kwargs["prog"]:
@@ -241,15 +242,15 @@
     )
     return len(new_media)
 
 
 def links_add() -> None:
     args, _parser = parse_args(prog="library links-add", usage=usage.links_add)
 
-    if args.no_extract:
+    if args.insert_only:
         media_new = set()
         media_known = set()
         for p in arg_utils.gen_paths(args):
             if db_media.exists(args, p):
                 media_known.add(p)
                 if args.category:
                     update_category(args, p)
```

### Comparing `xklb-2.6.5/xklb/scripts/mcda.py` & `xklb-2.6.6/xklb/scripts/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/merge_dbs.py` & `xklb-2.6.6/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/merge_folders.py` & `xklb-2.6.6/xklb/scripts/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/merge_online_local.py` & `xklb-2.6.6/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/move_list.py` & `xklb-2.6.6/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/open_links.py` & `xklb-2.6.6/xklb/scripts/open_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/optimize_db.py` & `xklb-2.6.6/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/places_import.py` & `xklb-2.6.6/xklb/scripts/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/playback_control.py` & `xklb-2.6.6/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/playlists.py` & `xklb-2.6.6/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/process_ffmpeg.py` & `xklb-2.6.6/xklb/scripts/process_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/process_image.py` & `xklb-2.6.6/xklb/scripts/process_image.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/redownload.py` & `xklb-2.6.6/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/rel_mv.py` & `xklb-2.6.6/xklb/scripts/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/sample_compare.py` & `xklb-2.6.6/xklb/scripts/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/sample_hash.py` & `xklb-2.6.6/xklb/scripts/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/scatter.py` & `xklb-2.6.6/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/search_db.py` & `xklb-2.6.6/xklb/scripts/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/streaming_tab_loader.py` & `xklb-2.6.6/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/web_add.py` & `xklb-2.6.6/xklb/scripts/web_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 def web_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args, _parser = parse_args(prog=f"library {SC.webadd}", usage=usage.webadd)
     web.requests_session(args)  # configure session
 
-    if args.no_extract:
+    if args.insert_only:
         media_new = set()
         media_known = set()
         for p in arg_utils.gen_paths(args):
             if db_media.exists(args, p):
                 media_known.add(p)
             else:
                 add_media(args, [p])
```

### Comparing `xklb-2.6.5/xklb/scripts/mining/extract_links.py` & `xklb-2.6.6/xklb/scripts/mining/extract_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         else:
             printing.pipe_print(link)
 
 
 def extract_links() -> None:
     args = parse_args()
 
-    if args.no_extract:
+    if args.insert_only:
         for url in arg_utils.gen_paths(args):
             url = web.url_decode(url).strip()
             if args.download:
                 web.download_url(url)
             else:
                 printing.pipe_print(url)
         return
```

### Comparing `xklb-2.6.5/xklb/scripts/mining/extract_text.py` & `xklb-2.6.6/xklb/scripts/mining/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/mining/markdown_links.py` & `xklb-2.6.6/xklb/scripts/mining/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.6.6/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/mining/nouns.py` & `xklb-2.6.6/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/mining/pushshift.py` & `xklb-2.6.6/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.6.6/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/mining/substack.py` & `xklb-2.6.6/xklb/scripts/mining/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/scripts/mining/tildes.py` & `xklb-2.6.6/xklb/scripts/mining/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/arg_utils.py` & `xklb-2.6.6/xklb/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/arggroups.py` & `xklb-2.6.6/xklb/utils/arggroups.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/argparse_utils.py` & `xklb-2.6.6/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/consts.py` & `xklb-2.6.6/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/db_utils.py` & `xklb-2.6.6/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/devices.py` & `xklb-2.6.6/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/file_utils.py` & `xklb-2.6.6/xklb/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/gui.py` & `xklb-2.6.6/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/iterables.py` & `xklb-2.6.6/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/log_utils.py` & `xklb-2.6.6/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/mpv_utils.py` & `xklb-2.6.6/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/nums.py` & `xklb-2.6.6/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/objects.py` & `xklb-2.6.6/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/path_utils.py` & `xklb-2.6.6/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/pd_utils.py` & `xklb-2.6.6/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/printing.py` & `xklb-2.6.6/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/processes.py` & `xklb-2.6.6/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/sql_utils.py` & `xklb-2.6.6/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/strings.py` & `xklb-2.6.6/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/utils/web.py` & `xklb-2.6.6/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/xklb/assets/kotobago.png` & `xklb-2.6.6/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/.gitignore` & `xklb-2.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/pyproject.toml` & `xklb-2.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.5/.github/README.md` & `xklb-2.6.6/.github/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
 Should also work on Mac OS.
+<img align="right" width="400" src="https://raw.githubusercontent.com/chapmanjacobd/library/main/.github/examples/tubeadd.svg" />
 
 ### External dependencies
 
 Required: `ffmpeg`
 
 Some features work better with: `mpv`, `firefox`, `fish`
 
@@ -91,15 +92,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.005)
+    xk media library subcommands (v2.6.006)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
```

### Comparing `xklb-2.6.5/PKG-INFO` & `xklb-2.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.6.5
+Version: 2.6.6
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -97,14 +97,15 @@
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
 Should also work on Mac OS.
+<img align="right" width="400" src="https://raw.githubusercontent.com/chapmanjacobd/library/main/.github/examples/tubeadd.svg" />
 
 ### External dependencies
 
 Required: `ffmpeg`
 
 Some features work better with: `mpv`, `firefox`, `fish`
 
@@ -179,15 +180,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.005)
+    xk media library subcommands (v2.6.006)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
```


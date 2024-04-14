# Comparing `tmp/py_ptsl-101.1.0.tar.gz` & `tmp/py_ptsl-301.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ptsl-101.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_ptsl-301.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_ptsl-101.1.0.tar` & `py_ptsl-301.0.0.tar`

### file list

```diff
@@ -1,83 +1,89 @@
--rw-r--r--   0        0        0     1498 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/LICENSE
--rw-r--r--   0        0        0     2270 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/README.md
--rw-r--r--   0        0        0    53243 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/PTSL_pb2.py
--rw-r--r--   0        0        0    74192 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/PTSL_pb2.pyi
--rw-r--r--   0        0        0     4008 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/PTSL_pb2_grpc.py
--rw-r--r--   0        0        0     1075 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/__init__.py
--rw-r--r--   0        0        0     3926 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/builders/create_session_builder.py
--rw-r--r--   0        0        0     4277 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/builders/export_text_builder.py
--rw-r--r--   0        0        0     4611 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/builders/import_builder.py
--rw-r--r--   0        0        0    11768 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/client.py
--rw-r--r--   0        0        0    25347 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/engine.py
--rw-r--r--   0        0        0     1416 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/errors.py
--rw-r--r--   0        0        0     3654 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/__init__.py
--rw-r--r--   0        0        0       80 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/authorize_connection.py
--rw-r--r--   0        0        0       66 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/clear.py
--rw-r--r--   0        0        0       73 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/clear_special.py
--rw-r--r--   0        0        0       73 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/close_session.py
--rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/consolidate_clip.py
--rw-r--r--   0        0        0       65 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/copy.py
--rw-r--r--   0        0        0       72 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/copy_special.py
--rw-r--r--   0        0        0       87 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/create_fades_based_on_preset.py
--rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/create_session.py
--rw-r--r--   0        0        0       64 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/cut.py
--rw-r--r--   0        0        0       71 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/cut_special.py
--rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_clips_as_files.py
--rw-r--r--   0        0        0       70 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_mix.py
--rw-r--r--   0        0        0       89 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_selected_tracks_as_aaf_omf.py
--rw-r--r--   0        0        0       84 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_session_info_as_text.py
--rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/extend_selection_to_target_tracks.py
--rw-r--r--   0        0        0       81 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_dyamic_properties.py
--rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_file_location.py
--rw-r--r--   0        0        0      695 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_playback_mode.py
--rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_ptsl_version.py
--rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_record_mode.py
--rw-r--r--   0        0        0       82 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_audio_format.py
--rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_audio_rate_pull_settings.py
--rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_bit_depth.py
--rw-r--r--   0        0        0       85 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_feet_frames_rate.py
--rw-r--r--   0        0        0      537 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_interleaved_state.py
--rw-r--r--   0        0        0       77 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_length.py
--rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_name.py
--rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_path.py
--rw-r--r--   0        0        0      631 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_sample_rate.py
--rw-r--r--   0        0        0       80 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_start_time.py
--rw-r--r--   0        0        0       83 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_time_code_rate.py
--rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_video_rate_pull_settings.py
--rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_task_status.py
--rw-r--r--   0        0        0      774 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_track_list.py
--rw-r--r--   0        0        0       78 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_transport_armed.py
--rw-r--r--   0        0        0       78 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_transport_state.py
--rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/host_ready_check.py
--rw-r--r--   0        0        0       69 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/import_command.py
--rw-r--r--   0        0        0      127 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/memory_locations.py
--rw-r--r--   0        0        0       72 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/open_session.py
--rw-r--r--   0        0        0     2771 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/operation.py
--rw-r--r--   0        0        0       66 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/paste.py
--rw-r--r--   0        0        0       73 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/paste_special.py
--rw-r--r--   0        0        0       89 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/refresh_all_modified_audio_files.py
--rw-r--r--   0        0        0       84 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/refresh_target_audio_files.py
--rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/register_connection.py
--rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/rename_selected_clip.py
--rw-r--r--   0        0        0       77 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/rename_target_clip.py
--rw-r--r--   0        0        0       78 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/rename_target_track.py
--rw-r--r--   0        0        0       72 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/save_session.py
--rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/save_session_as.py
--rw-r--r--   0        0        0       82 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/select_all_clips_on_track.py
--rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_playback_mode.py
--rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_record_mode.py
--rw-r--r--   0        0        0       82 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_audio_format.py
--rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_audio_rate_pull_settings.py
--rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_bit_depth.py
--rw-r--r--   0        0        0       85 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_feet_frames_rate.py
--rw-r--r--   0        0        0       87 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_interleaved_state.py
--rw-r--r--   0        0        0       77 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_length.py
--rw-r--r--   0        0        0       80 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_start_time.py
--rw-r--r--   0        0        0       83 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_time_code_rate.py
--rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_video_rate_pull_settings.py
--rw-r--r--   0        0        0       65 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/spot.py
--rw-r--r--   0        0        0      212 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/toggle_play_state.py
--rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/trim_to_selection.py
--rw-r--r--   0        0        0     4821 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/util.py
--rw-r--r--   0        0        0     1759 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/pyproject.toml
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 py_ptsl-101.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-04-14 02:43:38.233406 py_ptsl-301.0.0/LICENSE
+-rw-r--r--   0        0        0     2578 2024-04-14 02:43:38.233406 py_ptsl-301.0.0/README.md
+-rw-r--r--   0        0        0    74671 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/PTSL_pb2.py
+-rw-r--r--   0        0        0   121696 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/PTSL_pb2.pyi
+-rw-r--r--   0        0        0     4466 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/PTSL_pb2_grpc.py
+-rw-r--r--   0        0        0     1075 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/__init__.py
+-rw-r--r--   0        0        0     3928 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/builders/create_session_builder.py
+-rw-r--r--   0        0        0     4277 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/builders/export_text_builder.py
+-rw-r--r--   0        0        0     4611 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/builders/import_builder.py
+-rw-r--r--   0        0        0    11897 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/client.py
+-rw-r--r--   0        0        0    32277 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/engine.py
+-rw-r--r--   0        0        0     1450 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/errors.py
+-rw-r--r--   0        0        0     4032 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/authorize_connection.py
+-rw-r--r--   0        0        0       66 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/clear.py
+-rw-r--r--   0        0        0       73 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/clear_special.py
+-rw-r--r--   0        0        0       73 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/close_session.py
+-rw-r--r--   0        0        0       76 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/consolidate_clip.py
+-rw-r--r--   0        0        0       65 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/copy.py
+-rw-r--r--   0        0        0       72 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/copy_special.py
+-rw-r--r--   0        0        0       87 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/create_fades_based_on_preset.py
+-rw-r--r--   0        0        0       76 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/create_new_tracks.py
+-rw-r--r--   0        0        0       74 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/create_session.py
+-rw-r--r--   0        0        0       64 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/cut.py
+-rw-r--r--   0        0        0       71 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/cut_special.py
+-rw-r--r--   0        0        0      209 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/edit_mode.py
+-rw-r--r--   0        0        0      113 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/edit_tool.py
+-rw-r--r--   0        0        0       79 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/export_clips_as_files.py
+-rw-r--r--   0        0        0       70 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/export_mix.py
+-rw-r--r--   0        0        0       89 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/export_selected_tracks_as_aaf_omf.py
+-rw-r--r--   0        0        0       84 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/export_session_info_as_text.py
+-rw-r--r--   0        0        0       92 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/extend_selection_to_target_tracks.py
+-rw-r--r--   0        0        0       81 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_dyamic_properties.py
+-rw-r--r--   0        0        0       76 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_file_location.py
+-rw-r--r--   0        0        0      695 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_playback_mode.py
+-rw-r--r--   0        0        0       75 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_ptsl_version.py
+-rw-r--r--   0        0        0       74 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_record_mode.py
+-rw-r--r--   0        0        0       82 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_audio_format.py
+-rw-r--r--   0        0        0       92 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_audio_rate_pull_settings.py
+-rw-r--r--   0        0        0       79 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_bit_depth.py
+-rw-r--r--   0        0        0       85 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_feet_frames_rate.py
+-rw-r--r--   0        0        0      537 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_interleaved_state.py
+-rw-r--r--   0        0        0       77 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_length.py
+-rw-r--r--   0        0        0       75 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_name.py
+-rw-r--r--   0        0        0       75 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_path.py
+-rw-r--r--   0        0        0      631 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_sample_rate.py
+-rw-r--r--   0        0        0       80 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_start_time.py
+-rw-r--r--   0        0        0       83 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_time_code_rate.py
+-rw-r--r--   0        0        0       92 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_session_video_rate_pull_settings.py
+-rw-r--r--   0        0        0       74 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_task_status.py
+-rw-r--r--   0        0        0      774 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_track_list.py
+-rw-r--r--   0        0        0       78 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_transport_armed.py
+-rw-r--r--   0        0        0       78 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/get_transport_state.py
+-rw-r--r--   0        0        0       75 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/host_ready_check.py
+-rw-r--r--   0        0        0       69 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/import_command.py
+-rw-r--r--   0        0        0      177 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/memory_locations.py
+-rw-r--r--   0        0        0       72 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/open_session.py
+-rw-r--r--   0        0        0     2771 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/operation.py
+-rw-r--r--   0        0        0       66 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/paste.py
+-rw-r--r--   0        0        0       73 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/paste_special.py
+-rw-r--r--   0        0        0       89 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/refresh_all_modified_audio_files.py
+-rw-r--r--   0        0        0       84 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/refresh_target_audio_files.py
+-rw-r--r--   0        0        0       79 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/register_connection.py
+-rw-r--r--   0        0        0       79 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/rename_selected_clip.py
+-rw-r--r--   0        0        0       77 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/rename_target_clip.py
+-rw-r--r--   0        0        0       78 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/rename_target_track.py
+-rw-r--r--   0        0        0       72 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/save_session.py
+-rw-r--r--   0        0        0       74 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/save_session_as.py
+-rw-r--r--   0        0        0       82 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/select_all_clips_on_track.py
+-rw-r--r--   0        0        0       79 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/select_tracks.py
+-rw-r--r--   0        0        0       76 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_playback_mode.py
+-rw-r--r--   0        0        0       74 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_record_mode.py
+-rw-r--r--   0        0        0       82 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_audio_format.py
+-rw-r--r--   0        0        0       92 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_audio_rate_pull_settings.py
+-rw-r--r--   0        0        0       79 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_bit_depth.py
+-rw-r--r--   0        0        0       85 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_feet_frames_rate.py
+-rw-r--r--   0        0        0       87 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_interleaved_state.py
+-rw-r--r--   0        0        0       77 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_length.py
+-rw-r--r--   0        0        0       80 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_start_time.py
+-rw-r--r--   0        0        0       83 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_time_code_rate.py
+-rw-r--r--   0        0        0       92 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/set_session_video_rate_pull_settings.py
+-rw-r--r--   0        0        0       65 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/spot.py
+-rw-r--r--   0        0        0      131 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/timeline_selection.py
+-rw-r--r--   0        0        0      212 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/toggle_play_state.py
+-rw-r--r--   0        0        0       76 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/trim_to_selection.py
+-rw-r--r--   0        0        0       77 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/ops/zoom_preset.py
+-rw-r--r--   0        0        0     4821 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/ptsl/util.py
+-rw-r--r--   0        0        0     1802 2024-04-14 02:43:38.237406 py_ptsl-301.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 py_ptsl-301.0.0/PKG-INFO
```

### Comparing `py_ptsl-101.1.0/LICENSE` & `py_ptsl-301.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/README.md` & `py_ptsl-301.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [![Lint and Test](https://github.com/iluvcapra/py-ptsl/actions/workflows/lint_and_pytest.yml/badge.svg)](https://github.com/iluvcapra/py-ptsl/actions/workflows/lint_and_pytest.yml)
 [![codecov](https://codecov.io/gh/iluvcapra/py-ptsl/branch/master/graph/badge.svg?token=PR6SUQJISZ)](https://codecov.io/gh/iluvcapra/py-ptsl)
 [![Documentation Status](https://readthedocs.org/projects/py-ptsl/badge/?version=latest)](https://py-ptsl.readthedocs.io/en/latest/?badge=latest)
 ![GitHub last commit](https://img.shields.io/github/last-commit/iluvcapra/py-ptsl)
 
 ![](https://img.shields.io/pypi/pyversions/py-ptsl.svg) [![](https://img.shields.io/pypi/v/py-ptsl.svg)](https://pypi.org/project/py-ptsl/) ![](https://img.shields.io/pypi/wheel/py-ptsl.svg)
 
-[![Pro Tools Version - 2023.6](https://img.shields.io/static/v1?label=Pro+Tools+Version&message=2023.6&color=8f228f)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
-[![PTSL Version - 1](https://img.shields.io/static/v1?label=PTSL+Version&message=1&color=0000ff)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
+[![Pro Tools Version - 2023.9](https://img.shields.io/static/v1?label=Pro+Tools+Version&message=2023.9&color=8f228f)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
+[![PTSL Version - 3](https://img.shields.io/static/v1?label=PTSL+Version&message=3&color=0000ff)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
 
 # py-ptsl
 
 Native Python PTSL (Pro Tools Scripting Library) RPC interface
 
 ## Important Notice! 
 
@@ -27,21 +27,26 @@
 - [session_info.py](examples/session_info.py) - This example 
   prints a list of gettable properties from the currently-open
       session.
 - [print_tracks.py](examples/print_tracks.py) - This example prints
   a list of every track in the currently-open session, including state
   information like selection, mute and solo state, track color and 
   track ID.
+- [make_session.py](examples/make_session.py) - Creates a new
+  session interactively from the terminal.
+- [pt_set.py](examples/pt_set.py) - Allows several session setup
+  options to be set from the terminal.
+- [pt_pasteboard.py](examples/pt_pasteboard.py) - Demonstrates
+  triggering cut/copy/paste actions.
 
 
 ### Sending Commands To Pro Tools with the `Engine` class
 
 The `Engine` class exposes `ptsl` commands with a method call interface.
 
 ```python
 from ptsl import open_engine
 
 with open_engine(company_name="MY_COMPANY", application_name="MY_TOOL") as engine:
     session_name = engine.session_name()
-
 ```
```

### Comparing `py_ptsl-101.1.0/ptsl/PTSL_pb2_grpc.py` & `py_ptsl-301.0.0/ptsl/PTSL_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.SendGrpcRequest = channel.unary_unary(
-                '/ptsl.PTSL/SendGrpcRequest',
-                request_serializer=PTSL__pb2.Request.SerializeToString,
-                response_deserializer=PTSL__pb2.Response.FromString,
-                )
+            '/ptsl.PTSL/SendGrpcRequest',
+            request_serializer=PTSL__pb2.Request.SerializeToString,
+            response_deserializer=PTSL__pb2.Response.FromString,
+        )
         self.SendGrpcStreamingRequest = channel.unary_stream(
-                '/ptsl.PTSL/SendGrpcStreamingRequest',
-                request_serializer=PTSL__pb2.Request.SerializeToString,
-                response_deserializer=PTSL__pb2.Response.FromString,
-                )
+            '/ptsl.PTSL/SendGrpcStreamingRequest',
+            request_serializer=PTSL__pb2.Request.SerializeToString,
+            response_deserializer=PTSL__pb2.Response.FromString,
+        )
 
 
 class PTSLServicer(object):
     """*
     Service for handling different types of ProTools commands using PTSL Client.
     """
 
@@ -48,62 +48,63 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_PTSLServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'SendGrpcRequest': grpc.unary_unary_rpc_method_handler(
-                    servicer.SendGrpcRequest,
-                    request_deserializer=PTSL__pb2.Request.FromString,
-                    response_serializer=PTSL__pb2.Response.SerializeToString,
-            ),
-            'SendGrpcStreamingRequest': grpc.unary_stream_rpc_method_handler(
-                    servicer.SendGrpcStreamingRequest,
-                    request_deserializer=PTSL__pb2.Request.FromString,
-                    response_serializer=PTSL__pb2.Response.SerializeToString,
-            ),
+        'SendGrpcRequest': grpc.unary_unary_rpc_method_handler(
+            servicer.SendGrpcRequest,
+            request_deserializer=PTSL__pb2.Request.FromString,
+            response_serializer=PTSL__pb2.Response.SerializeToString,
+        ),
+        'SendGrpcStreamingRequest': grpc.unary_stream_rpc_method_handler(
+            servicer.SendGrpcStreamingRequest,
+            request_deserializer=PTSL__pb2.Request.FromString,
+            response_serializer=PTSL__pb2.Response.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'ptsl.PTSL', rpc_method_handlers)
+        'ptsl.PTSL', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
-
  # This class is part of an EXPERIMENTAL API.
+
+
 class PTSL(object):
     """*
     Service for handling different types of ProTools commands using PTSL Client.
     """
 
     @staticmethod
     def SendGrpcRequest(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                        target,
+                        options=(),
+                        channel_credentials=None,
+                        call_credentials=None,
+                        insecure=False,
+                        compression=None,
+                        wait_for_ready=None,
+                        timeout=None,
+                        metadata=None):
         return grpc.experimental.unary_unary(request, target, '/ptsl.PTSL/SendGrpcRequest',
-            PTSL__pb2.Request.SerializeToString,
-            PTSL__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             PTSL__pb2.Request.SerializeToString,
+                                             PTSL__pb2.Response.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SendGrpcStreamingRequest(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                                 target,
+                                 options=(),
+                                 channel_credentials=None,
+                                 call_credentials=None,
+                                 insecure=False,
+                                 compression=None,
+                                 wait_for_ready=None,
+                                 timeout=None,
+                                 metadata=None):
         return grpc.experimental.unary_stream(request, target, '/ptsl.PTSL/SendGrpcStreamingRequest',
-            PTSL__pb2.Request.SerializeToString,
-            PTSL__pb2.Response.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                              PTSL__pb2.Request.SerializeToString,
+                                              PTSL__pb2.Response.FromString,
+                                              options, channel_credentials,
+                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `py_ptsl-101.1.0/ptsl/__init__.py` & `py_ptsl-301.0.0/ptsl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 - The first element of the version triple is the PTSL version as
   supported by the client * 100, plus the major version of this module.
 - The second element increments with feature enhancements. Support for
   new versions of Pro Tools will always increment this value.
 - The third element increments with bug fixes or modifcations to docs,
   build system, etc.
 
-
 """
 
+
 from .client import Client
 from .engine import Engine, open_engine
 from .errors import CommandError
 
-__version__ = '101.1.0'
+__version__ = '301.0.0'
```

### Comparing `py_ptsl-101.1.0/ptsl/builders/create_session_builder.py` & `py_ptsl-301.0.0/ptsl/builders/create_session_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ptsl.PTSL_pb2 import SAF_AIFF, SAF_WAVE,\
+from ptsl.PTSL_pb2 import SAF_AIFF, SAF_WAVE, \
     SR_48000, Bit16, Bit24, Bit32Float, \
     IO_Last, IO_StereoMix, IO_51SMPTEMix
 
 import ptsl
 from ptsl import ops, util
 
 
@@ -54,15 +54,15 @@
 
     def stereo_io_settings(self):
         self._io_settings = IO_StereoMix
 
     def smpte51_io_settings(self):
         self._io_settings = IO_51SMPTEMix
 
-    def interlaved(self, value: bool):
+    def interleaved(self, value: bool):
         self._is_interleaved = value
 
     def create(self) -> None:
         op = ops.CreateSession(
             session_name=self._session_name,
             file_type=self._audio_format,
             sample_rate=self._sample_rate,
```

### Comparing `py_ptsl-101.1.0/ptsl/builders/export_text_builder.py` & `py_ptsl-301.0.0/ptsl/builders/export_text_builder.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/ptsl/builders/import_builder.py` & `py_ptsl-301.0.0/ptsl/builders/import_builder.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/ptsl/client.py` & `py_ptsl-301.0.0/ptsl/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from google.protobuf import json_format
 
 from ptsl import PTSL_pb2_grpc
 from ptsl import PTSL_pb2 as pt
 from ptsl.errors import CommandError
 from ptsl.ops import Operation
 
-PTSL_VERSION = 1
+
+PTSL_VERSION = 3
 
 
 @contextmanager
 def open_client(*args, **kwargs):
     client = Client(*args, **kwargs)
 
     try:
@@ -148,19 +149,20 @@
         # convert the request body into JSON
         request_body_json = self._prepare_operation_request_json(operation)
         response = self._send_sync_request(operation.command_id(),
                                            request_body_json)
         operation.status = response.header.status
 
         if response.header.status == pt.Failed:
-            cleaned_response_error_json = self._response_error_json_cleanup(
-                response.response_error_json)
-            command_error = json_format.Parse(cleaned_response_error_json,
-                                              pt.CommandError())
-            raise CommandError(command_error)
+            cleaned_response_error_json = response.response_error_json
+            # self._response_error_json_cleanup(
+            # response.response_error_json)
+            command_errors = json_format.Parse(cleaned_response_error_json,
+                                               pt.ResponseError())
+            raise CommandError(command_errors.errors)
 
         elif response.header.status == pt.Completed:
             self._handle_completed_response(operation, response)
         else:
             # FIXME: dump out for now, will be on the lookout for when
             # this happens
             assert False, \
@@ -191,25 +193,27 @@
         """
         This is a shim that will take a `command_error_type` value
         from the response error json and convert it into a PT_UnknownError
         if the `command_error_type` value is mis-formatted by the server
         (for instance, if the server returns a symbold name or numeric string
         value, as it sometimes has done in the past. (See `errata`).
         """
-        error_dict = json.loads(json_in)
-        old_val = error_dict['command_error_type']
+
+        errors = json.loads(json_in)
+        error_dict = errors['errors'][0]
+        old_val = errors['errors'][0]['command_error_type']
+
         if isinstance(old_val, str):
             if old_val.isdigit():
                 error_dict['command_error_type'] = int(old_val)
             elif old_val in pt.CommandErrorType.keys():
                 error_dict['command_error_type'] = \
                     pt.CommandErrorType.Value(old_val)
             else:
                 error_dict['command_error_type'] = pt.PT_UnknownError
-
         return json.dumps(error_dict)
 
     def _handle_completed_response(self, operation, response):
         """
         Accept the response message from the server, parse
         the response body JSON if present, and hand the results
         to the operation.
@@ -278,16 +282,18 @@
         This method is called automatically by the initializer.
         """
 
         req = pt.RegisterConnectionRequestBody(
             company_name=company_name,
             application_name=application_name)
 
-        req_json = json_format.MessageToJson(req,
-                                             preserving_proto_field_name=True)
+        req_json = json_format.MessageToJson(
+            req,
+            including_default_value_fields=True,
+            preserving_proto_field_name=True)
 
         response = self._send_sync_request(pt.RegisterConnection,
                                            req_json)
 
         if response.header.status == pt.Failed:
             print("An error occurred")
             print(response)
```

### Comparing `py_ptsl-101.1.0/ptsl/engine.py` & `py_ptsl-301.0.0/ptsl/engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,23 +14,27 @@
     CreateSessionFromAAFBuilder
 from ptsl.builders.export_text_builder import \
     ExportSessionTextBuilder
 from ptsl.builders.import_builder import \
     ImportSessionDataBuilder
 
 import ptsl.PTSL_pb2 as pt
-from ptsl.PTSL_pb2 import SessionAudioFormat, BitDepth,  FileLocation, \
+from ptsl.PTSL_pb2 import SessionAudioFormat, BitDepth, FileLocation, \
     EM_FileType, EM_SourceInfo, EM_AudioInfo, EM_VideoInfo, \
     EM_LocationInfo, EM_DolbyAtmosInfo, TripleBool, SessionTimeCodeRate, \
     SessionFeetFramesRate, SessionRatePull, Track, \
     PM_PlaybackMode, RM_RecordMode, AutomationDataOptions, \
     PasteSpecialOptions, TrackOffsetOptions, TrackListInvertibleFilter, \
     ExportFileType, ResolveDuplicateNamesBy, ExportFormat, \
     MemoryLocationReference, MemoryLocationProperties, \
-    TimeProperties, CL_ClipLocation
+    TimeProperties, CL_ClipLocation, \
+    TrackFormat, TrackType, TrackTimebase, \
+    AudioOperations, MediaDestination, MediaLocation, \
+    SpotLocationType, Start, TimeCode, \
+    TimelineUpdateVideo, SelectionMode
 
 
 @contextmanager
 def open_engine(*args, **kwargs):
     """
     Open a ptsl engine. Engine will close with the context.
     :param company_name: The company name to register.
@@ -112,15 +116,26 @@
         """
         self.client.run(ops.HostReadyCheck())
 
     def create_session(self,
                        name: str,
                        path: str) -> CreateSessionBuilder:
         """
-        Create a new Pro Tools session.
+        Create a new Pro Tools session. Returns a
+        :class:`~ptsl.builders.create_session_builder.CreateSessionBuilder`
+        object used to customize the creation request.
+
+        .. sourcecode:: python
+           :caption: Creating a session with a builder
+
+           b = engine.create_session("My Session", "/Path/to/Session")
+           b.wave_format()
+           b.sample_rate(96000)
+           b.bit_depth(32)
+           b.create() # Session is created
 
         :param str name: Session Name
         :param str path: Path to the new session
         """
         return CreateSessionBuilder(engine=self, name=name, path=path)
 
     def create_session_from_template(
@@ -201,14 +216,43 @@
                     session_path: str
                     ) -> ImportSessionDataBuilder:
         """
         Import session data into the currently-open session.
         """
         return ImportSessionDataBuilder(self, session_path)
 
+    def import_audio(self,
+                     file_list: List[str],
+                     destination_path: Optional[str] = None,
+                     audio_operations: Optional[AudioOperations] = None,
+                     audio_destination: Optional[MediaDestination] = None,
+                     audio_location: Optional[MediaLocation] = None,
+                     timecode: Optional[str] = None,
+                     location_type: Optional[SpotLocationType] = Start,
+                     location_options: Optional[TrackOffsetOptions] = TimeCode
+                     ) -> None:
+        """
+        Import audio data into the currently-open session.
+        location_data needs to be provided regardless if empty.
+        Just a basic implementation for audio data import TC based only.
+        """
+        location_data = pt.SpotLocationData(location_type=location_type,
+                                            location_options=location_options,
+                                            location_value=timecode
+                                            )
+        audio_data = pt.AudioData(file_list=file_list,
+                                  destination_path=destination_path,
+                                  audio_operations=audio_operations,
+                                  audio_destination=audio_destination,
+                                  audio_location=audio_location,
+                                  location_data=location_data
+                                  )
+        op = ops.Import(import_type=1, audio_data=audio_data)
+        self.client.run(op)
+
     def select_all_clips_on_track(self, track_name: str):
         """
         Select all clips on track.
 
         :param str track_name: Name of the track to select all clips on.
         """
         op = ops.SelectAllClipsOnTrack(track_name=track_name)
@@ -308,14 +352,62 @@
 
     def record_half_speed(self):
         """
         Record at half speed.
         """
         self.client.run(ops.RecordHalfSpeed())
 
+    def create_memory_location(
+            self,
+            start_time: Optional[str] = None,
+            memory_number: Optional[int] = None,
+            name: Optional[str] = None,
+            end_time: Optional[str] = None,
+            location: Optional[str] = None,
+            track_name: Optional[str] = None,
+            time_properties:
+            Optional[TimeProperties] = None,
+            reference: Optional[MemoryLocationReference] = None,
+            general_properties: Optional[MemoryLocationProperties] = None,
+            comments: Optional[str] = None,
+            color_index: Optional[int] = None
+    ) -> None:
+        """
+        Create a new memory location.
+        """
+        if general_properties is None:
+            general_properties = MemoryLocationProperties(
+                track_visibility=False)
+        op = ops.CreateMemoryLocation(
+            number=memory_number,
+            name=name,
+            start_time=start_time,
+            end_time=end_time,
+            track_name=track_name,
+            time_properties=time_properties,
+            reference=reference,
+            general_properties=general_properties,
+            comments=comments,
+            location=location,
+            color_index=color_index
+        )
+        self.client.run(op)
+
+    def get_edit_mode(self):
+        """
+        :returns: The current edit mode and options:
+        """
+        op = ops.GetEditMode()
+        self.client.run(op)
+        # mode = op.response.current_setting
+
+        op2 = ops.GetEditModeOptions()
+        self.client.run(op2)
+        # options = op.response.edit_mode_options
+
     def edit_memory_location(self, location_number: int,
                              name: str,
                              start_time: str, end_time: str,
                              time_properties: 'TimeProperties',
                              reference: 'MemoryLocationReference',
                              general_properties: 'MemoryLocationProperties',
                              comments: str):
@@ -409,15 +501,15 @@
             If none, defaults
             to [:attr:`~ptsl.PTSL_pb2.FileLocationTypeFilter.All_Files`]
         :returns: a List of :py:class:`~ptsl.PTSL_pb2.FileLocation`
         """
         if filters is None:
             filters = [pt.All_Files]
         op = ops.GetFileLocation(
-            page_limit=10000,
+            pagination_request=pt.PaginationRequest(limit=1000, offset=0),
             file_filters=filters)
         self.client.run(op)
 
         return op.response.file_locations
 
     def export_mix(
             self,
@@ -607,16 +699,16 @@
             [:attr:`ptsl.PTSL_pb2.TrackListFilter.All`]
         """
         if len(filters) == 0:
             filters = [pt.TrackListInvertibleFilter(filter=pt.All,
                                                     is_inverted=False)]
 
         op = ops.GetTrackList(
-            page_limit=1000,
-            track_filter_list=filters
+            track_filter_list=filters,
+            pagination_request=pt.PaginationRequest(limit=1000, offset=0)
         )
 
         self.client.run(op)
 
         return op.track_list
 
     def set_playback_mode(self, new_mode: 'PM_PlaybackMode'):
@@ -717,14 +809,59 @@
     def set_session_video_rate_pull(self, pull_rate: 'SessionRatePull'):
         """
         Set session video rate pull.
         """
         op = ops.SetSessionVideoRatePullSettings(video_rate_pull=pull_rate)
         self.client.run(op)
 
+    def set_timeline_selection(self,
+                               in_time: Optional[str],
+                               play_start_marker_time: Optional[str] = None,
+                               out_time: Optional[str] = None,
+                               pre_roll_start_time: Optional[str] = None,
+                               post_roll_stop_time: Optional[str] = None,
+                               pre_roll_enabled: Optional[TripleBool] = None,
+                               update_video_to:
+                               Optional[TimelineUpdateVideo] = None,
+                               propagate_to_satellites:
+                               Optional[TripleBool] = None
+                               ):
+        """
+        Set Selection at Timecode
+        """
+        op = ops.SetTimelineSelection(
+            play_start_marker_time=play_start_marker_time,
+            in_time=in_time,
+            out_time=out_time,
+            pre_roll_start_time=pre_roll_start_time,
+            post_roll_stop_time=post_roll_stop_time,
+            pre_roll_enabled=pre_roll_enabled,
+            update_video_to=update_video_to,
+            propagate_to_satellites=propagate_to_satellites
+        )
+        self.client.run(op)
+
+    def create_new_tracks(self,
+                          number_of_tracks: Optional[int] = None,
+                          track_name: Optional[str] = None,
+                          track_format: Optional[TrackFormat] = None,
+                          track_type: Optional[TrackType] = None,
+                          track_timebase: Optional[TrackTimebase] = None
+                          ):
+        """
+        Create new Tracks
+        """
+        op = ops.CreateNewTracks(number_of_tracks=number_of_tracks,
+                                 track_name=track_name,
+                                 track_format=track_format,
+                                 track_type=track_type,
+                                 track_timebase=track_timebase
+                                 )
+        self.client.run(op)
+
     def cut(self, special: Optional['AutomationDataOptions'] = None):
         """
         Execute an Edit > Cut.
         """
         if special is not None:
             op = ops.CutSpecial(automation_data_option=special)
         else:
@@ -770,12 +907,39 @@
         Refresh target audio files.
 
         :param files: A list of files to refresh.
         """
         op = ops.RefreshAllModifiedAudioFiles(file_list=files)
         self.client.run(op)
 
-    def refresh_all_modified_audio_flles(self):
+    def refresh_all_modified_audio_files(self):
         """
         Refreshes all modified audio files.
         """
         self.client.run(ops.RefreshAllModifiedAudioFiles())
+
+    # PT 2023.9
+    # TODO add remaining new methods, add proper docstrings, expose
+    # remaining parameters
+    # CreateNewTracks
+    # GetEditMode, SetEditMode, GetEditModeOptions, SetEditModeOptions
+    # GetEditTool, SetEditTool
+    # RecallZoomPreset
+
+    def select_tracks_by_name(self, names: List[str],
+                              mode: Optional['SelectionMode'] = pt.SM_Replace):
+        """
+        Selects all tracks matching any of the passed names literally.
+        """
+        # TODO: handle pagination request?
+        op = ops.SelectTracksByName(track_names=names, selection_mode=mode)
+        self.client.run(op)
+
+    def get_timeline_selection(self) -> Tuple[str, str]:
+        """
+        Returns data about the current timeline selection.
+        :returns: a Tuple of the In and Out time.
+        """
+        op = ops.GetMemoryLocations()
+        response = self.client.run(op)
+
+        return (response.in_time, response.out_time)
```

### Comparing `py_ptsl-101.1.0/ptsl/errors.py` & `py_ptsl-301.0.0/ptsl/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
 ptsl Exceptions
 """
 
-from typing import Optional
+from typing import Optional, List
 
 from ptsl.PTSL_pb2 import CommandError as CommandErrorResponse
 from ptsl.PTSL_pb2 import CommandErrorType
 
 
 class CommandError(RuntimeError):
     """
     A :class:`Exception` for :class:`CommandError` results
     """
-    error_response: CommandErrorResponse
+    error_responses: List[CommandErrorResponse]
 
-    def __init__(self, error_response: CommandErrorResponse) -> None:
-        self.error_response = error_response
+    def __init__(self, error_responses: List[CommandErrorResponse]) -> None:
+        self.error_responses = error_responses
         super().__init__()
 
     def __str__(self) -> str:
         return super().__str__() + \
             f"ErrType {self.error_type}: {self.error_name} ({self.message})"
 
     @property
     def is_warning(self) -> bool:
         """
         `True` if command error message is marked as a warning.
         """
-        return self.error_response.is_warning
+        return self.error_responses[0].is_warning
 
     @property
     def error_type(self) -> CommandErrorType:
         """
         :class:`ptsl.PTSL_pb2.CommandErrorType` enumeration value.
         """
-        return self.error_response.command_error_type
+        return self.error_responses[0].command_error_type
 
     @property
     def error_name(self) -> Optional[str]:
         """
         Error name, if available.
         """
         if self.error_type in CommandErrorType.values():
@@ -47,8 +47,8 @@
         return None
 
     @property
     def message(self) -> str:
         """
         Error message as returned by the client.
         """
-        return self.error_response.command_error_message
+        return self.error_responses[0].command_error_message
```

### Comparing `py_ptsl-101.1.0/ptsl/ops/__init__.py` & `py_ptsl-301.0.0/ptsl/ops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,28 @@
 from .set_session_interleaved_state import SetSessionInterleavedState
 from .set_session_length import SetSessionLength
 from .set_session_start_time import SetSessionStartTime
 from .set_session_time_code_rate import SetSessionTimeCodeRate
 from .set_session_video_rate_pull_settings import \
     SetSessionVideoRatePullSettings
 
+
 # Pro Tools 2023.3
 
 from .register_connection import RegisterConnection
 from .rename_selected_clip import RenameSelectedClip
 from .rename_target_clip import RenameTargetClip
 from .toggle_play_state import \
     TogglePlayState, ToggleRecordEnable, \
     PlayHalfSpeed, RecordHalfSpeed
 
 from .memory_locations import EditMemoryLocation, GetMemoryLocations
+
+# Pro Tools 2023.9
+
+from .create_new_tracks import CreateNewTracks
+from .select_tracks import SelectTracksByName
+from .edit_mode import GetEditMode, SetEditMode, GetEditModeOptions, \
+        SetEditModeOptions
+from .edit_tool import GetEditTool, SetEditTool
+from .zoom_preset import RecallZoomPreset
+from .timeline_selection import SetTimelineSelection, GetTimelineSelection
```

### Comparing `py_ptsl-101.1.0/ptsl/ops/get_playback_mode.py` & `py_ptsl-301.0.0/ptsl/ops/get_playback_mode.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/ptsl/ops/get_session_interleaved_state.py` & `py_ptsl-301.0.0/ptsl/ops/get_session_interleaved_state.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/ptsl/ops/get_session_sample_rate.py` & `py_ptsl-301.0.0/ptsl/ops/get_session_sample_rate.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/ptsl/ops/get_track_list.py` & `py_ptsl-301.0.0/ptsl/ops/get_track_list.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/ptsl/ops/operation.py` & `py_ptsl-301.0.0/ptsl/ops/operation.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/ptsl/util.py` & `py_ptsl-301.0.0/ptsl/util.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.1.0/pyproject.toml` & `py_ptsl-301.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dynamic = ["version", "description"]
 license = {file = 'LICENSE'}
 requires-python = "~=3.8"
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
   "Topic :: Software Development :: Libraries :: Python Modules",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.8",
   "Topic :: Multimedia :: Sound/Audio :: Editors",
 ]
 keywords = [
@@ -24,15 +25,15 @@
   "scripting", 
   "grpc", 
   "automation", 
   "avid"
 ]
 dependencies = [
     'grpcio >= 1.51.1', 
-    'protobuf >= 4.21.12'
+    'protobuf == 4.25.3'
 ]
 
 [tool.flit.module]
 name = "ptsl"
 
 [project.optional-dependencies]
 doc = [
```

### Comparing `py_ptsl-101.1.0/PKG-INFO` & `py_ptsl-301.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: py-ptsl
-Version: 101.1.0
+Version: 301.0.0
 Summary: Native Python PTSL (Pro Tools Scripting Library) RPC interface
 Keywords: pro tools,scripting,grpc,automation,avid
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
 Requires-Dist: grpcio >= 1.51.1
-Requires-Dist: protobuf >= 4.21.12
+Requires-Dist: protobuf == 4.25.3
 Requires-Dist: grpcio-tools >= 1.53.0 ; extra == "dev"
 Requires-Dist: sphinx >= 5.3.0 ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme >= 1.1.1 ; extra == "doc"
 Project-URL: Documentation, https://py-ptsl.readthedocs.io
 Project-URL: Home, https://github.com/iluvcapra/py-ptsl
 Project-URL: Source, https://github.com/iluvcapra/py-ptsl
 Project-URL: Tracker, https://github.com/iluvcapra/py-ptsl/issues
@@ -29,16 +30,16 @@
 [![Lint and Test](https://github.com/iluvcapra/py-ptsl/actions/workflows/lint_and_pytest.yml/badge.svg)](https://github.com/iluvcapra/py-ptsl/actions/workflows/lint_and_pytest.yml)
 [![codecov](https://codecov.io/gh/iluvcapra/py-ptsl/branch/master/graph/badge.svg?token=PR6SUQJISZ)](https://codecov.io/gh/iluvcapra/py-ptsl)
 [![Documentation Status](https://readthedocs.org/projects/py-ptsl/badge/?version=latest)](https://py-ptsl.readthedocs.io/en/latest/?badge=latest)
 ![GitHub last commit](https://img.shields.io/github/last-commit/iluvcapra/py-ptsl)
 
 ![](https://img.shields.io/pypi/pyversions/py-ptsl.svg) [![](https://img.shields.io/pypi/v/py-ptsl.svg)](https://pypi.org/project/py-ptsl/) ![](https://img.shields.io/pypi/wheel/py-ptsl.svg)
 
-[![Pro Tools Version - 2023.6](https://img.shields.io/static/v1?label=Pro+Tools+Version&message=2023.6&color=8f228f)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
-[![PTSL Version - 1](https://img.shields.io/static/v1?label=PTSL+Version&message=1&color=0000ff)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
+[![Pro Tools Version - 2023.9](https://img.shields.io/static/v1?label=Pro+Tools+Version&message=2023.9&color=8f228f)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
+[![PTSL Version - 3](https://img.shields.io/static/v1?label=PTSL+Version&message=3&color=0000ff)](https://github.com/iluvcapra/py-ptsl/blob/master/docs/source/ptsl_versions.rst)
 
 # py-ptsl
 
 Native Python PTSL (Pro Tools Scripting Library) RPC interface
 
 ## Important Notice! 
 
@@ -55,22 +56,27 @@
 - [session_info.py](examples/session_info.py) - This example 
   prints a list of gettable properties from the currently-open
       session.
 - [print_tracks.py](examples/print_tracks.py) - This example prints
   a list of every track in the currently-open session, including state
   information like selection, mute and solo state, track color and 
   track ID.
+- [make_session.py](examples/make_session.py) - Creates a new
+  session interactively from the terminal.
+- [pt_set.py](examples/pt_set.py) - Allows several session setup
+  options to be set from the terminal.
+- [pt_pasteboard.py](examples/pt_pasteboard.py) - Demonstrates
+  triggering cut/copy/paste actions.
 
 
 ### Sending Commands To Pro Tools with the `Engine` class
 
 The `Engine` class exposes `ptsl` commands with a method call interface.
 
 ```python
 from ptsl import open_engine
 
 with open_engine(company_name="MY_COMPANY", application_name="MY_TOOL") as engine:
     session_name = engine.session_name()
-
 ```
```


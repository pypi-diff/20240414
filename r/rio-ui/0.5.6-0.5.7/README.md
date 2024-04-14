# Comparing `tmp/rio_ui-0.5.6.tar.gz` & `tmp/rio_ui-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio_ui-0.5.6.tar", max compression
+gzip compressed data, was "rio_ui-0.5.7.tar", max compression
```

## Comparing `rio_ui-0.5.6.tar` & `rio_ui-0.5.7.tar`

### file list

```diff
@@ -1,206 +1,216 @@
--rw-r--r--   0        0        0    35149 2024-04-06 18:09:28.058340 rio_ui-0.5.6/LICENSE.txt
--rw-r--r--   0        0        0     5057 2024-04-12 20:47:24.408950 rio_ui-0.5.6/README.md
--rw-r--r--   0        0        0     2441 2024-04-13 19:41:02.000187 rio_ui-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      676 2024-04-08 18:37:44.149116 rio_ui-0.5.6/rio/__init__.py
--rw-r--r--   0        0        0       91 2024-04-06 18:09:28.078340 rio_ui-0.5.6/rio/__main__.py
--rw-r--r--   0        0        0    19313 2024-04-09 19:38:54.555684 rio_ui-0.5.6/rio/app.py
--rw-r--r--   0        0        0    32013 2024-04-12 12:19:28.616661 rio_ui-0.5.6/rio/app_server.py
--rw-r--r--   0        0        0      233 2024-04-06 18:09:28.081673 rio_ui-0.5.6/rio/assets/hosted/README.md
--rw-r--r--   0        0        0   557380 2024-04-06 18:09:28.088340 rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
--rw-r--r--   0        0        0   401608 2024-04-06 18:09:28.091673 rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
--rw-r--r--   0        0        0   403724 2024-04-06 18:09:28.095007 rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
--rw-r--r--   0        0        0   556216 2024-04-06 18:09:28.098340 rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
--rw-r--r--   0        0        0     4449 2024-04-06 18:09:28.098340 rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/OFL.txt
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.101673 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2024-04-06 18:09:28.101673 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2024-04-06 18:09:28.105007 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2024-04-06 18:09:28.105007 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2024-04-06 18:09:28.105007 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.098340 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2024-04-06 18:09:28.098340 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2024-04-06 18:09:28.101673 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2024-04-06 18:09:28.101673 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2024-04-06 18:09:28.101673 rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0    54189 2024-04-08 17:00:05.405088 rio_ui-0.5.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2024-04-06 18:09:28.105007 rio_ui-0.5.6/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081400 2024-04-07 20:27:02.369218 rio_ui-0.5.6/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    15424 2024-04-07 21:06:13.848440 rio_ui-0.5.6/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     8798 2024-04-12 12:19:28.613327 rio_ui-0.5.6/rio/assets.py
--rw-r--r--   0        0        0     3316 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/byte_serving.py
--rw-r--r--   0        0        0     7389 2024-04-10 21:00:39.348528 rio_ui-0.5.6/rio/cli/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6642 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    13832 2024-04-12 10:18:09.239288 rio_ui-0.5.6/rio/cli/project.py
--rw-r--r--   0        0        0    12661 2024-04-12 12:19:28.613327 rio_ui-0.5.6/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4172 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/cli/rioignore.py
--rw-r--r--   0        0        0      107 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5404 2024-04-08 16:50:31.798904 rio_ui-0.5.6/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    20827 2024-04-12 12:19:28.613327 rio_ui-0.5.6/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      423 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     3828 2024-04-12 10:18:09.239288 rio_ui-0.5.6/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     3982 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0    19604 2024-04-09 19:38:54.559018 rio_ui-0.5.6/rio/color.py
--rw-r--r--   0        0        0     7924 2024-04-12 12:19:28.613327 rio_ui-0.5.6/rio/common.py
--rw-r--r--   0        0        0     1552 2024-04-10 18:34:30.899371 rio_ui-0.5.6/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2024-04-12 12:17:57.040111 rio_ui-0.5.6/rio/components/app_root.py
--rw-r--r--   0        0        0     4055 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/components/auto_form.py
--rw-r--r--   0        0        0     4751 2024-04-09 19:38:54.559018 rio_ui-0.5.6/rio/components/banner.py
--rw-r--r--   0        0        0      889 2024-04-07 08:57:25.524848 rio_ui-0.5.6/rio/components/build_failed.py
--rw-r--r--   0        0        0    13570 2024-04-12 20:47:24.392283 rio_ui-0.5.6/rio/components/button.py
--rw-r--r--   0        0        0     5064 2024-04-09 19:38:54.559018 rio_ui-0.5.6/rio/components/card.py
--rw-r--r--   0        0        0     1025 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/components/class_container.py
--rw-r--r--   0        0        0      352 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/components/code_explorer.py
--rw-r--r--   0        0        0     3745 2024-04-09 19:38:54.559018 rio_ui-0.5.6/rio/components/color_picker.py
--rw-r--r--   0        0        0    26039 2024-04-12 12:19:28.613327 rio_ui-0.5.6/rio/components/component.py
--rw-r--r--   0        0        0     1029 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/components/component_tree.py
--rw-r--r--   0        0        0     1225 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/container.py
--rw-r--r--   0        0        0      215 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4067 2024-04-06 18:09:28.108340 rio_ui-0.5.6/rio/components/devel_component.py
--rw-r--r--   0        0        0     3889 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/drawer.py
--rw-r--r--   0        0        0     6670 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/dropdown.py
--rw-r--r--   0        0        0     2922 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/flow_container.py
--rw-r--r--   0        0        0     5867 2024-04-10 17:00:38.844482 rio_ui-0.5.6/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7057 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/grid.py
--rw-r--r--   0        0        0      604 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/html.py
--rw-r--r--   0        0        0     7782 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/icon.py
--rw-r--r--   0        0        0     3676 2024-04-09 19:38:54.562351 rio_ui-0.5.6/rio/components/image.py
--rw-r--r--   0        0        0    13127 2024-04-09 19:38:54.565684 rio_ui-0.5.6/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     2981 2024-04-12 12:17:57.116777 rio_ui-0.5.6/rio/components/labeled_column.py
--rw-r--r--   0        0        0     8968 2024-04-09 19:38:54.585684 rio_ui-0.5.6/rio/components/linear_containers.py
--rw-r--r--   0        0        0     4478 2024-04-09 19:38:54.565684 rio_ui-0.5.6/rio/components/link.py
--rw-r--r--   0        0        0    10184 2024-04-12 12:17:57.146777 rio_ui-0.5.6/rio/components/list_items.py
--rw-r--r--   0        0        0     3527 2024-04-09 19:38:54.565684 rio_ui-0.5.6/rio/components/list_view.py
--rw-r--r--   0        0        0     1389 2024-04-09 19:38:54.565684 rio_ui-0.5.6/rio/components/markdown.py
--rw-r--r--   0        0        0     4917 2024-04-09 19:38:54.565684 rio_ui-0.5.6/rio/components/media_player.py
--rw-r--r--   0        0        0     6919 2024-04-09 19:38:54.565684 rio_ui-0.5.6/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5165 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1422 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/node_input.py
--rw-r--r--   0        0        0     1426 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/node_output.py
--rw-r--r--   0        0        0     8478 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/number_input.py
--rw-r--r--   0        0        0     2190 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/overlay.py
--rw-r--r--   0        0        0     5060 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/page_view.py
--rw-r--r--   0        0        0     4959 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/plot.py
--rw-r--r--   0        0        0     3280 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/popup.py
--rw-r--r--   0        0        0      975 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3560 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/progress_circle.py
--rw-r--r--   0        0        0     4106 2024-04-09 19:38:54.569018 rio_ui-0.5.6/rio/components/rectangle.py
--rw-r--r--   0        0        0     3688 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/revealer.py
--rw-r--r--   0        0        0     1857 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/components/root_components.py
--rw-r--r--   0        0        0     1889 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1213 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1114 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/separator.py
--rw-r--r--   0        0        0     6120 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/slider.py
--rw-r--r--   0        0        0     3649 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/slideshow.py
--rw-r--r--   0        0        0     1442 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/spacer.py
--rw-r--r--   0        0        0     2762 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/stack.py
--rw-r--r--   0        0        0     3154 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/switch.py
--rw-r--r--   0        0        0      879 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/switcher.py
--rw-r--r--   0        0        0     9237 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2305 2024-04-09 19:38:54.572351 rio_ui-0.5.6/rio/components/table.py
--rw-r--r--   0        0        0     2018 2024-04-09 19:38:54.575684 rio_ui-0.5.6/rio/components/text.py
--rw-r--r--   0        0        0     5380 2024-04-09 19:38:54.575684 rio_ui-0.5.6/rio/components/text_input.py
--rw-r--r--   0        0        0     1231 2024-04-09 19:38:54.575684 rio_ui-0.5.6/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     2861 2024-04-09 19:38:54.575684 rio_ui-0.5.6/rio/components/tooltip.py
--rw-r--r--   0        0        0      633 2024-04-09 19:38:54.575684 rio_ui-0.5.6/rio/components/website.py
--rw-r--r--   0        0        0      123 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/cursor_style.py
--rw-r--r--   0        0        0     5840 2024-04-08 18:37:44.152450 rio_ui-0.5.6/rio/dataclass.py
--rw-r--r--   0        0        0       53 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/debug/__init__.py
--rw-r--r--   0        0        0       41 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/debug/client_side_debugger/__init__.py
--rw-r--r--   0        0        0    10108 2024-04-12 12:17:57.300110 rio_ui-0.5.6/rio/debug/client_side_debugger/component_details.py
--rw-r--r--   0        0        0     3634 2024-04-12 12:19:28.609994 rio_ui-0.5.6/rio/debug/client_side_debugger/debugger.py
--rw-r--r--   0        0        0      795 2024-04-12 12:17:57.210110 rio_ui-0.5.6/rio/debug/client_side_debugger/deploy_page.py
--rw-r--r--   0        0        0      782 2024-04-12 12:17:57.210110 rio_ui-0.5.6/rio/debug/client_side_debugger/docs_page.py
--rw-r--r--   0        0        0    12359 2024-04-12 12:17:57.423443 rio_ui-0.5.6/rio/debug/client_side_debugger/icons_page.py
--rw-r--r--   0        0        0     2379 2024-04-12 12:17:57.236777 rio_ui-0.5.6/rio/debug/client_side_debugger/project_page.py
--rw-r--r--   0        0        0     2265 2024-04-08 18:37:44.155783 rio_ui-0.5.6/rio/debug/client_side_debugger/sample_icons_grid.py
--rw-r--r--   0        0        0    16597 2024-04-12 12:17:57.400110 rio_ui-0.5.6/rio/debug/client_side_debugger/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2024-04-10 18:34:30.899371 rio_ui-0.5.6/rio/debug/client_side_debugger/tree_page.py
--rw-r--r--   0        0        0     7224 2024-04-08 18:37:44.155783 rio_ui-0.5.6/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/debug/stress_client/__init__.py
--rw-r--r--   0        0        0      666 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/debug/stress_client/stress_client.py
--rw-r--r--   0        0        0      567 2024-04-08 18:37:44.155783 rio_ui-0.5.6/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14210 2024-04-12 12:19:28.613327 rio_ui-0.5.6/rio/debug/validator.py
--rw-r--r--   0        0        0       52 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/docs/__init__.py
--rw-r--r--   0        0        0     4867 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/docs/custom.py
--rw-r--r--   0        0        0     1124 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/docs/models.py
--rw-r--r--   0        0        0    14587 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/docs/parsers.py
--rw-r--r--   0        0        0      960 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/errors.py
--rw-r--r--   0        0        0     3173 2024-04-08 18:37:44.155783 rio_ui-0.5.6/rio/event.py
--rw-r--r--   0        0        0     6732 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/fills.py
--rw-r--r--   0        0        0   529227 2024-04-13 19:40:56.943532 rio_ui-0.5.6/rio/generated/index.html
--rw-r--r--   0        0        0      897 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/global_state.py
--rw-r--r--   0        0        0     9940 2024-04-07 11:32:34.208243 rio_ui-0.5.6/rio/icon_registry.py
--rw-r--r--   0        0        0     3500 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/inspection.py
--rw-r--r--   0        0        0     3625 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/maybes.py
--rw-r--r--   0        0        0     1577 2024-04-12 20:47:24.392283 rio_ui-0.5.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2024-04-12 20:47:24.392283 rio_ui-0.5.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      283 2024-04-13 19:40:36.493590 rio_ui-0.5.6/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     7380 2024-04-09 19:38:54.575684 rio_ui-0.5.6/rio/routing.py
--rw-r--r--   0        0        0      417 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/self_serializing.py
--rw-r--r--   0        0        0     8463 2024-04-06 18:09:28.111674 rio_ui-0.5.6/rio/serialization.py
--rw-r--r--   0        0        0    76913 2024-04-12 20:47:24.392283 rio_ui-0.5.6/rio/session.py
--rw-r--r--   0        0        0     1395 2024-04-06 18:09:28.115007 rio_ui-0.5.6/rio/snippets/README.md
--rw-r--r--   0        0        0    12287 2024-04-12 10:18:09.239288 rio_ui-0.5.6/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-09 16:47:56.822558 rio_ui-0.5.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2024-04-06 18:08:52.814883 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0      851 2024-04-10 17:01:52.454442 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py
--rw-r--r--   0        0        0      223 2024-04-07 08:57:25.591515 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1833 2024-04-08 18:37:44.155783 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2024-04-08 18:37:44.155783 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2024-04-08 18:37:44.155783 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2024-04-08 18:37:44.159116 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0     2227 2024-04-07 09:24:53.378316 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      184 2024-04-07 18:38:03.958535 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0       32 2024-04-06 18:08:52.818216 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2024-04-10 17:01:52.457775 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:08:52.814883 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0        0 2024-04-07 08:44:19.156096 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Empty/__init__.py
--rw-r--r--   0        0        0       98 2024-04-07 08:04:03.043617 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      504 2024-04-12 10:18:09.242621 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:09:28.115007 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0      714 2024-04-12 10:18:09.225955 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0        0 2024-04-10 16:49:08.284483 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/__init__.py
--rw-r--r--   0        0        0       68 2024-04-10 16:49:08.284483 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     4814 2024-04-12 10:18:09.225955 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     4139 2024-04-12 10:18:09.225955 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0     1685 2024-04-12 10:18:09.225955 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       55 2024-04-10 18:59:11.048460 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0       32 2024-04-10 16:49:08.284483 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     6618 2024-04-12 10:18:09.225955 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0     3586 2024-04-10 16:49:08.284483 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0      490 2024-04-08 13:25:22.132597 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0        0 2024-04-08 13:21:28.592126 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/__init__.py
--rw-r--r--   0        0        0       34 2024-04-12 12:20:05.616618 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2024-04-12 12:19:28.609994 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       92 2024-04-08 13:26:20.426025 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0       44 2024-04-08 15:32:19.997165 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4659 2024-04-12 12:19:28.593327 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     3344 2024-04-08 13:24:10.679136 rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-12 20:47:24.408950 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.412283 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4328 2024-04-12 20:47:24.412283 rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     8134 2024-04-08 18:37:44.159116 rio_ui-0.5.6/rio/state_properties.py
--rw-r--r--   0        0        0     3077 2024-04-06 18:09:28.115007 rio_ui-0.5.6/rio/text_style.py
--rw-r--r--   0        0        0    19432 2024-04-09 19:38:54.575684 rio_ui-0.5.6/rio/theme.py
--rw-r--r--   0        0        0     5167 2024-04-06 18:09:28.115007 rio_ui-0.5.6/rio/user_settings_module.py
--rw-r--r--   0        0        0     3890 2024-04-06 18:09:28.115007 rio_ui-0.5.6/rio/world_units.py
--rw-r--r--   0        0        0     7614 1970-01-01 00:00:00.000000 rio_ui-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-06 18:09:28.058340 rio_ui-0.5.7/LICENSE.txt
+-rw-r--r--   0        0        0     7217 2024-04-14 14:22:40.210263 rio_ui-0.5.7/README.md
+-rw-r--r--   0        0        0     2441 2024-04-14 19:53:24.034814 rio_ui-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      676 2024-04-08 18:37:44.149116 rio_ui-0.5.7/rio/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-06 18:09:28.078340 rio_ui-0.5.7/rio/__main__.py
+-rw-r--r--   0        0        0    19313 2024-04-09 19:38:54.555684 rio_ui-0.5.7/rio/app.py
+-rw-r--r--   0        0        0    32065 2024-04-14 19:29:03.548737 rio_ui-0.5.7/rio/app_server.py
+-rw-r--r--   0        0        0      233 2024-04-06 18:09:28.081673 rio_ui-0.5.7/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0   557380 2024-04-06 18:09:28.088340 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
+-rw-r--r--   0        0        0   401608 2024-04-06 18:09:28.091673 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
+-rw-r--r--   0        0        0   403724 2024-04-06 18:09:28.095007 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
+-rw-r--r--   0        0        0   556216 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
+-rw-r--r--   0        0        0     4449 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/OFL.txt
+-rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0    54189 2024-04-08 17:00:05.405088 rio_ui-0.5.7/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081400 2024-04-07 20:27:02.369218 rio_ui-0.5.7/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2024-04-14 09:27:29.097282 rio_ui-0.5.7/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     8798 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/assets.py
+-rw-r--r--   0        0        0     3316 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/byte_serving.py
+-rw-r--r--   0        0        0     7389 2024-04-10 21:00:39.348528 rio_ui-0.5.7/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6642 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    13832 2024-04-12 10:18:09.239288 rio_ui-0.5.7/rio/cli/project.py
+-rw-r--r--   0        0        0    12661 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4172 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/rioignore.py
+-rw-r--r--   0        0        0       40 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5404 2024-04-08 16:50:31.798904 rio_ui-0.5.7/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    20827 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      423 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     3828 2024-04-12 10:18:09.239288 rio_ui-0.5.7/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     3982 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0    19604 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/color.py
+-rw-r--r--   0        0        0     7924 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/common.py
+-rw-r--r--   0        0        0     1552 2024-04-10 18:34:30.899371 rio_ui-0.5.7/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2024-04-12 12:17:57.040111 rio_ui-0.5.7/rio/components/app_root.py
+-rw-r--r--   0        0        0     4055 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4751 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/components/banner.py
+-rw-r--r--   0        0        0      889 2024-04-07 08:57:25.524848 rio_ui-0.5.7/rio/components/build_failed.py
+-rw-r--r--   0        0        0    13570 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/components/button.py
+-rw-r--r--   0        0        0     5064 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/components/card.py
+-rw-r--r--   0        0        0     1025 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/class_container.py
+-rw-r--r--   0        0        0      352 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     3745 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26039 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/components/component.py
+-rw-r--r--   0        0        0     1029 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1225 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/container.py
+-rw-r--r--   0        0        0      215 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4067 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/devel_component.py
+-rw-r--r--   0        0        0     3889 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/drawer.py
+-rw-r--r--   0        0        0     6670 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/dropdown.py
+-rw-r--r--   0        0        0     2922 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/flow_container.py
+-rw-r--r--   0        0        0     5867 2024-04-10 17:00:38.844482 rio_ui-0.5.7/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7057 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/grid.py
+-rw-r--r--   0        0        0      604 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/html.py
+-rw-r--r--   0        0        0     7782 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/icon.py
+-rw-r--r--   0        0        0     3676 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/image.py
+-rw-r--r--   0        0        0    13127 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     2981 2024-04-12 12:17:57.116777 rio_ui-0.5.7/rio/components/labeled_column.py
+-rw-r--r--   0        0        0     8968 2024-04-09 19:38:54.585684 rio_ui-0.5.7/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     4478 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/link.py
+-rw-r--r--   0        0        0    10184 2024-04-12 12:17:57.146777 rio_ui-0.5.7/rio/components/list_items.py
+-rw-r--r--   0        0        0     3527 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/list_view.py
+-rw-r--r--   0        0        0     1389 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/markdown.py
+-rw-r--r--   0        0        0     4917 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/media_player.py
+-rw-r--r--   0        0        0     6919 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5165 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1422 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/node_input.py
+-rw-r--r--   0        0        0     1426 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/node_output.py
+-rw-r--r--   0        0        0     8478 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/number_input.py
+-rw-r--r--   0        0        0     2190 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/overlay.py
+-rw-r--r--   0        0        0     5060 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/page_view.py
+-rw-r--r--   0        0        0     4959 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/plot.py
+-rw-r--r--   0        0        0     3280 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/popup.py
+-rw-r--r--   0        0        0      975 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3560 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     4106 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/rectangle.py
+-rw-r--r--   0        0        0     3688 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/revealer.py
+-rw-r--r--   0        0        0     1857 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/components/root_components.py
+-rw-r--r--   0        0        0     1889 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1213 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1114 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/separator.py
+-rw-r--r--   0        0        0     6120 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/slider.py
+-rw-r--r--   0        0        0     3649 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1442 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/spacer.py
+-rw-r--r--   0        0        0     2762 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/stack.py
+-rw-r--r--   0        0        0     3154 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/switch.py
+-rw-r--r--   0        0        0      879 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/switcher.py
+-rw-r--r--   0        0        0     9237 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2305 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/table.py
+-rw-r--r--   0        0        0     2018 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/text.py
+-rw-r--r--   0        0        0     5380 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/text_input.py
+-rw-r--r--   0        0        0     1231 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     2861 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/tooltip.py
+-rw-r--r--   0        0        0      633 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/website.py
+-rw-r--r--   0        0        0      123 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cursor_style.py
+-rw-r--r--   0        0        0     5840 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/dataclass.py
+-rw-r--r--   0        0        0       53 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/debug/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/debug/client_side_debugger/__init__.py
+-rw-r--r--   0        0        0    10452 2024-04-14 09:27:29.090615 rio_ui-0.5.7/rio/debug/client_side_debugger/component_details.py
+-rw-r--r--   0        0        0     3729 2024-04-14 09:27:29.090615 rio_ui-0.5.7/rio/debug/client_side_debugger/debugger.py
+-rw-r--r--   0        0        0      795 2024-04-12 12:17:57.210110 rio_ui-0.5.7/rio/debug/client_side_debugger/deploy_page.py
+-rw-r--r--   0        0        0      782 2024-04-12 12:17:57.210110 rio_ui-0.5.7/rio/debug/client_side_debugger/docs_page.py
+-rw-r--r--   0        0        0    12359 2024-04-12 12:17:57.423443 rio_ui-0.5.7/rio/debug/client_side_debugger/icons_page.py
+-rw-r--r--   0        0        0     2379 2024-04-12 12:17:57.236777 rio_ui-0.5.7/rio/debug/client_side_debugger/project_page.py
+-rw-r--r--   0        0        0     2265 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/debug/client_side_debugger/sample_icons_grid.py
+-rw-r--r--   0        0        0    16597 2024-04-12 12:17:57.400110 rio_ui-0.5.7/rio/debug/client_side_debugger/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2024-04-10 18:34:30.899371 rio_ui-0.5.7/rio/debug/client_side_debugger/tree_page.py
+-rw-r--r--   0        0        0     7224 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14210 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/debug/validator.py
+-rw-r--r--   0        0        0       53 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/docs/__init__.py
+-rw-r--r--   0        0        0     4867 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/docs/custom.py
+-rw-r--r--   0        0        0     1124 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/docs/models.py
+-rw-r--r--   0        0        0    14587 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/docs/parsers.py
+-rw-r--r--   0        0        0      960 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/errors.py
+-rw-r--r--   0        0        0     3173 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/event.py
+-rw-r--r--   0        0        0     6732 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/fills.py
+-rw-r--r--   0        0        0   943434 2024-04-14 14:22:51.470276 rio_ui-0.5.7/rio/generated/index.html
+-rw-r--r--   0        0        0      897 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/global_state.py
+-rw-r--r--   0        0        0     9940 2024-04-07 11:32:34.208243 rio_ui-0.5.7/rio/icon_registry.py
+-rw-r--r--   0        0        0     3500 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/inspection.py
+-rw-r--r--   0        0        0     3625 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/maybes.py
+-rw-r--r--   0        0        0     1577 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      283 2024-04-13 19:40:36.493590 rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     7380 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/routing.py
+-rw-r--r--   0        0        0      417 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/self_serializing.py
+-rw-r--r--   0        0        0     8463 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/serialization.py
+-rw-r--r--   0        0        0    76913 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/session.py
+-rw-r--r--   0        0        0     1395 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/README.md
+-rw-r--r--   0        0        0    12317 2024-04-14 11:20:42.330273 rio_ui-0.5.7/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-09 16:47:56.822558 rio_ui-0.5.7/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0      684 2024-04-06 18:08:52.814883 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0      863 2024-04-14 06:35:30.859117 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2024-04-13 20:00:32.294184 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2024-04-08 18:37:44.159116 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0     2227 2024-04-07 09:24:53.378316 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      184 2024-04-07 18:38:03.958535 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0       44 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2024-04-10 17:01:52.457775 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0     3344 2024-04-06 18:08:52.814883 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0        0 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/__init__.py
+-rw-r--r--   0        0        0     7595 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0     6866 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     4602 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     3359 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0      628 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      226 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0       59 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     6789 2024-04-14 18:51:40.939394 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0     3586 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 08:44:19.156096 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/__init__.py
+-rw-r--r--   0        0        0       98 2024-04-07 08:04:03.043617 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      504 2024-04-12 10:18:09.242621 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0     3344 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0      714 2024-04-12 10:18:09.225955 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 16:49:08.284483 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     4821 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     4139 2024-04-12 10:18:09.225955 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0     1685 2024-04-12 10:18:09.225955 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       55 2024-04-10 18:59:11.048460 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0       44 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     6969 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0     3586 2024-04-10 16:49:08.284483 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0      490 2024-04-08 13:25:22.132597 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 13:21:28.592126 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-12 12:20:05.616618 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2024-04-12 12:19:28.609994 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       92 2024-04-08 13:26:20.426025 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0       61 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4659 2024-04-12 12:19:28.593327 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     3344 2024-04-08 13:24:10.679136 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.412283 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4328 2024-04-12 20:47:24.412283 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     8134 2024-04-08 18:37:44.159116 rio_ui-0.5.7/rio/state_properties.py
+-rw-r--r--   0        0        0     3077 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/text_style.py
+-rw-r--r--   0        0        0    19432 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/theme.py
+-rw-r--r--   0        0        0     5167 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/user_settings_module.py
+-rw-r--r--   0        0        0     3890 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/world_units.py
+-rw-r--r--   0        0        0     9774 1970-01-01 00:00:00.000000 rio_ui-0.5.7/PKG-INFO
```

### Comparing `rio_ui-0.5.6/LICENSE.txt` & `rio_ui-0.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/pyproject.toml` & `rio_ui-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 license = "LGPL-3.0" # TODO
 name = "rio-ui"
-version = "0.5.6"
+version = "0.5.7"
 description = "Build modern Websites and Apps just with Python"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>", "Paul Pinterits"]
 readme = "README.md"
 packages = [{ include = "rio" }]
 include = ["rio/generated/index.html"]
 keywords = [
     "web-development",
```

### Comparing `rio_ui-0.5.6/rio/__init__.py` & `rio_ui-0.5.7/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/app.py` & `rio_ui-0.5.7/rio/app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/app_server.py` & `rio_ui-0.5.7/rio/app_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,17 +141,18 @@
         validator_factory: Callable[[rio.Session], debug.Validator] | None,
         internal_on_app_start: Callable[[], None] | None,
     ):
         super().__init__(
             title=app_.name,
             # summary=...,
             # description=...,
-            openapi_url="/openapi.json" if debug_mode else None,
-            docs_url="/docs" if debug_mode else None,
-            redoc_url="/redoc" if debug_mode else None,
+            openapi_url=None,
+            # openapi_url="/openapi.json" if debug_mode else None,
+            # docs_url="/docs" if debug_mode else None,
+            # redoc_url="/redoc" if debug_mode else None,
             lifespan=__class__._lifespan,
         )
 
         self.app = app_
         self.debug_mode = debug_mode
         self.running_in_window = running_in_window
         self.validator_factory = validator_factory
@@ -853,30 +854,30 @@
 
         # Run any page guards for the initial page
         #
         # Guards have access to the session. Thus, it should be fully
         # initialized, or at least pretend to be. Fill in any not yet final
         # values with placeholders.
         sess._base_url = (
-            URL(initial_message.website_url)
+            URL(initial_message.website_url.lower())
             .with_path("")
             .with_query("")
             .with_fragment("")
         )
         sess._active_page_url = sess._base_url
         sess._active_page_instances = tuple()
 
         # Then, run the guards
         try:
             (
                 active_page_instances,
                 active_page_url_absolute,
             ) = routing.check_page_guards(
                 sess,
-                sess._base_url.join(rio.URL(initial_message.website_url)),
+                sess._base_url.join(rio.URL(initial_message.website_url.lower())),
             )
         except routing.NavigationFailed:
             # TODO: Notify the client? Show an error?
             raise fastapi.HTTPException(
                 status_code=fastapi.status.HTTP_500_INTERNAL_SERVER_ERROR,
                 detail=f'Navigation to initial page "{sess._active_page_url}" has failed.',
             ) from None
```

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Noto Sans/OFL.txt` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/LICENSE.txt` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.5.7/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.5.7/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.5.7/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.5.7/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/assets.py` & `rio_ui-0.5.7/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/byte_serving.py` & `rio_ui-0.5.7/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/__init__.py` & `rio_ui-0.5.7/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/cli_instance.py` & `rio_ui-0.5.7/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/nice_traceback.py` & `rio_ui-0.5.7/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/project.py` & `rio_ui-0.5.7/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/project_setup.py` & `rio_ui-0.5.7/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/rio_api.py` & `rio_ui-0.5.7/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/rioignore.py` & `rio_ui-0.5.7/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/run_project/app_loading.py` & `rio_ui-0.5.7/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/run_project/arbiter.py` & `rio_ui-0.5.7/rio/cli/run_project/arbiter.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.5.7/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.5.7/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/run_project/webview_worker.py` & `rio_ui-0.5.7/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/cli/tomlconfig.py` & `rio_ui-0.5.7/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/color.py` & `rio_ui-0.5.7/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/common.py` & `rio_ui-0.5.7/rio/common.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/__init__.py` & `rio_ui-0.5.7/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/app_root.py` & `rio_ui-0.5.7/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/auto_form.py` & `rio_ui-0.5.7/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/banner.py` & `rio_ui-0.5.7/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/build_failed.py` & `rio_ui-0.5.7/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/button.py` & `rio_ui-0.5.7/rio/components/button.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/card.py` & `rio_ui-0.5.7/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/class_container.py` & `rio_ui-0.5.7/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/color_picker.py` & `rio_ui-0.5.7/rio/components/color_picker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/component.py` & `rio_ui-0.5.7/rio/components/component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/component_tree.py` & `rio_ui-0.5.7/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/container.py` & `rio_ui-0.5.7/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/devel_component.py` & `rio_ui-0.5.7/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/drawer.py` & `rio_ui-0.5.7/rio/components/drawer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/dropdown.py` & `rio_ui-0.5.7/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/flow_container.py` & `rio_ui-0.5.7/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/fundamental_component.py` & `rio_ui-0.5.7/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/grid.py` & `rio_ui-0.5.7/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/html.py` & `rio_ui-0.5.7/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/icon.py` & `rio_ui-0.5.7/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/image.py` & `rio_ui-0.5.7/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/key_event_listener.py` & `rio_ui-0.5.7/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/labeled_column.py` & `rio_ui-0.5.7/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/linear_containers.py` & `rio_ui-0.5.7/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/link.py` & `rio_ui-0.5.7/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/list_items.py` & `rio_ui-0.5.7/rio/components/list_items.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/list_view.py` & `rio_ui-0.5.7/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/markdown.py` & `rio_ui-0.5.7/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/media_player.py` & `rio_ui-0.5.7/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/mouse_event_listener.py` & `rio_ui-0.5.7/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/multi_line_text_input.py` & `rio_ui-0.5.7/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/node_input.py` & `rio_ui-0.5.7/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/node_output.py` & `rio_ui-0.5.7/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/number_input.py` & `rio_ui-0.5.7/rio/components/number_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/overlay.py` & `rio_ui-0.5.7/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/page_view.py` & `rio_ui-0.5.7/rio/components/page_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/plot.py` & `rio_ui-0.5.7/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/popup.py` & `rio_ui-0.5.7/rio/components/popup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/progress_bar.py` & `rio_ui-0.5.7/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/progress_circle.py` & `rio_ui-0.5.7/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/rectangle.py` & `rio_ui-0.5.7/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/revealer.py` & `rio_ui-0.5.7/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/root_components.py` & `rio_ui-0.5.7/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/scroll_container.py` & `rio_ui-0.5.7/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/scroll_target.py` & `rio_ui-0.5.7/rio/components/scroll_target.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/separator.py` & `rio_ui-0.5.7/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/slider.py` & `rio_ui-0.5.7/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/slideshow.py` & `rio_ui-0.5.7/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/spacer.py` & `rio_ui-0.5.7/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/stack.py` & `rio_ui-0.5.7/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/switch.py` & `rio_ui-0.5.7/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/switcher.py` & `rio_ui-0.5.7/rio/components/switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/switcher_bar.py` & `rio_ui-0.5.7/rio/components/switcher_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/table.py` & `rio_ui-0.5.7/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/text.py` & `rio_ui-0.5.7/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/text_input.py` & `rio_ui-0.5.7/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/theme_context_switcher.py` & `rio_ui-0.5.7/rio/components/theme_context_switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/tooltip.py` & `rio_ui-0.5.7/rio/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/components/website.py` & `rio_ui-0.5.7/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/dataclass.py` & `rio_ui-0.5.7/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/component_details.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/component_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 rio.Spacer(),
                 *header_accessories,
                 margin_bottom=0.2,
                 spacing=0.5,
             ),
             row_index,
             0,
-            width=4,
+            width=5,
         )
         row_index += 1
 
         # Which file/line was this component instantiated from?
         file, line = target._creator_stackframe_
 
         try:
@@ -160,15 +160,15 @@
             rio.Text(
                 f"{file} line {line}",
                 style="dim",
                 justify="left",
             ),
             row_index,
             0,
-            width=4,
+            width=5,
         )
         row_index += 1
 
         # Custom properties
         #
         # Make sure to skip any which already have custom tailored cells
         debug_details = target.get_debug_details()
@@ -194,15 +194,15 @@
             value_limit = 30
             prop_str = repr(prop_value)
 
             if len(prop_str) > value_limit:
                 prop_str = prop_str[: value_limit - 1] + "…"
 
             add_cell(prop_name, 0, True)
-            add_cell(prop_str, 1, False, width=3)
+            add_cell(prop_str, 1, False, width=4)
             row_index += 1
 
         # Size
         if "width" in debug_details or "height" in debug_details:
             try:
                 py_width_str = debug_details["width"]
             except KeyError:
@@ -324,9 +324,18 @@
                 ),
                 row_index,
                 0,
                 width=2,
             )
             row_index += 1
 
+        # Push all of the content to the left. This could be done by aligning
+        # the entire Grid, but that would ellipsize some long texts. Instead,
+        # add a Spacer into a fifth column, which will take up any unused space.
+        result.add(
+            rio.Spacer(height=0),
+            row_index - 1,
+            4,
+        )
+
         # Done
         return result
```

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/debugger.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/debugger.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,63 +21,64 @@
             "docs",
             "deploy",
         ]
         | None
     ) = None
 
     def get_selected_page(self) -> rio.Component | None:
-        PAGE_WIDTH = 22
+        REGULAR_PAGE_WIDTH = 22
+        WIDE_PAGE_WIDTH = 32
 
         # Nothing selected
         if self.selected_page is None:
             return None
 
         # Project
         if self.selected_page == "project":
             return project_page.ProjectPage(
-                width=PAGE_WIDTH,
+                width=REGULAR_PAGE_WIDTH,
             )
 
         # Tree
         if self.selected_page == "tree":
             return tree_page.TreePage(
-                width=PAGE_WIDTH,
+                width=WIDE_PAGE_WIDTH,
             )
 
         # Icons
         if self.selected_page == "icons":
             return icons_page.IconsPage(
                 # This page contains wide source code. Constant changes to the
                 # size would cause unsightly resizes.
-                width=PAGE_WIDTH + 15
+                width=REGULAR_PAGE_WIDTH + 15
             )
 
         # Theme
         if self.selected_page == "theme":
             return theme_picker_page.ThemePickerPage(
-                width=35,
+                width=WIDE_PAGE_WIDTH,
             )
 
         # Docs
         if self.selected_page == "docs":
             return docs_page.DocsPage(
-                width=PAGE_WIDTH,
+                width=REGULAR_PAGE_WIDTH,
             )
 
         # Deploy
         if self.selected_page == "deploy":
             return deploy_page.DeployPage(
-                width=PAGE_WIDTH,
+                width=REGULAR_PAGE_WIDTH,
             )
 
         # Anything else / TODO
         return rio.Text(
             f"TODO: {self.selected_page}",
             margin=2,
-            width=PAGE_WIDTH,
+            width=REGULAR_PAGE_WIDTH,
         )
 
     def build(self) -> rio.Component:
         return rio.Row(
             # Big fat line to separate the debugger from the rest of the page
             rio.Rectangle(
                 width=0.3,
```

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/deploy_page.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/docs_page.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/icons_page.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/project_page.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/sample_icons_grid.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/theme_picker_page.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/client_side_debugger/tree_page.py` & `rio_ui-0.5.7/rio/debug/client_side_debugger/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/monkeypatches.py` & `rio_ui-0.5.7/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/typing_utils.py` & `rio_ui-0.5.7/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/debug/validator.py` & `rio_ui-0.5.7/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/docs/custom.py` & `rio_ui-0.5.7/rio/docs/custom.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/docs/models.py` & `rio_ui-0.5.7/rio/docs/models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/docs/parsers.py` & `rio_ui-0.5.7/rio/docs/parsers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/errors.py` & `rio_ui-0.5.7/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/event.py` & `rio_ui-0.5.7/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/fills.py` & `rio_ui-0.5.7/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/global_state.py` & `rio_ui-0.5.7/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/icon_registry.py` & `rio_ui-0.5.7/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/inspection.py` & `rio_ui-0.5.7/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/maybes.py` & `rio_ui-0.5.7/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/routing.py` & `rio_ui-0.5.7/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/serialization.py` & `rio_ui-0.5.7/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/session.py` & `rio_ui-0.5.7/rio/session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/README.md` & `rio_ui-0.5.7/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/__init__.py` & `rio_ui-0.5.7/rio/snippets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # THE ORDER MATTERS. `revel` will display the options in the same order as they
 # appear in the literal
 AvailableTemplatesLiteral: TypeAlias = Literal[
     # Keep the empty template first
     "Empty",
     # Sort the remainder alphabetically
     "AI Chatbot",
+    "Crypto Dashboard",
     "Simple CRUD",
     "Tic-Tac-Toe",
 ]
 
 
 @dataclass
 class _TemplateConfig(uniserde.Serde):
@@ -344,22 +345,22 @@
             elif snippet.file_path.suffix == ".py":
                 other_python_files.append(snippet)
 
             else:
                 assert False, f"Unrecognized snippet file `{snippet.file_path}`"
 
         # Create the project template
-        assert readme_snippet is not None, f"`README.md` snippet not found for {name}"
+        assert readme_snippet is not None, f"`README.md` snippet not found for `{name}`"
         assert (
             thumbnail_snippet is not None
         ), f"`thumbnail.svg` snippet not found for {name}"
-        assert metadata is not None, f"`meta.json` snippet not found for {name}"
+        assert metadata is not None, f"`meta.json` snippet not found for `{name}`"
         assert (
             root_init_snippet is not None
-        ), f"`__init__.py` snippet not found for {name}"
+        ), f"`__init__.py` snippet not found for `{name}`"
 
         return ProjectTemplate(
             name=name,
             level=metadata.level,
             summary=metadata.summary,
             description_markdown_source=readme_snippet.stripped_code(),
             thumbnail=thumbnail_snippet,
```

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # <additional-imports>
 import openai
 
+import rio
+
 # </additional-imports>
 
 
 # <additional-code>
 OPENAI_API_KEY = "<placeholder>"  # Replace this with your OpenAI API key
```

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 margin=0.5,
                 align_y=0,
             ),
             # The message content is displayed inside of a second card. By using
             # markdown to show the message the user and chatbot can apply
             # formatting to their messages.
             rio.Card(
-                rio.MarkdownView(
+                rio.Markdown(
                     self.model.text,
                     margin=1.5,
                 ),
                 width="grow",
                 color=color,
             ),
         )
```

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,24 +40,24 @@
         await self.call_event_handler(self.on_cancel_event)
 
     def on_change_name(self, ev: rio.TextInputChangeEvent) -> None:
         """
         Changes the name of the currently selected menu item.
 
         Args:
-            ev: The event object that contains the new text.
+            ev: The event object that contains the new name.
         """
         self.currently_selected_menu_item.name = ev.text
 
     def on_change_description(self, ev: rio.TextInputChangeEvent) -> None:
         """
         Changes the description of the currently selected menu item.
 
         Args:
-            ev: The event object that contains the new text.
+            ev: The event object that contains the new description.
         """
         self.currently_selected_menu_item.description = ev.text
 
     def on_change_price(self, ev: rio.NumberInputChangeEvent) -> None:
         """
         Changes the price of the currently selected menu item.
```

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import *  # type:ignore
+
 import rio
 
 # <additional-imports>
 from .. import components as comps
 from .. import data_models
 
 # </additional-imports>
@@ -20,20 +22,22 @@
     method is used to handle the add new item event. The on_press_select_menu_item method is used to handle the selection
     of a menu item.
 
     Attributes:
         menu_item_set: A list of menu items.
         currently_selected_menu_item: The currently selected menu item.
         banner_text: The text to be displayed in the banner.
+        banner_style: The style of the banner (success, danger, info).
         is_new_entry: A flag to indicate if the currently selected menu item is a new entry.
     """
 
     menu_item_set: list[data_models.MenuItems] = []
     currently_selected_menu_item: data_models.MenuItems | None = None
     banner_text: str = ""
+    banner_style: Literal["success", "danger", "info"] = "success"
     is_new_entry: bool = False
 
     @rio.event.on_populate
     def on_populate(self) -> None:
         """
         Event handler that is called when the component is populated.
 
@@ -45,16 +49,18 @@
     async def on_press_delete_item(self, idx: int) -> None:
         """
         Perform actions when the "Delete" button is pressed.
 
         Args:
             idx: The index of the item to be deleted.
         """
+        # delete the item from the list
         self.menu_item_set.pop(idx)
         self.banner_text = "Item was deleted"
+        self.banner_style = "danger"
         self.currently_selected_menu_item = None
 
     async def on_press_cancel_event(self) -> None:
         """
         Perform actions when the "Cancel" button is pressed.
         """
         self.currently_selected_menu_item = None
@@ -68,18 +74,20 @@
         or updates the menu item set if it is an existing entry. It also updates the banner text and sets
         the is_new_entry flag to False.
         """
         assert self.currently_selected_menu_item is not None
         if self.is_new_entry:
             self.menu_item_set.append(self.currently_selected_menu_item)
             self.banner_text = "Item was added"
+            self.banner_style = "success"
             self.is_new_entry = False
             self.currently_selected_menu_item = None
         else:
             self.banner_text = "Item was updated"
+            self.banner_style = "info"
 
     async def on_press_add_new_item(self) -> None:
         """
         Perform actions when the "Add New" ListItem is pressed.
 
         This method sets the currently selected menu item to a new empty instance of models.MenuItems,
         clears the banner text, and sets the is_new_entry flag to True.
@@ -133,28 +141,28 @@
         #  +-------------------------------  #
         ######################################
 
         """
 
         if self.currently_selected_menu_item is None:
             return rio.Column(
-                rio.Banner(self.banner_text, style="danger"),
+                rio.Banner(self.banner_text, style=self.banner_style),
                 comps.ItemList(
                     menu_item_set=self.menu_item_set,
                     on_add_new_item_event=self.on_press_add_new_item,
                     on_delete_item_event=self.on_press_delete_item,
                     on_select_item_event=self.on_press_select_menu_item,
                     align_y=0,
                 ),
                 align_y=0,
                 margin=3,
             )
         else:
             return rio.Column(
-                rio.Banner(self.banner_text, style="danger"),
+                rio.Banner(self.banner_text, style=self.banner_style),
                 rio.Row(
                     comps.ItemList(
                         menu_item_set=self.menu_item_set,
                         on_add_new_item_event=self.on_press_add_new_item,
                         on_delete_item_event=self.on_press_delete_item,
                         on_select_item_event=self.on_press_select_menu_item,
                         align_y=0,
```

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/state_properties.py` & `rio_ui-0.5.7/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/text_style.py` & `rio_ui-0.5.7/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/theme.py` & `rio_ui-0.5.7/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/user_settings_module.py` & `rio_ui-0.5.7/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/rio/world_units.py` & `rio_ui-0.5.7/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.6/PKG-INFO` & `rio_ui-0.5.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-ui
-Version: 0.5.6
+Version: 0.5.7
 Summary: Build modern Websites and Apps just with Python
 Home-page: https://rio.dev
 License: LGPL-3.0
 Keywords: web-development,web-framework,framework,functional,type-safe,typing,typed,react,web,app,user-interface,web-app,local-app,modern,rio
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -66,29 +66,29 @@
 
 🌊 You've arrived at **Rio**, an easy to use framework for creating websites and
 apps.
 
 🐍 Rio is based **entirely on Python**. You **won't need a single line of HTML, CSS, or
 JavaScript** to create beautiful, modern apps.
 
-[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) -  [Docs](https://rio.dev/docs) - [Source Code](https://gitlab.com/team-rio/rio)
+[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) - [Docs](https://rio.dev/docs) - [Source Code](https://gitlab.com/team-rio/rio)
 
 Rio brings React-style components to Python. Pull from a wealth of built-in
 components and combine them to create your own custom components. Then combine
 those into entire apps. Best of all, Rio apps can run both locally on your
 machine and on the web.
 
 ## Features 🧩
 
-- Modern, **declarative UI** framework
-- **100% Python** - Zero HTML, CSS, or JavaScript required
-- Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
-- Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
-- Apps can run **both locally and on the web**
-- **Open Source & Free forever**
+-   Modern, **declarative UI** framework
+-   **100% Python** - Zero HTML, CSS, or JavaScript required
+-   Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
+-   Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
+-   Apps can run **both locally and on the web**
+-   **Open Source & Free forever**
 
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
 pip install rio-ui
@@ -101,18 +101,105 @@
 ```bash
 rio new
 ```
 
 You can choose from a variety of built-in templates to get you started. Here's a complete example to create a project based on the tic-tac-toe template:
 
 ```bash
-rio new my-app --type website --template 'Tic-Tac-Toe'
+rio new my-app --type website --template "Tic-Tac-Toe"
 cd my-project
 rio run
 ```
 
 You'll have your first app up and running in seconds!
 
 ## How it works 🧠
 
 TODO: Minimal example
 
+```python
+from typing import *  # type: ignore
+import rio
+from openai import AsyncOpenAI
+
+client = AsyncOpenAI()
+
+
+class DallEPage(rio.Component):
+
+    prompt: str = ""
+    image_url: str = ""
+    is_loading: bool = False
+
+    async def get_image(self) -> None:
+        """Get an image by prompt."""
+
+        self.is_loading = True
+        await self.force_refresh()
+
+        if self.prompt == "":
+            self.image_url = ""
+            self.is_loading = False
+            return
+
+        try:
+            response = await client.images.generate(
+                model="dall-e-2",
+                prompt=self.prompt,
+                size="256x256",
+                quality="standard",
+                n=1,
+            )
+            self.image_url = response.data[0].url
+
+        finally:
+            self.is_loading = False
+
+    def build(self) -> rio.Component:
+
+        return rio.Rectangle(
+            content=rio.Card(
+                rio.Column(
+                    rio.Text("DALL-E", style="heading1"),
+                    rio.TextInput(
+                        text=self.bind().prompt,
+                        label="Prompt:",
+                    ),
+                    rio.Button(
+                        "Create Image",
+                        on_press=self.get_image,
+                        is_loading=self.is_loading,
+                    ),
+                    # Add the image to the page if it exists
+                    *(
+                        [
+                            rio.Image(
+                                rio.URL(self.image_url),
+                                height=36,
+                            )
+                        ]
+                        if self.image_url
+                        else []
+                    ),
+                    spacing=1,
+                    margin=2,
+                ),
+                width=40,
+                align_x=0.5,
+                align_y=0.5,
+                margin=2,
+            ),
+            fill=rio.Color.GREY,
+        )
+
+
+# Run the app
+app = rio.App(
+    pages=[
+        rio.Page(
+            page_url="",
+            build=DallEPage,
+        ),
+    ],
+)
+```
+
```


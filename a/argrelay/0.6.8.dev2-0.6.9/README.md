# Comparing `tmp/argrelay-0.6.8.dev2.tar.gz` & `tmp/argrelay-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argrelay-0.6.8.dev2.tar", last modified: Mon Mar 11 15:27:06 2024, max compression
+gzip compressed data, was "argrelay-0.6.9.tar", last modified: Sat Mar 16 19:19:34 2024, max compression
```

## Comparing `argrelay-0.6.8.dev2.tar` & `argrelay-0.6.9.tar`

### file list

```diff
@@ -1,392 +1,396 @@
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.483511 argrelay-0.6.8.dev2/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.6.8.dev2/LICENSE
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-03-11 15:27:06.483511 argrelay-0.6.8.dev2/PKG-INFO
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.449511 argrelay-0.6.8.dev2/docs/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.452511 argrelay-0.6.8.dev2/docs/dev_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5523 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/bootstrap_procedure.1.project_creation.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2509 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1924 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/brief_history.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/code_style.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/docs/dev_notes/completion_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/completion_perf_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/gui_tests_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/dev_notes/how_search_works.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/library_vs_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/mongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1469 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/next_steps_tutorial.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/origin_story.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/dev_notes/query_perf_10_x_more_data_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/dev_notes/query_perf_cache_vs_no_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/dev_notes/query_perf_mongomock_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/dev_notes/query_perf_pymongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/docs/dev_notes/release_procedure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/screencast_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      787 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/scripts_summary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/semver_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5694 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/term_dictionary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11130 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/top_todos.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/dev_notes/version_format.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.457511 argrelay-0.6.8.dev2/docs/feature_stories/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3725 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_01_89_09_24.interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1838 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_14_59_14_06.pending_requests.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      885 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_15_79_76_85.line_processor.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1470 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      956 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_20_88_05_60.named_args.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      555 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_26_43_73_72.func_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3596 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_29_54_67_86.dir_structure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_31_70_49_15.search_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      628 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_33_76_82_84.global_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1135 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_36_17_84_44.check_script.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_39_58_01_91.query_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_46_96_59_05.init_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1280 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_47_63_35_61.env_vars.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1557 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_55_57_45_04.enum_selector.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1756 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_58_61_77_69.dev_shell.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_62_25_92_06.assigned_context.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_63_63_14_08.generated_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_66_17_43_42.test_infra.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-03-10 08:59:31.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_67_16_61_97.git_plugin.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_71_87_33_52.help_hint.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_72_40_53_00.fill_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_78_91_27_22.interp_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2381 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4506 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      322 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1729 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_91_88_07_23.jump_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_94_30_49_28.help_doc.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_98_55_40_77.invoke_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/feature_stories/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.459511 argrelay-0.6.8.dev2/docs/release_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.0.0.dev0.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.0.0.dev27.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.0.0.dev28.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.0.0.dev42.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.0.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.1.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.2.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.2.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.3.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.4.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.5.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.5.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.5.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.6.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.6.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.6.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.6.3.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/release_notes/v0.6.4.final.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.461511 argrelay-0.6.8.dev2/docs/task_refs/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      420 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2977 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-03-10 09:04:27.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      497 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      648 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2669 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/docs/task_refs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.461511 argrelay-0.6.8.dev2/docs/test_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      694 2023-07-22 05:41:07.000000 argrelay-0.6.8.dev2/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/docs/test_data/TD_38_03_48_51.large_data_set.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10511 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/test_data/TD_63_37_05_36.demo_services_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.6.8.dev2/docs/test_data/TD_70_69_38_46.no_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      400 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/docs/test_data/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.6.8.dev2/pyproject.toml
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    14601 2024-03-11 14:44:45.000000 argrelay-0.6.8.dev2/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-03-11 15:27:06.483511 argrelay-0.6.8.dev2/setup.cfg
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4182 2024-03-10 15:39:33.000000 argrelay-0.6.8.dev2/setup.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.448511 argrelay-0.6.8.dev2/src/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.461511 argrelay-0.6.8.dev2/src/argrelay/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.462511 argrelay-0.6.8.dev2/src/argrelay/client_command_local/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_local/AbstractLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_local/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.462511 argrelay-0.6.8.dev2/src/argrelay/client_command_remote/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3936 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/client_command_remote/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.463511 argrelay-0.6.8.dev2/src/argrelay/client_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3749 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_spec/ShellContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/client_spec/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.464511 argrelay-0.6.8.dev2/src/argrelay/custom_integ/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8382 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/BaseConfigDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2326 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3640 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3511 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1597 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/FuncConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-03-11 14:06:24.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8391 2024-03-11 13:56:23.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1849 2024-03-10 12:37:03.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-10 08:55:11.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12637 2024-03-11 14:10:25.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1605 2024-03-10 08:11:16.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      830 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15820 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      188 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    59880 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-03-10 07:46:06.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/git_utils.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      371 2024-03-10 10:14:50.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ/value_constants.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.465511 argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6919 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/argrelay_common_lib.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8106 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/argrelay_rc.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    32228 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3392 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/dev_shell.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3672 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/init_shell_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2644 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/upgrade_all_packages.bash
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.466511 argrelay-0.6.8.dev2/src/argrelay/enum_desc/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/ArgSource.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/CallConv.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/CompScope.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/CompType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/DistinctValuesQuery.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/InterpStep.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/PluginType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/ReservedArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/ReservedEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/RunMode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/ServerAction.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      105 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/SpecialChar.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/SpecialFunc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2905 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/TermColor.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/TokenType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/enum_desc/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.467511 argrelay-0.6.8.dev2/src/argrelay/handler_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_request/AbstractServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1535 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3103 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/handler_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.467511 argrelay-0.6.8.dev2/src/argrelay/handler_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_response/AbstractClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9137 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/handler_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.467511 argrelay-0.6.8.dev2/src/argrelay/misc_helper_common/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/misc_helper_common/ElapsedTime.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/misc_helper_common/TypeDesc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1550 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/misc_helper_common/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.468511 argrelay-0.6.8.dev2/src/argrelay/misc_helper_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/misc_helper_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.468511 argrelay-0.6.8.dev2/src/argrelay/mongo_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-03-10 13:03:02.000000 argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoClientWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoServerWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.8.dev2/src/argrelay/mongo_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.468511 argrelay-0.6.8.dev2/src/argrelay/plugin_config/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_config/AbstractConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_config/DefaultConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_config/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.469511 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/AbstractDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3147 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2418 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/EchoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1847 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/ErrorDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5882 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/HelpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5561 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/InterceptDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1201 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/NoopDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/QueryEnumDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.470511 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2431 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/AbstractInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/AbstractInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FirstArgInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4862 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FirstArgInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    14009 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FuncTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11293 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1449 2024-03-10 10:14:11.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7003 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/InterpTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5262 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2805 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/NoopInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/NoopInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7555 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/TreeWalker.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.471511 argrelay-0.6.8.dev2/src/argrelay/plugin_loader/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_loader/AbstractLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_loader/NoopLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/plugin_loader/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.471511 argrelay-0.6.8.dev2/src/argrelay/relay_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      967 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/AbstractClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/AbstractClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/AbstractClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/RemoteClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/RemoteClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4629 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/__main__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3702 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/proc_parent.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2102 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_client/proc_split.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.472511 argrelay-0.6.8.dev2/src/argrelay/relay_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11191 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/CustomFlaskApp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/GuiBannerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/HelpHintCache.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7312 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/LocalServer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/QueryCacheConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/QueryEngine.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/QueryResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.472511 argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_static/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_static/argrelay_client.js
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_static/argrelay_style.css
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_static/external_link.svg
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.472511 argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_templates/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_templates/argrelay_main.html
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4948 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/route_api.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/relay_server/route_gui.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.473511 argrelay-0.6.8.dev2/src/argrelay/runtime_context/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2841 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_context/AbstractPlugin.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4093 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_context/EnvelopeContainer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_context/InitControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13607 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_context/InterpContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5861 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_context/ParsedContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_context/SearchControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_context/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.474511 argrelay-0.6.8.dev2/src/argrelay/runtime_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/AssignedValue.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      376 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/ClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-01-17 14:42:50.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/ConnectionConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/EnvelopeCollection.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/PluginEntry.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/ServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/ServerPluginControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/StaticData.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.8.dev2/src/argrelay/runtime_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.474511 argrelay-0.6.8.dev2/src/argrelay/sample_conf/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/sample_conf/argrelay.client.json
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31479 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/src/argrelay/sample_conf/argrelay.server.yaml
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.474511 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2690 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_client/ClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1094 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_client/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.475511 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3001 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      890 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1104 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2226 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/MongoConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1279 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1301 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6931 2024-03-10 14:41:02.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/ServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1630 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1249 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/StaticDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.475511 argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1073 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/InitControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3158 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/SearchControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.475511 argrelay-0.6.8.dev2/src/argrelay/schema_config_plugin/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2284 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_plugin/PluginEntrySchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/schema_config_plugin/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.475511 argrelay-0.6.8.dev2/src/argrelay/schema_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3285 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_request/CallContextSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/schema_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.476511 argrelay-0.6.8.dev2/src/argrelay/schema_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/ArgValues.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1625 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/ArgValuesSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1417 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/AssignedValueSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3087 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/EnvelopeContainerSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1311 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/InterpResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2371 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/InterpResultSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      950 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/InvocationInput.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1732 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/InvocationInputSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.8.dev2/src/argrelay/schema_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.477511 argrelay-0.6.8.dev2/src/argrelay/server_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/server_spec/CallContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/server_spec/DescribeLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/server_spec/ProposeArgValuesSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/server_spec/RelayLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.8.dev2/src/argrelay/server_spec/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/server_spec/const_int.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/server_spec/server_data_schema.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.478511 argrelay-0.6.8.dev2/src/argrelay/test_infra/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/BaseTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/ClientServerTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/CustomTestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/CustomVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/End2EndTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    37631 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/EnvMockBuilder.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11529 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/InOutTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/JsonTestOutputVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/LocalClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2785 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/LocalClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4828 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/LocalTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/OpenFileMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3419 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/PopenMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4370 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/RemoteTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/ServerOnlyTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/TestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-09 17:26:58.000000 argrelay-0.6.8.dev2/src/argrelay/test_infra/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-11 15:27:06.462511 argrelay-0.6.8.dev2/src/argrelay.egg-info/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-03-11 15:27:06.000000 argrelay-0.6.8.dev2/src/argrelay.egg-info/PKG-INFO
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    30769 2024-03-11 15:27:06.000000 argrelay-0.6.8.dev2/src/argrelay.egg-info/SOURCES.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-03-11 15:27:06.000000 argrelay-0.6.8.dev2/src/argrelay.egg-info/dependency_links.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      171 2024-03-11 15:27:06.000000 argrelay-0.6.8.dev2/src/argrelay.egg-info/requires.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-03-11 15:27:06.000000 argrelay-0.6.8.dev2/src/argrelay.egg-info/top_level.txt
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.630345 argrelay-0.6.9/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.6.9/LICENSE
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1127 2024-03-16 19:19:34.630345 argrelay-0.6.9/PKG-INFO
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.595345 argrelay-0.6.9/docs/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.596345 argrelay-0.6.9/docs/dev_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5523 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.1.project_creation.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2509 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1924 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/brief_history.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/code_style.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.6.9/docs/dev_notes/completion_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/completion_perf_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/gui_tests_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/how_search_works.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/library_vs_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/mongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1469 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/next_steps_tutorial.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/origin_story.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_10_x_more_data_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_cache_vs_no_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_mongomock_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_pymongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.6.9/docs/dev_notes/release_procedure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/screencast_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      787 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/scripts_summary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/semver_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5694 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/term_dictionary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11130 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/top_todos.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/version_format.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.602345 argrelay-0.6.9/docs/feature_stories/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3725 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_01_89_09_24.interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1839 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_14_59_14_06.pending_requests.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      886 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_15_79_76_85.line_processor.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1470 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      956 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_20_88_05_60.named_args.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      917 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_26_43_73_72.func_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3596 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_29_54_67_86.dir_structure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_31_70_49_15.search_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      628 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_33_76_82_84.global_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1135 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_36_17_84_44.check_script.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_39_58_01_91.query_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      792 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_46_96_59_05.init_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1280 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_47_63_35_61.env_vars.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.6.9/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1557 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_55_57_45_04.enum_selector.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1756 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_58_61_77_69.dev_shell.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_62_25_92_06.assigned_context.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_63_63_14_08.generated_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_66_17_43_42.test_infra.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_67_16_61_97.git_plugin.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_71_87_33_52.help_hint.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_72_40_53_00.fill_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1370 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_78_91_27_22.interp_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2391 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4506 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1841 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1729 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_91_88_07_23.jump_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.6.9/docs/feature_stories/FS_94_30_49_28.help_doc.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_98_55_40_77.invoke_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.604345 argrelay-0.6.9/docs/release_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev0.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev27.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev28.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev42.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.1.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.2.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.2.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.3.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.4.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.5.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.5.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.5.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.3.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.4.final.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.606345 argrelay-0.6.9/docs/task_refs/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      420 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2977 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      497 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/task_refs/TODO_70_48_96_29.be_able_to_assert_unconsumed_arg_vals.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      648 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2669 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.607345 argrelay-0.6.9/docs/test_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.6.9/docs/test_data/TD_38_03_48_51.large_data_set.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10511 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/test_data/TD_63_37_05_36.demo_services_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.6.9/docs/test_data/TD_70_69_38_46.no_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      550 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.6.9/docs/test_data/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.6.9/pyproject.toml
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    14598 2024-03-13 15:12:40.000000 argrelay-0.6.9/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-03-16 19:19:34.630345 argrelay-0.6.9/setup.cfg
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4177 2024-03-16 19:14:19.000000 argrelay-0.6.9/setup.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.593345 argrelay-0.6.9/src/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.607345 argrelay-0.6.9/src/argrelay/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.608345 argrelay-0.6.9/src/argrelay/client_command_local/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/AbstractLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/client_command_local/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.608345 argrelay-0.6.9/src/argrelay/client_command_remote/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3936 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/client_command_remote/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.608345 argrelay-0.6.9/src/argrelay/client_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3749 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_spec/ShellContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_spec/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.610345 argrelay-0.6.9/src/argrelay/custom_integ/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8495 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2326 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3640 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3511 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1597 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/FuncConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8391 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1849 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12645 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1605 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      830 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    16189 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      217 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    65313 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/custom_integ/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/git_utils.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      371 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/value_constants.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.611345 argrelay-0.6.9/src/argrelay/custom_integ_res/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7005 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_common_lib.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8106 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_rc.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    32228 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3392 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/dev_shell.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3672 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/init_shell_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2644 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/upgrade_all_packages.bash
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.612345 argrelay-0.6.9/src/argrelay/enum_desc/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ArgSource.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/CallConv.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/CompScope.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/CompType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/enum_desc/DistinctValuesQuery.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/enum_desc/InterpStep.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/PluginType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ReservedArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ReservedEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/RunMode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ServerAction.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      105 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/enum_desc/SpecialChar.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/SpecialFunc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2905 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/TermColor.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/TokenType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/enum_desc/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.612345 argrelay-0.6.9/src/argrelay/handler_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/AbstractServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1535 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3103 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/handler_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.613345 argrelay-0.6.9/src/argrelay/handler_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/AbstractClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9137 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/handler_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.613345 argrelay-0.6.9/src/argrelay/misc_helper_common/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_common/ElapsedTime.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_common/TypeDesc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1550 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_common/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.613345 argrelay-0.6.9/src/argrelay/misc_helper_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.614345 argrelay-0.6.9/src/argrelay/mongo_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoClientWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoServerWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.9/src/argrelay/mongo_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.614345 argrelay-0.6.9/src/argrelay/plugin_config/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/AbstractConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.615345 argrelay-0.6.9/src/argrelay/plugin_delegator/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3147 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2418 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/EchoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1847 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5882 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/HelpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5639 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/InterceptDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1201 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/NoopDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/QueryEnumDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.616345 argrelay-0.6.9/src/argrelay/plugin_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3680 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_interp/AbstractInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/AbstractInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4862 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15370 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11293 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1449 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7437 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5262 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2805 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/NoopInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/NoopInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7555 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/TreeWalker.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/plugin_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.617345 argrelay-0.6.9/src/argrelay/plugin_loader/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_loader/AbstractLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.6.9/src/argrelay/plugin_loader/NoopLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/plugin_loader/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.618345 argrelay-0.6.9/src/argrelay/relay_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      967 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/AbstractClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/AbstractClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/AbstractClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.6.9/src/argrelay/relay_client/RemoteClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/RemoteClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.6.9/src/argrelay/relay_client/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4629 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/__main__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3702 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/proc_parent.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2102 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/proc_split.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.619345 argrelay-0.6.9/src/argrelay/relay_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11191 2024-03-16 18:22:38.000000 argrelay-0.6.9/src/argrelay/relay_server/CustomFlaskApp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/relay_server/GuiBannerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/HelpHintCache.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7312 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/LocalServer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/relay_server/QueryCacheConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/QueryEngine.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/QueryResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.6.9/src/argrelay/relay_server/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/relay_server/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.619345 argrelay-0.6.9/src/argrelay/relay_server/gui_static/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_client.js
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_style.css
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/external_link.svg
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.619345 argrelay-0.6.9/src/argrelay/relay_server/gui_templates/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_templates/argrelay_main.html
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4948 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/route_api.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/route_gui.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.620345 argrelay-0.6.9/src/argrelay/runtime_context/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2841 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_context/AbstractPlugin.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4186 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/runtime_context/EnvelopeContainer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/runtime_context/InitControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    14498 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/runtime_context/InterpContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5861 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_context/ParsedContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_context/SearchControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.9/src/argrelay/runtime_context/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.621345 argrelay-0.6.9/src/argrelay/runtime_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/runtime_data/AssignedValue.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      376 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/ClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/runtime_data/ConnectionConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/EnvelopeCollection.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/PluginEntry.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/ServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/ServerPluginControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/StaticData.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/runtime_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.621345 argrelay-0.6.9/src/argrelay/sample_conf/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/sample_conf/argrelay.client.json
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31479 2024-03-16 14:33:33.000000 argrelay-0.6.9/src/argrelay/sample_conf/argrelay.server.yaml
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.621345 argrelay-0.6.9/src/argrelay/schema_config_core_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2690 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_client/ClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1094 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_core_client/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.622345 argrelay-0.6.9/src/argrelay/schema_config_core_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3001 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      890 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1104 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2226 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1279 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1301 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6951 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1630 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1249 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/StaticDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.623345 argrelay-0.6.9/src/argrelay/schema_config_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1073 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/InitControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3158 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/SearchControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.623345 argrelay-0.6.9/src/argrelay/schema_config_plugin/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2284 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_plugin/PluginEntrySchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_plugin/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.623345 argrelay-0.6.9/src/argrelay/schema_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3285 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_request/CallContextSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.624345 argrelay-0.6.9/src/argrelay/schema_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/ArgValues.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1625 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/ArgValuesSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1417 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/AssignedValueSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3087 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/EnvelopeContainerSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1311 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InterpResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2371 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InterpResultSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      950 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InvocationInput.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1732 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InvocationInputSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.624345 argrelay-0.6.9/src/argrelay/server_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/CallContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/DescribeLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/ProposeArgValuesSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/RelayLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.9/src/argrelay/server_spec/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/const_int.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/server_data_schema.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.626345 argrelay-0.6.9/src/argrelay/test_infra/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/BaseTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/ClientServerTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/CustomTestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/CustomVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/End2EndTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    37631 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/EnvMockBuilder.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11214 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/test_infra/InOutTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/JsonTestOutputVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/LocalClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2785 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/LocalClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4818 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/test_infra/LocalTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/OpenFileMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3419 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/PopenMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4365 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/test_infra/RemoteTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/ServerOnlyTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/TestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.607345 argrelay-0.6.9/src/argrelay.egg-info/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1127 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/PKG-INFO
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    30872 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/SOURCES.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/dependency_links.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      171 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/requires.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/top_level.txt
```

### Comparing `argrelay-0.6.8.dev2/LICENSE` & `argrelay-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/PKG-INFO` & `argrelay-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.6.8.dev2
+Version: 0.6.9
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/bootstrap_procedure.1.project_creation.md` & `argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.1.project_creation.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md` & `argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md` & `argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/brief_history.md` & `argrelay-0.6.9/docs/dev_notes/brief_history.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/code_style.md` & `argrelay-0.6.9/docs/dev_notes/code_style.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/completion_notes.md` & `argrelay-0.6.9/docs/dev_notes/completion_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/completion_perf_notes.md` & `argrelay-0.6.9/docs/dev_notes/completion_perf_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/gui_tests_notes.md` & `argrelay-0.6.9/docs/dev_notes/gui_tests_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/how_search_works.md` & `argrelay-0.6.9/docs/dev_notes/how_search_works.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/library_vs_framework.md` & `argrelay-0.6.9/docs/dev_notes/library_vs_framework.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/mongo_notes.md` & `argrelay-0.6.9/docs/dev_notes/mongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/next_steps_tutorial.md` & `argrelay-0.6.9/docs/dev_notes/next_steps_tutorial.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/origin_story.md` & `argrelay-0.6.9/docs/dev_notes/origin_story.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/query_perf_10_x_more_data_notes.md` & `argrelay-0.6.9/docs/dev_notes/query_perf_10_x_more_data_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/query_perf_cache_vs_no_cache.md` & `argrelay-0.6.9/docs/dev_notes/query_perf_cache_vs_no_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/query_perf_mongomock_notes.md` & `argrelay-0.6.9/docs/dev_notes/query_perf_mongomock_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/query_perf_pymongo_notes.md` & `argrelay-0.6.9/docs/dev_notes/query_perf_pymongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/release_procedure.md` & `argrelay-0.6.9/docs/dev_notes/release_procedure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/screencast_notes.md` & `argrelay-0.6.9/docs/dev_notes/screencast_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/scripts_summary.md` & `argrelay-0.6.9/docs/dev_notes/scripts_summary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/semver_notes.md` & `argrelay-0.6.9/docs/dev_notes/semver_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/term_dictionary.md` & `argrelay-0.6.9/docs/dev_notes/term_dictionary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/top_todos.md` & `argrelay-0.6.9/docs/dev_notes/top_todos.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/dev_notes/version_format.md` & `argrelay-0.6.9/docs/dev_notes/version_format.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_00_13_77_97.plugin_framework.md` & `argrelay-0.6.9/docs/feature_stories/FS_00_13_77_97.plugin_framework.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_01_89_09_24.interp_tree.md` & `argrelay-0.6.9/docs/feature_stories/FS_01_89_09_24.interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md` & `argrelay-0.6.9/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_06_99_43_60.list_arg_value.md` & `argrelay-0.6.9/docs/feature_stories/FS_06_99_43_60.list_arg_value.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md` & `argrelay-0.6.9/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     Yes, especially those values part of options avoided by setting default (FS_72_53_55_13).
 
 *   `ArgSource.ImplicitValue`: Yes
 
     The implicit values are debatable: if it is already selected, should we highlight it of user to override?
 
-    Solution: yes, highlight for now because override is possible - see FS_90_48_11_45 (force-assignment).
+    Solution: yes, highlight for now because override is possible - see FS_90_48_11_45 (forced assignment).
 
 *   `ArgSource.ExplicitPosArg`: Yes
 
     Yes, because of the diff between `ServerAction.DescribeLineArgs` and `ServerAction.ProposeArgValues` (above).
 
 *   `ArgSource.ExplicitNamedArg`: TODO: FS_20_88_05_60 named args
```

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md` & `argrelay-0.6.9/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_14_59_14_06.pending_requests.md` & `argrelay-0.6.9/docs/feature_stories/FS_14_59_14_06.pending_requests.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_15_79_76_85.line_processor.md` & `argrelay-0.6.9/docs/feature_stories/FS_15_79_76_85.line_processor.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This feature defines a concept of (command) line processor.
 
 As of now, there is a single implementation:
 
 *   FS_55_57_45_04 enum selector
 
-    Use has to select a function and its args as enum items.
+    User has to select a function and its args as enum items.
 
 TODO: Factor out abstract `LineProcessor` with their individual implementations.
 
 TODO: Select (command) line processor via FS_42_76_93_51 first arg.
 
 NOTE: Any new implementation (e.g. ML) of (command) line processor will likely also require:
       *   Different implementation of REST APIs (see `ServerAction`).
```

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md` & `argrelay-0.6.9/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md` & `argrelay-0.6.9/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_20_88_05_60.named_args.md` & `argrelay-0.6.9/docs/feature_stories/FS_20_88_05_60.named_args.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md` & `argrelay-0.6.9/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_26_43_73_72.func_tree.md` & `argrelay-0.6.9/docs/feature_stories/FS_26_43_73_72.func_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_29_54_67_86.dir_structure.md` & `argrelay-0.6.9/docs/feature_stories/FS_29_54_67_86.dir_structure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_31_70_49_15.search_control.md` & `argrelay-0.6.9/docs/feature_stories/FS_31_70_49_15.search_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_33_76_82_84.global_tree.md` & `argrelay-0.6.9/docs/feature_stories/FS_33_76_82_84.global_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_36_17_84_44.check_script.md` & `argrelay-0.6.9/docs/feature_stories/FS_36_17_84_44.check_script.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md` & `argrelay-0.6.9/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_39_58_01_91.query_cache.md` & `argrelay-0.6.9/docs/feature_stories/FS_39_58_01_91.query_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md` & `argrelay-0.6.9/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md` & `argrelay-0.6.9/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_47_63_35_61.env_vars.md` & `argrelay-0.6.9/docs/feature_stories/FS_47_63_35_61.env_vars.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md` & `argrelay-0.6.9/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md` & `argrelay-0.6.9/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ---
 feature_story: FS_51_67_38_37
 feature_title: impossible arg combinations
-feature_status: TEST
+feature_status: OBSOLETE
 ---
 
+NOTE: This feature is obsoleted by FS_44_36_84_88 consume args one by one.
+NOTE: This feature (or rather situation) is the result of FS_90_48_11_45 forced assignment from entire type value space.
+
 TODO: There is no a single test tagged by this feature - add existing test or create new.
 
 It is possible to input impossible combination of args which will all get consumed, for example:
 
 ```sh
 relay_demo goto service dev upstream apac xx
 ```
```

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_55_57_45_04.enum_selector.md` & `argrelay-0.6.9/docs/feature_stories/FS_55_57_45_04.enum_selector.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md` & `argrelay-0.6.9/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md` & `argrelay-0.6.9/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_58_61_77_69.dev_shell.md` & `argrelay-0.6.9/docs/feature_stories/FS_58_61_77_69.dev_shell.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md` & `argrelay-0.6.9/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_62_25_92_06.assigned_context.md` & `argrelay-0.6.9/docs/feature_stories/FS_62_25_92_06.assigned_context.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_63_63_14_08.generated_config.md` & `argrelay-0.6.9/docs/feature_stories/FS_63_63_14_08.generated_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md` & `argrelay-0.6.9/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_66_17_43_42.test_infra.md` & `argrelay-0.6.9/docs/feature_stories/FS_66_17_43_42.test_infra.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_67_16_61_97.git_plugin.md` & `argrelay-0.6.9/docs/feature_stories/FS_67_16_61_97.git_plugin.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_71_87_33_52.help_hint.md` & `argrelay-0.6.9/docs/feature_stories/FS_71_87_33_52.help_hint.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_72_40_53_00.fill_control.md` & `argrelay-0.6.9/docs/feature_stories/FS_72_40_53_00.fill_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_80_45_89_81.integrated_functions.md` & `argrelay-0.6.9/docs/feature_stories/FS_80_45_89_81.integrated_functions.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md` & `argrelay-0.6.9/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ---
 feature_story: FS_80_82_13_35
 feature_title: option list on describe with prefix
-feature_status: TODO
+feature_status: TBD
 ---
 
 This feature uses tangent token (FS_23_62_89_43) to narrow down enum items listed on `ServerAction.DescribeLineArgs`
 (even if tangent token is considered unspecified = not consumed).
 
 Currently, instead of reducing options on `ServerAction.DescribeLineArgs` (as described in this feature below),
 prefix highlight (FS_11_87_76_73) is used to alleviate the need for this feature (FS_80_82_13_35).
 
-However, when arg value is incomplete (its value does not match any enum item),
+The point: when arg value is incomplete (its value does not match entirely any enum item),
 there is no reduction of options shown in description:
 
 ```sh
 some_command goto host pro|
 ```
 
 Actual:
```

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md` & `argrelay-0.6.9/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md` & `argrelay-0.6.9/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md` & `argrelay-0.6.9/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 ---
 feature_story: FS_90_48_11_45
-feature_title: force-assignment from entire type value space
-feature_status: TEST
+feature_title: forced assignment from entire type value space
+feature_status: OBSOLETE
 ---
 
+NOTE: This feature is obsoleted by FS_44_36_84_88 consume args one by one.
+TODO: This behavior is changed (review all the docs related to this and update):
+      Such incompatible values will not be "eaten" because
+      we eat values one-by-one narrowing down (querying) envelopes step-by-step now.
+
 TODO: This was written ahead of the implementation - fix description when implemented.
 TODO: This feature is actually special case of FS_62_25_92_06/FS_13_51_07_97 where `ArgSource.ExplicitValue` overrides `ArgSource.ImplicitValue`.
+NOTE: This feature causes FS_51_67_38_37 impossible arg combinations.
 
 When some args narrow down possible selection,
 then "incompatible" with that selection value appear on the command line,
 it should not be ignored simply because it does not match pre-filtered value set for that next `ArgType`.
 
 For example:
```

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_91_88_07_23.jump_tree.md` & `argrelay-0.6.9/docs/feature_stories/FS_91_88_07_23.jump_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/feature_stories/FS_92_75_93_01.clean_command_line.md` & `argrelay-0.6.9/docs/feature_stories/FS_92_75_93_01.clean_command_line.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/readme.md` & `argrelay-0.6.9/docs/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/release_notes/readme.md` & `argrelay-0.6.9/docs/release_notes/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/release_notes/v0.0.0.dev27.md` & `argrelay-0.6.9/docs/release_notes/v0.0.0.dev27.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md` & `argrelay-0.6.9/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md` & `argrelay-0.6.9/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md` & `argrelay-0.6.9/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md` & `argrelay-0.6.9/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md` & `argrelay-0.6.9/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md` & `argrelay-0.6.9/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md` & `argrelay-0.6.9/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md` & `argrelay-0.6.9/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md` & `argrelay-0.6.9/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 *   But if user puts an arg value matching the single value from the remaining arg types, consume it.
     TODO: This might be controversial.
           This also might complicate implementation and
           reasoning about consumption behavior.
 
 See also both:
 *   `FS_13_51_07_97` for singled out implicit values.
-*   `FS_90_48_11_45` for force-assignment.
+*   `FS_90_48_11_45` for forced assignment.
     However, in case of this `test_data: TD_27_59_80_86`, there is no force assignment,
     the assignment is matching.
```

### Comparing `argrelay-0.6.8.dev2/docs/test_data/TD_63_37_05_36.demo_services_data.md` & `argrelay-0.6.9/docs/test_data/TD_63_37_05_36.demo_services_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/docs/test_data/TD_70_69_38_46.no_data.md` & `argrelay-0.6.9/docs/test_data/TD_70_69_38_46.no_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/readme.md` & `argrelay-0.6.9/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <!--
 See: docs/dev_notes/screencast_notes.md
 -->
 
 <a name="argrelay-about"></a>
 # What's this?
 
-A framework to "ergonomically" select **custom data** input for command line interface (CLI) tools.
+A method to "ergonomically" select **custom data** input for command line interface (CLI) tools.
 
 The aim is to enrich two-way &#10231; interaction by **"pre-pared"** data:
 *   &#10230; You input args you **remember** (via `Tab`-auto-completion) in **relaxed order**.
 *   &#10229; It reports (via `Alt+Shift+Q` query):
     *   What args it **matched**.
     *   What **else** it needs.
```

### Comparing `argrelay-0.6.8.dev2/setup.py` & `argrelay-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # All paths start with `top_dir_path`:
     return file_paths
 
 
 setuptools.setup(
     name = "argrelay",
     # See `docs/dev_notes/version_format.md`:
-    version = "0.6.8.dev2",
+    version = "0.6.9",
     author = "uvsmtid",
     author_email = "uvsmtid@gmail.com",
     description = "Tab-completion & data search server = total recall for Bash shell",
     long_description = """
 See: https://github.com/argrelay/argrelay
     """,
     long_description_content_type = "text/markdown",
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_local/AbstractLocalClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_local/AbstractLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py` & `argrelay-0.6.9/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/client_spec/ShellContext.py` & `argrelay-0.6.9/src/argrelay/client_spec/ShellContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/BaseConfigDelegator.py` & `argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegator.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,16 +160,19 @@
                     fill_control: dict = fill_control_list[interp_ctx.curr_container_ipos]
                     for prop_name, prop_value_template in fill_control.items():
                         if prop_value_template is not None:
                             # The input is trusted (from config), right? Then:
                             # https://stackoverflow.com/a/54071505/441652
                             prop_value = eval(f'f"""{prop_value_template}"""')
 
-                            set_default_to(prop_name, prop_value, interp_ctx.curr_container)
-                            any_assignment = True
+                            any_assignment = (
+                                set_default_to(prop_name, prop_value, interp_ctx.curr_container)
+                                or
+                                any_assignment
+                            )
 
         return any_assignment
 
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py` & `argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyDelegator.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyLoader.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/FuncConfigSchema.py` & `argrelay-0.6.9/src/argrelay/custom_integ/FuncConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoArgType.py` & `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoDelegator.py` & `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py` & `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoLoader.py` & `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
                             GitRepoArgType.git_repo_root_rel_path.name: repo_root_rel_path,
                             GitRepoArgType.git_repo_root_abs_path.name: repo_root_abs_path,
                             GitRepoArgType.git_repo_root_base_name.name: repo_root_base_name,
                             #
                             GitRepoArgType.git_repo_commit_id.name: git_commit.hexsha,
                             GitRepoArgType.git_repo_short_commit_id.name: git_commit.hexsha[:7],
                             GitRepoArgType.git_repo_commit_author_name.name: git_commit.author.name,
-                            GitRepoArgType.git_repo_commit_author_email.name: git_commit.author.email,
+                            GitRepoArgType.git_repo_commit_author_email.name: git_commit.author.email.lower(),
                             GitRepoArgType.git_repo_commit_message.name: git_commit.message,
                             GitRepoArgType.git_repo_commit_date.name: commit_date_utc,
                             GitRepoArgType.git_repo_commit_time.name: commit_time_utc,
                         })
                         self.enrich_git_repo_object(commit_envelope)
                         commit_envelopes.append(commit_envelope)
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py` & `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceArgType.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ServiceArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceDelegator.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ServiceDelegator.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,27 +46,29 @@
 from argrelay.schema_response.InvocationInput import InvocationInput
 
 host_container_ipos_ = 1
 service_container_ipos_ = 1
 access_container_ipos_ = 2
 
 
-def set_default_to(arg_type, arg_val, envelope_container):
+def set_default_to(arg_type, arg_val, envelope_container) -> bool:
     if arg_type in envelope_container.search_control.types_to_keys_dict:
         if arg_type not in envelope_container.assigned_types_to_values:
             if arg_type in envelope_container.remaining_types_to_values:
                 if arg_val in envelope_container.remaining_types_to_values[arg_type]:
                     del envelope_container.remaining_types_to_values[arg_type]
                     envelope_container.assigned_types_to_values[arg_type] = AssignedValue(
                         arg_val,
                         ArgSource.DefaultValue,
                     )
+                    return True
         else:
             # Setting `ArgSource.DefaultValue`: it cannot override any, right? No point to handle assigned case:
             pass
+    return False
 
 
 def redirect_to_no_func_error(
     interp_ctx,
     server_config,
 ):
     return redirect_to_error(
@@ -170,15 +172,15 @@
                 {"dc": ServiceArgType.data_center.name},
                 {"ip": ServiceArgType.ip_address.name},
             ],
         )
 
         access_search_control = populate_search_control(
             class_to_collection_map,
-            ServiceArgType.access_type.name,
+            ServiceEnvelopeClass.ClassAccessType.name,
             [
                 {"access": ServiceArgType.access_type.name},
             ],
         )
 
         func_envelopes = [
             {
@@ -266,14 +268,15 @@
         return True
 
     def run_fill_control(
         self,
         interp_ctx: "InterpContext",
     ) -> bool:
         func_id = get_func_id_from_interp_ctx(interp_ctx)
+        any_assignment = False
         if func_id in [
             goto_host_func_,
             goto_service_func_,
         ]:
             assert host_container_ipos_ == service_container_ipos_
             object_container_ipos = host_container_ipos_
 
@@ -289,28 +292,35 @@
                 )]
 
                 # Select default value to search `access_type` `data_envelope` based on `code_maturity`:
                 code_arg_type = ServiceArgType.code_maturity.name
                 if code_arg_type in data_envelope:
                     code_arg_val = data_envelope[code_arg_type]
                     if code_arg_val == "prod":
-                        set_default_to(ServiceArgType.access_type.name, "ro", access_container)
+                        any_assignment = (
+                            set_default_to(ServiceArgType.access_type.name, "ro", access_container)
+                            or
+                            any_assignment
+                        )
                     else:
-                        set_default_to(ServiceArgType.access_type.name, "rw", access_container)
-                    return True
+                        any_assignment = (
+                            set_default_to(ServiceArgType.access_type.name, "rw", access_container)
+                            or
+                            any_assignment
+                        )
 
         elif func_id in [
             list_host_func_,
             list_service_func_,
         ]:
             pass
         else:
             raise RuntimeError
 
-        return False
+        return any_assignment
 
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
         assert interp_ctx.is_func_found(), "the (first) function envelope must be found"
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceLoader.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoader.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         class_to_collection_map: dict = self.server_config.class_to_collection_map
 
         class_names = [
             ServiceEnvelopeClass.ClassCluster.name,
             ServiceEnvelopeClass.ClassHost.name,
             ServiceEnvelopeClass.ClassService.name,
-            ServiceArgType.access_type.name,
+            ServiceEnvelopeClass.ClassAccessType.name,
         ]
 
         init_envelop_collections(
             self.server_config,
             class_names,
             # Same index fields for all collections (can be fine-tuned later):
             lambda collection_name, class_name: [enum_item.name for enum_item in ServiceArgType]
@@ -87,28 +87,33 @@
         host_envelopes = static_data.envelope_collections[
             class_to_collection_map[ServiceEnvelopeClass.ClassHost.name]
         ].data_envelopes
         service_envelopes = static_data.envelope_collections[
             class_to_collection_map[ServiceEnvelopeClass.ClassService.name]
         ].data_envelopes
         access_envelopes = static_data.envelope_collections[
-            class_to_collection_map[ServiceArgType.access_type.name]
+            class_to_collection_map[ServiceEnvelopeClass.ClassAccessType.name]
         ].data_envelopes
 
         self.populate_common_access_type(access_envelopes)
         self.populate_TD_63_37_05_36_default(
             cluster_envelopes,
             host_envelopes,
             service_envelopes,
         )
         self.populate_TD_76_09_29_31_overlapped(
             cluster_envelopes,
             host_envelopes,
             service_envelopes,
         )
+        self.populate_TD_99_99_88_75_mutually_exclusive(
+            cluster_envelopes,
+            host_envelopes,
+            service_envelopes,
+        )
         self.populate_TD_38_03_48_51_large_generated(
             cluster_envelopes,
             host_envelopes,
             service_envelopes,
         )
         self.populate_TD_43_24_76_58_single(
             cluster_envelopes,
@@ -218,21 +223,21 @@
 
             ############################################################################################################
             # `access_type`: FS_24_50_40_64
 
             {
                 envelope_payload_: {
                 },
-                ReservedArgType.EnvelopeClass.name: ServiceArgType.access_type.name,
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassAccessType.name,
                 ServiceArgType.access_type.name: "ro",
             },
             {
                 envelope_payload_: {
                 },
-                ReservedArgType.EnvelopeClass.name: ServiceArgType.access_type.name,
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassAccessType.name,
                 ServiceArgType.access_type.name: "rw",
             },
         ])
 
     def populate_TD_63_37_05_36_default(
         self,
         cluster_envelopes: list[dict],
@@ -1120,24 +1125,37 @@
                 },
                 test_data_: "TD_76_09_29_31",  # overlapped
                 ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
                 ServiceArgType.code_maturity.name: "dev",
                 ServiceArgType.geo_region.name: "amer",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-amer-downstream",
-                # host_name is intentionally mathing another host_name from different geo_region (also named alike):
+                # host_name is intentionally matching another host_name from different geo_region (also named alike):
                 ServiceArgType.host_name.name: "emea",
             },
 
             {
                 envelope_payload_: {
                 },
                 test_data_: "TD_76_09_29_31",  # overlapped
                 ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
                 ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "amer",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-amer-downstream",
+                # host_name is intentionally matching another host_name from different geo_region (also named alike):
+                ServiceArgType.host_name.name: "host-3-amer",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_76_09_29_31",  # overlapped
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
                 # TD_76_09_29_31 geo_region set overlaps with host_name set:
                 ServiceArgType.geo_region.name: "emea",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-emea-downstream",
                 # TD_76_09_29_31 host_name set overlaps with geo_region set:
                 ServiceArgType.host_name.name: "emea",
             },
@@ -1147,17 +1165,119 @@
                 },
                 test_data_: "TD_76_09_29_31",  # overlapped
                 ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
                 ServiceArgType.code_maturity.name: "dev",
                 ServiceArgType.geo_region.name: "emea",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-emea-downstream",
-                # host_name is intentionally mathing another host_name from different geo_region (also named alike):
+                # host_name is intentionally matching another host_name from different geo_region (also named alike):
                 ServiceArgType.host_name.name: "amer",
             },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_76_09_29_31",  # overlapped
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+                # host_name is intentionally matching another host_name from different geo_region (also named alike):
+                ServiceArgType.host_name.name: "host-3-emea",
+            },
+        ])
+
+    def populate_TD_99_99_88_75_mutually_exclusive(
+        self,
+        cluster_envelopes: list[dict],
+        host_envelopes: list[dict],
+        service_envelopes: list[dict],
+    ):
+        if not self.is_test_data_allowed("TD_99_99_88_75"):
+            return
+
+        cluster_envelopes.extend([
+
+            ############################################################################################################
+            # TD_99_99_88_75 # mutually exclusive: clusters
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_99_99_88_75",  # mutually exclusive
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassCluster.name,
+                ServiceArgType.code_maturity.name: "qa",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-amer-downstream",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_99_99_88_75",  # mutually exclusive
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassCluster.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+            },
+        ])
+
+        host_envelopes.extend([
+
+            ############################################################################################################
+            # TD_99_99_88_75 # mutually exclusive: hosts
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_99_99_88_75",  # mutually exclusive
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "qa",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "qa-apac-downstream",
+                ServiceArgType.host_name.name: "host-a-1",
+            },
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_99_99_88_75",  # mutually exclusive
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "qa",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "qa-apac-downstream",
+                ServiceArgType.host_name.name: "host-a-2",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_99_99_88_75",  # mutually exclusive
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+                ServiceArgType.host_name.name: "host-b-1",
+            },
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_99_99_88_75",  # mutually exclusive
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+                ServiceArgType.host_name.name: "host-b-2",
+            },
         ])
 
     def populate_TD_38_03_48_51_large_generated(
         self,
         cluster_envelopes: list[dict],
         host_envelopes: list[dict],
         service_envelopes: list[dict],
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py` & `argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ/git_utils.py` & `argrelay-0.6.9/src/argrelay/custom_integ/git_utils.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/argrelay_common_lib.bash` & `argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_common_lib.bash`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     test -n "${VIRTUAL_ENV}"
 
     # Ensure `@/conf` is already in place:
     test -d "${argrelay_dir}/conf"
 }
 
 function remove_pid_file_if_stale {
-    # Use case: clean up stale pid file.
+    # Use case (FS_86_73_43_45): clean up stale pid file.
 
     pid_file="${1}"
 
     if [[ -f "${pid_file}" ]]
     then
         pid_value="$( cat "${pid_file}" )"
         if [[ -d "/proc/${pid_value}" ]]
@@ -83,15 +83,15 @@
             log_on_stderr "INFO" "pid [${pid_value}] does not have running process, removing pid file [${pid_file}]"
             rm "${pid_file}"
         fi
     fi
 }
 
 function kill_via_pid_file_or_ensure_closed_port {
-    # Use case: trigger server shut down if pid file exists or ensure server is down otherwise.
+    # Use case (FS_86_73_43_45): trigger server shut down if pid file exists or ensure server is down otherwise.
     # Unlike `wait_for_closed_port`, this func does not wait for port to close.
     # It only ensures port is closed when there is no pid file.
 
     pid_file="${1}"
     server_host_name="${2}"
     server_port_number="${3}"
 
@@ -122,15 +122,15 @@
         else
             log_on_stderr "INFO" "port [${server_port_number}] is closed, as expected with missing pid file"
         fi
     fi
 }
 
 function exit_if_port_open {
-    # Use case: do nothing if server is up (exit current process).
+    # Use case (FS_86_73_43_45): do nothing if server is up (exit current process).
 
     server_host_name="${1}"
     server_port_number="${2}"
 
     set +e
     # Note that it is only assumed that the right server runs on that port
     # (no way to 100% ensure it is not something else):
@@ -144,15 +144,15 @@
         exit 0
     else
         log_on_stderr "INFO" "port [${server_port_number}] is closed, need to start server"
     fi
 }
 
 function wait_for_open_port {
-    # Use case: ensure server is up before return.
+    # Use case (FS_86_73_43_45): ensure server is up before return.
 
     timeout_sec="${1}"
     pid_file="${2}"
     server_host_name="${3}"
     server_port_number="${4}"
 
     end_time_sec="$(( $( date "+%s" ) + ${timeout_sec} ))"
@@ -178,15 +178,15 @@
         sleep 5
     done
 
     log_on_stderr "INFO" "port is open now: ${server_host_name}:${server_port_number}"
 }
 
 function wait_for_closed_port {
-    # Use case: ensure server is down before return.
+    # Use case  (FS_86_73_43_45): ensure server is down before return.
     # Unlike `kill_via_pid_file_or_ensure_closed_port`, this func does not trigger server shut down.
 
     timeout_sec="${1}"
     server_host_name="${2}"
     server_port_number="${3}"
 
     end_time_sec="$(( $( date "+%s" ) + ${timeout_sec} ))"
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/argrelay_rc.bash` & `argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_rc.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/bootstrap_dev_env.bash` & `argrelay-0.6.9/src/argrelay/custom_integ_res/bootstrap_dev_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/dev_shell.bash` & `argrelay-0.6.9/src/argrelay/custom_integ_res/dev_shell.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/init_shell_env.bash` & `argrelay-0.6.9/src/argrelay/custom_integ_res/init_shell_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/custom_integ_res/upgrade_all_packages.bash` & `argrelay-0.6.9/src/argrelay/custom_integ_res/upgrade_all_packages.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/ArgSource.py` & `argrelay-0.6.9/src/argrelay/enum_desc/ArgSource.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/CallConv.py` & `argrelay-0.6.9/src/argrelay/enum_desc/CallConv.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/CompScope.py` & `argrelay-0.6.9/src/argrelay/enum_desc/CompScope.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/CompType.py` & `argrelay-0.6.9/src/argrelay/enum_desc/CompType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/DistinctValuesQuery.py` & `argrelay-0.6.9/src/argrelay/enum_desc/DistinctValuesQuery.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,27 +17,27 @@
         ================================
         use_mongomock: True
         use_single_collection: True
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.009     0.030     0.115     0.440     1.632     6.137    33.669
-                         native_distinct     0.038     0.122     0.363     0.969     2.183     4.740     7.102
-                        native_aggregate     0.044     0.151     0.679     2.899    13.257    49.728   292.153
+                  original_find_and_loop     0.011     0.035     0.122     0.461     1.650     5.945    27.836
+                         native_distinct     0.062     0.192     0.576     1.455     2.993     6.287    10.603
+                        native_aggregate     0.084     0.212     0.909     3.650    15.173    58.340   326.188
         ================================
         use_mongomock: True
         use_single_collection: False
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.006     0.018     0.113     0.414     1.662     5.831    29.375
-                         native_distinct     0.027     0.096     0.327     0.812     1.830     3.578     6.403
-                        native_aggregate     0.020     0.066     0.258     1.108     4.923    17.561    95.461
+                  original_find_and_loop     0.007     0.028     0.096     0.439     1.672     5.939    27.561
+                         native_distinct     0.048     0.159     0.465     1.224     2.725     5.539     9.572
+                        native_aggregate     0.031     0.109     0.398     1.758     7.802    28.463   126.566
         ```
 
         *   The fastest on small collections is `original_find_and_loop`.
         *   The fastest on large collections is `native_distinct`.
 
     *   `pymongo`:
 
@@ -45,27 +45,27 @@
         ================================
         use_mongomock: False
         use_single_collection: True
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.013     0.023     0.043     0.090     0.182     0.428     0.746
-                         native_distinct     0.041     0.065     0.117     0.241     0.462     0.796     1.458
-                        native_aggregate     0.022     0.027     0.050     0.081     0.125     0.210     0.368
+                  original_find_and_loop     0.022     0.031     0.065     0.115     0.222     0.505     0.748
+                         native_distinct     0.063     0.102     0.195     0.435     0.857     1.493     2.591
+                        native_aggregate     0.022     0.038     0.064     0.109     0.165     0.324     0.469
         ================================
         use_mongomock: False
         use_single_collection: False
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.015     0.020     0.039     0.087     0.148     0.345     0.633
-                         native_distinct     0.044     0.048     0.087     0.173     0.299     0.512     0.903
-                        native_aggregate     0.016     0.021     0.033     0.054     0.086     0.159     0.231
+                  original_find_and_loop     0.020     0.025     0.048     0.144     0.175     0.383     0.590
+                         native_distinct     0.048     0.067     0.123     0.228     0.365     0.594     0.991
+                        native_aggregate     0.022     0.027     0.040     0.067     0.109     0.176     0.271
         ```
 
         The fastest is `native_aggregate`.
     """
 
     original_find_and_loop = auto()
     """
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/ReservedArgType.py` & `argrelay-0.6.9/src/argrelay/enum_desc/ReservedArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/RunMode.py` & `argrelay-0.6.9/src/argrelay/enum_desc/RunMode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/TermColor.py` & `argrelay-0.6.9/src/argrelay/enum_desc/TermColor.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/enum_desc/TokenType.py` & `argrelay-0.6.9/src/argrelay/enum_desc/TokenType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/handler_request/AbstractServerRequestHandler.py` & `argrelay-0.6.9/src/argrelay/handler_request/AbstractServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py` & `argrelay-0.6.9/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py` & `argrelay-0.6.9/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py` & `argrelay-0.6.9/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py` & `argrelay-0.6.9/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py` & `argrelay-0.6.9/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py` & `argrelay-0.6.9/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/misc_helper_common/ElapsedTime.py` & `argrelay-0.6.9/src/argrelay/misc_helper_common/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/misc_helper_common/TypeDesc.py` & `argrelay-0.6.9/src/argrelay/misc_helper_common/TypeDesc.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/misc_helper_common/__init__.py` & `argrelay-0.6.9/src/argrelay/misc_helper_common/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/misc_helper_server/__init__.py` & `argrelay-0.6.9/src/argrelay/misc_helper_server/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoClientWrapper.py` & `argrelay-0.6.9/src/argrelay/mongo_data/MongoClientWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoConfig.py` & `argrelay-0.6.9/src/argrelay/mongo_data/MongoConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/mongo_data/MongoServerWrapper.py` & `argrelay-0.6.9/src/argrelay/mongo_data/MongoServerWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_config/AbstractConfigurator.py` & `argrelay-0.6.9/src/argrelay/plugin_config/AbstractConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_config/DefaultConfigurator.py` & `argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_config/DefaultConfiguratorConfig.py` & `argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py` & `argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/AbstractDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/AbstractJumpDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractJumpDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/EchoDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/EchoDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/ErrorDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/HelpDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/HelpDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/InterceptDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/InterceptDelegator.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
     json_format = auto()
     repr_format = auto()
     text_format = auto()
     table_format = auto()
 
 
-# TODO: Add searching for `json` or `repr` param:
 class InterceptDelegator(AbstractJumpDelegator):
 
     def get_supported_func_envelopes(
         self,
     ) -> list[dict]:
 
         class_to_collection_map: dict = self.server_config.class_to_collection_map
@@ -77,25 +76,30 @@
         return True
 
     def run_fill_control(
         self,
         interp_ctx: InterpContext,
     ) -> bool:
         func_id = get_func_id_from_interp_ctx(interp_ctx)
+        any_assignment = False
         if func_id in [
             SpecialFunc.intercept_invocation_func.name,
         ]:
             # If we need to specify `output_format_class_name` `data_envelope`:
             if interp_ctx.curr_container_ipos == interp_ctx.curr_interp.base_container_ipos + format_output_container_ipos_:
                 format_output_container = interp_ctx.envelope_containers[(
                     interp_ctx.curr_interp.base_container_ipos + format_output_container_ipos_
                 )]
-                set_default_to(output_format_prop_name, OutputFormat.json_format.name, format_output_container)
-                return True
-        return False
+                any_assignment = (
+                    set_default_to(output_format_prop_name, OutputFormat.json_format.name, format_output_container)
+                    or
+                    any_assignment
+                )
+
+        return any_assignment
 
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
         assert interp_ctx.is_func_found(), "the (first) function envelope must be found"
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/NoopDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/NoopDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_delegator/QueryEnumDelegator.py` & `argrelay-0.6.9/src/argrelay/plugin_delegator/QueryEnumDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/AbstractInterpFactory.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/AbstractInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FirstArgInterp.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FirstArgInterpFactory.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FuncTreeInterp.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterp.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,45 +94,69 @@
         # Function `search_control` is populated based on
         # tree path (FS_01_89_09_24 interp tree + FS_26_43_73_72 func tree)
         # and plugin config (rather than data found in `data_envelope`):
         self.interp_ctx.curr_container.search_control = search_control_desc.dict_schema.load(
             self.interp_tree_node_config_dict[func_search_control_]
         )
 
-    def consume_key_args(self) -> None:
-        # TODO: FS_20_88_05_60 named args: stub
-        pass
 
-    def consume_pos_args(self) -> None:
+    def consume_pos_args(self) -> bool:
         """
         Scans through `unconsumed_tokens` and tries to match its value against values of each type.
+
+        Implements:
+        *   FS_76_29_13_28 arg consumption priorities
+        *   FS_44_36_84_88 consume args one by one
+            This func consumes all until the first unconsumed non-singled out arg.
         """
 
         consumed_token_ipos_list = []
+        any_consumed = False
+        # Related to FS_13_51_07_97 singled out implicit values:
+        # Whether we can consume more than one (without creating FS_51_67_38_37 impossible arg combinations)
+        # depends on whether first set of consumed args are already singled out.
+        # If arg is singled out but still matches unconsumed arg, it must be assigned as `ArgSource.ExplicitPosArg`
+        # rather than be left unconsumed and (later) be assigned as `ArgSource.ImplicitValue`.
+        can_consume_more = True
         for unconsumed_token_ipos in self.interp_ctx.unconsumed_tokens:
             unconsumed_token = self.interp_ctx.parsed_ctx.all_tokens[unconsumed_token_ipos]
-            # See if token matches any type by value:
 
+            # TODO: FS_76_29_13_28 Why not define the order based on FS_31_70_49_15 `search_control`
+            #       (instead of whatever internal order `remaining_types_to_values` has)?
+            #       It could already be the case that `remaining_types_to_values` are ordered as `search_control`.
+            #       Why not make it explicit?
+
+            # See if token matches any type by value:
             for arg_type, arg_values in self.interp_ctx.curr_container.remaining_types_to_values.items():
                 if unconsumed_token in arg_values:
                     self.interp_ctx.curr_container.assigned_types_to_values[arg_type] = AssignedValue(
                         unconsumed_token,
                         ArgSource.ExplicitPosArg,
                     )
+                    if len(arg_values) != 1:
+                        # This was not singled out arg:
+                        # stop consuming to avoid FS_51_67_38_37 impossible arg combinations.
+                        can_consume_more = False
+                    any_consumed = True
                     consumed_token_ipos_list.append(unconsumed_token_ipos)
                     self.interp_ctx.consumed_tokens.append(unconsumed_token_ipos)
                     # TD_76_09_29_31: overlapped
                     # Assign matching unconsumed arg value to the first type it matches (only once):
                     del self.interp_ctx.curr_container.remaining_types_to_values[arg_type]
                     break
 
+            if not can_consume_more:
+                break
+
         # perform list modifications out of the prev loop:
         for consumed_token_ipos in consumed_token_ipos_list:
             self.interp_ctx.unconsumed_tokens.remove(consumed_token_ipos)
 
+        return any_consumed
+
     def try_iterate(self) -> InterpStep:
         """
         Try to consume more args if possible.
 
         *   If function was found, start with search for its first envelope class.
         *   If curr envelope class is found, move to the next (until all are found).
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FuncTreeInterpFactory.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/InterpTreeInterp.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterp.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,30 +48,37 @@
         self.next_interp_factory_id: Union[str, None] = None
         self.interp_tree_rel_path: list[str] = []
 
         # TODO: Why hard-coded? Isn't it possible for this plugin to be plugged into any depth of the tree?
         # Token with ipos = 0 is the command name eaten by `FirstArgInterp` (FS_42_76_93_51 first interp):
         self.base_token_ipos: int = 1
 
-    def consume_pos_args(self) -> None:
+    def consumes_args_at_once(self) -> bool:
+        return True
+
+    def consume_pos_args(self) -> bool:
         """
         Consumes heading args in `unconsumed_tokens` according to the `interp_selector_tree`.
+
+        Unlike normal guideline to consume one arg at time (FS_44_36_84_88), this func consumes all possible
+        because args are selected according to the `interp_selector_tree` (not via query)
+        and do not become incompatible by consuming all (causing FS_51_67_38_37 impossible arg combinations).
         """
 
-        self.interp_tree_rel_path: list[str] = []
         curr_sub_tree = self.interp_selector_tree
+        any_consumed = False
         while True:
             if isinstance(curr_sub_tree, str):
                 # Tree leaf is reached - use it:
                 self.next_interp_factory_id = curr_sub_tree
-                return
+                return any_consumed
 
             if not self.interp_ctx.unconsumed_tokens:
                 self.set_default_factory_id(curr_sub_tree)
-                return
+                return any_consumed
 
             # Always consume next unconsumed token:
             # TODO: Is this assumption valid/safe that next unconsumed `ipos` is in the order it appears on command line?
             #       Apparently, it is fine as we keep deleting head of `unconsumed_tokens` below:
             curr_token_ipos = self.interp_ctx.unconsumed_tokens[0]
             curr_token_value = self.interp_ctx.parsed_ctx.all_tokens[curr_token_ipos]
             assert self.is_pos_arg(curr_token_ipos)
@@ -79,18 +86,19 @@
             if isinstance(curr_sub_tree, dict):
                 if curr_token_value in curr_sub_tree:
                     # Consume one more arg into path:
                     self.interp_tree_rel_path.append(curr_token_value)
                     self.interp_ctx.consumed_tokens.append(curr_token_ipos)
                     del self.interp_ctx.unconsumed_tokens[0]
                     curr_sub_tree = curr_sub_tree[curr_token_value]
+                    any_consumed = True
                     continue
                 else:
                     self.set_default_factory_id(curr_sub_tree)
-                    return
+                    return any_consumed
             else:
                 raise LookupError()
 
     def set_default_factory_id(
         self,
         curr_sub_tree,
     ):
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/InterpTreeInterpFactory.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/NoopInterpFactory.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/NoopInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/plugin_interp/TreeWalker.py` & `argrelay-0.6.9/src/argrelay/plugin_interp/TreeWalker.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_client/AbstractClient.py` & `argrelay-0.6.9/src/argrelay/relay_client/AbstractClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_client/RemoteClient.py` & `argrelay-0.6.9/src/argrelay/relay_client/RemoteClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_client/RemoteClientCommandFactory.py` & `argrelay-0.6.9/src/argrelay/relay_client/RemoteClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_client/__main__.py` & `argrelay-0.6.9/src/argrelay/relay_client/__main__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_client/proc_parent.py` & `argrelay-0.6.9/src/argrelay/relay_client/proc_parent.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_client/proc_split.py` & `argrelay-0.6.9/src/argrelay/relay_client/proc_split.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/CustomFlaskApp.py` & `argrelay-0.6.9/src/argrelay/relay_server/CustomFlaskApp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/HelpHintCache.py` & `argrelay-0.6.9/src/argrelay/relay_server/HelpHintCache.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/LocalServer.py` & `argrelay-0.6.9/src/argrelay/relay_server/LocalServer.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/QueryEngine.py` & `argrelay-0.6.9/src/argrelay/relay_server/QueryEngine.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/QueryResult.py` & `argrelay-0.6.9/src/argrelay/relay_server/QueryResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_static/argrelay_client.js` & `argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_client.js`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_static/argrelay_style.css` & `argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_style.css`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/gui_templates/argrelay_main.html` & `argrelay-0.6.9/src/argrelay/relay_server/gui_templates/argrelay_main.html`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/route_api.py` & `argrelay-0.6.9/src/argrelay/relay_server/route_api.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/relay_server/route_gui.py` & `argrelay-0.6.9/src/argrelay/relay_server/route_gui.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_context/AbstractPlugin.py` & `argrelay-0.6.9/src/argrelay/runtime_context/AbstractPlugin.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_context/EnvelopeContainer.py` & `argrelay-0.6.9/src/argrelay/runtime_context/EnvelopeContainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     Only keys for those `arg_type`-s which have `ArgSource.InitValue` in `assigned_types_to_values` are listed here.
     """
 
     def populate_implicit_arg_values(
         self,
     ) -> bool:
         """
+        When possible arg_values are singled out, assign them as `ArgSource.ImplicitValue`.
+
         When `data_envelope` is singled out, all remaining single-value `arg_type`-s become `ArgSource.ImplicitValue`.
 
         Implements FS_13_51_07_97 singled out implicit values.
 
         Return:
         *   True if any value was assigned.
         *   False otherwise.
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_context/InterpContext.py` & `argrelay-0.6.9/src/argrelay/runtime_context/InterpContext.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,89 +144,111 @@
             self.curr_container.assigned_types_to_values,
         )
         self.curr_container.remaining_types_to_values = query_result.remaining_types_to_values
         self.curr_container.data_envelopes = query_result.data_envelopes
         self.curr_container.found_count = query_result.found_count
         ElapsedTime.measure(f"end_query_envelopes: {query_dict} {self.curr_container.found_count}")
 
-    # TODO: Move all dynamic and non-serializable objects into `InterpRuntime` (or something like that) together with this loop:
-    def interpret_command(
+    def consume_args(
         self,
-        first_interp_factory_id: str,
-    ) -> None:
-        """
-        Implements FS_55_57_45_04 enum selector version of FS_15_79_76_85 line processor.
-
-        Start with initial interpreter and continue until curr interpreter returns no more next interpreter.
-        """
-
-        interp_n: int = 0
-
-        # FS_01_89_09_24 interp tree:
-        # start of tracking interp tree abs path while processing command
-        # (to pass it to the next interp factory to create next interp):
-        self.interp_tree_abs_path = tuple([])
-
-        self.curr_interp = self.create_next_interp(first_interp_factory_id)
+        interp_n: int
+    ):
+        # Query envelope values only - they will be used for consumption of command line args:
+        ElapsedTime.measure(f"[i={interp_n}]: before_init_query: {self.curr_interp}")
+        self.query_prop_values()
         while True:
-            interp_n += 1
-
-            # Query envelope values only - they will be used for consumption of command line args:
-            ElapsedTime.measure(f"[i={interp_n}]: before_init_query: {self.curr_interp}")
-            self.query_prop_values()
+            # Reset to False as we just executed new query:
+            query_changed = False
+            arg_was_consumed = False
 
             # Because each `prop_value` set (per `prop_type`) is treated independently,
             # assignment of `prop_value`-s from args may set combinations
             # which yields no search result in subsequent query.
             # Logically, it is better to consume args one by one and running query after each consumption,
             # but this is not done due to query overhead.
             # Note that Tab-completion and selection (via manual step by human) in separate requests to server and
             # separate `interpret_command` calls is close to that logically better approach.
-            ElapsedTime.measure(f"[i={interp_n}]: before_consume_args: {self.curr_interp}")
-            self.curr_interp.consume_key_args()
-            self.curr_interp.consume_pos_args()
+            if not query_changed:
+                ElapsedTime.measure(f"[i={interp_n}]: before_consume_key_args: {self.curr_interp}")
+                arg_was_consumed = self.curr_interp.consume_key_args()
+                query_changed = arg_was_consumed
+            if not query_changed:
+                ElapsedTime.measure(f"[i={interp_n}]: before_consume_pos_args: {self.curr_interp}")
+                arg_was_consumed = self.curr_interp.consume_pos_args()
+                query_changed = arg_was_consumed
 
-            ElapsedTime.measure(f"[i={interp_n}]: before_reduce_query: {self.curr_interp}")
-            self.query_prop_values()
-            # Reset to False as we just executed new query:
-            query_changed = False
+            if query_changed:
+                ElapsedTime.measure(f"[i={interp_n}]: before_reduce_query: {self.curr_interp}")
+                self.query_prop_values()
+                query_changed = False
 
             if self.curr_container:
-                query_changed = (
-                    self.curr_container.populate_implicit_arg_values()
-                    or
-                    query_changed
-                )
+                # Set implicit values (so that applying defaults knows what they are):
+                self.curr_container.populate_implicit_arg_values()
 
             if self.curr_interp.has_fill_control():
                 if self.parsed_ctx.server_action is ServerAction.DescribeLineArgs:
                     # TODO: FS_72_53_55_13: options before defaults
                     # Describing args will need to show options except default - query values before defaults:
                     ElapsedTime.measure(f"[i={interp_n}]: before_query_without_defaults: {self.curr_interp}")
                     self.query_prop_values()
                     # Reset to False as we just executed new query:
                     query_changed = False
 
                     self._save_potentially_hidden_by_defaults()
 
-                # Apply defaults:
+                # Apply defaults (they may apply more than single value at a time):
                 query_changed = (
                     self.curr_interp.delegate_fill_control()
                     or
                     query_changed
                 )
                 self._leave_only_hidden_by_defaults()
 
+
             # Query envelopes after all implicit and default values assigned:
             # TODO: We could probably select whether to query only envelopes or
             #       query their values depending on `ServerAction`.
             #       But init of next envelope depends on prev envelope found.
             if query_changed:
                 ElapsedTime.measure(f"[i={interp_n}]: before_final_query: {self.curr_interp}")
                 self.query_prop_values()
+                if self.curr_interp.consumes_args_at_once():
+                    break
+            elif arg_was_consumed:
+                # Run next cycle to see if one more can be consumed:
+                if self.curr_interp.consumes_args_at_once():
+                    break
+            else:
+                break
+
+
+    # TODO: Move all dynamic and non-serializable objects into `InterpRuntime` (or something like that) together with this loop:
+    def interpret_command(
+        self,
+        first_interp_factory_id: str,
+    ) -> None:
+        """
+        Implements FS_55_57_45_04 enum selector version of FS_15_79_76_85 line processor.
+
+        Start with initial interpreter and continue until curr interpreter returns no more next interpreter.
+        """
+
+        interp_n: int = 0
+
+        # FS_01_89_09_24 interp tree:
+        # start of tracking interp tree abs path while processing command
+        # (to pass it to the next interp factory to create next interp):
+        self.interp_tree_abs_path = tuple([])
+
+        self.curr_interp = self.create_next_interp(first_interp_factory_id)
+        while True:
+            interp_n += 1
+
+            self.consume_args(interp_n)
 
             ElapsedTime.measure(f"[i={interp_n}]: before_try_iterate: {self.curr_interp}")
             interp_step: InterpStep = self.curr_interp.try_iterate()
             ElapsedTime.measure(f"[i={interp_n}]: after_try_iterate: {self.curr_interp}: {interp_step}")
             if interp_step is InterpStep.NextEnvelope:
                 continue
             elif interp_step is InterpStep.StopAll:
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_context/ParsedContext.py` & `argrelay-0.6.9/src/argrelay/runtime_context/ParsedContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_context/SearchControl.py` & `argrelay-0.6.9/src/argrelay/runtime_context/SearchControl.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_data/EnvelopeCollection.py` & `argrelay-0.6.9/src/argrelay/runtime_data/EnvelopeCollection.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_data/ServerConfig.py` & `argrelay-0.6.9/src/argrelay/runtime_data/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/runtime_data/StaticData.py` & `argrelay-0.6.9/src/argrelay/runtime_data/StaticData.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/sample_conf/argrelay.server.yaml` & `argrelay-0.6.9/src/argrelay/sample_conf/argrelay.server.yaml`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_client/ClientConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_client/ClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/MongoConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/ServerConfigSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerConfigSchema.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         mongo_config_: mongo_config_desc.dict_example,
         query_cache_config_: query_cache_config_desc.dict_example,
         gui_banner_config_: gui_banner_config_desc.dict_example,
         class_to_collection_map_: {
             ServiceEnvelopeClass.ClassCluster.name: ServiceEnvelopeClass.ClassCluster.name,
             ServiceEnvelopeClass.ClassHost.name: ServiceEnvelopeClass.ClassHost.name,
             ServiceEnvelopeClass.ClassService.name: ServiceEnvelopeClass.ClassService.name,
-            ServiceArgType.access_type.name: ServiceArgType.access_type.name,
+            ServiceEnvelopeClass.ClassAccessType.name: ServiceEnvelopeClass.ClassAccessType.name,
         },
         server_plugin_control_: server_plugin_control_desc.dict_example,
         plugin_instance_entries_: {
             "some_plugin_instance_id": plugin_entry_desc.dict_example,
             "some_plugin_instance_id1": plugin_entry_desc.dict_example,
             "some_plugin_instance_id2": plugin_entry_desc.dict_example,
         },
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_core_server/StaticDataSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_core_server/StaticDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/DataEnvelopeSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_interp/DataEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/InitControlSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_interp/InitControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_interp/SearchControlSchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_interp/SearchControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_config_plugin/PluginEntrySchema.py` & `argrelay-0.6.9/src/argrelay/schema_config_plugin/PluginEntrySchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_request/CallContextSchema.py` & `argrelay-0.6.9/src/argrelay/schema_request/CallContextSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_response/ArgValuesSchema.py` & `argrelay-0.6.9/src/argrelay/schema_response/ArgValuesSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_response/AssignedValueSchema.py` & `argrelay-0.6.9/src/argrelay/schema_response/AssignedValueSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_response/EnvelopeContainerSchema.py` & `argrelay-0.6.9/src/argrelay/schema_response/EnvelopeContainerSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_response/InterpResult.py` & `argrelay-0.6.9/src/argrelay/schema_response/InterpResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_response/InterpResultSchema.py` & `argrelay-0.6.9/src/argrelay/schema_response/InterpResultSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_response/InvocationInput.py` & `argrelay-0.6.9/src/argrelay/schema_response/InvocationInput.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/schema_response/InvocationInputSchema.py` & `argrelay-0.6.9/src/argrelay/schema_response/InvocationInputSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/server_spec/CallContext.py` & `argrelay-0.6.9/src/argrelay/server_spec/CallContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/server_spec/DescribeLineArgsSpec.py` & `argrelay-0.6.9/src/argrelay/server_spec/DescribeLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/server_spec/ProposeArgValuesSpec.py` & `argrelay-0.6.9/src/argrelay/server_spec/ProposeArgValuesSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/server_spec/RelayLineArgsSpec.py` & `argrelay-0.6.9/src/argrelay/server_spec/RelayLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/server_spec/const_int.py` & `argrelay-0.6.9/src/argrelay/server_spec/const_int.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/server_spec/server_data_schema.py` & `argrelay-0.6.9/src/argrelay/server_spec/server_data_schema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/BaseTestClass.py` & `argrelay-0.6.9/src/argrelay/test_infra/BaseTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/ClientServerTestClass.py` & `argrelay-0.6.9/src/argrelay/test_infra/ClientServerTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/CustomTestCase.py` & `argrelay-0.6.9/src/argrelay/test_infra/CustomTestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/CustomVerifier.py` & `argrelay-0.6.9/src/argrelay/test_infra/CustomVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/End2EndTestClass.py` & `argrelay-0.6.9/src/argrelay/test_infra/End2EndTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/EnvMockBuilder.py` & `argrelay-0.6.9/src/argrelay/test_infra/EnvMockBuilder.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/InOutTestClass.py` & `argrelay-0.6.9/src/argrelay/test_infra/InOutTestClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         envelope_ipos_to_field_values: Union[dict[int, dict[str, str]], None],
         expected_suggestions: Union[list[str], None],
         envelope_containers: list[EnvelopeContainer],
     ):
         try:
 
             if expected_suggestions is not None:
-                # If `expected_suggestions`, verify them:
                 self.assertEqual(expected_suggestions, actual_suggestions)
 
             if container_ipos_to_expected_assignments is not None:
                 self.verify_envelope_containers(
                     envelope_containers,
                     container_ipos_to_expected_assignments,
                 )
@@ -76,23 +75,20 @@
 
             # Check if there are some obvious test input mistakes:
 
             if call_ctx.server_action is ServerAction.ProposeArgValues:
                 self.assertIsNone(delegator_class)
                 self.assertIsNone(envelope_ipos_to_field_values)
             elif call_ctx.server_action is ServerAction.DescribeLineArgs:
-                # TODO: TODO_11_77_28_50 suggestions are already in all responses:
-                self.assertIsNone(expected_suggestions)
                 # TODO: TODO_42_81_01_90: assert data instead of print out: there will be no delegator_class, but a mock to intercept response for enum query:
                 self.assertIsNone(delegator_class)
                 # TODO: TODO_42_81_01_90: assert data instead of print out: the data should be available:
                 self.assertIsNone(envelope_ipos_to_field_values)
             elif call_ctx.server_action is ServerAction.RelayLineArgs:
-                # TODO: TODO_11_77_28_50 suggestions are already in all responses:
-                self.assertIsNone(expected_suggestions)
+                pass
             else:
                 raise RuntimeError
 
             # Rethrow previous error:
             raise
 
     def verify_envelope_containers(
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/JsonTestOutputVerifier.py` & `argrelay-0.6.9/src/argrelay/test_infra/JsonTestOutputVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/LocalClient.py` & `argrelay-0.6.9/src/argrelay/test_infra/LocalClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/LocalClientCommandFactory.py` & `argrelay-0.6.9/src/argrelay/test_infra/LocalClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/LocalTestClass.py` & `argrelay-0.6.9/src/argrelay/test_infra/LocalTestClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,27 +41,27 @@
         test_line: str,
         comp_type: CompType,
         expected_suggestions: Union[list[str], None],
         container_ipos_to_expected_assignments: Union[dict[int, dict[str, AssignedValue]], None],
         delegator_class: Union[Type[AbstractDelegator], None],
         envelope_ipos_to_field_values: Union[dict[int, dict[str, str]], None],
     ):
-        self.verify_output_with_via_local_client(
+        self.verify_output_via_local_client(
             test_data,
             test_line,
             comp_type,
             expected_suggestions,
             container_ipos_to_expected_assignments,
             None,
             delegator_class,
             envelope_ipos_to_field_values,
             LocalClientEnvMockBuilder(),
         )
 
-    def verify_output_with_via_local_client(
+    def verify_output_via_local_client(
         self,
         test_data: str,
         test_line: str,
         comp_type: CompType,
         expected_suggestions: Union[list[str], None],
         container_ipos_to_expected_assignments: Union[dict[int, dict[str, AssignedValue]], None],
         container_ipos_to_options_hidden_by_default_value: Union[dict[int, dict[str, list[str]]], None],
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/OpenFileMock.py` & `argrelay-0.6.9/src/argrelay/test_infra/OpenFileMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/PopenMock.py` & `argrelay-0.6.9/src/argrelay/test_infra/PopenMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/RemoteTestClass.py` & `argrelay-0.6.9/src/argrelay/test_infra/RemoteTestClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Supports FS_66_17_43_42 test_infra / special test mode #2.
 
     This class is similar to `LocalTestClass` as it is supposed to use `EnvMockBuilder`
     to capture server response, but, unlike `LocalTestClass`, requests go to separate OS process with running server.
     """
 
     # TODO: Allow intercepting subprocess.* invocation and asserting their input (e.g. whether specific command was invoked).
-    def verify_output_with_via_remote_client(
+    def verify_output_via_remote_client(
         self,
         test_line: str,
         comp_type: CompType,
         expected_suggestions: Union[list[str], None],
         container_ipos_to_expected_assignments: Union[dict[int, dict[str, AssignedValue]], None],
         delegator_class: Union[Type[AbstractDelegator], None],
         envelope_ipos_to_field_values: Union[dict[int, dict[str, str]], None],
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/ServerOnlyTestClass.py` & `argrelay-0.6.9/src/argrelay/test_infra/ServerOnlyTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/TestCase.py` & `argrelay-0.6.9/src/argrelay/test_infra/TestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay/test_infra/__init__.py` & `argrelay-0.6.9/src/argrelay/test_infra/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.8.dev2/src/argrelay.egg-info/PKG-INFO` & `argrelay-0.6.9/src/argrelay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.6.8.dev2
+Version: 0.6.9
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.6.8.dev2/src/argrelay.egg-info/SOURCES.txt` & `argrelay-0.6.9/src/argrelay.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 ./docs/feature_stories/FS_33_76_82_84.global_tree.md
 ./docs/feature_stories/FS_36_17_84_44.check_script.md
 ./docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
 ./docs/feature_stories/FS_39_58_01_91.query_cache.md
 ./docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
 ./docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
 ./docs/feature_stories/FS_43_50_57_71.echo_args_func.md
+./docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
 ./docs/feature_stories/FS_46_96_59_05.init_control.md
 ./docs/feature_stories/FS_47_63_35_61.env_vars.md
 ./docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
 ./docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
 ./docs/feature_stories/FS_53_81_66_18.types_and_classes.md
 ./docs/feature_stories/FS_55_57_45_04.enum_selector.md
 ./docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
@@ -69,22 +70,23 @@
 ./docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
 ./docs/feature_stories/FS_66_17_43_42.test_infra.md
 ./docs/feature_stories/FS_67_16_61_97.git_plugin.md
 ./docs/feature_stories/FS_71_87_33_52.help_hint.md
 ./docs/feature_stories/FS_72_40_53_00.fill_control.md
 ./docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
 ./docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
+./docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
 ./docs/feature_stories/FS_78_91_27_22.interp_control.md
 ./docs/feature_stories/FS_80_45_89_81.integrated_functions.md
 ./docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
 ./docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
 ./docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
 ./docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
 ./docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
-./docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
+./docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
 ./docs/feature_stories/FS_91_88_07_23.jump_tree.md
 ./docs/feature_stories/FS_92_75_93_01.clean_command_line.md
 ./docs/feature_stories/FS_94_30_49_28.help_doc.md
 ./docs/feature_stories/FS_98_55_40_77.invoke_control.md
 ./docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
 ./docs/feature_stories/readme.md
 ./docs/release_notes/readme.md
@@ -118,27 +120,29 @@
 ./docs/task_refs/TODO_37_15_12_91.Popen_mock.md
 ./docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
 ./docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
 ./docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
 ./docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
 ./docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
 ./docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
+./docs/task_refs/TODO_70_48_96_29.be_able_to_assert_unconsumed_arg_vals.md
 ./docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
 ./docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
 ./docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
 ./docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
 ./docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
 ./docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
 ./docs/task_refs/readme.md
 ./docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
 ./docs/test_data/TD_38_03_48_51.large_data_set.md
 ./docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
 ./docs/test_data/TD_63_37_05_36.demo_services_data.md
 ./docs/test_data/TD_70_69_38_46.no_data.md
 ./docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
+./docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
 ./docs/test_data/readme.md
 ./src/argrelay/__init__.py
 ./src/argrelay.egg-info/PKG-INFO
 ./src/argrelay.egg-info/SOURCES.txt
 ./src/argrelay.egg-info/dependency_links.txt
 ./src/argrelay.egg-info/requires.txt
 ./src/argrelay.egg-info/top_level.txt
@@ -382,15 +386,14 @@
 docs/feature_stories/FS_58_61_77_69.dev_shell.md
 docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
 docs/feature_stories/FS_62_25_92_06.assigned_context.md
 docs/feature_stories/FS_71_87_33_52.help_hint.md
 docs/feature_stories/FS_72_40_53_00.fill_control.md
 docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
 docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
-docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
 docs/feature_stories/FS_94_30_49_28.help_doc.md
 docs/feature_stories/readme.md
 docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
 docs/test_data/TD_38_03_48_51.large_data_set.md
 docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
 docs/test_data/TD_63_37_05_36.demo_services_data.md
 docs/test_data/TD_70_69_38_46.no_data.md
@@ -434,15 +437,14 @@
 src/argrelay/../../docs/feature_stories/FS_58_61_77_69.dev_shell.md
 src/argrelay/../../docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
 src/argrelay/../../docs/feature_stories/FS_62_25_92_06.assigned_context.md
 src/argrelay/../../docs/feature_stories/FS_71_87_33_52.help_hint.md
 src/argrelay/../../docs/feature_stories/FS_72_40_53_00.fill_control.md
 src/argrelay/../../docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
 src/argrelay/../../docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
-src/argrelay/../../docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
 src/argrelay/../../docs/feature_stories/FS_94_30_49_28.help_doc.md
 src/argrelay/../../docs/feature_stories/readme.md
 src/argrelay/../../docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
 src/argrelay/../../docs/test_data/TD_38_03_48_51.large_data_set.md
 src/argrelay/../../docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
 src/argrelay/../../docs/test_data/TD_63_37_05_36.demo_services_data.md
 src/argrelay/../../docs/test_data/TD_70_69_38_46.no_data.md
```


# Comparing `tmp/argrelay-0.7.1.dev9.tar.gz` & `tmp/argrelay-0.7.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argrelay-0.7.1.dev9.tar", last modified: Sat May 25 05:50:56 2024, max compression
+gzip compressed data, was "argrelay-0.7.2.dev0.tar", last modified: Sun Jun  2 14:52:42 2024, max compression
```

## Comparing `argrelay-0.7.1.dev9.tar` & `argrelay-0.7.2.dev0.tar`

### file list

```diff
@@ -1,417 +1,425 @@
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.470121 argrelay-0.7.1.dev9/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2024-05-19 10:16:55.000000 argrelay-0.7.1.dev9/LICENSE
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-25 05:50:56.469121 argrelay-0.7.1.dev9/PKG-INFO
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.424121 argrelay-0.7.1.dev9/docs/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.427121 argrelay-0.7.1.dev9/docs/dev_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5535 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/dev_notes/bootstrap_procedure.1.project_creation.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2509 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1924 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/brief_history.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/code_style.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev9/docs/dev_notes/completion_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/completion_perf_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/dev_notes/gui_tests_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/dev_notes/how_search_works.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/library_vs_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/mongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1469 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/docs/dev_notes/next_steps_tutorial.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/origin_story.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/dev_notes/query_perf_10_x_more_data_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/dev_notes/query_perf_cache_vs_no_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/dev_notes/query_perf_mongomock_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/dev_notes/query_perf_pymongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev9/docs/dev_notes/release_procedure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/screencast_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      787 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/dev_notes/scripts_summary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1128 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/docs/dev_notes/semver_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5697 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/docs/dev_notes/term_dictionary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11129 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/dev_notes/top_todos.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/dev_notes/version_format.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.434121 argrelay-0.7.1.dev9/docs/feature_stories/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3725 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_01_89_09_24.interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-04-21 14:23:13.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1839 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_14_59_14_06.pending_requests.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1130 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_15_79_76_85.line_processor.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1476 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_20_88_05_60.named_args.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      917 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_26_43_73_72.func_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_27_16_67_19.line_syntax.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3596 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_29_54_67_86.dir_structure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_31_70_49_15.search_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      649 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_33_76_82_84.composite_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1829 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_36_17_84_44.check_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_39_58_01_91.query_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      792 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_46_96_59_05.init_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1278 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_47_63_35_61.env_vars.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1556 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_55_57_45_04.enum_selector.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1744 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_58_61_77_69.dev_shell.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_62_25_92_06.assigned_context.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_63_63_14_08.generated_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_66_17_43_42.test_infra.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_67_16_61_97.git_plugin.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_71_87_33_52.help_hint.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_72_40_53_00.fill_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1370 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_78_91_27_22.interp_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2391 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4514 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1841 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_91_88_07_23.jump_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_94_30_49_28.help_doc.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1653 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_97_64_39_94.arg_buckets.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_98_55_40_77.invoke_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/feature_stories/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.436121 argrelay-0.7.1.dev9/docs/release_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.0.0.dev0.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.0.0.dev27.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.0.0.dev28.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.0.0.dev42.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.0.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.1.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.2.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.2.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.3.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.4.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.5.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.5.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.5.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.6.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.6.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.6.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.6.3.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/release_notes/v0.6.4.final.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.439121 argrelay-0.7.1.dev9/docs/task_refs/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      418 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2979 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2661 2024-05-25 03:08:09.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      352 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_40_10_18_32.add_custom_base_to_all_schemas.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_43_41_95_86.use_server_logger_to_disable_stdout.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      497 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      224 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_70_48_96_29.be_able_to_assert_remaining_arg_vals.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      422 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_75_52_01_67.arg_buckets_to_support_multiple_var_args.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      170 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_79_67_28_83.recursive_dict_schema.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      652 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3051 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/docs/task_refs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.439121 argrelay-0.7.1.dev9/docs/test_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/docs/test_data/TD_38_03_48_51.large_data_set.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11158 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/test_data/TD_63_37_05_36.demo_services_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.7.1.dev9/docs/test_data/TD_70_69_38_46.no_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      550 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/docs/test_data/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev9/pyproject.toml
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15739 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-05-25 05:50:56.470121 argrelay-0.7.1.dev9/setup.cfg
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4262 2024-05-25 03:23:17.000000 argrelay-0.7.1.dev9/setup.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.422121 argrelay-0.7.1.dev9/src/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.440121 argrelay-0.7.1.dev9/src/argrelay/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/src/argrelay/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.441121 argrelay-0.7.1.dev9/src/argrelay/client_command_local/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_local/AbstractLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_local/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.441121 argrelay-0.7.1.dev9/src/argrelay/client_command_remote/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3981 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/client_command_remote/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.442121 argrelay-0.7.1.dev9/src/argrelay/client_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3787 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/client_spec/ShellContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/client_spec/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.443121 argrelay-0.7.1.dev9/src/argrelay/composite_tree/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      344 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeForest.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1138 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeForestSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2071 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeInfoType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1144 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeNode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeNodeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      657 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeNodeType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13703 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeTreeWalker.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11778 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/DictTreeWalker.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/composite_tree/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.445121 argrelay-0.7.1.dev9/src/argrelay/custom_integ/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8164 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/BaseConfigDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2325 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3643 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3533 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1598 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1737 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/FuncConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8075 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1869 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12644 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1615 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    18325 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      217 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    69098 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/git_utils.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      413 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ/value_constants.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.446121 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7009 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/argrelay_common_lib.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    33035 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     7248 2024-05-19 16:53:10.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/check_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3390 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/dev_shell.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3713 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/init_shell_env.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8092 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/shell_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2908 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/upgrade_all_packages.bash
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.447121 argrelay-0.7.1.dev9/src/argrelay/enum_desc/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/ArgSource.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/CallConv.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/CompScope.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/CompType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/DistinctValuesQuery.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/InterpStep.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/PluginType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/ReservedArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/ReservedEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/RunMode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/ServerAction.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      390 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/SpecialChar.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/SpecialFunc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3091 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/TermColor.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/TokenType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/src/argrelay/enum_desc/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.448121 argrelay-0.7.1.dev9/src/argrelay/handler_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/handler_request/AbstractServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3103 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev9/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/handler_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.448121 argrelay-0.7.1.dev9/src/argrelay/handler_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/handler_response/AbstractClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9401 2024-05-25 04:20:49.000000 argrelay-0.7.1.dev9/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-04-13 16:33:00.000000 argrelay-0.7.1.dev9/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/handler_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.449121 argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-05-18 02:28:39.000000 argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/ElapsedTime.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      741 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/ObjectSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/TypeDesc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.449121 argrelay-0.7.1.dev9/src/argrelay/misc_helper_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/misc_helper_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.449121 argrelay-0.7.1.dev9/src/argrelay/mongo_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoClientWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoServerWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev9/src/argrelay/mongo_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.450121 argrelay-0.7.1.dev9/src/argrelay/plugin_config/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_config/AbstractConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_config/DefaultConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_config/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.451121 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/AbstractDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4218 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1697 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2087 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/EchoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1516 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/ErrorDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5791 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/HelpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5308 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/InterceptDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      870 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/NoopDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/QueryEnumDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.452121 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3681 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/AbstractInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/AbstractInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-05-23 10:51:14.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FirstArgInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5508 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FirstArgInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1349 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17429 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FuncTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12865 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1684 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7238 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/InterpTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6270 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2925 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/NoopInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/NoopInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.452121 argrelay-0.7.1.dev9/src/argrelay/plugin_loader/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_loader/AbstractLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_loader/NoopLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/plugin_loader/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.453121 argrelay-0.7.1.dev9/src/argrelay/relay_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      965 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/AbstractClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/AbstractClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/AbstractClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/RemoteClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/RemoteClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2821 2024-05-25 03:08:09.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/__main__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4198 2024-05-25 05:37:58.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/proc_spinner.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3107 2024-05-25 05:39:10.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/proc_split.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2926 2024-05-25 04:31:43.000000 argrelay-0.7.1.dev9/src/argrelay/relay_client/proc_worker.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.454121 argrelay-0.7.1.dev9/src/argrelay/relay_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11191 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/CustomFlaskApp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/GuiBannerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/HelpHintCache.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7312 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/LocalServer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/QueryCacheConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/QueryEngine.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/QueryResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.454121 argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_static/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_static/argrelay_client.js
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_static/argrelay_style.css
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_static/external_link.svg
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.454121 argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_templates/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_templates/argrelay_main.html
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4947 2024-05-17 16:12:06.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/route_api.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/relay_server/route_gui.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.455121 argrelay-0.7.1.dev9/src/argrelay/runtime_context/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3180 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/AbstractPlugin.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4398 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/EnvelopeContainer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/InitControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    18127 2024-05-25 03:23:05.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/InterpContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6354 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/ParsedContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/SearchControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      440 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_context/arg_buckets_utils.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.456121 argrelay-0.7.1.dev9/src/argrelay/runtime_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/AssignedValue.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      407 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/ClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-03-18 13:46:05.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/ConnectionConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/EnvelopeCollection.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/PluginEntry.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/ServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      455 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/ServerPluginControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/StaticData.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.1.dev9/src/argrelay/runtime_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.456121 argrelay-0.7.1.dev9/src/argrelay/sample_conf/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/sample_conf/argrelay_client.json
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    35513 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/sample_conf/argrelay_server.yaml
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.456121 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2370 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_client/ClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1005 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_client/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.457121 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2839 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      736 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      976 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1767 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/MongoConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1068 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1054 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/ServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1822 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1148 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/StaticDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.458121 argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-04-22 16:25:28.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      953 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/InitControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2943 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/SearchControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.458121 argrelay-0.7.1.dev9/src/argrelay/schema_config_plugin/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_plugin/PluginEntrySchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/schema_config_plugin/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.458121 argrelay-0.7.1.dev9/src/argrelay/schema_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2634 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/schema_request/CallContextSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/schema_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.459121 argrelay-0.7.1.dev9/src/argrelay/schema_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/ArgValues.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1221 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/ArgValuesSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/AssignedValueSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2763 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/EnvelopeContainerSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2433 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/InterpResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2217 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/InterpResultSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1802 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/InvocationInput.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-05-05 14:32:52.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/InvocationInputSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.1.dev9/src/argrelay/schema_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.459121 argrelay-0.7.1.dev9/src/argrelay/server_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-05-19 16:08:16.000000 argrelay-0.7.1.dev9/src/argrelay/server_spec/CallContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/server_spec/DescribeLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/server_spec/ProposeArgValuesSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/server_spec/RelayLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.1.dev9/src/argrelay/server_spec/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-18 13:48:29.000000 argrelay-0.7.1.dev9/src/argrelay/server_spec/const_int.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/server_spec/server_data_schema.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.461121 argrelay-0.7.1.dev9/src/argrelay/test_infra/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/BaseTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/ClientServerTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/CustomTestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/CustomVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-05-19 16:07:53.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/End2EndTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    37764 2024-05-23 10:51:59.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/EnvMockBuilder.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12616 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/InOutTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/JsonTestOutputVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/LocalClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2785 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/LocalClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4990 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/LocalTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/OpenFileMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3449 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/PopenMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4519 2024-04-23 14:23:44.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/RemoteTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/ServerOnlyTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/TestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-18 13:51:36.000000 argrelay-0.7.1.dev9/src/argrelay/test_infra/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-25 05:50:56.440121 argrelay-0.7.1.dev9/src/argrelay.egg-info/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-25 05:50:56.000000 argrelay-0.7.1.dev9/src/argrelay.egg-info/PKG-INFO
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31836 2024-05-25 05:50:56.000000 argrelay-0.7.1.dev9/src/argrelay.egg-info/SOURCES.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-05-25 05:50:56.000000 argrelay-0.7.1.dev9/src/argrelay.egg-info/dependency_links.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      195 2024-05-25 05:50:56.000000 argrelay-0.7.1.dev9/src/argrelay.egg-info/requires.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-05-25 05:50:56.000000 argrelay-0.7.1.dev9/src/argrelay.egg-info/top_level.txt
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.952046 argrelay-0.7.2.dev0/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2024-05-19 10:16:55.000000 argrelay-0.7.2.dev0/LICENSE
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-06-02 14:52:42.951046 argrelay-0.7.2.dev0/PKG-INFO
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.913046 argrelay-0.7.2.dev0/docs/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.916046 argrelay-0.7.2.dev0/docs/dev_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5487 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/dev_notes/bootstrap_procedure.1.project_creation.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2489 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/dev_notes/bootstrap_procedure.2.initial_installation.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1891 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/brief_history.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/code_style.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.7.2.dev0/docs/dev_notes/completion_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/completion_perf_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/dev_notes/gui_tests_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/dev_notes/how_search_works.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/library_vs_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/mongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1476 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/dev_notes/next_steps_tutorial.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/origin_story.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/dev_notes/query_perf_10_x_more_data_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/dev_notes/query_perf_cache_vs_no_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/dev_notes/query_perf_mongomock_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/dev_notes/query_perf_pymongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.7.2.dev0/docs/dev_notes/release_procedure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/screencast_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      767 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/dev_notes/scripts_summary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1128 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/docs/dev_notes/semver_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5697 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/docs/dev_notes/term_dictionary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10895 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/dev_notes/top_todos.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/dev_notes/version_format.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.922046 argrelay-0.7.2.dev0/docs/feature_stories/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3619 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_01_89_09_24.interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-04-21 14:23:13.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1839 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_14_59_14_06.pending_requests.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1130 2024-05-23 10:51:59.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_15_79_76_85.line_processor.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1610 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_20_88_05_60.named_args.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      917 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_26_43_73_72.func_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_27_16_67_19.line_syntax.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3588 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_29_54_67_86.dir_structure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_31_70_49_15.search_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      649 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_33_76_82_84.composite_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1941 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_36_17_84_44.check_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_39_58_01_91.query_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      792 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_46_96_59_05.init_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1270 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_47_63_35_61.env_vars.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1048 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1556 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_55_57_45_04.enum_selector.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1740 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      750 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_58_61_77_69.dev_shell.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_62_25_92_06.assigned_context.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_63_63_14_08.generated_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-05-23 10:51:59.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_66_17_43_42.test_infra.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_67_16_61_97.git_plugin.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      476 2024-06-02 14:05:33.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_70_55_40_99.splitting_config_files.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_71_87_33_52.help_hint.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_72_40_53_00.fill_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      428 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1370 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_78_91_27_22.interp_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2391 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1438 2024-06-02 14:03:37.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_83_23_99_90.client_plugin_config_override.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4516 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_85_33_46_53.bootstrap_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1841 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_91_88_07_23.jump_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_94_30_49_28.help_doc.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1653 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_97_64_39_94.arg_buckets.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_98_55_40_77.invoke_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/feature_stories/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.924046 argrelay-0.7.2.dev0/docs/release_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.0.0.dev0.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.0.0.dev27.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.0.0.dev28.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.0.0.dev42.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.0.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.1.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.2.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.2.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.3.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.4.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.5.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.5.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.5.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.6.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.6.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.6.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.6.3.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/release_notes/v0.6.4.final.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.926046 argrelay-0.7.2.dev0/docs/task_refs/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      418 2024-05-23 10:51:59.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2979 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2661 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      908 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_39_25_11_76.data_envelopes_with_missing_props.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      352 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_40_10_18_32.add_custom_base_to_all_schemas.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_43_41_95_86.use_server_logger_to_disable_stdout.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      202 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_62_75_33_41.do_not_hardcode_plugin_instance_id.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_env_packages_before_test.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      224 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_70_48_96_29.be_able_to_assert_remaining_arg_vals.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      422 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_75_52_01_67.arg_buckets_to_support_multiple_var_args.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      170 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_79_67_28_83.recursive_dict_schema.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2291 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/docs/task_refs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.927046 argrelay-0.7.2.dev0/docs/test_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/docs/test_data/TD_38_03_48_51.large_data_set.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      166 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/docs/test_data/TD_39_25_11_76.data_envelopes_with_missing_props.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11158 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/test_data/TD_63_37_05_36.demo_services_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.7.2.dev0/docs/test_data/TD_70_69_38_46.no_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      550 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/docs/test_data/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.7.2.dev0/pyproject.toml
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15777 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-06-02 14:52:42.952046 argrelay-0.7.2.dev0/setup.cfg
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4306 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/setup.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.911046 argrelay-0.7.2.dev0/src/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.927046 argrelay-0.7.2.dev0/src/argrelay/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/src/argrelay/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.928046 argrelay-0.7.2.dev0/src/argrelay/client_command_local/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_local/AbstractLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_local/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.929046 argrelay-0.7.2.dev0/src/argrelay/client_command_remote/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3981 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/client_command_remote/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.929046 argrelay-0.7.2.dev0/src/argrelay/client_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3787 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/client_spec/ShellContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/client_spec/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.929046 argrelay-0.7.2.dev0/src/argrelay/composite_tree/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      344 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeForest.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1043 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeForestSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2070 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeInfoType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1144 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeNode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6372 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeNodeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      657 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeNodeType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13704 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeTreeWalker.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11914 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/DictTreeWalker.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/composite_tree/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.931046 argrelay-0.7.2.dev0/src/argrelay/custom_integ/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8164 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/BaseConfigDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2325 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3643 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3533 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1598 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1737 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/FuncConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-05-25 15:40:18.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8075 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1869 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13525 2024-06-02 14:31:35.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1615 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      815 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    18542 2024-06-02 06:38:45.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      217 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    74775 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/git_utils.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      413 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ/value_constants.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.932046 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7009 2024-05-23 10:51:59.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/argrelay_common_lib.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    32931 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/bootstrap_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     7216 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/check_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3382 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/dev_shell.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3689 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/init_shell_env.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8076 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/shell_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2877 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/upgrade_env_packages.bash
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.933046 argrelay-0.7.2.dev0/src/argrelay/enum_desc/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/ArgSource.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/CallConv.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/CompScope.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/CompType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/DistinctValuesQuery.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/InterpStep.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/PluginType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/ReservedArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/ReservedEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/RunMode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/ServerAction.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      390 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/SpecialChar.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/SpecialFunc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3091 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/TermColor.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/TokenType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/src/argrelay/enum_desc/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.933046 argrelay-0.7.2.dev0/src/argrelay/handler_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/handler_request/AbstractServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3130 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/handler_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.934046 argrelay-0.7.2.dev0/src/argrelay/handler_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/handler_response/AbstractClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9401 2024-05-25 04:20:49.000000 argrelay-0.7.2.dev0/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-04-13 16:33:00.000000 argrelay-0.7.2.dev0/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/handler_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.934046 argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-05-18 02:28:39.000000 argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/ElapsedTime.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      741 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/ObjectSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3512 2024-06-02 14:05:33.000000 argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/TypeDesc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.934046 argrelay-0.7.2.dev0/src/argrelay/misc_helper_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/misc_helper_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.935046 argrelay-0.7.2.dev0/src/argrelay/mongo_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-03-18 13:46:05.000000 argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoClientWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoServerWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.2.dev0/src/argrelay/mongo_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.935046 argrelay-0.7.2.dev0/src/argrelay/plugin_config/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_config/AbstractConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_config/DefaultConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_config/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.936046 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/AbstractDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4138 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1698 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2087 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/EchoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1516 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/ErrorDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5791 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/HelpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5308 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/InterceptDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      870 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/NoopDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/QueryEnumDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.938046 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3681 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/AbstractInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-04-22 16:25:28.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/AbstractInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-05-23 10:51:14.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FirstArgInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5508 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FirstArgInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1349 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17429 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FuncTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12865 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1684 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7265 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/InterpTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6270 2024-05-23 10:51:59.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2925 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/NoopInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/NoopInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.938046 argrelay-0.7.2.dev0/src/argrelay/plugin_loader/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_loader/AbstractLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_loader/NoopLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_loader/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      614 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/plugin_loader/client_utils.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.939046 argrelay-0.7.2.dev0/src/argrelay/relay_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      965 2024-05-23 10:51:59.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/AbstractClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/AbstractClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/AbstractClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/RemoteClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/RemoteClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2822 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/__main__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4297 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/proc_spinner.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3110 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/proc_split.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2928 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/relay_client/proc_worker.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.940046 argrelay-0.7.2.dev0/src/argrelay/relay_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11350 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/CustomFlaskApp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-03-18 13:46:05.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/GuiBannerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/HelpHintCache.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9560 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/LocalServer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-03-18 13:46:05.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/QueryCacheConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/QueryEngine.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/QueryResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.940046 argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_static/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_static/argrelay_client.js
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_static/argrelay_style.css
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_static/external_link.svg
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.940046 argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_templates/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_templates/argrelay_main.html
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4947 2024-05-17 16:12:06.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/route_api.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/relay_server/route_gui.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.941046 argrelay-0.7.2.dev0/src/argrelay/runtime_context/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3180 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/AbstractPlugin.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4398 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/EnvelopeContainer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-03-18 13:46:05.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/InitControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    18370 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/InterpContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6354 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/ParsedContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/SearchControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      440 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_context/arg_buckets_utils.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.942046 argrelay-0.7.2.dev0/src/argrelay/runtime_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-18 13:46:05.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/AssignedValue.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      407 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/ClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-03-18 13:46:05.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/ConnectionConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/EnvelopeCollection.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      686 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/PluginConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/PluginEntry.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3188 2024-06-02 14:24:43.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/ServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/ServerPluginControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/StaticData.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.2.dev0/src/argrelay/runtime_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.942046 argrelay-0.7.2.dev0/src/argrelay/sample_conf/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/sample_conf/argrelay_client.json
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    19583 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/sample_conf/argrelay_plugin.yaml
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15815 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/sample_conf/argrelay_server.yaml
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.942046 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2370 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_client/ClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1005 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_client/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.943046 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2839 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      736 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      976 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1767 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/MongoConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1049 2024-06-02 14:31:15.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1035 2024-06-02 14:31:15.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3709 2024-06-02 14:31:15.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/ServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1094 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1129 2024-06-02 14:31:15.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/StaticDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.944046 argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-04-22 16:25:28.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      953 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/InitControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2924 2024-06-02 14:31:15.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/SearchControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.944046 argrelay-0.7.2.dev0/src/argrelay/schema_config_plugin/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3989 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_plugin/PluginConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_plugin/PluginEntrySchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/schema_config_plugin/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.944046 argrelay-0.7.2.dev0/src/argrelay/schema_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2634 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/schema_request/CallContextSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/schema_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.945046 argrelay-0.7.2.dev0/src/argrelay/schema_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/ArgValues.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1221 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/ArgValuesSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/AssignedValueSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2763 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/EnvelopeContainerSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2433 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/InterpResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2217 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/InterpResultSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1802 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/InvocationInput.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-05-05 14:32:52.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/InvocationInputSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.2.dev0/src/argrelay/schema_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.945046 argrelay-0.7.2.dev0/src/argrelay/server_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-05-19 16:08:16.000000 argrelay-0.7.2.dev0/src/argrelay/server_spec/CallContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/server_spec/DescribeLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/server_spec/ProposeArgValuesSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/server_spec/RelayLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.2.dev0/src/argrelay/server_spec/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-18 13:48:29.000000 argrelay-0.7.2.dev0/src/argrelay/server_spec/const_int.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/server_spec/server_data_schema.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.947046 argrelay-0.7.2.dev0/src/argrelay/test_infra/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/BaseTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/ClientServerTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/CustomTestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/CustomVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-05-19 16:07:53.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/End2EndTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    41780 2024-06-02 07:01:27.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/EnvMockBuilder.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13114 2024-05-26 12:09:10.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/InOutTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/JsonTestOutputVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/LocalClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3082 2024-06-02 05:15:32.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/LocalClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4990 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/LocalTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/OpenFileMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3449 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/PopenMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4519 2024-04-23 14:23:44.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/RemoteTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/ServerOnlyTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/TestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-18 13:51:36.000000 argrelay-0.7.2.dev0/src/argrelay/test_infra/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-06-02 14:52:42.928046 argrelay-0.7.2.dev0/src/argrelay.egg-info/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-06-02 14:52:42.000000 argrelay-0.7.2.dev0/src/argrelay.egg-info/PKG-INFO
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    32121 2024-06-02 14:52:42.000000 argrelay-0.7.2.dev0/src/argrelay.egg-info/SOURCES.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-06-02 14:52:42.000000 argrelay-0.7.2.dev0/src/argrelay.egg-info/dependency_links.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      195 2024-06-02 14:52:42.000000 argrelay-0.7.2.dev0/src/argrelay.egg-info/requires.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-06-02 14:52:42.000000 argrelay-0.7.2.dev0/src/argrelay.egg-info/top_level.txt
```

### Comparing `argrelay-0.7.1.dev9/LICENSE` & `argrelay-0.7.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/PKG-INFO` & `argrelay-0.7.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.7.1.dev9
+Version: 0.7.2.dev0
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/bootstrap_procedure.1.project_creation.md` & `argrelay-0.7.2.dev0/docs/dev_notes/bootstrap_procedure.1.project_creation.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
-This procedure describes using [`FS_85_33_46_53.bootstrap_dev_env.md`][FS_85_33_46_53.bootstrap_dev_env.md] feature for step 1:
+This procedure describes using [`FS_85_33_46_53.bootstrap_env.md`][FS_85_33_46_53.bootstrap_env.md] feature for step 1:
 1.  project creation from scratch: [`bootstrap_procedure.1.project_creation.md`][bootstrap_procedure.1.project_creation.md]
-2.  initial deployment for existing project: [`bootstrap_procedure.2.initial_deployment.md`][bootstrap_procedure.2.initial_deployment.md]
+2.  initial installation for existing project: [`bootstrap_procedure.2.initial_installation.md`][bootstrap_procedure.2.initial_installation.md]
 3.  `argrelay` upgrade as (dependency for existing project): [`bootstrap_procedure.3.argrelay_upgrade.md`][bootstrap_procedure.3.argrelay_upgrade.md]
 
 # Project creation with bootstrap script
 
-Obtain (copy and paste or download) [`bootstrap_dev_env.bash`][bootstrap_dev_env.bash] into temporary path,<br/>
-for example, `/tmp/bootstrap_dev_env.bash`.
+Obtain (copy and paste or download) [`bootstrap_env.bash`][bootstrap_env.bash] into temporary path,<br/>
+for example, `/tmp/bootstrap_env.bash`.
 
 Then, run it **from the project root directory**:
 *   The project root dir is referred to as `@/` - see [`FS_29_54_67_86.dir_structure.md`][FS_29_54_67_86.dir_structure.md].
 *   The project root dir is not necessarily Git repo root dir - it might be any sub-dir.
 
 ```sh
 cd path/to/project/dir
-bash /tmp/bootstrap_dev_env.bash
+bash /tmp/bootstrap_env.bash
 ```
 
 It will likely fail first time (exits with code other than 0) due to missing config files,<br/>
 but it is meant to be re-run multiple times until it succeeds (until it exits with code 0).
 
 # Prepare `@/conf/` for the bootstrap of the current environment
 
@@ -49,15 +49,15 @@
 
 # What else might bootstrap need?
 
 Keep re-running bootstrap until it succeeds (until it exits with code 0) addressing all issues step by step:
 
 ```sh
 cd path/to/project/dir
-bash /tmp/bootstrap_dev_env.bash
+bash /tmp/bootstrap_env.bash
 ```
 
 If it is a new `argrelay`-based project created from scratch,<br/>
 bootstrap will fail (exits with code other than 0) due to many missing files and dirs.
 
 Normally, it is clear from the output what is the reason for the failure.
 
@@ -76,56 +76,56 @@
 
 *   Missing `@/conf/python_env.conf.bash` file.
 
     This file provides config for Python interpreter and creation of Python virtual environment.
 
     If missing, bootstrap prints initial copy-and-paste-able content of this file.
 
-*   Missing `@/exe/deploy_project.bash` file.
+*   Missing `@/exe/install_project.bash` file.
 
-    This file is project-specific custom script to deploy project packages into Python venv.
+    This file is project-specific custom script to install project packages into Python venv.
 
     If missing, bootstrap prints initial copy-and-paste-able content of this file.
 
 *   Missing `setup.py` file.
 
-    This is expected by template version of `@/exe/deploy_project.bash` file.
+    This is expected by template version of `@/exe/install_project.bash` file.
 
-    If missing, either create minimal `setup.py` or modify `@/exe/deploy_project.bash`.
+    If missing, either create minimal `setup.py` or modify `@/exe/install_project.bash`.
 
 *   Missing `argrelay` package.
 
     To generate client and server executables, bootstrap needs installed `argrelay` package
     in the venv (as configured in `@/conf/python_env.conf.bash`) used by the bootstrap process.
 
-    In turn, `@/exe/deploy_project.bash` script should deploy `argrelay` (directly or indirectly via dependencies).
+    In turn, `@/exe/install_project.bash` script should install `argrelay` (directly or indirectly via dependencies).
 
-    *   Long-term fix is to ensure `@/exe/deploy_project.bash` installs `argrelay`.
+    *   Long-term fix is to ensure `@/exe/install_project.bash` installs `argrelay`.
     *   Short-term fix is to activate the same venv (as configured in `@/conf/python_env.conf.bash`) and install `argrelay` manually.
 
 *   Other missing files.
 
     This could be:
 
-    *   `@/exe/deploy_config_files_conf.bash`
-    *   `@/exe/deploy_resource_files_conf.bash`
+    *   `@/exe/config_files.conf.bash`
+    *   `@/exe/resource_files.conf.bash`
     *   `@/exe/build_project.bash`
     *   ...
 
     When missing, bootstrap prints initial copy-and-paste-able content for these files.
 
 # When bootstrap succeeds
 
 Eventually, when bootstrap succeeds (exits with code 0),<br/>
-its copy will be stored into `@/exe/bootstrap_dev_env.bash` (it should be version-controlled).
+its copy will be stored into `@/exe/bootstrap_env.bash` (it should be version-controlled).
 
 To see how it works, try [`FS_58_61_77_69.dev_shell.md`][FS_58_61_77_69.dev_shell.md].
 
 [bootstrap_procedure.1.project_creation.md]: bootstrap_procedure.1.project_creation.md
-[bootstrap_procedure.2.initial_deployment.md]: bootstrap_procedure.2.initial_deployment.md
+[bootstrap_procedure.2.initial_installation.md]: bootstrap_procedure.2.initial_installation
 [bootstrap_procedure.3.argrelay_upgrade.md]: bootstrap_procedure.3.argrelay_upgrade.md
 
-[FS_85_33_46_53.bootstrap_dev_env.md]: ../feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+[FS_85_33_46_53.bootstrap_env.md]: ../feature_stories/FS_85_33_46_53.bootstrap_env.md
 [FS_29_54_67_86.dir_structure.md]: ../feature_stories/FS_29_54_67_86.dir_structure.md
 [FS_58_61_77_69.dev_shell.md]: ../feature_stories/FS_58_61_77_69.dev_shell.md
-[bootstrap_dev_env.bash]: ../../exe/bootstrap_dev_env.bash
+[bootstrap_env.bash]: ../../exe/bootstrap_env.bash
 [root_readme.md]: ../../readme.md
```

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md` & `argrelay-0.7.2.dev0/docs/dev_notes/bootstrap_procedure.2.initial_installation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
-This procedure describes using [`FS_85_33_46_53.bootstrap_dev_env.md`][FS_85_33_46_53.bootstrap_dev_env.md] feature for step 2:
+This procedure describes using [`FS_85_33_46_53.bootstrap_env.md`][FS_85_33_46_53.bootstrap_env.md] feature for step 2:
 1.  project creation from scratch: [`bootstrap_procedure.1.project_creation.md`][bootstrap_procedure.1.project_creation.md]
-2.  initial deployment for existing project: [`bootstrap_procedure.2.initial_deployment.md`][bootstrap_procedure.2.initial_deployment.md]
+2.  initial installation for existing project: [`bootstrap_procedure.2.initial_installation.md`][bootstrap_procedure.2.initial_installation.md]
 3.  `argrelay` upgrade as (dependency for existing project): [`bootstrap_procedure.3.argrelay_upgrade.md`][bootstrap_procedure.3.argrelay_upgrade.md]
 
 # Creating config for current environment
 
 Directory `@/conf/` should be either|or:
 *   (conventionally) a symlink and point to one of the config dir under `@/dst/`
 *   (optionally) simply contain required files
 
 Note that, depending on the project, there could be no initial config required -<br/>
-in this case `@/exe/bootstrap_dev_env.bash` simply creates default config files.
+in this case `@/exe/bootstrap_env.bash` simply creates default config files.
 
 The documents follow the first conventional symlink approach (which allows all configs be stored under `@/dst`).
 
 When a project already exists, there could be many sample config dirs<br/>
 under `@/dst/` to copy and modify, then use it as `@/conf/` target, for example:
 
 ```sh
@@ -23,33 +23,33 @@
 ln -ns ./dst/this_config ./conf
 ```
 
 Modify files under `@/conf/` if necessary.
 
 # Running bootstrap
 
-Re-run `@/exe/bootstrap_dev_env.bash` until it succeeds (exit with non-0 code):
+Re-run `@/exe/bootstrap_env.bash` until it succeeds (exit with non-0 code):
 
 ```sh
-./exe/bootstrap_dev_env.bash
+./exe/bootstrap_env.bash
 ```
 
 There could be many things to fix if something wrong with the config or dependencies -<br/>
 some are explained in [`bootstrap_procedure.1.project_creation.md`][bootstrap_procedure.1.project_creation.md].
 
 # Project customization
 
-Most of the initial deployment details are specific to project customization -<br/>
+Most of the initial install details are specific to project customization -<br/>
 they depend on custom plugins (see `plugin_development.md`) and may require extra steps.
 
 To run real Mongo DB (instead of `mongomock`), see also `mongo_notes.md`.
 
-# Trying the deployment
+# Trying the installation
 
-To see how this deployment works, try [`FS_58_61_77_69.dev_shell.md`][FS_58_61_77_69.dev_shell.md].
+To see how this installation works, try [`FS_58_61_77_69.dev_shell.md`][FS_58_61_77_69.dev_shell.md].
 
 [bootstrap_procedure.1.project_creation.md]: bootstrap_procedure.1.project_creation.md
-[bootstrap_procedure.2.initial_deployment.md]: bootstrap_procedure.2.initial_deployment.md
+[bootstrap_procedure.2.initial_installation.md]: bootstrap_procedure.2.initial_installation
 [bootstrap_procedure.3.argrelay_upgrade.md]: bootstrap_procedure.3.argrelay_upgrade.md
 
-[FS_85_33_46_53.bootstrap_dev_env.md]: ../feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+[FS_85_33_46_53.bootstrap_env.md]: ../feature_stories/FS_85_33_46_53.bootstrap_env.md
 [FS_58_61_77_69.dev_shell.md]: ../feature_stories/FS_58_61_77_69.dev_shell.md
```

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md` & `argrelay-0.7.2.dev0/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 
-This procedure describes using [`FS_85_33_46_53.bootstrap_dev_env.md`][FS_85_33_46_53.bootstrap_dev_env.md] feature for step 3:
+This procedure describes using [`FS_85_33_46_53.bootstrap_env.md`][FS_85_33_46_53.bootstrap_env.md] feature for step 3:
 1.  project creation from scratch: [`bootstrap_procedure.1.project_creation.md`][bootstrap_procedure.1.project_creation.md]
-2.  initial deployment for existing project: [`bootstrap_procedure.2.initial_deployment.md`][bootstrap_procedure.2.initial_deployment.md]
+2.  initial installation for existing project: [`bootstrap_procedure.2.initial_installation.md`][bootstrap_procedure.2.initial_installation.md]
 3.  `argrelay` upgrade as (dependency for existing project): [`bootstrap_procedure.3.argrelay_upgrade.md`][bootstrap_procedure.3.argrelay_upgrade.md]
 
 # Upgrading `argrelay` as project dependency
 
-The steps below are explained as package management in [`FS_85_33_46_53.bootstrap_dev_env.md`][FS_85_33_46_53.bootstrap_dev_env.md].
+The steps below are explained as package management in [`FS_85_33_46_53.bootstrap_env.md`][FS_85_33_46_53.bootstrap_env.md].
 
 Run `@/exe/dev_shell.bash` to activate `venv`:
 
 ```sh
 ./exe/dev_shell.bash
 ```
 
-Remove saved `argrelay` entry from `@/conf/dev_env_packages.txt` (otherwise subsequent bootstrap will restore it):
+Remove saved `argrelay` entry from `@/conf/env_packages.txt` (otherwise subsequent bootstrap will restore it):
 
 ```sh
-sef -i "/argrelay/d" ./conf/dev_env_packages.txt
+sef -i "/argrelay/d" ./conf/env_packages.txt
 ```
 
 Upgrade `argrelay` package to newer version:
 
 ```sh
 pip install --upgrade --force-reinstall argrelay
 ```
 
-Re-run `@/exe/bootstrap_dev_env.bash`:
+Re-run `@/exe/bootstrap_env.bash`:
 
 ```sh
-./exe/bootstrap_dev_env.bash
+./exe/bootstrap_env.bash
 ```
 
 # Upgrading project customization
 
 Most of the upgrade details are specific to project customization -<br/>
 they depend on custom plugins (see `plugin_development.md`) and may require extra steps.
 
 # Trying the upgrade
 
 To see how it works after upgrade, try [`FS_58_61_77_69.dev_shell.md`][FS_58_61_77_69.dev_shell.md].
 
 [bootstrap_procedure.1.project_creation.md]: bootstrap_procedure.1.project_creation.md
-[bootstrap_procedure.2.initial_deployment.md]: bootstrap_procedure.2.initial_deployment.md
+[bootstrap_procedure.2.initial_installation.md]: bootstrap_procedure.2.initial_installation
 [bootstrap_procedure.3.argrelay_upgrade.md]: bootstrap_procedure.3.argrelay_upgrade.md
 
-[FS_85_33_46_53.bootstrap_dev_env.md]: ../feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+[FS_85_33_46_53.bootstrap_env.md]: ../feature_stories/FS_85_33_46_53.bootstrap_env.md
 [FS_58_61_77_69.dev_shell.md]: ../feature_stories/FS_58_61_77_69.dev_shell.md
```

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/brief_history.md` & `argrelay-0.7.2.dev0/docs/dev_notes/brief_history.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/code_style.md` & `argrelay-0.7.2.dev0/docs/dev_notes/code_style.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/completion_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/completion_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/completion_perf_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/completion_perf_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/gui_tests_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/gui_tests_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/how_search_works.md` & `argrelay-0.7.2.dev0/docs/dev_notes/how_search_works.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/library_vs_framework.md` & `argrelay-0.7.2.dev0/docs/dev_notes/library_vs_framework.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/mongo_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/mongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/next_steps_tutorial.md` & `argrelay-0.7.2.dev0/docs/dev_notes/next_steps_tutorial.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 <a name="argrelay-next-steps"></a>
 # What's next?
 
 *   Modify [`ServiceLoader.py` plugin][link_to_load_data_envelopes] to provide data beyond [demo data set][TD_63_37_05_36.demo_services_data.md].
 
     The data can be simply hard-coded with different `test_data` tag<br/>
-    (other than `TD_63_37_05_36` demo) and selected in `argrelay_server.yaml`:
+    (other than `TD_63_37_05_36` demo) and selected in `argrelay_plugin.yaml` config:
 
     ```diff
         ServiceLoader:
             plugin_module_name: argrelay.custom_integ.ServiceLoader
             plugin_class_name: ServiceLoader
             plugin_config:
                 test_data_ids_to_load:
```

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/origin_story.md` & `argrelay-0.7.2.dev0/docs/dev_notes/origin_story.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/query_perf_10_x_more_data_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/query_perf_10_x_more_data_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/query_perf_cache_vs_no_cache.md` & `argrelay-0.7.2.dev0/docs/dev_notes/query_perf_cache_vs_no_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/query_perf_mongomock_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/query_perf_mongomock_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/query_perf_pymongo_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/query_perf_pymongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/release_procedure.md` & `argrelay-0.7.2.dev0/docs/dev_notes/release_procedure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/screencast_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/screencast_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/scripts_summary.md` & `argrelay-0.7.2.dev0/docs/dev_notes/scripts_summary.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 TODO: Move this into FS_29_54_67_86 `dir_structure`
 
 Table
 
-| Script                         | Sets `PATH` | Activates `venv` | Re-installs | Purpose                                                      |
-|--------------------------------|-------------|------------------|-------------|--------------------------------------------------------------|
-| `@/exe/bootstrap_dev_env.bash` | -           | -                | yes         | to set up dev env, re-install or upgrade `argrelay`, etc.    |
-| `@/exe/dev_shell.bash`         | yes         | yes              | no          | to start shell session with project-specific auto-completion |
-| `@/exe/shell_env.bash`         | yes         | no               | no          | to be used in `~/.bashrc` for all shell sessions             |
+| Script                     | Sets `PATH` | Activates `venv` | Re-installs | Purpose                                                      |
+|----------------------------|-------------|------------------|-------------|--------------------------------------------------------------|
+| `@/exe/bootstrap_env.bash` | -           | -                | yes         | to set up dev env, re-install or upgrade `argrelay`, etc.    |
+| `@/exe/dev_shell.bash`     | yes         | yes              | no          | to start shell session with project-specific auto-completion |
+| `@/exe/shell_env.bash`     | yes         | no               | no          | to be used in `~/.bashrc` for all shell sessions             |
```

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/semver_notes.md` & `argrelay-0.7.2.dev0/docs/dev_notes/semver_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/term_dictionary.md` & `argrelay-0.7.2.dev0/docs/dev_notes/term_dictionary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/top_todos.md` & `argrelay-0.7.2.dev0/docs/dev_notes/top_todos.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,19 @@
 *   CLOSED: The issue is done or being tracked otherwise = no need to keep this todo, but still kept to keep in the view.
 *   REGISTER: The item is not yet registered, requires new feature story (FS) entry.
 *   USER_VISIBLE: Something what is visible to user (rather than just making things better).
 *   DEV_VISIBLE: Something what is visible to dev (may not be visible for users as USER_VISIBLE, but helps dev).
 
 Top:
 
-
-*   Add color for envelope class in desc output - green if found 1, yellow if not yet (still N), gray if 0.
-    See also: FS_80_45_89_81 / list_envelope
-    FINALIZE
 *   If command accept one envelope, but not yet disambiguated, then it should be possible to provide generic hook to list envelopes based on existing filter.
     Basically, if 1, invoke target function, if N, invoke list, print error to stderr, exit with non 0.
     See also: FS_80_45_89_81 / list_envelope
     REGISTER
 
-*   Clean `#`-comments from command line arguments by parser.
-    Tracked via FS_92_75_93_01.clean_command_line.md
-    CLOSED
-
 *   Consumed and remaining tokens:
     *   Send them to invocation (e.g. to decide to run or not to run function and how they can be used).
     *   Verify them in tests.
     FINALIZE
 
 *   Meta function: list all objects of specified query.
     See also: FS_80_45_89_81 / list_envelope
@@ -156,26 +148,27 @@
 Ease integration into external project:
 
 *   There is constant need to distinguish (TODO: name it properly):
     *   argrelay_target_dir - the path to special dir (where venv is configured via relative path, artifacts generated, config files, etc.)
     *   argrelay_distrib_dir - the path to useful artifacts (where known after venv is sourced)
     TODO: Is this still a problem?
           Yes.
-          *   `argrelay_inst_dir` must be the project (where argrelay is used or itself, or where it is deployed).
+          *   `argrelay_inst_dir` must be the project (where `argrelay` is used itself, or where it is installed).
           *   Anything else like `argrelay_module_dir_path` obtained by running Python is package_dir
     See also: FS_29_54_67_86.dir_structure.md
     FINALIZE
 
 *   Make yaml config composable:
     *   reduce size and chances of merging unrelated parts
     *   avoid config modification by loading other parts from known (by convention) places
     *   allow loading external config which should plug itself into existing config
     Maybe it should be possible to provide just the list of configured plugins (their loading order)
     and they will load automatically from expected location?
     Also split core server config (open ports, mongo, cache) and plugin management.
+    See also: FS_83_23_99_90 client plugin config override.
     REGISTER
 
 *   Make Git plugin a bit more useful (e.g. in addition to loading commit data, be able to switch to pre-configured Git repos).
     Use `help_hint` (FS_71_87_33_52) for selection of the repo.
     FINALIZE
 
 *   Use `ssh` on selected service (a useful case).
```

### Comparing `argrelay-0.7.1.dev9/docs/dev_notes/version_format.md` & `argrelay-0.7.2.dev0/docs/dev_notes/version_format.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_00_13_77_97.plugin_framework.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_00_13_77_97.plugin_framework.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 ---
 feature_story: FS_00_13_77_97
 feature_title:  plugin framework
 feature_status: TEST
 ---
 
-TODO_94_66_41_94: make separate config for plugin (if `reusable_config_data` can still be used somehow).
-
 # Plugin framework
 
-Plugins are configured under `plugin_instance_entries` in `argrelay_server.yaml` config file (see also `ServerConfigSchema.py`).
+Plugins are configured under `plugin_instance_entries` in `argrelay_plugin.yaml` config file (see also `PluginConfigSchema.py`).
 
 Both plugin and plugin instance are used interchangeably to mean individual (runtime) plugin instance
 identified by `plugin_instance_id` and configured under `plugin_instance_entries`.
 
 Each plugin in configured in one place, but do not confuse (distinguish):
 *   `plugin_entry` which `argrelay` uses to manage plugin instances.
 *   `plugin_config` (part of `plugin_entry`) which is plugin-specific config (opaque to `argrelay`).
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_01_89_09_24.interp_tree.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_01_89_09_24.interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_06_99_43_60.list_arg_value.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_06_99_43_60.list_arg_value.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_14_59_14_06.pending_requests.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_14_59_14_06.pending_requests.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_15_79_76_85.line_processor.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_15_79_76_85.line_processor.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,37 +14,40 @@
 *   Highest priority: `ARGRELAY_CONF_BASE_DIR` env var: `${ARGRELAY_CONF_BASE_DIR}/*`
 
     If `ARGRELAY_CONF_BASE_DIR` is defined, config files will be looked up in, for example:
 
     ```sh
     ls ${ARGRELAY_CONF_BASE_DIR}/python_env.conf.bash
     ls ${ARGRELAY_CONF_BASE_DIR}/shell_env.conf.bash
-    ls ${ARGRELAY_CONF_BASE_DIR}/argrelay_server.yaml
     ls ${ARGRELAY_CONF_BASE_DIR}/argrelay_client.json
+    ls ${ARGRELAY_CONF_BASE_DIR}/argrelay_server.yaml
+    ls ${ARGRELAY_CONF_BASE_DIR}/argrelay_plugin.yaml
     # ...
     ```
 
 *   User home dir (or `~/`): `~/.argrelay.conf.d/*`
 
     For example:
 
     ```sh
     ls ~/.argrelay.conf.d/python_env.conf.bash
     ls ~/.argrelay.conf.d/shell_env.conf.bash
-    ls ~/.argrelay.conf.d/argrelay_server.yaml
     ls ~/.argrelay.conf.d/argrelay_client.json
+    ls ~/.argrelay.conf.d/argrelay_server.yaml
+    ls ~/.argrelay.conf.d/argrelay_plugin.yaml
     # ...
     ```
 
 *   Lowest priority: `argrelay_dir` (or `@/`): `@/conf/*`
 
     See also `FS_29_54_67_86.dir_structure.md`
 
     Project directory paths, for example:
 
     ```sh
     ls conf/python_env.conf.bash
     ls conf/shell_env.conf.bash
-    ls conf/argrelay_server.yaml
     ls conf/argrelay_client.json
+    ls conf/argrelay_server.yaml
+    ls conf/argrelay_plugin.yaml
     # ...
     ```
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_20_88_05_60.named_args.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_20_88_05_60.named_args.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_26_43_73_72.func_tree.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_26_43_73_72.func_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_27_16_67_19.line_syntax.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_27_16_67_19.line_syntax.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_29_54_67_86.dir_structure.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_29_54_67_86.dir_structure.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This features describes the directory structure (a convention):
 *   which `argrelay` uses for itself
 *   which should be used for integration projects based on `argrelay` (to make scripts re-use-able)
 
 To make it unambiguous that path is relative to project root dir,
 it is referred to as `argrelay_dir` in scripts and indicated as `@/` in docs and comments,
-for example: `@/exe/bootstrap_dev_env.bash`.
+for example: `@/exe/bootstrap_env.bash`.
 
 Every script knows its relative position to `argrelay_dir` (or `@/`) to locate it.
 
 Note that project root may or may not match repo root (e.g. Git):
 *   it does for `argrelay` itself
 *   but it may not for `argrelay`-based projects
 
@@ -47,44 +47,44 @@
 
 # `@/exe/`
 
 Dir `@/exe/` contains immediately executable files.
 
 # `@/conf/`
 
-Dir `@/conf/` contains configuration files specific to target deployment environment.
+Dir `@/conf/` contains configuration files specific to target installation environment.
 
 Normally, it is a symlink.
 
 The symlink itself is not supposed to be version controlled by this repo, but the dir it points to can be:
 *   one of `@/dst/*` dirs under the same repo
 *   any other dir
 
 In practice, to keep config under version control within the same repo, `@/conf/` can be a symlink which
-points to different version controlled dir (see sub-dirs under `@/dst/`) depending on the target deployment environment.
+points to different version controlled dir (see sub-dirs under `@/dst/`) depending on the target installation environment.
 
-To avoid being detected as modified when target deployment environment changes, this `@/conf/` symlink is not committed.
+To avoid being detected as modified when target installation environment changes, this `@/conf/` symlink is not committed.
 
 This path is the default (lowest priority) - see [`FS_16_07_78_84.conf_dir_priority.md`][FS_16_07_78_84.conf_dir_priority.md].
 
 # `@/dst/`
 
 This dir contains sub-dirs with config files for multiple target environments.
 
 For example:
 *   Dir `@/dst/` may contain sub-dirs: `@/dst/target_env_a` and `@/dst/target_env_b`.
-*   When the project is deployed to environment `target_env_a`, `@/conf/` should be a symlink to `@/dst/target_env_a`.
-*   When the project is deployed to environment `target_env_b`, `@/conf/` should be a symlink to `@/dst/target_env_b`.
+*   When the project is installed to environment `target_env_a`, `@/conf/` should be a symlink to `@/dst/target_env_a`.
+*   When the project is installed to environment `target_env_b`, `@/conf/` should be a symlink to `@/dst/target_env_b`.
 
-# `@/exe/bootstrap_dev_env.bash`
+# `@/exe/bootstrap_env.bash`
 
-See FS_85_33_46_53 `bootstrap_dev_env`.
+See FS_85_33_46_53 `bootstrap_env`.
 
 # `@/exe/dev_shell.bash`
 
 See FS_58_61_77_69 `dev_shell`.
 
-# `@/conf/dev_shell_rc.conf.bash`
+# `@/conf/dev_shell_env.bash`
 
 It is used by `@/exe/dev_shell.bash`.
 
 [FS_16_07_78_84.conf_dir_priority.md]: FS_16_07_78_84.conf_dir_priority.md
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_31_70_49_15.search_control.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_31_70_49_15.search_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_33_76_82_84.composite_tree.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_33_76_82_84.composite_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_36_17_84_44.check_env.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_36_17_84_44.check_env.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 feature_story: FS_36_17_84_44
 feature_title: check_env script
 feature_status: TODO
 ---
 
 The script is supposed to provide single place to perform multi-level verification.
 
-This script may overlap with functions from FS_85_33_46_53 `bootstrap_dev_env`.
+This script may overlap with functions from FS_85_33_46_53 `bootstrap_env`.
 
 See also FS_86_73_43_45 server control scripts.
 
 It can start with checking:
 *   Python version
 *   `venv` existence
 *   `argrelay` package existence
@@ -21,14 +21,17 @@
 *   whether completion is configured in shell
 *   config locations used
 *   any useful missing (or useless existing) settings in `~/.inputrc`
 *   server availability
 *   server version and compatibility
 *   prints server instance id and whatever we can query to verify its state
 *   print plugin list (serialized DAG) with types and activation status
+*   verify whether there is any issues between:
+    *   client-side plugin config
+    *   server-side plugin config
 *   any useful `readline` settings set or not
 *   FS_57_36_37_48 (multiple clients) show all registered clients
 *   show all registered commands (FS_57_36_37_48 per client)
 *   print the same line info what `@/exe/dev_shell.bash` prints about version, conf, URL, etc.
 
 What else?
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_39_58_01_91.query_cache.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_39_58_01_91.query_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_47_63_35_61.env_vars.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_47_63_35_61.env_vars.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     To produce debug output:
     *   Some logic simply needs to detect whether `ARGRELAY_DEBUG` is defined or not.
     *   For shell scripts, `ARGRELAY_DEBUG` value must contains char `s` ("script").
     *   For client-server perf output, `ARGRELAY_DEBUG` value must contains char `p` ("performance").
 
 *   `ARGRELAY_DEV_SHELL` used while running `@/exe/dev_shell.bash`, for example, to run some tests conditionally.
 
-*   `ARGRELAY_BOOTSTRAP_DEV_ENV` used while running `@/exe/bootstrap_dev_env.bash`, for example, to run some tests conditionally.
+*   `ARGRELAY_BOOTSTRAP_ENV` used while running `@/exe/bootstrap_env.bash`, for example, to run some tests conditionally.
 
 *   `ARGRELAY_CONF_BASE_DIR` specifies base dir for all config files (default ~ = user home).
 
     See also `FS_16_07_78_84.conf_dir_priority.md`.
 
 *   `ARGRELAY_CLIENT_COMMAND` provides the first (any) command name configured in `@/conf/shell_env.conf.bash`.
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ---
 feature_story: FS_49_96_50_77
 feature_title: config-only plugins
 feature_status: TEST
 ---
 
-TODO: Make it possible to override server-side plugin_config on client-side.
+TODO: FS_83_23_99_90 client plugin config override:
+      Make it possible to override server-side plugin_config on client-side.
       Because it should work for config-only plugins, it is a framework-defined approach
       (even though non-config-only plugins may choose whatever approach they want, there should be a suggested one).
 
 Keywords: `config_only` `config_only_plugins`
 
 Add config-only (demo) plugins:
 *   loader
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_55_57_45_04.enum_selector.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_55_57_45_04.enum_selector.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,13 +29,13 @@
 Ideally, the wish was to make it also work via nesting `@/exe/dev_shell.bash` from different installations
 (not only via `source`-ing `@/exe/shell_env.bash`).
 
 To make the feature work for `Alt+Shift+Q`, a map is used (see `argrelay_basename_to_client_path_map`).
 But maps in Bash are not `export`-able and cannot be used
 to communicate from (outer) `@/exe/dev_shell.bash` to nested (inner) `@/exe/dev_shell.bash`.
 
-Current workaround is to use `@/conf/dev_shell_rc.conf.bash` (see FS_58_61_77_69 `dev_shell`), for example:
+Current workaround is to use `@/conf/dev_shell_env.bash` (see FS_58_61_77_69 `dev_shell`), for example:
 ```
 source /path/to/argrelay/with/client_x/exe/shell_env.bash
 source /path/to/argrelay/with/client_y/exe/shell_env.bash
 ```
 This has to be configured manually per `argrelay` installation where extra command are required.
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_58_61_77_69.dev_shell.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_58_61_77_69.dev_shell.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ---
 feature_story: FS_58_61_77_69
 feature_title: convenient `dev_shell`
 feature_status: TEST
 ---
 
-See also FS_85_33_46_53 `bootstrap_dev_env`.
+See also FS_85_33_46_53 `bootstrap_env`.
 
 # Idea
 
 This feature supports quick non-intrusive shell session with configured `argrelay`:
 *   quick: single command `@/exe/dev_shell.bash` should do all the necessary steps to set up environment temporarily
 *   non-intrusive: user environment is not affected (e.g. no changes to `~/.bashrc`) - only current shell session
 
 See demo from the main [`readme.md`][root_readme.md] how it is used.
 
 # Config
 
 The script is normally immutable (symlink-ed to installed Python package).
 
-In order to automate adding some extra shell settings use mutable `@/conf/dev_shell_rc.conf.bash`.
+In order to automate adding some extra shell settings use mutable `@/conf/dev_shell_env.bash`.
 
 [root_readme.md]: ../../readme.md
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_62_25_92_06.assigned_context.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_62_25_92_06.assigned_context.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_63_63_14_08.generated_config.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_63_63_14_08.generated_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_66_17_43_42.test_infra.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_66_17_43_42.test_infra.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_67_16_61_97.git_plugin.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_67_16_61_97.git_plugin.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_71_87_33_52.help_hint.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_71_87_33_52.help_hint.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_72_40_53_00.fill_control.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_72_40_53_00.fill_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_80_45_89_81.integrated_functions.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_80_45_89_81.integrated_functions.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_85_33_46_53.bootstrap_env.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 ---
 feature_story: FS_85_33_46_53
-feature_title: process to `bootstrap_dev_env`
+feature_title: process to `bootstrap_env`
 feature_status: TEST
 ---
 
 See also FS_58_61_77_69 `dev_shell`.
 
 # Purpose
 
 This feature covers initial setup and upgrades of `argrelay`-integrated projects (their development environments).
 
 This may overlap with functions from FS_36_17_84_44 check_env script.
 
-The idea is to have a single `@/exe/bootstrap_dev_env.bash` script which:
+The idea is to have a single `@/exe/bootstrap_env.bash` script which:
 *   Loads `@/conf/python_env.conf.bash` (or prompts user if it does not exist) and inits `venv`.
-*   Runs project-specific custom `@/exe/deploy_project.bash` (or prompts user if it does not exist).
+*   Runs project-specific custom `@/exe/install_project.bash` (or prompts user if it does not exist).
 *   Copies fresh version of itself from `argrelay` (for future use) and starts it to ensure it works.
 *   Runs project-specific custom `@/exe/build_project.bash` (or prompts user if it does not exist).
-*   Deploys necessary configs and scripts.
+*   Installs necessary configs and scripts.
 *   Generates client and server executables under `@/bin/`.
-*   Updates `@/conf/dev_env_packages.txt`.
+*   Updates `@/conf/env_packages.txt`.
 *   ...
 
-Script `@/exe/bootstrap_dev_env.bash` is supposed to be version controlled in the target project.
+Script `@/exe/bootstrap_env.bash` is supposed to be version controlled in the target project.
 It is added to the target project repo so that it can be re-run during subsequent upgrades<br/>
 (without searching for it outside the project repo).
 
 # Scenarios
 
-There are three scenarios for `@/exe/bootstrap_dev_env.bash` (but it can be re-run at any time):
+There are three scenarios for `@/exe/bootstrap_env.bash` (but it can be re-run at any time):
 1. [`bootstrap_procedure.1.project_creation.md`][bootstrap_procedure.1.project_creation.md]
-2. [`bootstrap_procedure.2.initial_deployment.md`][bootstrap_procedure.2.initial_deployment.md]
+2. [`bootstrap_procedure.2.initial_installation.md`][bootstrap_procedure.2.initial_installation.md]
 3. [`bootstrap_procedure.3.argrelay_upgrade.md`][bootstrap_procedure.3.argrelay_upgrade.md]
 
 # Package management
 
-DEP = `@/conf/dev_env_packages.txt`
+DEP = `@/conf/env_packages.txt`
 
 Essentially, DEP is what normally called [`requirements.txt`][requirements_txt] and [generated via `pip freeze`][DEP_generation].
 
 DEP excludes packages installed locally in [editable mode][editable_mode] because:
 *   version info (e.g. Git commit id) for editable mode quickly become obsolete (not worth committing to the DEP)
-*   details of deployment are outsourced/delegated to `@/exe/deploy_project.bash` (already version-controlled)
+*   details of installation are outsourced/delegated to `@/exe/install_project.bash` (already version-controlled)
 
 ## Requirement
 
-There are requirements bootstrap script implements (package deployment steps):
+There are requirements bootstrap script implements (package installation steps):
 
 *   S1: Install (non-local) packages as specified by DEP.
 
     Purpose: be able to reproduce dev env.
 
 *   S2: Install local packages (owned by the target repo) on top of that.
 
@@ -61,37 +61,37 @@
 
 Note how output of S3 becomes intput of S1.
 
 ## Implementation
 
 The bootstrap script should take special care to respect DEP, but:
 
-*   Entire deployment process (S1 and S2) is delegated to `@/exe/deploy_project.bash` instead.
+*   Entire installation process (S1 and S2) is delegated to `@/exe/install_project.bash` instead.
 
-    It is expected that `@/exe/deploy_project.bash` (normally, not necessarily):
-    *   S1: [installs DEP via `pip install`][DEP_deployment]
-    *   S2: [installs any local packages in editable mode][local_deployment]
+    It is expected that `@/exe/install_project.bash` (normally, not necessarily):
+    *   S1: [installs DEP via `pip install`][DEP_installation]
+    *   S2: [installs any local packages in editable mode][local_installation]
 
 *   What bootstrap script takes care of directly is S3 above only.
 
     S3 captures result of S1 and S2.
 
     Note that if S1 and S2 are implemented as expected, the DEP file **stays unchanged**<br/>
     after repeated bootstrap invocation.
 
 ## Package upgrade procedure
 
 In order to upgrade (or downgrade) any DEP package:
-*   specify new version in DEP or remove its entry (to give freedom to deployment scripts to select other version)
-*   install either manually via `pip` or automatically via bootstrap to let `@/exe/deploy_project.bash` do it
-*   re-run bootstrap to re-deploy and re-capture new DEP
+*   specify new version in DEP or remove its entry (to give freedom to installation scripts to select other version)
+*   install either manually via `pip` or automatically via bootstrap to let `@/exe/install_project.bash` do it
+*   re-run bootstrap to re-install and re-capture new DEP
 
 [bootstrap_procedure.1.project_creation.md]: ../dev_notes/bootstrap_procedure.1.project_creation.md
-[bootstrap_procedure.2.initial_deployment.md]: ../dev_notes/bootstrap_procedure.2.initial_deployment.md
+[bootstrap_procedure.2.initial_installation.md]: ../dev_notes/bootstrap_procedure.2.initial_installation
 [bootstrap_procedure.3.argrelay_upgrade.md]: ../dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
 
 [requirements_txt]: https://www.google.com/search?q=python+requirements.txt
 [editable_mode]: https://github.com/pypa/packaging.python.org/blob/6c27b1f0517ba3db46558a7d0b821ce701307b80/source/guides/distributing-packages-using-setuptools.rst#working-in-development-mode
-[DEP_generation]: https://github.com/argrelay/argrelay/blob/v0.5.0.final/exe/bootstrap_dev_env.bash#L499
-[DEP_deployment]: https://github.com/argrelay/argrelay/blob/v0.5.0.final/exe/deploy_project.bash#L10
-[local_deployment]: https://github.com/argrelay/argrelay/blob/v0.5.0.final/exe/deploy_project.bash#L14
+[DEP_generation]: https://github.com/argrelay/argrelay/blob/v0.5.0.final/exe/bootstrap_env.bash#L499
+[DEP_installation]: https://github.com/argrelay/argrelay/blob/v0.5.0.final/exe/install_project.bash#L10
+[local_installation]: https://github.com/argrelay/argrelay/blob/v0.5.0.final/exe/install_project.bash#L14
```

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_91_88_07_23.jump_tree.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_91_88_07_23.jump_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_92_75_93_01.clean_command_line.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_92_75_93_01.clean_command_line.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/feature_stories/FS_97_64_39_94.arg_buckets.md` & `argrelay-0.7.2.dev0/docs/feature_stories/FS_97_64_39_94.arg_buckets.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/readme.md` & `argrelay-0.7.2.dev0/docs/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/release_notes/readme.md` & `argrelay-0.7.2.dev0/docs/release_notes/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/release_notes/v0.0.0.dev27.md` & `argrelay-0.7.2.dev0/docs/release_notes/v0.0.0.dev27.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_30_69_19_14.infinite_spinner.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md` & `argrelay-0.7.2.dev0/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md`

 * *Files 27% similar despite different names*

```diff
@@ -3,43 +3,32 @@
 
 TODO:
 *   Introduce `@/data/` dir. And make importable yaml (e.g. from `@/data/`) for server config.
 
 *   TODO: Move `argrelay_client` and `argrelay_server` out of `@/bin/` because multiple servers will clash in PATH.
           OR... Will it still work (simply the last added will be invoked, but it invoked via symlinks -> always correct one)? If yes, keep it.
 
-*   Rename `deploy` in some config/script files to `install`.
-
 Main scripts:
-*   TODO: Rename `bootstarp_dev_env` to `bootstrap_env`.
-*   TODO: Rename? `dev_shell` to `env_shell`. Maybe keep as is?
+*   TODO: Rename? `dev_shell` to `test_shell`. Maybe keep as is? Consider that it is required by many scripts...
 
 *   TODO: Rename rest API:
     *   `describe_line_args` -> `query_enum_items` (to match func_id)
     *   `propose_arg_values` -> `complete_line`
     *   `relay_line_args` -> `invoke_line`
 
+*   TODO: Rename: `ReservedArgType` to `ReservedPropName`
+
+*   TODO: Rename: convert item inside `ReservedArgType.*` to `camel_case`.
+
 *   TODO: Rename: `relay_demo` to something not cut-off `relay`, at least, both `a` and `r` (something `*ar*`) should be included.
           Something unique yet single word better containing `a` and `r`.
 
-*   DONE: Rename: `argrelay.server.*` -> `argrelay_server` (to search `argrelay_server` and find relevant stuff).
-*   DONE: Rename: `argrelay.client.*` -> `argrelay_client` (to search `argrelay_client` and find relevant stuff).
 *   TODO: Rename: `relay_server` package to `argrelay_server` (to search `argrelay_server` and find relevant stuff).
 *   TODO: Rename: `relay_client` package to `argrelay_client` (to search `argrelay_client` and find relevant stuff).
 
-TODO: Decide `[script].conf` vs `[script].conf.bash` ? I think 2nd is more systematic.
-
-*   DONE: Rename: `@/conf/python_conf.bash` -> `@/conf/python_env.conf.bash`
-*   DONE: Rename: `@/exe/argrelay_rc.bash` -> `@/exe/shell_env.bash`
-*   DONE: Rename: `@/conf/argrelay_rc_conf.bash` -> `@/conf/shell_env.conf.bash`
-*   TODO: Rename: `@/exe/deploy_config_files_conf.bash` -> `@/exe/install_config_files.conf.bash`
-
-*   TODO: Rename? `@/conf/dev_shell_rc.conf.bash` -> `@/conf/dev_shell_env.conf.bash`
-*   TODO: Review for rename: `dev_shell_rc.conf.bash` - is it `*.conf.bash` or simply `*.bash`?
-
 TODO:
 *   Rename all enum items to underscore (e.g. `ServerAction.ProposeArgValues` -> `ServerAction.propse_args_values`).
 *   Consider renaming URL, for example (`_` to `-`, shorten, rethink):
     *   propose_arg_values -> propose-options
     *   describe_line_args -> enum-options
     *   relay_line_args -> invoke-with-options
 
@@ -50,8 +39,8 @@
 *   TODO: Rename all `func_id` to be prefixed with `func_id`, for example, `query_enum_items_func` -> `func_id_query_enum_items`.
 *   Rename: prefix all `func_id` with `func_id`, for example: `goto_service_func` -> `func_id_goto_service`
 
 TODO:
 *   Shorten name `EnvelopeContainer.filled_types_to_values_hidden_by_defaults` to `default_override`-s.
 
 TODO:
-*   TODO: `deploy_files_procedure` should use 4 config params (instead of 3) - one more is destination dir (not hardcoded `conf`, not hardcoded `exe`, but also `data`, or something else).
+*   TODO: `install_files_procedure` should use 4 config params (instead of 3) - one more is destination dir (not hardcoded `conf`, not hardcoded `exe`, but also `data`, or something else).
```

### Comparing `argrelay-0.7.1.dev9/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md` & `argrelay-0.7.2.dev0/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/test_data/TD_63_37_05_36.demo_services_data.md` & `argrelay-0.7.2.dev0/docs/test_data/TD_63_37_05_36.demo_services_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/test_data/TD_70_69_38_46.no_data.md` & `argrelay-0.7.2.dev0/docs/test_data/TD_70_69_38_46.no_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md` & `argrelay-0.7.2.dev0/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md` & `argrelay-0.7.2.dev0/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/readme.md` & `argrelay-0.7.2.dev0/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -195,16 +195,17 @@
 
     ```sh
     less ./logs/relay_demo.bash.log
     ```
 
 *   Inspect configs:
 
-    *   `@/conf/argrelay_server.yaml`
     *   `@/conf/argrelay_client.json`
+    *   `@/conf/argrelay_server.yaml`
+    *   `@/conf/argrelay_plugin.yaml`
 
 *   To reset the demo, remove `@/conf`:
 
     ```sh
     rm conf
     ```
```

### Comparing `argrelay-0.7.1.dev9/setup.py` & `argrelay-0.7.2.dev0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # All paths start with `top_dir_path`:
     return file_paths
 
 
 setuptools.setup(
     name = "argrelay",
     # See `docs/dev_notes/version_format.md`:
-    version = "0.7.1.dev9",
+    version = "0.7.2.dev0",
     author = "uvsmtid",
     author_email = "uvsmtid@gmail.com",
     description = "Tab-completion & data search server = total recall for Bash shell",
     long_description = """
 See: https://github.com/argrelay/argrelay
     """,
     long_description_content_type = "text/markdown",
@@ -91,32 +91,33 @@
         "argrelay_docs": "./",
         "argrelay_data": "./",
     },
     package_data = {
         "argrelay": [
 
             # config files:
-            "sample_conf/argrelay_server.yaml",
             "sample_conf/argrelay_client.json",
+            "sample_conf/argrelay_server.yaml",
+            "sample_conf/argrelay_plugin.yaml",
 
             # GUI client:
             "relay_server/gui_static/argrelay_client.js",
             "relay_server/gui_static/argrelay_favicon.ico",
             "relay_server/gui_static/argrelay_style.css",
             "relay_server/gui_static/external_link.svg",
             "relay_server/gui_templates/argrelay_main.html",
 
             # other resource files:
             "custom_integ_res/argrelay_common_lib.bash",
             "custom_integ_res/shell_env.bash",
-            "custom_integ_res/bootstrap_dev_env.bash",
+            "custom_integ_res/bootstrap_env.bash",
             "custom_integ_res/check_env.bash",
             "custom_integ_res/dev_shell.bash",
             "custom_integ_res/init_shell_env.bash",
-            "custom_integ_res/upgrade_all_packages.bash",
+            "custom_integ_res/upgrade_env_packages.bash",
 
         ],
         "argrelay_docs": list_dir("./docs/") + [
             "readme.md",
         ],
         "argrelay_data": list_dir("./data/"),
     },
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_local/AbstractLocalClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_local/AbstractLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py` & `argrelay-0.7.2.dev0/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/client_spec/ShellContext.py` & `argrelay-0.7.2.dev0/src/argrelay/client_spec/ShellContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeForestSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeForestSchema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from marshmallow import fields, RAISE
 
 from argrelay.composite_tree.CompositeForest import CompositeForest
-from argrelay.composite_tree.CompositeNodeSchema import CompositeNodeSchema, node_type_, sub_tree_, zero_arg_node_desc
-from argrelay.composite_tree.CompositeNodeType import CompositeNodeType
+from argrelay.composite_tree.CompositeNodeSchema import CompositeNodeSchema, zero_arg_node_desc
 from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 
 tree_roots_ = "tree_roots"
 
 
 class CompositeForestSchema(ObjectSchema):
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeInfoType.py` & `argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeInfoType.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     zero_arg_interp_tree = auto()
     """
     See FS_42_76_93_51 very first zero arg mapping interp.
 
     TODO: It is identical to `interp_tree`, but `interp_tree` does not include zero arg components.
     """
 
-
     jump_tree = auto()
     """
     See FS_91_88_07_23 jump tree.
 
     A tree of `CompositeNodeType.interp_tree_node` under `CompositeNodeType.zero_arg_node`
     with leaves set to absolute jump path within `composite_tree`.
     """
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeNode.py` & `argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeNode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeNodeSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeNodeSchema.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         *   Note that `BaseNodeSchema` has no `node_type` (instead, it is defined in `CompositeNodeSchema`).
         """
         return type(self).model_class(
             **input_dict,
             node_type = self.node_type,
         )
 
+
 class ZeroArgNodeSchema(BaseNodeSchema):
     """
     See FS_42_76_93_51 very first zero arg mapping interp.
     """
 
     class Meta:
         unknown = RAISE
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeNodeType.py` & `argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeNodeType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/composite_tree/CompositeTreeWalker.py` & `argrelay-0.7.2.dev0/src/argrelay/composite_tree/CompositeTreeWalker.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,15 @@
         elif self.curr_node.node_type is CompositeNodeType.tree_path_node:
             return TraverseDecision.skip_sub_tree
         elif self.curr_node.node_type is CompositeNodeType.func_tree_node:
             return TraverseDecision.skip_sub_tree
         else:
             raise Exception(f"Unknown: {self.curr_node.node_type}")
 
+
 class _CompositeTreeWalker_jump_tree(AbstractCompositeTreeWalker):
 
     def __init__(
         self,
         composite_forest: CompositeForest,
         info_type: CompositeInfoType,
     ):
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/composite_tree/DictTreeWalker.py` & `argrelay-0.7.2.dev0/src/argrelay/composite_tree/DictTreeWalker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import string
 from collections.abc import Callable
 from copy import deepcopy
 from typing import Union, Sequence
 
 from argrelay.composite_tree.CompositeInfoType import CompositeInfoType
 
 surrogate_node_id_ = ""
@@ -125,14 +126,21 @@
                 return False
         else:
             # `outer_seq` is smaller than `inner_seq`:
             return False
     return True
 
 
+def contains_whitespace(s):
+    for c in s:
+        if c in string.whitespace:
+            return True
+    return False
+
+
 class DictTreeWalker:
     """
     This tree walker is used to build various data structures extracted from (simple) `dict` trees:
     *   FS_01_89_09_24 interp tree
     *   FS_26_43_73_72 func tree
     *   FS_91_88_07_23 jump tree
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/BaseConfigDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/BaseConfigDelegator.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         function_container = interp_ctx.envelope_containers[function_container_ipos_]
         delegator_plugin_instance_id = (
             function_container.data_envelopes[0][instance_data_]
             [delegator_plugin_instance_id_]
         )
         invocation_input = InvocationInput.with_interp_context(
             interp_ctx,
-            delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+            delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
                 delegator_plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
 
     @staticmethod
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyLoader.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/FuncConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/FuncConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoArgType.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoDelegator.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         function_container = interp_ctx.envelope_containers[function_container_ipos_]
         delegator_plugin_instance_id = (
             function_container.data_envelopes[0][instance_data_]
             [delegator_plugin_instance_id_]
         )
         invocation_input = InvocationInput.with_interp_context(
             interp_ctx,
-            delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+            delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
                 delegator_plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
 
     @staticmethod
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoLoader.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoLoader.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,36 @@
 from argrelay.schema_config_core_server.EnvelopeCollectionSchema import init_envelop_collections
 from argrelay.schema_config_interp.DataEnvelopeSchema import (
     envelope_id_,
     envelope_payload_,
 )
 
 
+def normalize_single_line_to_black_spaces(
+    s: str,
+) -> str:
+    """
+    Get rid of white spaces.
+
+    See FS_99_81_19_25 no space in options.
+    """
+    return s.strip().replace(" ", "_")
+
+
+def normalize_multiple_lines_to_black_spaces(
+    s: str,
+) -> str:
+    """
+    Get rid of multiple lines (take the first one only) and white spaces.
+
+    See FS_99_81_19_25 no space in options.
+    """
+    return s.partition('\n')[0].strip().replace(" ", "_")
+
+
 class GitRepoLoader(AbstractLoader):
     """
     Implements FS_67_16_61_97 git_plugin.
     """
 
     def load_config(
         self,
@@ -105,15 +127,15 @@
                 repo_base_abs_path = repo_base_path
             else:
                 repo_base_abs_path = os.path.join(get_argrelay_dir(), repo_base_path)
 
             # Process repo entries collecting `repo_root_rel_path` and `repo_root_abs_path`:
             for repo_entry in repo_entries:
 
-                repo_root_rel_path: str = repo_entry[repo_rel_path_]
+                repo_root_rel_path: str = repo_entry[repo_rel_path_] or "."
                 repo_root_abs_path: str = os.path.join(repo_base_abs_path, repo_root_rel_path)
 
                 if not repo_entry[is_repo_enabled_]:
                     eprint(f"INFO: disabled repo: {repo_root_abs_path}")
                     continue
 
                 # Deduplicate Git root paths:
@@ -190,17 +212,21 @@
                             GitRepoArgType.git_repo_root_abs_path.name: repo_root_abs_path,
                             GitRepoArgType.git_repo_root_base_name.name: repo_root_base_name,
                             #
                             GitRepoArgType.git_repo_tag_name.name: git_tag.name,
                             #
                             GitRepoArgType.git_repo_commit_id.name: git_commit.hexsha,
                             GitRepoArgType.git_repo_short_commit_id.name: git_commit.hexsha[:7],
-                            GitRepoArgType.git_repo_commit_author_name.name: git_commit.author.name,
-                            GitRepoArgType.git_repo_commit_author_email.name: git_commit.author.email,
-                            GitRepoArgType.git_repo_commit_message.name: git_commit.message,
+                            GitRepoArgType.git_repo_commit_author_name.name: normalize_single_line_to_black_spaces(
+                                git_commit.author.name,
+                            ),
+                            GitRepoArgType.git_repo_commit_author_email.name: git_commit.author.email.lower(),
+                            GitRepoArgType.git_repo_commit_message.name: normalize_multiple_lines_to_black_spaces(
+                                git_commit.message,
+                            ),
                             GitRepoArgType.git_repo_commit_date.name: commit_date_utc,
                             GitRepoArgType.git_repo_commit_time.name: commit_time_utc,
                         })
                         self.enrich_git_repo_object(tag_envelope)
                         tag_envelopes.append(tag_envelope)
 
                 load_repo_commits = repo_entry[load_repo_commits_]
@@ -228,17 +254,21 @@
                             ReservedArgType.EnvelopeClass.name: GitRepoEnvelopeClass.ClassGitCommit.name,
                             GitRepoArgType.git_repo_root_rel_path.name: repo_root_rel_path,
                             GitRepoArgType.git_repo_root_abs_path.name: repo_root_abs_path,
                             GitRepoArgType.git_repo_root_base_name.name: repo_root_base_name,
                             #
                             GitRepoArgType.git_repo_commit_id.name: git_commit.hexsha,
                             GitRepoArgType.git_repo_short_commit_id.name: git_commit.hexsha[:7],
-                            GitRepoArgType.git_repo_commit_author_name.name: git_commit.author.name,
-                            GitRepoArgType.git_repo_commit_author_email.name: git_commit.author.email.lower(),
-                            GitRepoArgType.git_repo_commit_message.name: git_commit.message,
+                            GitRepoArgType.git_repo_commit_author_name.name: normalize_single_line_to_black_spaces(
+                                git_commit.author.name,
+                            ),
+                            GitRepoArgType.git_repo_commit_author_email.name: git_commit.author.email,
+                            GitRepoArgType.git_repo_commit_message.name: normalize_multiple_lines_to_black_spaces(
+                                git_commit.message,
+                            ),
                             GitRepoArgType.git_repo_commit_date.name: commit_date_utc,
                             GitRepoArgType.git_repo_commit_time.name: commit_time_utc,
                         })
                         self.enrich_git_repo_object(commit_envelope)
                         commit_envelopes.append(commit_envelope)
 
         return static_data
@@ -260,15 +290,15 @@
     def enrich_git_repo_object(
         self,
         data_envelope: dict,
     ) -> None:
         object_categories: list[str] = self.categorize_git_object(data_envelope)
 
         if not object_categories:
-            object_categories.append("UKNOWN_category")
+            object_categories.append("UNKNOWN_category")
 
         data_envelope.update({
             GitRepoArgType.git_repo_object_category.name: object_categories,
         })
 
     def categorize_git_object(
         self,
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceArgType.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceArgType.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,12 +37,12 @@
 
     access_type = auto()
 
     # ---
 
     live_status = auto()
     """
-    TODO: Currently `live_status` is not used - it can be thought of as manually or dynamically assigned to the resource.
+    A value manually or dynamically assigned to the resource indicating its status.
     """
 
     def __str__(self):
         return self.name
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceDelegator.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     error_delegator_custom_data_desc,
     error_delegator_stub_custom_data_example,
 )
 from argrelay.plugin_delegator.NoopDelegator import NoopDelegator
 from argrelay.relay_server.LocalServer import LocalServer
 from argrelay.runtime_context.InterpContext import InterpContext
 from argrelay.runtime_data.AssignedValue import AssignedValue
+from argrelay.runtime_data.PluginConfig import PluginConfig
 from argrelay.runtime_data.ServerConfig import ServerConfig
 from argrelay.schema_config_interp.DataEnvelopeSchema import (
     instance_data_,
 )
 from argrelay.schema_config_interp.FunctionEnvelopeInstanceDataSchema import (
     delegator_plugin_instance_id_,
     search_control_list_,
@@ -69,41 +70,41 @@
             # Setting `ArgSource.DefaultValue`: it cannot override any, right? No point to handle assigned case:
             pass
     return False
 
 
 def redirect_to_no_func_error(
     interp_ctx,
-    server_config,
+    plugin_config,
 ):
     return redirect_to_error(
         interp_ctx,
-        server_config,
+        plugin_config,
         "ERROR: objects cannot be searched until function is fully qualified",
         1,
     )
 
 
 def redirect_to_error(
     interp_ctx,
-    server_config,
+    plugin_config: PluginConfig,
     error_message,
     error_code,
 ):
     # Redirect to `ErrorDelegator`:
-    # TODO: Do not hardcode plugin id (instance of `ErrorDelegator`):
+    # TODO: TODO_62_75_33_41: Do not hardcode plugin instance id (instance of `ErrorDelegator`):
     delegator_plugin_instance_id = f"{ErrorDelegator.__name__}.default"
     custom_plugin_data = {
         error_message_: error_message,
         error_code_: error_code,
     }
     error_delegator_custom_data_desc.validate_dict(custom_plugin_data)
     invocation_input = InvocationInput.with_interp_context(
         interp_ctx,
-        delegator_plugin_entry = server_config.plugin_instance_entries[delegator_plugin_instance_id],
+        delegator_plugin_entry = plugin_config.plugin_instance_entries[delegator_plugin_instance_id],
         custom_plugin_data = custom_plugin_data,
     )
     return invocation_input
 
 
 class ServiceDelegator(AbstractDelegator):
 
@@ -144,14 +145,15 @@
                 {"code": ServiceArgType.code_maturity.name},
                 {"stage": ServiceArgType.flow_stage.name},
                 {"region": ServiceArgType.geo_region.name},
                 {"cluster": ServiceArgType.cluster_name.name},
                 # ClassHost:
                 {"host": ServiceArgType.host_name.name},
                 # ---
+                {"status": ServiceArgType.live_status.name},
                 {"ip": ServiceArgType.ip_address.name},
             ],
         )
 
         service_search_control = populate_search_control(
             class_to_collection_map,
             ServiceEnvelopeClass.ClassService.name,
@@ -208,28 +210,28 @@
                 ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
                 ReservedArgType.HelpHint.name: "Go (log in) to remote host and dir path with specified service",
                 ReservedArgType.FuncId.name: goto_service_func_,
             },
             {
                 instance_data_: {
                     func_id_: desc_host_func_,
-                    # TODO: Do not hardcode plugin id (instance of `NoopDelegator`):
+                    # TODO: DTODO_62_75_33_41: Do not hardcode plugin instance id (instance of `NoopDelegator`):
                     delegator_plugin_instance_id_: f"{NoopDelegator.__name__}.default",
                     search_control_list_: [
                         host_search_control,
                     ],
                 },
                 ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
                 ReservedArgType.HelpHint.name: "Describe remote host",
                 ReservedArgType.FuncId.name: desc_host_func_,
             },
             {
                 instance_data_: {
                     func_id_: desc_service_func_,
-                    # TODO: Do not hardcode plugin id (instance of `NoopDelegator`):
+                    # TODO: TODO_62_75_33_41: Do not hardcode plugin instance id (instance of `NoopDelegator`):
                     delegator_plugin_instance_id_: f"{NoopDelegator.__name__}.default",
                     search_control_list_: [
                         service_search_control,
                     ],
                 },
                 ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
                 ReservedArgType.HelpHint.name: "Describe service instance",
@@ -395,28 +397,28 @@
                 .get_query_engine()
                 .query_data_envelopes_for(vararg_container)
             )
 
             # Actual implementation is not defined for demo:
             return redirect_to_error(
                 interp_ctx,
-                local_server.server_config,
+                local_server.plugin_config,
                 error_delegator_stub_custom_data_example[error_message_],
                 error_delegator_stub_custom_data_example[error_code_],
             )
         elif func_id in [
             diff_service_func_,
         ]:
             # TODO_75_52_01_67: `arg_bucket`-s to support multiple var args:
             #                   query both service lists and compare them.
 
             # Actual implementation is not defined for demo:
             return redirect_to_error(
                 interp_ctx,
-                local_server.server_config,
+                local_server.plugin_config,
                 error_delegator_stub_custom_data_example[error_message_],
                 error_delegator_stub_custom_data_example[error_code_],
             )
         elif func_id in [
             list_host_func_,
             list_service_func_,
         ]:
@@ -431,15 +433,15 @@
                 )
 
                 # Plugin to invoke on client side:
                 delegator_plugin_instance_id = self.plugin_instance_id
                 # Package into `InvocationInput` payload object:
                 invocation_input = InvocationInput.with_interp_context(
                     interp_ctx,
-                    delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+                    delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
                         delegator_plugin_instance_id
                     ],
                     custom_plugin_data = {},
                 )
                 return invocation_input
             else:
                 return redirect_to_no_func_error(
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceLoader.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,19 @@
             service_envelopes,
         )
         self.populate_TD_43_24_76_58_single(
             cluster_envelopes,
             host_envelopes,
             service_envelopes,
         )
+        self.populate_TD_39_25_11_76_missing_props(
+            cluster_envelopes,
+            host_envelopes,
+            service_envelopes,
+        )
 
         self.generate_envelope_id(cluster_envelopes + host_envelopes + service_envelopes)
 
         self.generate_help_hints(
             class_to_collection_map,
             static_data,
         )
@@ -181,15 +186,16 @@
         help_hint_envelopes = help_hint_envelope_collection.data_envelopes
 
         # Init index fields (if they do not exist):
         for help_hint_index_field in [
             ReservedArgType.EnvelopeClass.name,
             ReservedArgType.ArgType.name,
             ReservedArgType.ArgValue.name,
-            ReservedArgType.HelpHint.name,
+            # `ReservedArgType.HelpHint` is not indexed (and uses as search param) - instead, it is a search result:
+            # ReservedArgType.HelpHint.name,
         ]:
             if help_hint_index_field not in help_hint_index_fields:
                 help_hint_index_fields.append(help_hint_index_field)
 
         # Generating
         host_envelopes = static_data.envelope_collections[
             class_to_collection_map[ServiceEnvelopeClass.ClassHost.name]
@@ -1506,7 +1512,130 @@
                 ServiceArgType.code_maturity.name: "dev",
                 ServiceArgType.geo_region.name: "emea",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-emea-downstream",
                 ServiceArgType.host_name.name: "asdf",
             },
         ])
+
+    def populate_TD_39_25_11_76_missing_props(
+        self,
+        cluster_envelopes: list[dict],
+        host_envelopes: list[dict],
+        service_envelopes: list[dict],
+    ):
+        if not self.is_test_data_allowed("TD_39_25_11_76"):
+            return
+
+        cluster_envelopes.extend([
+
+            ############################################################################################################
+            # TD_39_25_11_76 # missing props: clusters
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassCluster.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-apac-downstream",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassCluster.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+            },
+
+        ])
+
+        host_envelopes.extend([
+
+            ############################################################################################################
+            # TD_39_25_11_76 # missing props: hosts
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-apac-downstream",
+                ServiceArgType.host_name.name: "qwer",
+                ServiceArgType.live_status.name: "green",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-apac-downstream",
+                ServiceArgType.host_name.name: "asdf",
+                ServiceArgType.live_status.name: "yellow",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-apac-downstream",
+                ServiceArgType.host_name.name: "zxcv",
+                # NOTE: `ServiceArgType.live_status` for this `data_envelope` is missing only in `apac` (not in `emea`).
+                # ServiceArgType.live_status.name: "red",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+                ServiceArgType.host_name.name: "qwer",
+                ServiceArgType.live_status.name: "green",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+                ServiceArgType.host_name.name: "asdf",
+                ServiceArgType.live_status.name: "yellow",
+            },
+
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_39_25_11_76",  # missing props
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassHost.name,
+                ServiceArgType.code_maturity.name: "dev",
+                ServiceArgType.geo_region.name: "emea",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "dev-emea-downstream",
+                ServiceArgType.host_name.name: "zxcv",
+                ServiceArgType.live_status.name: "red",
+            },
+        ])
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ/git_utils.py` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ/git_utils.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/argrelay_common_lib.bash` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/argrelay_common_lib.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/bootstrap_dev_env.bash` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/bootstrap_env.bash`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # Define with `s` in value to debug:
 if [[ "${ARGRELAY_DEBUG-}" == *s* ]]
 then
     set -x
     set -v
 fi
 
-if [[ -n "${bootstrap_dev_env_old_opts+x}" ]] ; then exit 1 ; fi
+if [[ -n "${bootstrap_env_old_opts+x}" ]] ; then exit 1 ; fi
 
 # Save `set`-able options to restore them at the end of this source-able script:
 # https://unix.stackexchange.com/a/383581/23886
 # Not saving history because:
 # *   it is not modified within `argrelay` scripts
 # *   it should not be restored in non-interactive files (disabled by default)
-bootstrap_dev_env_old_opts="$( set +o | grep -v "[[:space:]]history$" )"
+bootstrap_env_old_opts="$( set +o | grep -v "[[:space:]]history$" )"
 case "${-}" in
-    *e*) bootstrap_dev_env_old_opts="${bootstrap_dev_env_old_opts}; set -e" ;;
-      *) bootstrap_dev_env_old_opts="${bootstrap_dev_env_old_opts}; set +e" ;;
+    *e*) bootstrap_env_old_opts="${bootstrap_env_old_opts}; set -e" ;;
+      *) bootstrap_env_old_opts="${bootstrap_env_old_opts}; set +e" ;;
 esac
 
 ########################################################################################################################
 
 # Keep output-related `set`-able options same when this script is sourced
 # (otherwise, full debug output for bootstrap is adequate as it runs in hardly predictable target environment):
 if [[ "${0}" == "${BASH_SOURCE[0]}" ]] ; then
@@ -101,25 +101,25 @@
         echo -e "${failure_color}FAILURE:${reset_color} ${BASH_SOURCE[0]}: exit_code: ${exit_code}" 1>&2
         "${ret_command}" "${exit_code}"
     fi
 }
 
 trap color_failure_and_success_bootstrap_env EXIT
 
-# Let some code know that it runs under `@/exe/bootstrap_dev_env.bash` (e.g to run some tests conditionally):
-ARGRELAY_BOOTSTRAP_DEV_ENV="$(date)"
-export ARGRELAY_BOOTSTRAP_DEV_ENV
+# Let some code know that it runs under `@/exe/bootstrap_env.bash` (e.g to run some tests conditionally):
+ARGRELAY_BOOTSTRAP_ENV="$(date)"
+export ARGRELAY_BOOTSTRAP_ENV
 
 script_source="${BASH_SOURCE[0]}"
 # shellcheck disable=SC2034
 script_name="$( basename -- "${script_source}" )"
 # The dir of this script:
 # shellcheck disable=SC2034
 script_dir="$( cd -- "$( dirname -- "${script_source}" )" &> /dev/null && pwd )"
-# Note: In case of `bootstrap_dev_env.bash`, `argrelay_dir` is not `script_dir`, but always the current directory
+# Note: In case of `bootstrap_env.bash`, `argrelay_dir` is not `script_dir`, but always the current directory
 # (it is supposed to be started from the dir where project is being set up).
 # FS_29_54_67_86 dir_structure: current dir = `@/`:
 argrelay_dir="$( dirname "." )"
 
 # There are several cases this script is called:
 # *   (initial bootstrap) directly: in that case `script_dir` is inside orig `argrelay` distrib package
 # *   (`@/exe/dev_shell.bash`) indirectly: in that case `script_dir` is in `@/exe/` inside integration project dir
@@ -212,15 +212,15 @@
 
 if [[ ! -f "${argrelay_dir}/conf/python_env.conf.bash" ]]
 then
     echo "ERROR: \`${argrelay_dir}/conf/python_env.conf.bash\` does not exists" 1>&2
     echo "It is required to init \`venv\` with specific base Python interpreter." 1>&2
     echo "Provide \`${argrelay_dir}/conf/python_env.conf.bash\`, for example (copy and paste and modify):" 1>&2
     echo "" 1>&2
-    cat << 'deploy_project_EOF'
+    cat << 'python_env_conf_EOF'
 ########################################################################################################################
 # `argrelay` integration file: https://github.com/argrelay/argrelay
 # This config file is supposed to be owned and version-controlled by target project integrated with `argrelay`.
 
 # Path to `venv` to create or reuse:
 # shellcheck disable=SC2034
 path_to_venvX="venv"
@@ -229,15 +229,15 @@
 path_to_pythonX="/usr/local/bin/python3.7"
 # Custom prompt prefix - see:
 # https://docs.python.org/3/library/venv.html
 # --prompt PROMPT Provides an alternative prompt prefix for this environment.
 # shellcheck disable=SC2034
 venv_prompt_prefix="@"
 ########################################################################################################################
-deploy_project_EOF
+python_env_conf_EOF
     "${ret_command}" 1
 fi
 
 # Load user config for env vars:
 # *   path_to_pythonX
 # *   path_to_venvX
 source "${argrelay_dir}/conf/python_env.conf.bash"
@@ -301,26 +301,26 @@
 fi
 
 # Verify that Python versions for `path_to_pythonX` and `abs_path_to_venvX/bin/python` match:
 python_version_a="$( "${path_to_pythonX}" --version )"
 python_version_b="$( "${abs_path_to_venvX}/bin/python" --version )"
 if [[ "${python_version_a}" != "${python_version_b}" ]]
 then
-    # One way to attempt to resolve this is to remove `venv` and re-run `@/exe/bootstrap_dev_env.bash`:
+    # One way to attempt to resolve this is to remove `venv` and re-run `@/exe/bootstrap_env.bash`:
     echo "ERROR: version mismatch for Python to init \`venv\` and Python in existing \`venv\`: ${python_version_a} ${python_version_b}" 1>&2
     "${ret_command}" 1
 fi
 
 # Verify that `/path/to/python` after activation is the same file pointed to by `path_to_pythonX`.
 # If not, it is likely that chain of `python` symlinks within the new `venv` is broken
 # (leads to non-existing `python` binary) which should fail fast (otherwise, partially working state is confusing):
 full_path_to_python="$( command which python )"
 if [[ ! "${full_path_to_python}" -ef "${path_to_pythonX}" ]]
 then
-    # One way to attempt to resolve this is to remove `venv` and re-run `@/exe/bootstrap_dev_env.bash`:
+    # One way to attempt to resolve this is to remove `venv` and re-run `@/exe/bootstrap_env.bash`:
     echo "ERROR: path to \`python\` binary = \`${full_path_to_python}\` after activation of \`venv\` = \`${abs_path_to_venvX}\` is not linked to \`python\` binary = \`${path_to_pythonX}\` used to create this \`venv\`" 1>&2
     "${ret_command}" 1
 fi
 
 # Verify shebang using `/path/to/python` does not exceed the limit
 # (otherwise, shebang for client and server scripts will not work):
 # https://stackoverflow.com/a/10813634/441652
@@ -331,60 +331,60 @@
     echo "ERROR: path to \`python\` binary = \`${full_path_to_python}\` after activation of \`venv\` = \`${abs_path_to_venvX}\` exceeds 127 chars" 1>&2
     "${ret_command}" 1
 fi
 
 if [[ -n "${activate_venv_only_flag:-}" ]]
 then
     # Ths script is being run by `@/exe/dev_shell.bash` (sourced by `@/exe/init_shell_env.bash`).
-    # If bootstrap procedure is required, call `@/exe/bootstrap_dev_env.bash` itself without `activate_venv_only_flag`.
+    # If bootstrap procedure is required, call `@/exe/bootstrap_env.bash` itself without `activate_venv_only_flag`.
     # Python `venv` has already been activated - return, ignore the rest:
     "${ret_command}" 0
 fi
 
 # Continue with Python from `"${path_to_pythonX}"`:
 # - Use latest `pip`:
 python -m pip install --upgrade pip
 # - This avoids error on `import pkg_resources`:
 #   ModuleNotFoundError: No module named 'pkg_resources'
 python -m pip install --upgrade setuptools
 
-# Ensure `@/conf/dev_env_packages.txt` exists:
-touch "${argrelay_dir}/conf/dev_env_packages.txt"
+# Ensure `@/conf/env_packages.txt` exists:
+touch "${argrelay_dir}/conf/env_packages.txt"
 
 ########################################################################################################################
-# Deploy project dependencies.
+# Install project dependencies.
 
-if [[ ! -f "${argrelay_dir}/exe/deploy_project.bash" ]]
+if [[ ! -f "${argrelay_dir}/exe/install_project.bash" ]]
 then
-    echo "ERROR: \`${argrelay_dir}/exe/deploy_project.bash\` does not exists" 1>&2
+    echo "ERROR: \`${argrelay_dir}/exe/install_project.bash\` does not exists" 1>&2
     echo "It is required to install packages to extract artifacts from them." 1>&2
-    echo "Provide \`${argrelay_dir}/exe/deploy_project.bash\`, for example (copy and paste and modify):" 1>&2
+    echo "Provide \`${argrelay_dir}/exe/install_project.bash\`, for example (copy and paste and modify):" 1>&2
     echo "" 1>&2
     # TODO: This matches content of default config stored in `argrelay` repo - try to deduplicate.
-    cat << 'deploy_project_EOF'
+    cat << 'install_project_EOF'
 ########################################################################################################################
 # `argrelay` integration file: https://github.com/argrelay/argrelay
 
-# This is a custom deployment script *sourced* by `@/exe/bootstrap_dev_env.bash`.
+# This is a custom install script *sourced* by `@/exe/bootstrap_env.bash`.
 # Python `venv` is already activated before it is sourced.
 
-# Normally, for integration project, the deploy scripts like this should pip-install itself (in the editable mode).
+# Normally, for integration project, the install scripts like this should pip-install itself (in the editable mode).
 
-# Saved dev dependencies (if clean deployment is required, make `@/conf/dev_env_packages.txt` file empty):
-python -m pip install -r "${argrelay_dir}/conf/dev_env_packages.txt"
+# Saved env dependencies (if clean install is required, make `@/conf/env_packages.txt` file empty):
+python -m pip install -r "${argrelay_dir}/conf/env_packages.txt"
 
 # Use editable mode:
 # https://pip.pypa.io/en/latest/topics/local-project-installs/
 python -m pip install -e .[tests]
 ########################################################################################################################
-deploy_project_EOF
+install_project_EOF
     "${ret_command}" 1
 fi
 
-source "${argrelay_dir}/exe/deploy_project.bash"
+source "${argrelay_dir}/exe/install_project.bash"
 
 # Get path of `argrelay` module:
 argrelay_module_file_path="$(
 python << 'python_module_path_EOF'
 import argrelay
 print(argrelay.__file__)
 python_module_path_EOF
@@ -393,83 +393,83 @@
 
 ########################################################################################################################
 # Recurse into fresh copy of bootstrap.
 
 if [[ -z "${recursion_flag:-}" ]]
 then
     # Overwrite itself:
-    cp -p "${argrelay_module_dir_path}/custom_integ_res/bootstrap_dev_env.bash" "${argrelay_dir}/exe/"
+    cp -p "${argrelay_module_dir_path}/custom_integ_res/bootstrap_env.bash" "${argrelay_dir}/exe/"
     # Recursively call itself again (now with `recursion_flag`):
-    "${argrelay_dir}/exe/bootstrap_dev_env.bash" "recursion_flag"
+    "${argrelay_dir}/exe/bootstrap_env.bash" "recursion_flag"
     # Recursive call should have executed the rest of file:
     "${ret_command}" 0
 fi
 
 ########################################################################################################################
-# Define common deployment functions.
+# Define common install functions.
 
-function detect_file_deployment_command {
+function detect_file_install_command {
     # This func is used for the editable install mode cases.
-    # When config files (not resource files) need to be deployed from a distribution package,
+    # When config files (not resource files) need to be installed from a distribution package,
     # that package might be installed in editable mode.
     # *   If in editable mode, use symlinks.
     # *   If not in editable mode, use copy.
     # The detection of editable mode is done by looking at the `venv` path in the orig file.
     #
-    # Detect file deployment method based on path of the source (if copy) or the target (if symlink):
+    # Detect file install method based on path of the source (if copy) or the target (if symlink):
     # *   If the path contains path to `venv` (file is from orig package), copy.
     # *   If the path does not contain path to `venv` (file is from sources), symlink.
 
     # This is the source (if copy) or the target (if symlink):
     primary_path="$( realpath "${1}" )"
     # This is the target (if copy) or the link (if symlink):
     secondary_path="$( realpath "${2}" )"
     # `venv` path from `@/conf/python_env.conf.bash`:
     # shellcheck disable=SC2154
     abs_path_to_venvX="$( realpath "${path_to_venvX}")"
 
     if [[ "${primary_path}" == "${abs_path_to_venvX}"* ]]
     then
-        file_deployment_command="cp -p"
+        file_install_command="cp -p"
     else
-        file_deployment_command="ln -sn"
+        file_install_command="ln -sn"
     fi
 
-    eval "${file_deployment_command}" "${primary_path}" "${secondary_path}"
+    eval "${file_install_command}" "${primary_path}" "${secondary_path}"
 }
 
-function deploy_files_procedure {
+function install_files_procedure {
 
-    deploy_files_conf_path="${1}"
-    deployment_mode="${2}"
+    install_files_conf_path="${1}"
+    install_mode="${2}"
     target_dir="${3}"
     # Whether override should be used or not depends on whether the file is a config or it is a resource:
     # *   config files are specific to target environment and are kept untouched (manually updated if needed)
-    # *   resource files are common for all deployments - they represent the latest update and should be overriden
+    # *   resource files are common for all installs - they represent the latest update and should be overriden
     override_target_file="${4}"
 
     # Load user config for env vars:
     # *   module_path_file_tuples
     # shellcheck disable=SC1090
-    source "${deploy_files_conf_path}"
+    source "${install_files_conf_path}"
 
-    case "${deployment_mode}" in
+    case "${install_mode}" in
         "symlink_method")
             # Use symlinks (e.g. to modify files when they are part of Git repo):
-            file_deployment_command="ln -sn"
+            file_install_command="ln -sn"
         ;;
         "copy_method")
             # Use copies (e.g. to avoid modifying orig package content):
-            file_deployment_command="cp -p"
+            file_install_command="cp -p"
         ;;
         "detect_method")
-            file_deployment_command="detect_file_deployment_command"
+            file_install_command="detect_file_install_command"
         ;;
         *)
-            echo "ERROR: unknown deployment_mode: \"${deployment_mode}\"" 1>&2
+            echo "ERROR: unknown install_mode: \"${install_mode}\"" 1>&2
             "${ret_command}" 1
         ;;
     esac
 
     # Verify number of items in `module_path_file_tuples` is divisible by 3:
     # shellcheck disable=SC2154
     if [[ "$((${#module_path_file_tuples[@]}%3))" != "0" ]]
@@ -500,60 +500,61 @@
                 return 1
             fi
 
             # Test existence of the source file:
             config_file_path="${module_path}/${relative_dir_path}/${file_name}"
             test -f "${config_file_path}"
 
-            # Deploy file to the target:
+            # Install file to the target:
             if [[ ! -e "${target_dir}/${file_name}" ]] && [[ ! -L "${target_dir}/${file_name}" ]]
             then
-                eval "${file_deployment_command}" "${config_file_path}" "${target_dir}/${file_name}"
+                eval "${file_install_command}" "${config_file_path}" "${target_dir}/${file_name}"
             else
                 if [[ "${override_target_file}" == "override_target_file" ]]
                 then
                     rm "${target_dir}/${file_name}"
-                    eval "${file_deployment_command}" "${config_file_path}" "${target_dir}/${file_name}"
+                    eval "${file_install_command}" "${config_file_path}" "${target_dir}/${file_name}"
                 fi
             fi
         fi
     done
 }
 
 ########################################################################################################################
-# Prepare artifacts: deploy configs (conditionally copies or symlinks).
+# Prepare artifacts: install configs (conditionally copies or symlinks).
 
-deploy_files_conf_path="${argrelay_dir}/exe/deploy_config_files_conf.bash"
+install_files_conf_path="${argrelay_dir}/exe/config_files.conf.bash"
 
-if [[ ! -f "${deploy_files_conf_path}" ]]
+if [[ ! -f "${install_files_conf_path}" ]]
 then
-    echo "ERROR: \`${deploy_files_conf_path}\` does not exists" 1>&2
-    echo "It is required to know list of configs to be deployed." 1>&2
-    echo "Provide \`${deploy_files_conf_path}\`, for example (copy and paste and modify):" 1>&2
+    echo "ERROR: \`${install_files_conf_path}\` does not exists" 1>&2
+    echo "It is required to know list of configs to be installed." 1>&2
+    echo "Provide \`${install_files_conf_path}\`, for example (copy and paste and modify):" 1>&2
     echo "" 1>&2
     # TODO: This matches content of default config stored in `argrelay` repo - try to deduplicate.
-    cat << 'deploy_config_files_conf_EOF'
+    cat << 'config_files_conf_EOF'
 ########################################################################################################################
 # `argrelay` integration file: https://github.com/argrelay/argrelay
 # This config file is supposed to be owned and version-controlled by target project integrated with `argrelay`.
-# It is *sourced* by `@/exe/bootstrap_dev_env.bash` to configure `module_path_file_tuples` below.
+# It is *sourced* by `@/exe/bootstrap_env.bash` to configure `module_path_file_tuples` below.
 
 # Tuples specifying config files, format:
 # module_name relative_dir_path config_file_name
 module_path_file_tuples=(
     # Note: a project integrating `argrelay` must provide its own set of
     #       customized `argrelay` config files instead (from its own module).
     #       Integration assumes different plugins, their configs, etc.
 
     # For example:
-    # project_module sample_conf argrelay_server.yaml
     # project_module sample_conf argrelay_client.json
+    # project_module sample_conf argrelay_server.yaml
+    # project_module sample_conf argrelay_plugin.yaml
 )
 ########################################################################################################################
-deploy_config_files_conf_EOF
+config_files_conf_EOF
     "${ret_command}" 1
 fi
 
 # See `FS_16_07_78_84.conf_dir_priority.md`:
 if [[ -n "${ARGRELAY_CONF_BASE_DIR+x}" ]]
 then
     argrelay_conf_base_dir="${ARGRELAY_CONF_BASE_DIR}"
@@ -573,56 +574,56 @@
     if [[ ! -d "${argrelay_conf_base_dir}" ]]
     then
         echo "ERROR: (see FS_16_07_78_84.conf_dir_priority.md) path must be a dir or a symlink to dir: ${argrelay_conf_base_dir}" 1>&2
         "${ret_command}" 1
     fi
 fi
 
-deploy_files_procedure "${deploy_files_conf_path}" "detect_method" "${argrelay_conf_base_dir}" "do_not_override"
+install_files_procedure "${install_files_conf_path}" "detect_method" "${argrelay_conf_base_dir}" "do_not_override"
 
 ########################################################################################################################
-# Prepare artifacts: deploy resources (symlinks).
+# Prepare artifacts: install resources (symlinks).
 
-deploy_files_conf_path="${argrelay_dir}/exe/deploy_resource_files_conf.bash"
+install_files_conf_path="${argrelay_dir}/exe/resource_files.conf.bash"
 
-if [[ ! -f "${deploy_files_conf_path}" ]]
+if [[ ! -f "${install_files_conf_path}" ]]
 then
-    echo "ERROR: \`${deploy_files_conf_path}\` does not exists" 1>&2
-    echo "It is required to know list of resources to be deployed." 1>&2
-    echo "Provide \`${deploy_files_conf_path}\`, for example (copy and paste and modify):" 1>&2
+    echo "ERROR: \`${install_files_conf_path}\` does not exists" 1>&2
+    echo "It is required to know list of resources to be installed." 1>&2
+    echo "Provide \`${install_files_conf_path}\`, for example (copy and paste and modify):" 1>&2
     echo "" 1>&2
     # TODO: This matches content of default config stored in `argrelay` repo - try to deduplicate.
-    cat << 'deploy_resource_files_conf_EOF'
+    cat << 'resource_files_conf_EOF'
 ########################################################################################################################
 # `argrelay` integration file: https://github.com/argrelay/argrelay
 # This resource file is supposed to be owned and version-controlled by target project integrated with `argrelay`.
-# It is *sourced* by `@/exe/bootstrap_dev_env.bash` to configure `module_path_file_tuples` below.
+# It is *sourced* by `@/exe/bootstrap_env.bash` to configure `module_path_file_tuples` below.
 
 # Tuples specifying resource files, format:
 # module_name relative_dir_path resource_file_name
 module_path_file_tuples=(
     argrelay custom_integ_res argrelay_common_lib.bash
     argrelay custom_integ_res shell_env.bash
     argrelay custom_integ_res check_env.bash
     argrelay custom_integ_res dev_shell.bash
     argrelay custom_integ_res init_shell_env.bash
-    argrelay custom_integ_res upgrade_all_packages.bash
+    argrelay custom_integ_res upgrade_env_packages.bash
 )
 ########################################################################################################################
-deploy_resource_files_conf_EOF
+resource_files_conf_EOF
     "${ret_command}" 1
 fi
 
-deploy_files_procedure "${deploy_files_conf_path}" "symlink_method" "${argrelay_dir}/exe/" "override_target_file"
+install_files_procedure "${install_files_conf_path}" "symlink_method" "${argrelay_dir}/exe/" "override_target_file"
 
 ########################################################################################################################
 # Prepare artifacts: generate resources.
 
 # Generate `@/exe/run_argrelay_server`:
-cat << PYTHON_SERVER_EOF > "${argrelay_dir}/exe/run_argrelay_server"
+cat << run_argrelay_server_EOF > "${argrelay_dir}/exe/run_argrelay_server"
 #!$(which python)
 # \`argrelay\`-generated integration file: https://github.com/argrelay/argrelay
 # It is NOT supposed to be version-controlled per project as it:
 # *   is generated
 # *   differs per environment (due to different abs path to \`venv\`)
 # It should rather be added to \`.gitignore\`.
 
@@ -633,18 +634,18 @@
 # FS_29_54_67_86 dir_structure: \`@/exe/run_argrelay_server\` -> \`@/\`:
 misc_helper_common.set_argrelay_dir(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 from argrelay.relay_server.__main__ import main
 
 if __name__ == '__main__':
     main()
-PYTHON_SERVER_EOF
+run_argrelay_server_EOF
 
 # Generate `@/exe/run_argrelay_client`:
-cat << PYTHON_CLIENT_EOF > "${argrelay_dir}/exe/run_argrelay_client"
+cat << run_argrelay_client_EOF > "${argrelay_dir}/exe/run_argrelay_client"
 #!$(which python)
 # \`argrelay\`-generated integration file: https://github.com/argrelay/argrelay
 # It is NOT supposed to be version-controlled per project as it:
 # *   is generated
 # *   differs per environment (due to different abs path to \`venv\`)
 # It should rather be added to \`.gitignore\`.
 
@@ -655,43 +656,43 @@
 # FS_29_54_67_86 dir_structure: \`@/exe/run_argrelay_client\` -> \`@/\`:
 misc_helper_common.set_argrelay_dir(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 from argrelay.relay_client.__main__ import main
 
 if __name__ == '__main__':
     main()
-PYTHON_CLIENT_EOF
+run_argrelay_client_EOF
 
 # Make both executable:
 chmod u+x "${argrelay_dir}/exe/run_argrelay_client"
 chmod u+x "${argrelay_dir}/exe/run_argrelay_server"
 
 ########################################################################################################################
 # Generate source-able Bash config file and generate symlinks for command to be used with `argrelay`.
 
 if [[ ! -f "${argrelay_dir}/conf/shell_env.conf.bash" ]]
 then
     echo "ERROR: \`${argrelay_dir}/conf/shell_env.conf.bash\` does not exists" 1>&2
     echo "It is required to know which command names will have \`argrelay\` auto-completion." 1>&2
     echo "Provide \`${argrelay_dir}/conf/shell_env.conf.bash\`, for example (copy and paste and modify):" 1>&2
     echo "" 1>&2
-    cat << 'argelay_rc_conf_EOF'
+    cat << 'shell_env_conf_EOF'
 ########################################################################################################################
 # `argrelay` integration file: https://github.com/argrelay/argrelay
 # This config file is supposed to be owned and version-controlled by target project integrated with `argrelay`.
 
 # Bash array of command names (names of symlinks to `@/exe/run_argrelay_client`):
 # shellcheck disable=SC2034
 argrelay_bind_command_basenames=(
     relay_demo
     some_command
     service_relay_demo
 )
 ########################################################################################################################
-argelay_rc_conf_EOF
+shell_env_conf_EOF
     "${ret_command}" 1
 fi
 
 # Load user config for env vars:
 # *   argrelay_bind_command_basenames
 source "${argrelay_dir}/conf/shell_env.conf.bash"
 
@@ -744,15 +745,15 @@
     echo "Provide \`${argrelay_dir}/exe/build_project.bash\`, for example (copy and paste and modify):" 1>&2
     echo "" 1>&2
     # TODO: This matches content of default config stored in `argrelay` repo - try to deduplicate.
     cat << 'build_project_EOF'
 ########################################################################################################################
 # `argrelay` integration file: https://github.com/argrelay/argrelay
 
-# This is a custom build script *sourced* by `@/exe/bootstrap_dev_env.bash`.
+# This is a custom build script *sourced* by `@/exe/bootstrap_env.bash`.
 # Python `venv` is already activated before it is sourced.
 
 # Normally, for integration project, the build scripts like this should build and test itself.
 
 # It is fine to run tox on every start of FS_58_61_77_69 `dev_shell` because it is only used by `argrelay` devs:
 # Build and test:
 python -m tox
@@ -763,27 +764,27 @@
 
 # Provide project-specific build script:
 source "${argrelay_dir}/exe/build_project.bash"
 
 ########################################################################################################################
 # Capture dependencies.
 
-# Update `@/conf/dev_env_packages.txt` to know what was there at the time of bootstrapping:
-cat << 'REQUIREMENTS_EOF' > "${argrelay_dir}/conf/dev_env_packages.txt"
+# Update `@/conf/env_packages.txt` to know what was there at the time of bootstrapping:
+cat << 'REQUIREMENTS_EOF' > "${argrelay_dir}/conf/env_packages.txt"
 ###############################################################################
 # Note that these dependencies are not necessarily required ones,
 # those required are listed in `setup.py` script and can be installed as:
 # pip install -e .
 ###############################################################################
 REQUIREMENTS_EOF
 # FS_85_33_46_53 bootstrap package management:
 # Ignore `argrelay` itself (or anything installed in editable mode):
-pip freeze --exclude-editable >> "${argrelay_dir}/conf/dev_env_packages.txt"
+pip freeze --exclude-editable >> "${argrelay_dir}/conf/env_packages.txt"
 
 ########################################################################################################################
 
-eval "${bootstrap_dev_env_old_opts}"
-unset bootstrap_dev_env_old_opts
+eval "${bootstrap_env_old_opts}"
+unset bootstrap_env_old_opts
 
 ########################################################################################################################
 # EOF
 ########################################################################################################################
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/check_env.bash` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/check_env.bash`

 * *Files 3% similar despite different names*

```diff
@@ -57,40 +57,40 @@
     fi
 }
 
 trap color_failure_and_success_check_env EXIT
 
 ########################################################################################################################
 
-# This wrapper function is required to avoid `@/exe/bootstrap_dev_env.bash` exiting this script
+# This wrapper function is required to avoid `@/exe/bootstrap_env.bash` exiting this script
 # (otherwise this script will miss the chance to provide detailed error description).
 # The problem is that `return` command executed within boostrap are actually executed here -
 # when wrapped into a func, `return` within bootstrap will exist just that func:
 function activate_venv {
     # Bootstrap should be run from `argrelay_dir`:
     cd "${argrelay_dir}"
     # Run bootstrap to activate venv only:
     set +e
-    source "${argrelay_dir}/exe/bootstrap_dev_env.bash" activate_venv_only_flag
+    source "${argrelay_dir}/exe/bootstrap_env.bash" activate_venv_only_flag
     exit_code="${?}"
     # Restore trap (overridden by bootstrap):
     trap color_failure_and_success_check_env EXIT
     set -e
     return "${exit_code}"
 }
 
 ########################################################################################################################
 # Report `script_dir`:
 echo -e "${success_color}INFO:${reset_color} ${field_color}script_dir:${reset_color} ${script_dir}"
 
 ########################################################################################################################
-# Report `argrelay_dir` by verifying that `argrelay_dir` contains `@/exe/bootstrap_dev_env.bash`:
-if [[ ! -f "${argrelay_dir}/exe/bootstrap_dev_env.bash" ]]
+# Report `argrelay_dir` by verifying that `argrelay_dir` contains `@/exe/bootstrap_env.bash`:
+if [[ ! -f "${argrelay_dir}/exe/bootstrap_env.bash" ]]
 then
-    echo -e "${failure_color}ERROR:${reset_color} \`argrelay_dir\` must have \`@/exe/bootstrap_dev_env.bash\` script, but it is missing: ${argrelay_dir}/exe/bootstrap_dev_env.bash"
+    echo -e "${failure_color}ERROR:${reset_color} \`argrelay_dir\` must have \`@/exe/bootstrap_env.bash\` script, but it is missing: ${argrelay_dir}/exe/bootstrap_env.bash"
     exit 1
 fi
 echo -e "${success_color}INFO:${reset_color} ${field_color}argrelay_dir:${reset_color} ${argrelay_dir}"
 
 ########################################################################################################################
 # Report `@/conf/` target:
 if [[ -L "${argrelay_dir}/conf" ]]
@@ -113,15 +113,15 @@
 fi
 echo -e "${success_color}INFO:${reset_color} ${field_color}@/conf:${reset_color} ${conf_target}"
 
 ########################################################################################################################
 # Report `venv_path`:
 if ! activate_venv
 then
-    echo -e "${failure_color}ERROR:${reset_color} \`venv\` activation via \`@/exe/bootstrap_dev_env.bash\` script failed - re-run bootstrap manually and inspect the reason why it fails via its extensive debug output: ${argrelay_dir}/exe/bootstrap_dev_env.bash"
+    echo -e "${failure_color}ERROR:${reset_color} \`venv\` activation via \`@/exe/bootstrap_env.bash\` script failed - re-run bootstrap manually and inspect the reason why it fails via its extensive debug output: ${argrelay_dir}/exe/bootstrap_env.bash"
     exit 1
 fi
 echo -e "${success_color}INFO:${reset_color} ${field_color}venv_path:${reset_color} ${VIRTUAL_ENV}"
 
 ########################################################################################################################
 # Report `python_version`:
 # shellcheck disable=SC2154 # `path_to_pythonX` is assigned by bootstrap:
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/dev_shell.bash` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/dev_shell.bash`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     # Any output on stdout on shell init creates problems for many other commands (e.g. `ssh`).
     if [[ -n "$( bash -l -i -c "true" 2> /dev/null )" ]]
     then
         echo "ERROR: shell init generates stdout - redirect that output to stderr instead" 1>&2
         exit 1
     fi
 
-    # See `@/exe/bootstrap_dev_env.bash` regarding `history`:
+    # See `@/exe/bootstrap_env.bash` regarding `history`:
     # shellcheck disable=SC2034
     # shellcheck disable=SC2155
     export ARGRELAY_USER_SHELL_OPTS="$( unset ARGRELAY_DEBUG ; bash -l -i -c " set +o | grep -v \"[[:space:]]history$\" " 2> /dev/null )"
 fi
 
 # Define with `s` in value to debug:
 if [[ "${ARGRELAY_DEBUG-}" == *s* ]]
@@ -28,15 +28,15 @@
     set -v
 fi
 
 if [[ -n "${dev_shell_old_opts+x}" ]] ; then exit 1 ; fi
 
 # Save `set`-able options to restore them at the end of this source-able script:
 # https://unix.stackexchange.com/a/383581/23886
-# See `@/exe/bootstrap_dev_env.bash` regarding `history`:
+# See `@/exe/bootstrap_env.bash` regarding `history`:
 dev_shell_old_opts="$( set +o | grep -v "[[:space:]]history$" )"
 case "${-}" in
     *e*) dev_shell_old_opts="${dev_shell_old_opts}; set -e" ;;
       *) dev_shell_old_opts="${dev_shell_old_opts}; set +e" ;;
 esac
 
 # Debug: Print commands before execution:
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/init_shell_env.bash` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/init_shell_env.bash`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env bash
 # `argrelay` integration file: https://github.com/argrelay/argrelay
 
 # This script is NOT supposed to be run or sourced directly.
 # Instead, run `@/exe/dev_shell.bash`.
 
 # The steps this script implements FS_58_61_77_69 dev_shell:
-# *   Runs `@/exe/bootstrap_dev_env.bash` to activate Python `venv`.
+# *   Runs `@/exe/bootstrap_env.bash` to activate Python `venv`.
 # *   Runs `@/exe/shell_env.bash` to configure auto-completion for this shell session.
 
 # Note that enabling exit on error (like `set -e` below) will exit parent
 # `@/exe/dev_shell.bash` script (as this one is sourced) - that is intentional.
 
 # Define with `s` in value to debug:
 if [[ "${ARGRELAY_DEBUG-}" == *s* ]]
@@ -18,15 +18,15 @@
     set -v
 fi
 
 if [[ -n "${init_shell_env_old_opts+x}" ]] ; then exit 1 ; fi
 
 # Save `set`-able options to restore them at the end of this source-able script:
 # https://unix.stackexchange.com/a/383581/23886
-# See `@/exe/bootstrap_dev_env.bash` regarding `history`:
+# See `@/exe/bootstrap_env.bash` regarding `history`:
 init_shell_env_old_opts="$( set +o | grep -v "[[:space:]]history$" )"
 case "${-}" in
     *e*) init_shell_env_old_opts="${init_shell_env_old_opts}; set -e" ;;
       *) init_shell_env_old_opts="${init_shell_env_old_opts}; set +e" ;;
 esac
 
 # Debug: Print commands before execution:
@@ -50,17 +50,17 @@
 # The dir of this script:
 script_dir="$( cd -- "$( dirname -- "${script_source}" )" &> /dev/null && pwd )"
 # FS_29_54_67_86 dir_structure: `@/exe/` -> `@/`:
 argrelay_dir="$( dirname "${script_dir}" )"
 
 # It is expected that `@/exe/dev_shell.bash` switches to the target project dir itself (not this script).
 
-# FS_85_33_46_53: a copy of script `@/exe/bootstrap_dev_env.bash` has to be stored within the project
+# FS_85_33_46_53: a copy of script `@/exe/bootstrap_env.bash` has to be stored within the project
 # as the creator of everything:
-source "${argrelay_dir}/exe/bootstrap_dev_env.bash" activate_venv_only_flag
+source "${argrelay_dir}/exe/bootstrap_env.bash" activate_venv_only_flag
 
 # Collect info about `@/conf/`:
 if [[ -L "${argrelay_dir}/conf" ]]
 then
     conf_status="$( readlink -- "${argrelay_dir}/conf" )"
     if [[ ! -d "${argrelay_dir}/conf" ]]
     then
@@ -70,17 +70,17 @@
 then
     conf_status="[dir]"
 else
     conf_status="[error]"
 fi
 
 # Source extra config:
-if [[ -f "${argrelay_dir}/conf/dev_shell_rc.conf.bash" ]]
+if [[ -f "${argrelay_dir}/conf/dev_shell_env.bash" ]]
 then
-    source "${argrelay_dir}/conf/dev_shell_rc.conf.bash"
+    source "${argrelay_dir}/conf/dev_shell_env.bash"
 fi
 
 # Enable auto-completion:
 source "${argrelay_dir}/exe/shell_env.bash"
 
 # TODO: FS_16_07_78_84: respect conf dir priority:
 server_host_name="$( jq --raw-output ".connection_config.server_host_name" "${argrelay_dir}/conf/argrelay_client.json" )"
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/shell_env.bash` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/shell_env.bash`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # The main purposes of this script:
 # *   enable auto-completion for the commands configured via `argrelay_bind_command_basenames`
 # *   add the commands to PATH
 
 # Normally, this script is a symlink to orig artifact from `argrelay` distrib package.
 # The path where this symlink (or copy) is located is supposed to contain:
-# *   `@/exe/run_argrelay_client` artifact (generated by `@/exe/bootstrap_dev_env.bash`)
+# *   `@/exe/run_argrelay_client` artifact (generated by `@/exe/bootstrap_env.bash`)
 # *   `@/conf/shell_env.conf.bash` defining `argrelay_bind_command_basenames` env var
-# The symlinks for all command names are created by `@/exe/bootstrap_dev_env.bash` and
+# The symlinks for all command names are created by `@/exe/bootstrap_env.bash` and
 # point to `@/exe/run_argrelay_client`.
 
 # Note that enabling exit on error (like `set -e` below) will exit parent Bash shell (as this one is sourced).
 # Use these options with care as it prevents starting any shell in case of errors.
 
 # Define with `s` in value to debug:
 if [[ "${ARGRELAY_DEBUG-}" == *s* ]]
@@ -26,15 +26,15 @@
     set -v
 fi
 
 if [[ -n "${argrelay_rc_old_opts+x}" ]] ; then exit 1 ; fi
 
 # Save `set`-able options to restore them at the end of this source-able script:
 # https://unix.stackexchange.com/a/383581/23886
-# See `@/exe/bootstrap_dev_env.bash` regarding `history`:
+# See `@/exe/bootstrap_env.bash` regarding `history`:
 argrelay_rc_old_opts="$( set +o | grep -v "[[:space:]]history$" )"
 case "${-}" in
     *e*) argrelay_rc_old_opts="${argrelay_rc_old_opts}; set -e" ;;
       *) argrelay_rc_old_opts="${argrelay_rc_old_opts}; set +e" ;;
 esac
 
 # Debug: Print commands before execution:
@@ -57,15 +57,15 @@
 argrelay_rc_script_source="${BASH_SOURCE[0]}"
 # It is expected that `@/exe/shell_env.bash` is sourced from the project dir.
 # The dir of this script:
 argrelay_rc_script_dir="$( cd -- "$( dirname -- "${argrelay_rc_script_source}" )" &> /dev/null && pwd )"
 # FS_29_54_67_86 dir_structure: `@/exe/` -> `@/`:
 argrelay_rc_argrelay_dir="$( dirname "${argrelay_rc_script_dir}" )"
 
-# Test files generated by `@/exe/bootstrap_dev_env.bash` script:
+# Test files generated by `@/exe/bootstrap_env.bash` script:
 test -f "${argrelay_rc_argrelay_dir}/exe/run_argrelay_server" || return 1
 test -f "${argrelay_rc_argrelay_dir}/exe/run_argrelay_client" || return 1
 test -f "${argrelay_rc_argrelay_dir}/conf/shell_env.conf.bash" || return 1
 
 # Load user config for env vars:
 # *   argrelay_bind_command_basenames
 source "${argrelay_rc_argrelay_dir}/conf/shell_env.conf.bash"
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/custom_integ_res/upgrade_all_packages.bash` & `argrelay-0.7.2.dev0/src/argrelay/custom_integ_res/upgrade_env_packages.bash`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env bash
 
 # This script upgrades all Python packages in `venv`.
 #
 # If Python has to be upgraded as well based on the latest version in `@/conf/python_env.conf.bash`,
-# remove the `venv` first and re-run `@/exe/bootstrap_dev_env.bash`.
+# remove the `venv` first and re-run `@/exe/bootstrap_env.bash`.
 #
 # The basic steps are:
-# *   remove all package version records in `@/conf/dev_env_packages.txt`
-# *   optionally, set user-specified `argrelay` version in `@/conf/dev_env_packages.txt`
+# *   remove all package version records in `@/conf/env_packages.txt`
+# *   optionally, set user-specified `argrelay` version in `@/conf/env_packages.txt`
 # *   uninstall everything from `venv`
-# *   let `@/exe/bootstrap_dev_env.bash` re-install all (transitive) dependencies at their latest versions
+# *   let `@/exe/bootstrap_env.bash` re-install all (transitive) dependencies at their latest versions
 
 # Define with `s` in value to debug:
 if [[ "${ARGRELAY_DEBUG-}" == *s* ]]
 then
     set -x
     set -v
 fi
@@ -47,34 +47,34 @@
 fi
 
 # TODO_64_79_28_85: deduplicate this file with publish_package.bash (move upgrade function here from there).
 
 # Switch to `@/` to avoid creating temporary dirs somewhere else:
 cd "${argrelay_dir}" || exit 1
 
-# Run `@/exe/bootstrap_dev_env.bash` if this file does not exits:
+# Run `@/exe/bootstrap_env.bash` if this file does not exits:
 source "${argrelay_dir}/exe/argrelay_common_lib.bash"
 ensure_inside_dev_shell
 
 # Clear all package versions:
-true > "conf/dev_env_packages.txt"
+true > "conf/env_packages.txt"
 
 if [[ -n "${exact_argrelay_version+x}" ]]
 then
     # Set `argrelay` to the specified exact version:
-    echo "argrelay==${exact_argrelay_version}" > "conf/dev_env_packages.txt"
+    echo "argrelay==${exact_argrelay_version}" > "conf/env_packages.txt"
 elif [[ "$( pip show argrelay | grep '^Version:' | cut -f2 -d' ' || true )" == *dev* ]]
 then
     # Do not allow upgrades without specifying `exact_argrelay_version` if current version is a pre-release one:
     echo "ERROR: package \`argrelay\` has pre-release version - specify its next version manually" 1>&2
     exit 1
 fi
 
 # TODO: The step below also uninstalls `argrelay` (which provides this script) -
 #       subsequently, if bootstrap fails to install `argrelay` again,
 #       this script will be missing to re-try upgrade and user will have to `pip install argrelay` manually.
 # Clear `venv` (only to be restored in the next step):
 pip uninstall -y -r <( pip freeze )
 
-# Bootstrap to let `@/exe/deploy_project.bash` install all packages
+# Bootstrap to let `@/exe/install_project.bash` install all packages
 # via transitive dependencies and at their latest versions:
-"${argrelay_dir}/exe/bootstrap_dev_env.bash"
+"${argrelay_dir}/exe/bootstrap_env.bash"
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/ArgSource.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/ArgSource.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/CallConv.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/CallConv.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/CompScope.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/CompScope.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/CompType.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/CompType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/DistinctValuesQuery.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/DistinctValuesQuery.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/ReservedArgType.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/ReservedArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/RunMode.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/RunMode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/TermColor.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/TermColor.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/enum_desc/TokenType.py` & `argrelay-0.7.2.dev0/src/argrelay/enum_desc/TokenType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/handler_request/AbstractServerRequestHandler.py` & `argrelay-0.7.2.dev0/src/argrelay/handler_request/AbstractServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py` & `argrelay-0.7.2.dev0/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py` & `argrelay-0.7.2.dev0/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py` & `argrelay-0.7.2.dev0/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 .envelope_containers[function_container_ipos_]
                 .data_envelopes[0][instance_data_][delegator_plugin_instance_id_]
             )
         else:
             is_error = True
             error_message = "ERROR: Function is not selected, try help, or press Tab to complete selection."
             error_code = 1
-            # TODO: Do not hardcode plugin id (instance of `ErrorDelegator`):
+            # TODO: TODO_62_75_33_41: Do not hardcode plugin instance id (instance of `ErrorDelegator`):
             delegator_plugin_instance_id = f"{ErrorDelegator.__name__}.default"
 
         delegator_plugin: AbstractDelegator = self.local_server.server_config.action_delegators[
             delegator_plugin_instance_id
         ]
         invocation_input: InvocationInput = delegator_plugin.run_invoke_control(
             self.interp_ctx,
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py` & `argrelay-0.7.2.dev0/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py` & `argrelay-0.7.2.dev0/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py` & `argrelay-0.7.2.dev0/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/ElapsedTime.py` & `argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/ObjectSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/ObjectSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/TypeDesc.py` & `argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/TypeDesc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 def construct_include(
     yaml_loader: SafeLoader,
     yaml_node: yaml.Node,
 ) -> Any:
     """
     Method which allows `!include`-ing files in YAML.
 
+    Implements FS_70_55_40_99 splitting config files.
+
     See:
     https://stackoverflow.com/a/9577670/441652
     """
 
     file_name = os.path.abspath(os.path.join(
         # All paths should be relative to `@/` = `argrelay_dir`:
         get_argrelay_dir(),
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/misc_helper_common/__init__.py` & `argrelay-0.7.2.dev0/src/argrelay/misc_helper_common/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/misc_helper_server/__init__.py` & `argrelay-0.7.2.dev0/src/argrelay/misc_helper_server/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoClientWrapper.py` & `argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoClientWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoConfig.py` & `argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/mongo_data/MongoServerWrapper.py` & `argrelay-0.7.2.dev0/src/argrelay/mongo_data/MongoServerWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_config/AbstractConfigurator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_config/AbstractConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_config/DefaultConfigurator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_config/DefaultConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_config/DefaultConfiguratorConfig.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/AbstractDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/AbstractDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/AbstractJumpDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/AbstractJumpDelegator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 from typing import Union
 
-from argrelay.composite_tree.CompositeForestSchema import composite_forest_desc
 from argrelay.composite_tree.CompositeInfoType import CompositeInfoType
 from argrelay.composite_tree.CompositeTreeWalker import extract_tree_abs_path_to_interp_id
 from argrelay.composite_tree.DictTreeWalker import DictTreeWalker
 from argrelay.misc_helper_common import eprint
 from argrelay.plugin_delegator.AbstractDelegator import AbstractDelegator
 from argrelay.plugin_delegator.AbstractJumpDelegatorConfigSchema import (
     tree_abs_path_to_interp_id_,
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 
 single_func_id_ = "single_func_id"
 # TODO_10_72_28_05: This should be removed with FS_33_76_82_84 composite tree:
 tree_abs_path_to_interp_id_ = "tree_abs_path_to_interp_id"
 
+
 # TODO_40_10_18_32: add custom base to all schemas:
 class AbstractJumpDelegatorConfigSchema(Schema):
     class Meta:
         unknown = RAISE
         strict = True
 
     single_func_id = fields.String(
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/EchoDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/EchoDelegator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
         invocation_input = InvocationInput.with_interp_context(
             interp_ctx,
-            delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+            delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
                 self.plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
 
     @staticmethod
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/ErrorDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/ErrorDelegator.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class ErrorDelegator(AbstractDelegator):
 
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
-        delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+        delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
             self.plugin_instance_id
         ]
         invocation_input = InvocationInput.with_interp_context(
             interp_ctx,
             delegator_plugin_entry = delegator_plugin_entry,
             custom_plugin_data = {},
         )
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/HelpDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/HelpDelegator.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
             delegator_plugin_instance_id = self.plugin_instance_id
 
             custom_plugin_data = search_control_desc.dict_schema.dump(subsequent_function_container.search_control)
 
             invocation_input = InvocationInput.with_interp_context(
                 interp_ctx,
-                delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+                delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
                     delegator_plugin_instance_id
                 ],
                 custom_plugin_data = custom_plugin_data,
             )
             return invocation_input
         else:
             return redirect_to_no_func_error(
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/InterceptDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/InterceptDelegator.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         assert interp_ctx.is_func_found(), "the (first) function envelope must be found"
 
         # TODO: Fail (send to ErrorDelegator) if next function is not specified -
         #       showing the payload in this case is misleading.
         delegator_plugin_instance_id = self.plugin_instance_id
         invocation_input = InvocationInput.with_interp_context(
             interp_ctx,
-            delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+            delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
                 delegator_plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
 
     @staticmethod
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/NoopDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/NoopDelegator.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
         invocation_input = InvocationInput.with_interp_context(
             interp_ctx,
-            delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
+            delegator_plugin_entry = local_server.plugin_config.plugin_instance_entries[
                 self.plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
 
     @staticmethod
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_delegator/QueryEnumDelegator.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_delegator/QueryEnumDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/AbstractInterp.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/AbstractInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/AbstractInterpFactory.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/AbstractInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FirstArgInterp.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FirstArgInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FirstArgInterpFactory.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FirstArgInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FuncTreeInterp.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FuncTreeInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FuncTreeInterpFactory.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/InterpTreeInterp.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/InterpTreeInterp.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         self,
         curr_sub_tree,
     ):
         # Impossible to consume more arg - use default of the current sub-tree:
         if surrogate_node_id_ in curr_sub_tree:
             self.next_interp_factory_id = curr_sub_tree[surrogate_node_id_]
         else:
-            # TODO: Do not hardcode plugin id (instance of `NoopInterpFactory`):
+            # TODO: TODO_62_75_33_41: Do not hardcode plugin instance id (instance of `NoopInterpFactory`):
             self.next_interp_factory_id = f"{NoopInterpFactory.__name__}.default"
 
     def try_iterate(self) -> InterpStep:
         return InterpStep.NextInterp
 
     def next_interp(self) -> "AbstractInterp":
         # Selected `next_interp_factory_id` need to be given one of the paths in the FS_01_89_09_24 interp tree
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/InterpTreeInterpFactory.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from marshmallow import Schema, RAISE, fields, validates_schema, ValidationError
 
+from argrelay.composite_tree.DictTreeWalker import surrogate_node_id_
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.plugin_interp.FuncTreeInterpFactory import FuncTreeInterpFactory
-from argrelay.composite_tree.DictTreeWalker import surrogate_node_id_
 
 interp_selector_tree_ = "interp_selector_tree"
 
 ignored_func_ids_list_ = "ignored_func_ids_list"
 
 
 def validate_tree_node(interp_selector_sub_tree: dict):
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/plugin_interp/NoopInterpFactory.py` & `argrelay-0.7.2.dev0/src/argrelay/plugin_interp/NoopInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_client/AbstractClient.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_client/AbstractClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_client/RemoteClient.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_client/RemoteClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_client/RemoteClientCommandFactory.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_client/RemoteClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_client/__main__.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_client/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     command_obj = worker_main(
         call_ctx,
         client_config,
         shell_ctx,
     )
     return command_obj
 
+
 def load_client_config(file_path):
     import json
     with open(file_path) as config_file:
         client_config_dict = json.load(config_file)
     client_config = client_config_dict_to_object(client_config_dict)
     return client_config
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_client/proc_spinner.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_client/proc_spinner.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 def is_child_running(
     child_pid: int,
 ):
     (
         child_pid,
         child_status,
     ) = os.waitpid(child_pid, os.WNOHANG)
+    # NOTE: `os.waitpid` and `is_child_exited` are not atomic - do we need to keep `assert` below?
     if child_pid == 0 and child_status == 0:
         assert not is_child_exited()
         return True
     else:
         assert is_child_exited()
         return False
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_client/proc_split.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_client/proc_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 import signal
 import sys
 import typing
 from typing import Union
 
 _child_exited: bool = False
 
+
 def _signal_handler(signal_number, signal_frame):
     if signal_number == signal.SIGCHLD:
         global _child_exited
         _child_exited = True
 
+
 def is_child_exited() -> bool:
     global _child_exited
     return _child_exited
 
+
 def split_process() -> (
     bool,
     int,
     Union[None, typing.TextIO],
 ):
     """
     Part of FS_14_59_14_06 pending requests implementation.
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_client/proc_worker.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_client/proc_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 from argrelay.enum_desc.ServerAction import ServerAction
 from argrelay.misc_helper_common import eprint
 from argrelay.misc_helper_common.ElapsedTime import ElapsedTime
 
 has_error_happened = False
 
+
 def _signal_handler(signal_number, signal_frame):
     if signal_number == signal.SIGALRM:
         # Import hanged:
         eprint("ERROR: `import` hanged - see: https://github.com/argrelay/argrelay/issues/89")
         global has_error_happened
         has_error_happened = True
 
+
 def worker_main(
     call_ctx,
     client_config,
     shell_ctx
 ) -> "AbstractClientCommand":
     if client_config.use_local_requests:
         # This branch with `use_local_requests` is used only for testing
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/CustomFlaskApp.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/CustomFlaskApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from argrelay.custom_integ.git_utils import get_git_repo_root_path
 from argrelay.misc_helper_common import get_argrelay_dir
 from argrelay.plugin_config.AbstractConfigurator import AbstractConfigurator
 from argrelay.relay_server.LocalServer import LocalServer
 from argrelay.relay_server.route_api import create_blueprint_api
 from argrelay.relay_server.route_gui import create_blueprint_gui
 from argrelay.schema_config_core_server.ServerConfigSchema import server_config_desc
+from argrelay.schema_config_plugin.PluginConfigSchema import plugin_config_desc
 from argrelay.server_spec.const_int import API_SPEC_PATH, API_DOCS_PATH, ARGRELAY_GUI_PATH
 
 # Set this here (because `require` function may fail in other contexts):
 server_version = pkg_resources.require("argrelay")[0].version
 server_title = relay_server.__name__
 
 
@@ -35,15 +36,18 @@
     ):
         super().__init__(
             import_name = import_name,
             static_folder = static_folder,
             template_folder = template_folder,
             static_url_path = static_url_path,
         )
-        self.local_server: LocalServer = LocalServer(server_config_desc.obj_from_default_file())
+        self.local_server: LocalServer = LocalServer(
+            server_config_desc.obj_from_default_file(),
+            plugin_config_desc.obj_from_default_file(),
+        )
 
     def run_with_config(self):
         # Use custom logging at DEBUG level - see: `log_request` and `log_response:
         self.logger.setLevel(logging.DEBUG)
         # Log only at ERROR level by default logger:
         # https://stackoverflow.com/a/18379764/441652
         logging.getLogger("werkzeug").setLevel(logging.ERROR)
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/HelpHintCache.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/HelpHintCache.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/LocalServer.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/LocalServer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import time
 import uuid
 from copy import deepcopy
 
 from pymongo import MongoClient
 
+from argrelay.composite_tree.DictTreeWalker import contains_whitespace
 from argrelay.enum_desc.PluginType import PluginType
 from argrelay.enum_desc.ReservedArgType import ReservedArgType
 from argrelay.misc_helper_common import eprint
 from argrelay.mongo_data import MongoClientWrapper
 from argrelay.mongo_data.MongoServerWrapper import MongoServerWrapper
 from argrelay.plugin_delegator.AbstractDelegator import AbstractDelegator
 from argrelay.plugin_interp.AbstractInterpFactory import AbstractInterpFactory
 from argrelay.plugin_loader.AbstractLoader import AbstractLoader
 from argrelay.relay_server.HelpHintCache import HelpHintCache
 from argrelay.relay_server.QueryEngine import QueryEngine
 from argrelay.runtime_context.AbstractPlugin import instantiate_plugin, AbstractPlugin
 from argrelay.runtime_data.EnvelopeCollection import EnvelopeCollection
+from argrelay.runtime_data.PluginConfig import PluginConfig
 from argrelay.runtime_data.PluginEntry import PluginEntry
 from argrelay.runtime_data.ServerConfig import ServerConfig
 from argrelay.schema_config_core_server.StaticDataSchema import static_data_desc
 
 
 class LocalServer:
     """
@@ -27,17 +29,19 @@
 
     The API-wrapper exposing `LocalServer` over the network is `CustomFlaskApp`.
     """
 
     def __init__(
         self,
         server_config: ServerConfig,
+        plugin_config: PluginConfig,
     ):
         self.server_instance_id = uuid.uuid4()
         self.server_config: ServerConfig = server_config
+        self.plugin_config: PluginConfig = plugin_config
         self.mongo_server: MongoServerWrapper = MongoServerWrapper()
         self.mongo_client: MongoClient = MongoClientWrapper.get_mongo_client(self.server_config.mongo_config)
         self.query_engine: QueryEngine = QueryEngine(
             self.server_config.query_cache_config,
             self.get_mongo_database(),
             self.server_config.mongo_config.distinct_values_query,
         )
@@ -65,16 +69,16 @@
         return self.query_engine
 
     def _activate_plugins(self):
         """
         Calls each plugin to update :class:`StaticData`.
         """
 
-        for plugin_instance_id in self.server_config.plugin_instance_id_activate_list:
-            plugin_entry: PluginEntry = self.server_config.plugin_instance_entries[plugin_instance_id]
+        for plugin_instance_id in self.plugin_config.plugin_instance_id_activate_list:
+            plugin_entry: PluginEntry = self.plugin_config.plugin_instance_entries[plugin_instance_id]
 
             if not plugin_entry.plugin_enabled:
                 continue
 
             plugin_instance: AbstractPlugin = instantiate_plugin(
                 self.server_config,
                 plugin_instance_id,
@@ -114,14 +118,15 @@
 
         eprint("validating data...")
         self._validate_static_data()
 
     def _validate_static_data(self):
         self._validate_static_data_schema()
         self._validata_static_data_by_plugins()
+        self._validate_data_envelope_string_prop_values()
 
     def _validate_static_data_schema(self):
         # Note that this is slow for large data sets:
         static_data_dict = static_data_desc.dict_schema.dump(self.server_config.static_data)
         static_data_desc.validate_dict(static_data_dict)
 
     def _validata_static_data_by_plugins(self):
@@ -129,14 +134,51 @@
         all_plugins.extend(self.server_config.data_loaders.values())
         all_plugins.extend(self.server_config.interp_factories.values())
         all_plugins.extend(self.server_config.action_delegators.values())
 
         for plugin_instance in all_plugins:
             plugin_instance.validate_loaded_data(self.server_config.static_data)
 
+    def _validate_data_envelope_string_prop_values(self):
+        """
+        This validation ensures there is no blank values (`None`, whitespace, etc.) in `index_field`-s.
+
+        See also FS_99_81_19_25 no space in options.
+        """
+        for envelope_collection in self.server_config.static_data.envelope_collections.values():
+            for index_field in envelope_collection.index_fields:
+                for data_envelope in envelope_collection.data_envelopes:
+                    if index_field not in data_envelope:
+                        # TODO: TODO_39_25_11_76: `data_envelope`-s with missing props:
+                        #       even if it may lead to confusion, it is allowed to happen.
+                        continue
+                    envelope_class = data_envelope[ReservedArgType.EnvelopeClass.name]
+                    prop_value_or_values = data_envelope[index_field]
+                    if isinstance(prop_value_or_values, list):
+                        for prop_value in prop_value_or_values:
+                            self._validate_string_prop_value(envelope_class, index_field, prop_value)
+                    else:
+                        prop_value = prop_value_or_values
+                        self._validate_string_prop_value(envelope_class, index_field, prop_value)
+
+    def _validate_string_prop_value(
+        self,
+        envelope_class,
+        index_field,
+        prop_value,
+    ):
+        if isinstance(prop_value, str):
+            if not prop_value and prop_value.strip():
+                raise ValueError(f"`{envelope_class}.{index_field}` [{prop_value}] has to be non-blank string")
+            if contains_whitespace(prop_value):
+                raise ValueError(f"`{envelope_class}.{index_field}` [{prop_value}] cannot contain whitespace")
+        else:
+            # FS_06_99_43_60: list arg value:
+            raise ValueError(f"`{envelope_class}.{index_field}` has to be a `list` of `str` or `str`")
+
     def _start_mongo_server(self):
         self.mongo_server.start_mongo_server(self.server_config.mongo_config)
 
     def _stop_mongo_server(self):
         self.mongo_server.stop_mongo_server()
 
     def _load_mongo_data(self):
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/QueryEngine.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/QueryEngine.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/QueryResult.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/QueryResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_static/argrelay_client.js` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_static/argrelay_client.js`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_static/argrelay_style.css` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_static/argrelay_style.css`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/gui_templates/argrelay_main.html` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/gui_templates/argrelay_main.html`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/route_api.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/route_api.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/relay_server/route_gui.py` & `argrelay-0.7.2.dev0/src/argrelay/relay_server/route_gui.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_context/AbstractPlugin.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_context/AbstractPlugin.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_context/EnvelopeContainer.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_context/EnvelopeContainer.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_context/InterpContext.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_context/InterpContext.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,23 +251,26 @@
             query_changed = False
 
             if self.curr_container:
                 # Set implicit values (so that applying defaults knows what they are):
                 self.curr_container.populate_implicit_arg_values()
 
             if self.curr_interp.has_fill_control():
-                if self.parsed_ctx.server_action is ServerAction.DescribeLineArgs:
-                    # TODO: FS_72_53_55_13: options before defaults
-                    # Describing args will need to show options except default - query values before defaults:
-                    ElapsedTime.measure(f"[i={interp_n}]: before_query_without_defaults: {self.curr_interp}")
-                    self.query_prop_values()
-                    # Reset to False as we just executed new query:
-                    query_changed = False
+                # FS_72_53_55_13: options before defaults
+                # Describing args will need to show options except default - query values before applying defaults:
+                ElapsedTime.measure(f"[i={interp_n}]: before_query_without_defaults: {self.curr_interp}")
+                # This step may be optimized away and is only needed to detect non-default options for
+                # `ServerAction.DescribeLineArgs` but we perform it for all requests to
+                # ensure they have common view in case of possible data issues
+                # (e.g. TODO_39_25_11_76: `data_envelope`-s with missing props).
+                self.query_prop_values()
+                # Reset to False as we just executed new query:
+                query_changed = False
 
-                    self._save_potentially_hidden_by_defaults()
+                self._save_potentially_hidden_by_defaults()
 
                 # Apply defaults (they may apply more than single value at a time):
                 query_changed = (
                     self.curr_interp.delegate_fill_control()
                     or
                     query_changed
                 )
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_context/ParsedContext.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_context/ParsedContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_context/SearchControl.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_context/SearchControl.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_data/EnvelopeCollection.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_data/EnvelopeCollection.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_data/ServerConfig.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_data/ServerConfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,41 +3,28 @@
 from dataclasses import dataclass, field
 
 from argrelay.enum_desc.PluginType import PluginType
 from argrelay.mongo_data.MongoConfig import MongoConfig
 from argrelay.relay_server.GuiBannerConfig import GuiBannerConfig
 from argrelay.relay_server.QueryCacheConfig import QueryCacheConfig
 from argrelay.runtime_data.ConnectionConfig import ConnectionConfig
-from argrelay.runtime_data.PluginEntry import PluginEntry
 from argrelay.runtime_data.ServerPluginControl import ServerPluginControl
 from argrelay.runtime_data.StaticData import StaticData
 from argrelay.schema_config_plugin.PluginEntrySchema import plugin_enabled_, plugin_dependencies_
 
 
 @dataclass
 class ServerConfig:
     connection_config: ConnectionConfig = field()
     mongo_config: MongoConfig = field()
     query_cache_config: QueryCacheConfig = field()
     gui_banner_config: GuiBannerConfig = field()
     class_to_collection_map: dict = field()
     server_plugin_control: ServerPluginControl = field()
 
-    plugin_instance_id_activate_list: list[str] = field()
-    """
-    List of `plugin_instance_id`-s in order of activation generated by
-    walking through a DAG described by `plugin_dependencies`.
-    Each `plugin_instance_id` is a key into `plugin_instance_entries`.
-    """
-
-    plugin_instance_entries: dict[str, PluginEntry] = field()
-    """
-    Key = `plugin_instance_id`
-    """
-
     # TODO_00_79_72_55: remove in the future:
     static_data: StaticData = field()
 
     # TODO: Keep this runtime objects in separate (`ServerRuntime`?) class. Ensure/implement ServerConfig dumping on request (for troubleshooting).
     data_loaders: dict[str, "AbstractLoader"] = field(default_factory = lambda: {})
     """
     Entries in `data_loaders` are not directly loaded from config.
@@ -54,17 +41,19 @@
     # TODO: Keep this runtime objects in separate (`ServerRuntime`?) class. Ensure/implement ServerConfig dumping on request (for troubleshooting).
     action_delegators: dict[str, "AbstractDelegator"] = field(default_factory = lambda: {})
     """
     Entries in `action_delegators` are not directly loaded from config.
     These are plugin instances created during plugin activation.
     """
 
+    # TODO: Keep this runtime objects in separate (`ServerRuntime`?) class. Ensure/implement ServerConfig dumping on request (for troubleshooting).
     server_configurators: dict[str, "AbstractConfigurator"] = field(default_factory = lambda: {})
 
 
+# TODO: move to PluginConfig:
 def assert_plugin_instance_id(
     server_config: ServerConfig,
     plugin_instance_id: str,
     plugin_type: PluginType,
 ):
     error_msg = f"plugin instance `{plugin_instance_id}` must: (A) be `{PluginType.DelegatorPlugin.name}`, (B) be `{plugin_enabled_}`, (C) be activated in the order of DAG via `{plugin_dependencies_}`"
     if plugin_type is PluginType.InterpFactoryPlugin:
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/runtime_data/StaticData.py` & `argrelay-0.7.2.dev0/src/argrelay/runtime_data/StaticData.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_client/ClientConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_client/ClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/MongoConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/MongoConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from marshmallow import Schema, fields, RAISE, post_load
+from marshmallow import fields, RAISE
 
 from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.mongo_data.MongoServerConfig import MongoServerConfig
 
 database_name_ = "database_name"
 start_server_ = "start_server"
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from marshmallow import Schema, fields, RAISE, post_load
+from marshmallow import fields, RAISE
 
 from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.relay_server.QueryCacheConfig import QueryCacheConfig
 
 enable_query_cache_ = "enable_query_cache"
 query_cache_ttl_sec_ = "query_cache_ttl_sec"
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_core_server/StaticDataSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_core_server/StaticDataSchema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from marshmallow import Schema, RAISE, fields, post_load
+from marshmallow import RAISE, fields
 
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
 from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_data.StaticData import StaticData
 from argrelay.schema_config_core_server.EnvelopeCollectionSchema import envelope_collection_desc
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/DataEnvelopeSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/DataEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/InitControlSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/InitControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_interp/SearchControlSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_interp/SearchControlSchema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from marshmallow import Schema, RAISE, fields, validates_schema, ValidationError, post_load
+from marshmallow import RAISE, fields, validates_schema, ValidationError
 
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
 from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_context.SearchControl import SearchControl
 
 collection_name_ = "collection_name"
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_config_plugin/PluginEntrySchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_config_plugin/PluginEntrySchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_request/CallContextSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_request/CallContextSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_response/ArgValuesSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_response/ArgValuesSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_response/AssignedValueSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_response/AssignedValueSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_response/EnvelopeContainerSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_response/EnvelopeContainerSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_response/InterpResult.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_response/InterpResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_response/InterpResultSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_response/InterpResultSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_response/InvocationInput.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_response/InvocationInput.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/schema_response/InvocationInputSchema.py` & `argrelay-0.7.2.dev0/src/argrelay/schema_response/InvocationInputSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/server_spec/CallContext.py` & `argrelay-0.7.2.dev0/src/argrelay/server_spec/CallContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/server_spec/DescribeLineArgsSpec.py` & `argrelay-0.7.2.dev0/src/argrelay/server_spec/DescribeLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/server_spec/ProposeArgValuesSpec.py` & `argrelay-0.7.2.dev0/src/argrelay/server_spec/ProposeArgValuesSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/server_spec/RelayLineArgsSpec.py` & `argrelay-0.7.2.dev0/src/argrelay/server_spec/RelayLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/server_spec/const_int.py` & `argrelay-0.7.2.dev0/src/argrelay/server_spec/const_int.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/server_spec/server_data_schema.py` & `argrelay-0.7.2.dev0/src/argrelay/server_spec/server_data_schema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/BaseTestClass.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/BaseTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/ClientServerTestClass.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/ClientServerTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/CustomTestCase.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/CustomTestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/CustomVerifier.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/CustomVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/End2EndTestClass.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/End2EndTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/EnvMockBuilder.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/EnvMockBuilder.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,17 +48,20 @@
     use_mongomock_,
     distinct_values_query_,
 )
 from argrelay.schema_config_core_server.QueryCacheConfigSchema import enable_query_cache_
 from argrelay.schema_config_core_server.ServerConfigSchema import (
     mongo_config_,
     server_config_desc,
-    plugin_instance_entries_,
     query_cache_config_,
 )
+from argrelay.schema_config_plugin.PluginConfigSchema import (
+    plugin_config_desc,
+    plugin_instance_entries_,
+)
 from argrelay.schema_config_plugin.PluginEntrySchema import plugin_config_, plugin_enabled_
 from argrelay.schema_response.InvocationInput import InvocationInput
 from argrelay.server_spec.CallContext import CallContext
 from argrelay.test_infra.LocalClientCommandFactory import LocalClientCommandFactory
 from argrelay.test_infra.OpenFileMock import OpenFileMock
 from argrelay.test_infra.PopenMock import PopenMock
 
@@ -74,16 +77,17 @@
 
         *   `_mock_client_input_in_completion_mode`
         *   `_mock_client_input_in_invocation_mode_with_args`
         *   `_mock_client_input_in_invocation_mode_with_line`
 
     *   Mock server and client config files - see usage of:
 
-        *   `set_server_config_dict`
         *   `set_client_config_dict`
+        *   `set_server_config_dict`
+        *   `set_plugin_config_dict`
 
     *   Capture `stdout` and `stderr` - see usage of:
 
         *   `set_capture_stdout`
         *   `set_capture_stderr`
 
     *   Whether client uses `LocalClient`/`LocalServer` or `RemoteClient` with `CustomFlaskApp` - see usage of:
@@ -156,21 +160,24 @@
     capture_stderr: bool = field(default = False)
 
     ####################################################################################################################
     # Config file mocking
 
     client_config_dict: Union[dict, None] = field(default_factory = lambda: None)
     server_config_dict: Union[dict, None] = field(default_factory = lambda: None)
+    plugin_config_dict: Union[dict, None] = field(default_factory = lambda: None)
 
     mock_client_config_file_read: bool = field(default = False)
     mock_server_config_file_read: bool = field(default = False)
+    mock_plugin_config_file_read: bool = field(default = False)
 
     # Implement FS_62_25_92_06 generated config for `out`-processes to read it (see FS_66_17_43_42 test infra):
     generate_client_config_file: bool = field(default = False)
     generate_server_config_file: bool = field(default = False)
+    generate_plugin_config_file: bool = field(default = False)
     temp_test_config_dir: Union[tempfile.TemporaryDirectory, None] = None
 
     ####################################################################################################################
     # General mocking
 
     file_mock: OpenFileMock = field(default_factory = lambda: OpenFileMock({}))
 
@@ -307,45 +314,83 @@
         client_config: Union[dict, None] = None,
     ):
         if client_config is None:
             client_config = client_config_desc.dict_from_default_file()
         self.client_config_dict = client_config
         return self
 
+    def clear_client_config_dict(
+        self,
+    ):
+        self.client_config_dict = None
+        return self
+
     def set_server_config_dict(
         self,
         server_config: Union[dict, None] = None,
     ):
         if server_config is None:
             server_config = server_config_desc.dict_from_default_file()
         self.server_config_dict = server_config
         return self
 
+    def clear_server_config_dict(
+        self,
+    ):
+        self.server_config_dict = None
+        return self
+
+    def set_plugin_config_dict(
+        self,
+        plugin_config: Union[dict, None] = None,
+    ):
+        if plugin_config is None:
+            plugin_config = plugin_config_desc.dict_from_default_file()
+        self.plugin_config_dict = plugin_config
+        return self
+
+    def clear_plugin_config_dict(
+        self,
+    ):
+        self.plugin_config_dict = None
+        return self
+
     def get_client_config_json(self):
         return json.dump(self.client_config_dict)
 
     def get_server_config_yaml(self):
         return yaml.dump(self.server_config_dict)
 
+    def get_plugin_config_yaml(self):
+        return yaml.dump(self.plugin_config_dict)
+
     def set_mock_client_config_file_read(self, given_val: bool):
         self.mock_client_config_file_read = given_val
         return self
 
     def set_mock_server_config_file_read(self, given_val: bool):
         self.mock_server_config_file_read = given_val
         return self
 
+    def set_mock_plugin_config_file_read(self, given_val: bool):
+        self.mock_plugin_config_file_read = given_val
+        return self
+
     def set_generate_client_config_file(self, given_val: bool):
         self.generate_client_config_file = given_val
         return self
 
     def set_generate_server_config_file(self, given_val: bool):
         self.generate_server_config_file = given_val
         return self
 
+    def set_generate_plugin_config_file(self, given_val: bool):
+        self.generate_plugin_config_file = given_val
+        return self
+
     ####################################################################################################################
     # General mocking
 
     @contextlib.contextmanager
     def mock_file_open(self):
         with mock.patch("builtins.open", self.file_mock.open) as file_mock:
             yield file_mock
@@ -425,27 +470,33 @@
 
         ################################################################################################################
         # Server config
 
         if self.server_config_dict is not None:
             self.assert_server_config_substitute_enabled()
 
-        if self.enable_demo_git_loader:
-            self.assert_server_config_substitute_enabled()
-
         if self.enable_query_cache is not None:
             self.assert_server_config_substitute_enabled()
 
         if self.distinct_values_query is not None:
             self.assert_server_config_substitute_enabled()
 
         if self.use_mongomock is not None:
             self.assert_server_config_substitute_enabled()
 
         ################################################################################################################
+        # Plugin config
+
+        if self.plugin_config_dict is not None:
+            self.assert_plugin_config_substitute_enabled()
+
+        if self.enable_demo_git_loader:
+            self.assert_plugin_config_substitute_enabled()
+
+        ################################################################################################################
 
         if self.mock_client_config_file_read or self.generate_client_config_file:
 
             assert self.client_config_dict is not None
 
             self.client_config_dict[use_local_requests_] = self.is_client_config_with_local_server
 
@@ -467,22 +518,14 @@
 
         if self.mock_server_config_file_read or self.generate_server_config_file:
             """
             Change server config data, then mock file access to return that data for tests.
             """
             assert self.server_config_dict is not None
 
-            # TODO: Do not hardcode plugin id (instance of `GitRepoLoader`):
-            plugin_entry = self.server_config_dict[plugin_instance_entries_][f"{GitRepoLoader.__name__}.default"]
-            plugin_entry[plugin_enabled_] = self.enable_demo_git_loader
-
-            # TODO: Do not hardcode plugin id (instance of `ServiceLoader`):
-            plugin_entry = self.server_config_dict[plugin_instance_entries_][f"{ServiceLoader.__name__}.default"]
-            plugin_entry[plugin_config_][test_data_ids_to_load_] = self.test_data_ids_to_load
-
             if self.enable_query_cache is not None:
                 self.server_config_dict[query_cache_config_][enable_query_cache_] = self.enable_query_cache
 
             if self.distinct_values_query is not None:
                 self.server_config_dict[mongo_config_][distinct_values_query_] = self.distinct_values_query.name
 
             if self.use_mongomock is not None:
@@ -490,14 +533,34 @@
 
             # set mocked file content:
             if self.mock_server_config_file_read:
                 self.file_mock.path_to_data[server_config_desc.get_adjusted_file_path()] = yaml.dump(
                     self.server_config_dict
                 )
 
+        if self.mock_plugin_config_file_read or self.generate_plugin_config_file:
+            """
+            Change server config data, then mock file access to return that data for tests.
+            """
+            assert self.plugin_config_dict is not None
+
+            # TODO: TODO_62_75_33_41: Do not hardcode plugin instance id (instance of `GitRepoLoader`):
+            plugin_entry = self.plugin_config_dict[plugin_instance_entries_][f"{GitRepoLoader.__name__}.default"]
+            plugin_entry[plugin_enabled_] = self.enable_demo_git_loader
+
+            # TODO: TODO_62_75_33_41: Do not hardcode plugin instance id (instance of `ServiceLoader`):
+            plugin_entry = self.plugin_config_dict[plugin_instance_entries_][f"{ServiceLoader.__name__}.default"]
+            plugin_entry[plugin_config_][test_data_ids_to_load_] = self.test_data_ids_to_load
+
+            # set mocked file content:
+            if self.mock_plugin_config_file_read:
+                self.file_mock.path_to_data[plugin_config_desc.get_adjusted_file_path()] = yaml.dump(
+                    self.plugin_config_dict
+                )
+
         with ExitStack() as exit_stack:
 
             # noinspection PyListCreation
             yield_list = []
 
             # Always mock file access - whether file data or mocked data is given depends on the mock config:
             yield_list.append(exit_stack.enter_context(self.mock_file_open()))
@@ -560,14 +623,16 @@
                     do_reset_local_server()
                 ))
 
             if (
                 self.generate_client_config_file
                 or
                 self.generate_server_config_file
+                or
+                self.generate_plugin_config_file
             ):
                 yield_list.append(exit_stack.enter_context(
                     self.generate_configs()
                 ))
 
             yield yield_list
 
@@ -580,14 +645,20 @@
             )
             and
             (
                 self.mock_server_config_file_read == self.generate_server_config_file == False
                 or
                 self.mock_server_config_file_read != self.generate_server_config_file
             )
+            and
+            (
+                self.mock_plugin_config_file_read == self.generate_plugin_config_file == False
+                or
+                self.mock_plugin_config_file_read != self.generate_plugin_config_file
+            )
         ), "FS_62_25_92_06: generated config: mocked config and generated config are mutually exclusive"
 
     def assert_client_config_substitute_enabled(self):
         assert (
             self.mock_client_config_file_read
             or
             self.generate_client_config_file
@@ -596,37 +667,57 @@
     def assert_server_config_substitute_enabled(self):
         assert (
             self.mock_server_config_file_read
             or
             self.generate_server_config_file
         ), "FS_62_25_92_06: generated config: when enabled: either mocked config or generated config"
 
+    def assert_plugin_config_substitute_enabled(self):
+        assert (
+            self.mock_plugin_config_file_read
+            or
+            self.generate_plugin_config_file
+        ), "FS_62_25_92_06: generated config: when enabled: either mocked config or generated config"
+
     @contextlib.contextmanager
     def assert_all_cm(self):
         try:
             yield
         finally:
             if self.mock_client_config_file_read:
                 self.assert_client_config_read()
             if self.mock_server_config_file_read and not self.was_server_started_on_build:
                 self.assert_server_config_read()
+            if self.mock_plugin_config_file_read and not self.was_server_started_on_build:
+                self.assert_plugin_config_read()
 
     def assert_client_config_read(self):
         self.assert_file_read(client_config_desc.get_adjusted_file_path())
 
     def assert_server_config_read(self):
         self.assert_file_read(server_config_desc.get_adjusted_file_path())
 
+    def assert_plugin_config_read(self):
+        self.assert_file_read(plugin_config_desc.get_adjusted_file_path())
+
     def assert_file_read(self, file_path: str):
         """
         Ensures that mocked file was actually accessed.
 
         If fails here, it means either/or:
-        *   test setup was over-mocked (e.g. see `mock_server_config_file_read`, `mock_client_config_file_read`)
+
+        *   test setup was over-mocked
+
+            see:
+            *   `mock_client_config_file_read`
+            *   `mock_server_config_file_read`
+            *   `mock_plugin_config_file_read`
+
         *   test did not hit functionality that is supposed to access the file
+
         """
         self.file_mock.path_to_mock[file_path].assert_called_with(file_path)
 
     @contextlib.contextmanager
     def generate_configs(
         self,
     ):
@@ -651,18 +742,24 @@
             self.temp_test_config_dir.name,
             client_config_desc.default_file_path,
         )
         server_config_path = os.path.join(
             self.temp_test_config_dir.name,
             server_config_desc.default_file_path,
         )
+        plugin_config_path = os.path.join(
+            self.temp_test_config_dir.name,
+            plugin_config_desc.default_file_path,
+        )
         if self.generate_client_config_file:
             self.generate_client_config(str(client_config_path))
         if self.generate_server_config_file:
             self.generate_server_config(str(server_config_path))
+        if self.generate_plugin_config_file:
+            self.generate_plugin_config(str(plugin_config_path))
 
     def generate_client_config(
         self,
         file_path: str,
     ):
         with open(file_path, "w") as json_file:
             json.dump(
@@ -676,14 +773,24 @@
     ):
         with open(file_path, "w") as yaml_file:
             yaml.dump(
                 self.server_config_dict,
                 yaml_file,
             )
 
+    def generate_plugin_config(
+        self,
+        file_path: str,
+    ):
+        with open(file_path, "w") as yaml_file:
+            yaml.dump(
+                self.plugin_config_dict,
+                yaml_file,
+            )
+
 
 ########################################################################################################################
 # Pre-configured mock builders
 
 @dataclass
 class EmptyEnvMockBuilder(EnvMockBuilder):
     """
@@ -697,14 +804,15 @@
     ):
         super().__init__()
         self.set_mock_client_input(False)
         self.set_reset_local_server(False)
         # Disable all mocks which set tripwires if not used:
         self.set_mock_client_config_file_read(False)
         self.set_mock_server_config_file_read(False)
+        self.set_mock_plugin_config_file_read(False)
         self.set_client_config_with_local_server(False)
         # Client config is not substituted but otherwise default `show_pending_spinner = False` requires it - use None:
         self.set_show_pending_spinner(None)
 
 
 @dataclass
 class LocalClientEnvMockBuilder(EnvMockBuilder):
@@ -722,20 +830,23 @@
         super().__init__()
 
         # TODO: enable validation that client code is actually invoked (e.g. invocation of make_request in proc_worker):
 
         # Ensure that client and server read their config files by test process:
         self.set_mock_client_config_file_read(True)
         self.set_mock_server_config_file_read(True)
+        self.set_mock_plugin_config_file_read(True)
         self.set_generate_client_config_file(False)
         self.set_generate_server_config_file(False)
+        self.set_generate_plugin_config_file(False)
 
         # Load default configs as file access mocks input:
         self.set_client_config_dict()
         self.set_server_config_dict()
+        self.set_plugin_config_dict()
 
         # For local client (with local server) tests,
         # ensure client uses `LocalClient` without marshalling data via HTTP:
         self.set_client_config_with_local_server(True)
         # Also, ensure non-optimized completion is used
         # (optimized directly uses network socket which will not give access to `LocalServer`):
         self.set_client_config_to_optimize_completion_request(False)
@@ -765,18 +876,21 @@
         # For server-only test, client config file read should not happen by test process
         # (if this mock is enabled, but not used, it fails):
         self.set_mock_client_config_file_read(False)
         self.set_generate_client_config_file(False)
 
         # For server-only test, use mocked server config file access (to control its content in test):
         self.set_mock_server_config_file_read(True)
+        self.set_mock_plugin_config_file_read(True)
         self.set_generate_server_config_file(False)
+        self.set_generate_plugin_config_file(False)
 
         # Load default server config as file access mock input:
         self.set_server_config_dict()
+        self.set_plugin_config_dict()
 
         # For server-only test, client code is not used, but if it is, try to fail via REST API:
         self.set_client_config_with_local_server(False)
 
         # For server-only test, client input mocking is not required:
         self.set_mock_client_input(False)
 
@@ -807,15 +921,17 @@
         self.set_generate_client_config_file(False)
         # Client config is not substituted but otherwise default `show_pending_spinner = False` requires it - use None:
         self.set_show_pending_spinner(None)
 
         # For live server test, server config file substitution should not happen by test process code
         # (because it happens within server process - un-verify-able from the test process):
         self.set_mock_server_config_file_read(False)
+        self.set_mock_plugin_config_file_read(False)
         self.set_generate_server_config_file(False)
+        self.set_generate_plugin_config_file(False)
 
         # For live server test, running local server contradicts with the live server - disable:
         self.set_client_config_with_local_server(False)
         # Optimized client prevents accessing internal server state via `LocalClient` and `LocalServer`,
         # but it is impossible with live server anyway.
         # Therefore, default is unspecified here = None
         # (whatever is set in the client config or dictated by its defaults):
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/InOutTestClass.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/InOutTestClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,22 @@
                         try:
                             if assigned_value is None:
                                 self.assertTrue(
                                     arg_type not in
                                     envelope_containers
                                     [container_ipos].assigned_types_to_values
                                 )
+                            elif isinstance(assigned_value, list):
+                                # A bit of hack: if `list`, then check if it matches `remaining_types_to_values`:
+                                self.assertTrue(
+                                    assigned_value,
+                                    envelope_containers
+                                    [container_ipos].remaining_types_to_values
+                                    [arg_type]
+                                )
                             else:
                                 self.assertEqual(
                                     assigned_value,
                                     envelope_containers
                                     [container_ipos].assigned_types_to_values
                                     [arg_type],
                                 )
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/JsonTestOutputVerifier.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/JsonTestOutputVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/LocalClient.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/LocalClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/LocalClientCommandFactory.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/LocalClientCommandFactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from argrelay.client_command_local.AbstractLocalClientCommand import AbstractLocalClientCommand
 from argrelay.enum_desc.ServerAction import ServerAction
 from argrelay.misc_helper_common.ElapsedTime import ElapsedTime
 from argrelay.relay_client.AbstractClientCommandFactory import AbstractClientCommandFactory
 from argrelay.relay_server.LocalServer import LocalServer
+from argrelay.runtime_data.PluginConfig import PluginConfig
 from argrelay.runtime_data.ServerConfig import ServerConfig
 from argrelay.schema_config_core_server.ServerConfigSchema import server_config_desc
+from argrelay.schema_config_plugin.PluginConfigSchema import plugin_config_desc
 from argrelay.server_spec.CallContext import CallContext
 
 
 class LocalClientCommandFactory(AbstractClientCommandFactory):
     local_server: LocalServer = None
     """
     This instance of `LocalServer` allows reusing server for multiple `LocalClient` invocation in tests.
@@ -17,16 +19,20 @@
 
     def __init__(self):
         self._start_local_server()
 
     def _start_local_server(self):
         if not LocalClientCommandFactory.local_server:
             self.server_config: ServerConfig = server_config_desc.obj_from_default_file()
+            self.plugin_config: PluginConfig = plugin_config_desc.obj_from_default_file()
             ElapsedTime.measure("after_server_config_load")
-            LocalClientCommandFactory.local_server = LocalServer(self.server_config)
+            LocalClientCommandFactory.local_server = LocalServer(
+                self.server_config,
+                self.plugin_config,
+            )
             LocalClientCommandFactory.local_server.start_local_server()
             ElapsedTime.measure("after_local_server_start")
         else:
             self.server_config: ServerConfig = LocalClientCommandFactory.local_server.server_config
 
     def create_command(
         self,
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/LocalTestClass.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/LocalTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/OpenFileMock.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/OpenFileMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/PopenMock.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/PopenMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/RemoteTestClass.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/RemoteTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/ServerOnlyTestClass.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/ServerOnlyTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/TestCase.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/TestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay/test_infra/__init__.py` & `argrelay-0.7.2.dev0/src/argrelay/test_infra/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.7.1.dev9/src/argrelay.egg-info/PKG-INFO` & `argrelay-0.7.2.dev0/src/argrelay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.7.1.dev9
+Version: 0.7.2.dev0
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.7.1.dev9/src/argrelay.egg-info/SOURCES.txt` & `argrelay-0.7.2.dev0/src/argrelay.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 pyproject.toml
 readme.md
 setup.py
 ./readme.md
 ./setup.py
 ./docs/readme.md
 ./docs/dev_notes/bootstrap_procedure.1.project_creation.md
-./docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
+./docs/dev_notes/bootstrap_procedure.2.initial_installation.md
 ./docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
 ./docs/dev_notes/brief_history.md
 ./docs/dev_notes/code_style.md
 ./docs/dev_notes/completion_notes.md
 ./docs/dev_notes/completion_perf_notes.md
 ./docs/dev_notes/gui_tests_notes.md
 ./docs/dev_notes/how_search_works.md
@@ -67,24 +67,26 @@
 ./docs/feature_stories/FS_58_61_77_69.dev_shell.md
 ./docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
 ./docs/feature_stories/FS_62_25_92_06.assigned_context.md
 ./docs/feature_stories/FS_63_63_14_08.generated_config.md
 ./docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
 ./docs/feature_stories/FS_66_17_43_42.test_infra.md
 ./docs/feature_stories/FS_67_16_61_97.git_plugin.md
+./docs/feature_stories/FS_70_55_40_99.splitting_config_files.md
 ./docs/feature_stories/FS_71_87_33_52.help_hint.md
 ./docs/feature_stories/FS_72_40_53_00.fill_control.md
 ./docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
 ./docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
 ./docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
 ./docs/feature_stories/FS_78_91_27_22.interp_control.md
 ./docs/feature_stories/FS_80_45_89_81.integrated_functions.md
 ./docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
 ./docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
-./docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+./docs/feature_stories/FS_83_23_99_90.client_plugin_config_override.md
+./docs/feature_stories/FS_85_33_46_53.bootstrap_env.md
 ./docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
 ./docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
 ./docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
 ./docs/feature_stories/FS_91_88_07_23.jump_tree.md
 ./docs/feature_stories/FS_92_75_93_01.clean_command_line.md
 ./docs/feature_stories/FS_94_30_49_28.help_doc.md
 ./docs/feature_stories/FS_97_64_39_94.arg_buckets.md
@@ -117,34 +119,36 @@
 ./docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
 ./docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
 ./docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
 ./docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
 ./docs/task_refs/TODO_30_69_19_14.infinite_spinner.md
 ./docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
 ./docs/task_refs/TODO_37_15_12_91.Popen_mock.md
+./docs/task_refs/TODO_39_25_11_76.data_envelopes_with_missing_props.md
 ./docs/task_refs/TODO_40_10_18_32.add_custom_base_to_all_schemas.md
 ./docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
 ./docs/task_refs/TODO_43_41_95_86.use_server_logger_to_disable_stdout.md
 ./docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
 ./docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
 ./docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
-./docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
+./docs/task_refs/TODO_62_75_33_41.do_not_hardcode_plugin_instance_id.md
+./docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_env_packages_before_test.md
 ./docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
 ./docs/task_refs/TODO_70_48_96_29.be_able_to_assert_remaining_arg_vals.md
 ./docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
 ./docs/task_refs/TODO_75_52_01_67.arg_buckets_to_support_multiple_var_args.md
 ./docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
 ./docs/task_refs/TODO_79_67_28_83.recursive_dict_schema.md
 ./docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
 ./docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
-./docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
 ./docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
 ./docs/task_refs/readme.md
 ./docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
 ./docs/test_data/TD_38_03_48_51.large_data_set.md
+./docs/test_data/TD_39_25_11_76.data_envelopes_with_missing_props.md
 ./docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
 ./docs/test_data/TD_63_37_05_36.demo_services_data.md
 ./docs/test_data/TD_70_69_38_46.no_data.md
 ./docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
 ./docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
 ./docs/test_data/readme.md
 ./src/argrelay/__init__.py
@@ -193,20 +197,20 @@
 ./src/argrelay/custom_integ/ServiceEnvelopeClass.py
 ./src/argrelay/custom_integ/ServiceLoader.py
 ./src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
 ./src/argrelay/custom_integ/__init__.py
 ./src/argrelay/custom_integ/git_utils.py
 ./src/argrelay/custom_integ/value_constants.py
 ./src/argrelay/custom_integ_res/argrelay_common_lib.bash
-./src/argrelay/custom_integ_res/bootstrap_dev_env.bash
+./src/argrelay/custom_integ_res/bootstrap_env.bash
 ./src/argrelay/custom_integ_res/check_env.bash
 ./src/argrelay/custom_integ_res/dev_shell.bash
 ./src/argrelay/custom_integ_res/init_shell_env.bash
 ./src/argrelay/custom_integ_res/shell_env.bash
-./src/argrelay/custom_integ_res/upgrade_all_packages.bash
+./src/argrelay/custom_integ_res/upgrade_env_packages.bash
 ./src/argrelay/enum_desc/ArgSource.py
 ./src/argrelay/enum_desc/CallConv.py
 ./src/argrelay/enum_desc/CompScope.py
 ./src/argrelay/enum_desc/CompType.py
 ./src/argrelay/enum_desc/DistinctValuesQuery.py
 ./src/argrelay/enum_desc/InterpStep.py
 ./src/argrelay/enum_desc/PluginType.py
@@ -269,14 +273,15 @@
 ./src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
 ./src/argrelay/plugin_interp/NoopInterp.py
 ./src/argrelay/plugin_interp/NoopInterpFactory.py
 ./src/argrelay/plugin_interp/__init__.py
 ./src/argrelay/plugin_loader/AbstractLoader.py
 ./src/argrelay/plugin_loader/NoopLoader.py
 ./src/argrelay/plugin_loader/__init__.py
+./src/argrelay/plugin_loader/client_utils.py
 ./src/argrelay/relay_client/AbstractClient.py
 ./src/argrelay/relay_client/AbstractClientCommand.py
 ./src/argrelay/relay_client/AbstractClientCommandFactory.py
 ./src/argrelay/relay_client/RemoteClient.py
 ./src/argrelay/relay_client/RemoteClientCommandFactory.py
 ./src/argrelay/relay_client/__init__.py
 ./src/argrelay/relay_client/__main__.py
@@ -307,20 +312,22 @@
 ./src/argrelay/runtime_context/SearchControl.py
 ./src/argrelay/runtime_context/__init__.py
 ./src/argrelay/runtime_context/arg_buckets_utils.py
 ./src/argrelay/runtime_data/AssignedValue.py
 ./src/argrelay/runtime_data/ClientConfig.py
 ./src/argrelay/runtime_data/ConnectionConfig.py
 ./src/argrelay/runtime_data/EnvelopeCollection.py
+./src/argrelay/runtime_data/PluginConfig.py
 ./src/argrelay/runtime_data/PluginEntry.py
 ./src/argrelay/runtime_data/ServerConfig.py
 ./src/argrelay/runtime_data/ServerPluginControl.py
 ./src/argrelay/runtime_data/StaticData.py
 ./src/argrelay/runtime_data/__init__.py
 ./src/argrelay/sample_conf/argrelay_client.json
+./src/argrelay/sample_conf/argrelay_plugin.yaml
 ./src/argrelay/sample_conf/argrelay_server.yaml
 ./src/argrelay/schema_config_core_client/ClientConfigSchema.py
 ./src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
 ./src/argrelay/schema_config_core_client/__init__.py
 ./src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
 ./src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
 ./src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
@@ -333,14 +340,15 @@
 ./src/argrelay/schema_config_core_server/__init__.py
 ./src/argrelay/schema_config_interp/DataEnvelopeSchema.py
 ./src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
 ./src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
 ./src/argrelay/schema_config_interp/InitControlSchema.py
 ./src/argrelay/schema_config_interp/SearchControlSchema.py
 ./src/argrelay/schema_config_interp/__init__.py
+./src/argrelay/schema_config_plugin/PluginConfigSchema.py
 ./src/argrelay/schema_config_plugin/PluginEntrySchema.py
 ./src/argrelay/schema_config_plugin/__init__.py
 ./src/argrelay/schema_request/CallContextSchema.py
 ./src/argrelay/schema_request/__init__.py
 ./src/argrelay/schema_response/ArgValues.py
 ./src/argrelay/schema_response/ArgValuesSchema.py
 ./src/argrelay/schema_response/AssignedValueSchema.py
@@ -405,15 +413,14 @@
 docs/feature_stories/FS_53_81_66_18.types_and_classes.md
 docs/feature_stories/FS_58_61_77_69.dev_shell.md
 docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
 docs/feature_stories/FS_62_25_92_06.assigned_context.md
 docs/feature_stories/FS_71_87_33_52.help_hint.md
 docs/feature_stories/FS_72_40_53_00.fill_control.md
 docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
-docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
 docs/feature_stories/FS_94_30_49_28.help_doc.md
 docs/feature_stories/readme.md
 docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
 docs/test_data/TD_38_03_48_51.large_data_set.md
 docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
 docs/test_data/TD_63_37_05_36.demo_services_data.md
 docs/test_data/TD_70_69_38_46.no_data.md
@@ -456,15 +463,14 @@
 src/argrelay/../../docs/feature_stories/FS_53_81_66_18.types_and_classes.md
 src/argrelay/../../docs/feature_stories/FS_58_61_77_69.dev_shell.md
 src/argrelay/../../docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
 src/argrelay/../../docs/feature_stories/FS_62_25_92_06.assigned_context.md
 src/argrelay/../../docs/feature_stories/FS_71_87_33_52.help_hint.md
 src/argrelay/../../docs/feature_stories/FS_72_40_53_00.fill_control.md
 src/argrelay/../../docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
-src/argrelay/../../docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
 src/argrelay/../../docs/feature_stories/FS_94_30_49_28.help_doc.md
 src/argrelay/../../docs/feature_stories/readme.md
 src/argrelay/../../docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
 src/argrelay/../../docs/test_data/TD_38_03_48_51.large_data_set.md
 src/argrelay/../../docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
 src/argrelay/../../docs/test_data/TD_63_37_05_36.demo_services_data.md
 src/argrelay/../../docs/test_data/TD_70_69_38_46.no_data.md
@@ -488,15 +494,14 @@
 src/argrelay/custom_integ/ServiceArgType.py
 src/argrelay/custom_integ/ServiceDelegator.py
 src/argrelay/custom_integ/ServiceEnvelopeClass.py
 src/argrelay/custom_integ/ServiceLoader.py
 src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
 src/argrelay/custom_integ/__init__.py
 src/argrelay/custom_integ/value_constants.py
-src/argrelay/custom_integ_res/bootstrap_dev_env.bash
 src/argrelay/custom_integ_res/dev_shell.bash
 src/argrelay/custom_integ_res/init_shell_env.bash
 src/argrelay/enum_desc/ArgSource.py
 src/argrelay/enum_desc/CompType.py
 src/argrelay/enum_desc/InterpStep.py
 src/argrelay/enum_desc/PluginType.py
 src/argrelay/enum_desc/ReservedArgType.py
```


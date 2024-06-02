# Comparing `tmp/robusta-cli-0.9.9.tar.gz` & `tmp/robusta_cli-1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robusta-cli-0.9.9.tar", max compression
+gzip compressed data, was "robusta_cli-1.0a0.tar", max compression
```

## Comparing `robusta-cli-0.9.9.tar` & `robusta_cli-1.0a0.tar`

### file list

```diff
@@ -1,174 +1,18 @@
--rw-r--r--   0        0        0     1072 2022-04-27 08:11:50.425188 robusta-cli-0.9.9/LICENSE
--rw-r--r--   0        0        0     2719 2022-04-27 08:12:06.645269 robusta-cli-0.9.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/__init__.py
--rw-r--r--   0        0        0       74 2022-04-27 08:12:06.645269 robusta-cli-0.9.9/src/robusta/_version.py
--rw-r--r--   0        0        0     1933 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/api/__init__.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/__init__.py
--rw-r--r--   0        0        0     4933 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/auth.py
--rw-r--r--   0        0        0     1189 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/backend_profile.py
--rw-r--r--   0        0        0     2045 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/integrations_cmd.py
--rwxr-xr-x   0        0        0    16946 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/main.py
--rw-r--r--   0        0        0    10995 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/playbooks_cmd.py
--rw-r--r--   0        0        0     3030 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/slack_feedback_message.py
--rw-r--r--   0        0        0     2838 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/slack_verification.py
--rw-r--r--   0        0        0     2831 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/utils.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/__init__.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/discovery/__init__.py
--rw-r--r--   0        0        0     2480 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/discovery/top_service_resolver.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/__init__.py
--rw-r--r--   0        0        0     4130 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/base_params.py
--rw-r--r--   0        0        0      172 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/cluster_status.py
--rw-r--r--   0        0        0     2750 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/env_vars.py
--rw-r--r--   0        0        0     3457 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/events.py
--rw-r--r--   0        0        0      120 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/k8s_operation_type.py
--rw-r--r--   0        0        0      939 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/nodes.py
--rw-r--r--   0        0        0     2549 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/pods.py
--rw-r--r--   0        0        0     1749 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/runner_config.py
--rw-r--r--   0        0        0      670 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/services.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/persistency/__init__.py
--rw-r--r--   0        0        0      585 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/persistency/in_memory.py
--rw-r--r--   0        0        0     2789 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/persistency/scheduled_jobs_states_dal.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/__init__.py
--rw-r--r--   0        0        0     3930 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/actions_registry.py
--rw-r--r--   0        0        0      806 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/base_trigger.py
--rw-r--r--   0        0        0     1831 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/common.py
--rw-r--r--   0        0        0     6526 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/generation.py
--rw-r--r--   0        0        0     2774 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/internal/discovery_events.py
--rw-r--r--   0        0        0     1179 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/playbook_utils.py
--rw-r--r--   0        0        0     1523 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/playbooks_event_handler.py
--rw-r--r--   0        0        0    11530 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/playbooks_event_handler_impl.py
--rw-r--r--   0        0        0     6698 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/prometheus_enrichment_utils.py
--rw-r--r--   0        0        0     1065 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/trigger.py
--rw-r--r--   0        0        0      236 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/__init__.py
--rw-r--r--   0        0        0     2070 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/action_requests.py
--rw-r--r--   0        0        0     4513 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/base.py
--rw-r--r--   0        0        0     9952 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/blocks.py
--rw-r--r--   0        0        0     1954 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/callbacks.py
--rw-r--r--   0        0        0     1250 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/consts.py
--rw-r--r--   0        0        0      457 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/custom_rendering.py
--rw-r--r--   0        0        0     1421 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/finding_subjects.py
--rw-r--r--   0        0        0     1109 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/utils.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/schedule/__init__.py
--rw-r--r--   0        0        0      932 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/schedule/model.py
--rw-r--r--   0        0        0     6113 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/schedule/scheduler.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/__init__.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/datadog/__init__.py
--rw-r--r--   0        0        0     4540 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/datadog/datadog_sink.py
--rw-r--r--   0        0        0      312 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/datadog/datadog_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/kafka/__init__.py
--rw-r--r--   0        0        0     2757 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/kafka/kafka_sink.py
--rw-r--r--   0        0        0      318 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/kafka/kafka_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/msteams/__init__.py
--rw-r--r--   0        0        0      626 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/msteams/msteams_sink.py
--rw-r--r--   0        0        0      318 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/msteams/msteams_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/opsgenie/__init__.py
--rw-r--r--   0        0        0     2558 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/opsgenie/opsgenie_sink.py
--rw-r--r--   0        0        0      393 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/opsgenie/opsgenie_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/__init__.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/dal/__init__.py
--rw-r--r--   0        0        0     5350 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/dal/model_conversion.py
--rw-r--r--   0        0        0    10151 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/dal/supabase_dal.py
--rw-r--r--   0        0        0    12836 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/robusta_sink.py
--rw-r--r--   0        0        0      468 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/robusta_sink_params.py
--rw-r--r--   0        0        0      894 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_base.py
--rw-r--r--   0        0        0      359 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_base_params.py
--rw-r--r--   0        0        0      320 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_config.py
--rw-r--r--   0        0        0     2094 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_factory.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/slack/__init__.py
--rw-r--r--   0        0        0      816 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/slack/slack_sink.py
--rw-r--r--   0        0        0      324 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/slack/slack_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/__init__.py
--rw-r--r--   0        0        0     1685 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_client.py
--rw-r--r--   0        0        0     3473 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_sink.py
--rw-r--r--   0        0        0      409 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_sink_params.py
--rw-r--r--   0        0        0     5260 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/transformer.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/webhook/__init__.py
--rw-r--r--   0        0        0     2708 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/webhook/webhook_sink.py
--rw-r--r--   0        0        0      335 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/webhook/webhook_sink_params.py
--rw-r--r--   0        0        0      564 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/triggers/custom_triggers.py
--rw-r--r--   0        0        0     3718 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/triggers/error_event_trigger.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/__init__.py
--rw-r--r--   0        0        0      859 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/argocd/argocd_client.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/git/__init__.py
--rw-r--r--   0        0        0     9793 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/git/git_repo.py
--rw-r--r--   0        0        0     3648 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/grafana.py
--rw-r--r--   0        0        0      394 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/helper.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/__init__.py
--rw-r--r--   0        0        0     8041 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/api_client_utils.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/__init__.py
--rw-r--r--   0        0        0    26674 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/events.py
--rw-r--r--   0        0        0      474 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/models.py
--rw-r--r--   0        0        0    36770 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/triggers.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v1/__init__.py
--rw-r--r--   0        0        0      657 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v1/models.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta1/__init__.py
--rw-r--r--   0        0        0      662 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta1/models.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta2/__init__.py
--rw-r--r--   0        0        0      662 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta2/models.py
--rw-r--r--   0        0        0     1283 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/base_event.py
--rw-r--r--   0        0        0     5144 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/base_triggers.py
--rw-r--r--   0        0        0    13383 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/custom_models.py
--rw-r--r--   0        0        0       88 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/model_not_found_exception.py
--rw-r--r--   0        0        0     5100 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/process_utils.py
--rw-r--r--   0        0        0      578 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/templates.py
--rw-r--r--   0        0        0        1 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/__init__.py
--rw-r--r--   0        0        0     1216 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files.py
--rw-r--r--   0        0        0     2504 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files_image.py
--rw-r--r--   0        0        0     7202 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files_text.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/__init__.py
--rw-r--r--   0        0        0     1088 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_action.py
--rw-r--r--   0        0        0      167 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_base.py
--rw-r--r--   0        0        0      759 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_card.py
--rw-r--r--   0        0        0     1115 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_column.py
--rw-r--r--   0        0        0      707 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_container.py
--rw-r--r--   0        0        0      941 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_images.py
--rw-r--r--   0        0        0     1141 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_table.py
--rw-r--r--   0        0        0     2056 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_text_block.py
--rw-r--r--   0        0        0      602 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_mark_down_fix_url.py
--rw-r--r--   0        0        0     6685 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_msg.py
--rw-r--r--   0        0        0     2223 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/sender.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/__init__.py
--rw-r--r--   0        0        0     5098 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/models.py
--rw-r--r--   0        0        0     5207 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/trigger.py
--rw-r--r--   0        0        0      851 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/utils.py
--rw-r--r--   0        0        0    10011 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/receiver.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/__init__.py
--rwxr-xr-x   0        0        0     5148 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/memory_analyzer.py
--rw-r--r--   0        0        0     4825 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/node_cpu_analyzer.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/__init__.py
--rw-r--r--   0        0        0      384 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/event.py
--rw-r--r--   0        0        0      128 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/models.py
--rw-r--r--   0        0        0      555 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler.py
--rw-r--r--   0        0        0      330 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler_manager.py
--rw-r--r--   0        0        0     5193 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler_manager_impl.py
--rw-r--r--   0        0        0     1318 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/trigger.py
--rw-r--r--   0        0        0       22 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/slack/__init__.py
--rw-r--r--   0        0        0    10632 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/slack/sender.py
--rw-r--r--   0        0        0     8402 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/model/config.py
--rw-r--r--   0        0        0      644 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/model/playbook_action.py
--rw-r--r--   0        0        0     1423 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/model/playbook_definition.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/__init__.py
--rw-r--r--   0        0        0    12233 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/config_loader.py
--rw-r--r--   0        0        0      927 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/log_init.py
--rw-r--r--   0        0        0     1341 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/main.py
--rw-r--r--   0        0        0      162 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/not_found_exception.py
--rw-r--r--   0        0        0      517 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/object_updater.py
--rw-r--r--   0        0        0      531 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/telemetry.py
--rw-r--r--   0        0        0     2088 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/telemetry_service.py
--rw-r--r--   0        0        0     3081 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/web.py
--rw-r--r--   0        0        0     1234 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/web_api.py
--rw-r--r--   0        0        0        0 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/__init__.py
--rw-r--r--   0        0        0     1700 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/auth_provider.py
--rw-r--r--   0        0        0     1337 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/common.py
--rw-r--r--   0        0        0      562 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/decorators.py
--rw-r--r--   0        0        0     1681 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/docs.py
--rw-r--r--   0        0        0     2424 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/documented_pydantic.py
--rw-r--r--   0        0        0     1648 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/file_system_watcher.py
--rw-r--r--   0        0        0      950 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/function_hashes.py
--rw-r--r--   0        0        0     6176 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/json_schema.py
--rw-r--r--   0        0        0      374 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/parsing.py
--rw-r--r--   0        0        0     1253 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/rate_limiter.py
--rw-r--r--   0        0        0      892 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/service_discovery.py
--rw-r--r--   0        0        0     2356 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/task_queue.py
--rw-r--r--   0        0        0     3048 2022-04-27 08:15:35.708116 robusta-cli-0.9.9/setup.py
--rw-r--r--   0        0        0     1966 2022-04-27 08:15:35.708514 robusta-cli-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/LICENSE
+-rw-r--r--   0        0        0       13 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/README.md
+-rw-r--r--   0        0        0      633 2024-06-02 10:35:02.833988 robusta_cli-1.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/__init__.py
+-rw-r--r--   0        0        0       78 2024-06-02 10:35:02.833988 robusta_cli-1.0a0/robusta_cli/_version.py
+-rw-r--r--   0        0        0     5794 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/auth.py
+-rw-r--r--   0        0        0     2005 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/backend_profile.py
+-rw-r--r--   0        0        0     5181 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/demo_alert.py
+-rw-r--r--   0        0        0      953 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/eula.py
+-rw-r--r--   0        0        0     5062 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/integrations_cmd.py
+-rwxr-xr-x   0        0        0    14346 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/main.py
+-rw-r--r--   0        0        0    11882 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/playbooks_cmd.py
+-rw-r--r--   0        0        0     7904 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/self_host.py
+-rw-r--r--   0        0        0      829 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/simple_sink_config.py
+-rw-r--r--   0        0        0     2991 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/slack_feedback_message.py
+-rw-r--r--   0        0        0     3448 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/slack_verification.py
+-rw-r--r--   0        0        0     4052 2024-06-02 10:34:38.117651 robusta_cli-1.0a0/robusta_cli/utils.py
+-rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 robusta_cli-1.0a0/PKG-INFO
```

### Comparing `robusta-cli-0.9.9/LICENSE` & `robusta_cli-1.0a0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Robusta Dev Ltd
+Copyright (c) 2024 Robusta
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `robusta-cli-0.9.9/src/robusta/cli/auth.py` & `robusta_cli-1.0a0/robusta_cli/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 import base64
-import json
+import re
 import subprocess
 import traceback
 import uuid
 from typing import Optional
+
 import click_spinner
-from dpath.util import get
 import requests
 import typer
 import yaml
-from cryptography.hazmat.primitives.serialization import Encoding, PrivateFormat, PublicFormat, NoEncryption
 from cryptography.hazmat.primitives.asymmetric import rsa
+from cryptography.hazmat.primitives.serialization import Encoding, NoEncryption, PrivateFormat, PublicFormat
+from dpath.util import get
 from pydantic import BaseModel
 
-from .backend_profile import backend_profile
-from .playbooks_cmd import NAMESPACE_EXPLANATION, get_playbooks_config
-from .utils import namespace_to_kubectl
+from robusta_cli.backend_profile import backend_profile
+from robusta_cli.playbooks_cmd import NAMESPACE_EXPLANATION, get_playbooks_config
+from robusta_cli.utils import exec_in_robusta_runner_output, namespace_to_kubectl
 
 AUTH_SECRET_NAME = "robusta-auth-config-secret"
-app = typer.Typer()
+app = typer.Typer(add_completion=False)
 
 
 class RSAKeyPair(BaseModel):
-    prv: str
-    pub: str
+    prv: str = None
+    pub: str = None
+    private: str = None
+    public: str = None
 
 
 def gen_rsa_pair() -> RSAKeyPair:
     # generate private/public key pair
     key = rsa.generate_private_key(public_exponent=65537, key_size=2048)
 
     # get public key in OpenSSH format
     public_key = key.public_key().public_bytes(Encoding.PEM, PublicFormat.SubjectPublicKeyInfo)
 
     # get private key in PEM container format
     pem = key.private_bytes(
-        encoding=Encoding.PEM,
-        format=PrivateFormat.TraditionalOpenSSL,
-        encryption_algorithm=NoEncryption()
+        encoding=Encoding.PEM, format=PrivateFormat.TraditionalOpenSSL, encryption_algorithm=NoEncryption()
     )
 
-    return RSAKeyPair(
-        pub=public_key.decode('utf-8'),
-        prv=pem.decode('utf-8')
-    )
+    return RSAKeyPair(public=base64.b64encode(public_key), private=base64.b64encode(pem))
 
 
 def get_existing_auth_config(namespace: str) -> Optional[RSAKeyPair]:
     try:
         secret_content = subprocess.check_output(
             f"kubectl get secret {namespace_to_kubectl(namespace)} {AUTH_SECRET_NAME} -o yaml",
             shell=True,
         )
     except Exception:
         return None
 
     auth_secret = yaml.safe_load(secret_content)
     return RSAKeyPair(
         prv=base64.b64decode(auth_secret["data"]["prv"]).decode(),
-        pub=base64.b64decode(auth_secret["data"]["pub"]).decode()
+        pub=base64.b64decode(auth_secret["data"]["pub"]).decode(),
     )
 
 
 class TokenDetails(BaseModel):
     pub: str
     account_id: str
     user_id: str
@@ -74,30 +72,32 @@
 def store_server_token(token_details: TokenDetails, debug: bool = False) -> bool:
     try:
         response = requests.post(backend_profile.robusta_store_token_url, json=token_details.dict())
         if debug and response.status_code != 201:
             typer.secho(f"Failed to store server token. status-code {response.status_code} text {response.text}")
 
         return response.status_code == 201
-    except Exception as e:
+    except Exception:
         if debug:
             typer.secho(f"Error trying to store server token. {traceback.format_exc()}")
         return False
 
 
+def _get_signing_key_from_env_variable(namespace: Optional[str], env_var_name: str) -> str:
+    return str(exec_in_robusta_runner_output(f'echo "${env_var_name}"', namespace), "utf-8").strip()
+
+
+@app.command(name="web-connect")  # TODO consider removing this
 @app.command()
 def gen_token(
     account_id: str = typer.Option(
         ...,
         help="Robusta account id",
     ),
-    user_id: str = typer.Option(
-        ...,
-        help="User id for which the token is created",
-    ),
+    user_id: str = typer.Option(..., help="User id for which the token is created"),
     session_token: str = typer.Option(
         ...,
         help="User session token. Created for an authenticated user via the Robusta UI",
     ),
     namespace: str = typer.Option(
         None,
         help=NAMESPACE_EXPLANATION,
@@ -106,35 +106,49 @@
 ):
     """Generate token required to run actions manually in Robusta UI"""
     typer.echo("connecting to cluster...")
     with click_spinner.spinner():
         auth_config = get_existing_auth_config(namespace)
 
     if not auth_config:
-        typer.secho("\nRSA auth isn't configured. "
-                    "Please update Robusta and run `robusta update-config` to configure it. Aborting!", fg="red")
+        typer.secho(
+            "\nRSA auth isn't configured. "
+            "Please update Robusta and run `robusta update-config` to configure it. Aborting!",
+            fg="red",
+        )
         return
 
     playbooks_config = get_playbooks_config(namespace)
     active_playbooks_file = playbooks_config["data"]["active_playbooks.yaml"]
     playbooks_config_yaml = yaml.safe_load(active_playbooks_file)
     signing_key = get(playbooks_config_yaml, "global_config/signing_key", default=None)
     if not signing_key:
         typer.secho("signing_key is not defined. Please update Robusta and run `robusta update-config`", fg="red")
         return
 
     try:
-        signing_key = uuid.UUID(signing_key)
+        env_match = re.fullmatch(r"\{\{\s*env\.(\S+)\s*}}", signing_key)
+        if env_match:
+            env_var_name = env_match.group(1)
+            typer.secho(f"Fetching secret key from an env var named: {env_var_name}")
+            signing_key = _get_signing_key_from_env_variable(namespace, env_var_name)
+            if not signing_key:
+                typer.secho(f"Could not find an env var named {env_var_name}", fg="red")
+                return
+        signing_key_uuid = uuid.UUID(signing_key)
     except Exception:
-        typer.secho("Bad format for signing_key. Please run `robusta update-config` to generate a new valid"
-                    " signing_key for your account.", fg="red")
+        typer.secho(
+            "Bad format for signing_key. Please run `robusta update-config` to generate a new valid"
+            " signing_key for your account.",
+            fg="red",
+        )
         return
 
     client_enc_key = uuid.uuid4()
-    server_enc_key = uuid.UUID(int=(signing_key.int ^ client_enc_key.int))
+    server_enc_key = uuid.UUID(int=(signing_key_uuid.int ^ client_enc_key.int))
     key_id = str(uuid.uuid4())
 
     token_response = TokenDetails(
         pub=auth_config.pub,
         account_id=account_id,
         user_id=user_id,
         session_token=session_token,
@@ -144,9 +158,9 @@
     if not store_server_token(token_response, debug):
         typer.secho("Failed to store server token. Aborting!", fg="red")
         return
 
     # client response is the same, only with a different enc_key
     token_response.enc_key = str(client_enc_key)
 
-    typer.secho(f"Token created successfully. Submit it in the Robusta UI", fg="green")
-    typer.secho(str(base64.b64encode(json.dumps(token_response.json(exclude={"session_token"})).encode("utf-8"))))
+    typer.secho("Token created successfully. Submit it in the Robusta UI", fg="green")
+    typer.secho(base64.b64encode(token_response.json(exclude={"session_token"}).encode("utf-8")).decode())
```

### Comparing `robusta-cli-0.9.9/src/robusta/cli/backend_profile.py` & `robusta_cli-1.0a0/robusta_cli/backend_profile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-import json
 import os
 import sys
 
 import typer
 from pydantic.main import BaseModel
 
+from robusta_cli.utils import host_for_params
+
 ROBUSTA_BACKEND_PROFILE = os.environ.get("ROBUSTA_BACKEND_PROFILE", "")
 
 
 class BackendProfile(BaseModel):
     robusta_cloud_api_host: str = ""
     robusta_ui_domain: str = ""
     robusta_relay_ws_address: str = ""
     robusta_relay_external_actions_url: str = ""
     robusta_telemetry_endpoint: str = ""
     robusta_store_token_url: str = ""
     custom_profile: bool = False
 
+    @classmethod
+    def fromDomainProvider(
+        cls, domain: str, api_endpoint_prefix: str, platform_endpoint_prefix: str, relay_endpoint_prefix: str
+    ):
+        return cls(
+            robusta_cloud_api_host=host_for_params(api_endpoint_prefix, domain),
+            robusta_ui_domain=host_for_params(platform_endpoint_prefix, domain),
+            robusta_relay_ws_address=host_for_params(relay_endpoint_prefix, domain, "wss"),
+            robusta_relay_external_actions_url=f"{host_for_params(api_endpoint_prefix, domain)}/integrations/generic/actions",
+            robusta_telemetry_endpoint=f"{host_for_params(api_endpoint_prefix, domain)}/telemetry",
+            robusta_store_token_url=f"{host_for_params(api_endpoint_prefix, domain)}/auth/server/tokens",
+        )
+
 
 # default values
 backend_profile = BackendProfile(
     robusta_cloud_api_host="https://api.robusta.dev",
     robusta_ui_domain="https://platform.robusta.dev",
-    robusta_store_token_url="https://api.robusta.dev/auth/server/tokens"
+    robusta_store_token_url="https://api.robusta.dev/auth/server/tokens",
 )
 
 if ROBUSTA_BACKEND_PROFILE:
     typer.secho(
         f"Using Robusta backend profile: {ROBUSTA_BACKEND_PROFILE}",
         color="blue",
     )
```

### Comparing `robusta-cli-0.9.9/src/robusta/cli/main.py` & `robusta_cli-1.0a0/robusta_cli/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,87 @@
 import base64
 import json
-import random
+import os
 import subprocess
 import time
-import urllib.request
-import uuid
-import click_spinner
-from distutils.version import StrictVersion
-from typing import Optional, List, Union, Dict
-from zipfile import ZipFile
 import traceback
+import uuid
+from typing import Dict, List, Optional, Union
 
-import requests
+import certifi
 import typer
 import yaml
-from kubernetes import config
+
 from pydantic import BaseModel, Extra
 
-# TODO - separate shared classes to a separated shared repo, to remove dependencies between the cli and runner
-from .auth import gen_rsa_pair, RSAKeyPair
-from .backend_profile import backend_profile
-from ..core.sinks.msteams.msteams_sink_params import (
-    MsTeamsSinkConfigWrapper,
-    MsTeamsSinkParams,
-)
-from ..core.sinks.robusta.robusta_sink_params import (
-    RobustaSinkConfigWrapper,
-    RobustaSinkParams,
-)
-from ..core.sinks.slack.slack_sink_params import SlackSinkConfigWrapper, SlackSinkParams
-from robusta._version import __version__
-from .integrations_cmd import app as integrations_commands, get_slack_key
-from .auth import app as auth_commands
-from .slack_verification import verify_slack_channel
-from .slack_feedback_message import SlackFeedbackMessagesSender, SlackFeedbackConfig
-from .playbooks_cmd import app as playbooks_commands
-from .utils import log_title, replace_in_file, namespace_to_kubectl
-
-FORWARDER_CONFIG_FOR_SMALL_CLUSTERS = "64Mi"
-RUNNER_CONFIG_FOR_SMALL_CLUSTERS = "512Mi"
-GRAFANA_RENDERER_CONFIG_FOR_SMALL_CLUSTERS = "64Mi"
+from robusta_cli._version import __version__
 
-app = typer.Typer()
-app.add_typer(playbooks_commands, name="playbooks", help="Playbooks commands menu")
-app.add_typer(
-    integrations_commands, name="integrations", help="Integrations commands menu"
-)
-app.add_typer(
-    auth_commands, name="auth", help="Authentication commands menu"
-)
+from robusta_cli.auth import app as auth_commands
+from robusta_cli.backend_profile import backend_profile
+from robusta_cli.eula import handle_eula
+from robusta_cli.integrations_cmd import app as integrations_commands
+from robusta_cli.integrations_cmd import get_slack_key, get_ui_key
+from robusta_cli.playbooks_cmd import app as playbooks_commands
+from robusta_cli.self_host import app as self_host_commands
+from robusta_cli.slack_feedback_message import SlackFeedbackMessagesSender
+from robusta_cli.slack_verification import verify_slack_channel
+from robusta_cli.utils import get_runner_pod, log_title, namespace_to_kubectl
+from robusta_cli.simple_sink_config import MsTeamsSinkConfigWrapper, MsTeamsSinkParams
+from robusta_cli.simple_sink_config import RobustaSinkConfigWrapper, RobustaSinkParams
+from robusta_cli.simple_sink_config import SlackSinkConfigWrapper, SlackSinkParams
+from robusta_cli.demo_alert import create_demo_alert, AlertManagerException
+
+ADDITIONAL_CERTIFICATE: str = os.environ.get("CERTIFICATE", "")
+
+
+def cert_already_exists(new_cert: bytes) -> bool:
+    with open(certifi.where(), "r") as outfile:
+        return str(new_cert, "utf-8") in outfile.read()
+
+
+def add_custom_certificate(custom_ca: str):
+    if custom_ca:
+        new_cert = base64.b64decode(custom_ca)
+        if not cert_already_exists(new_cert):
+            with open(certifi.where(), "ab") as outfile:
+                outfile.write(base64.b64decode(custom_ca))
+                return True
+        else:
+            typer.secho("using custom certificate", fg="green")
+
+    return False
 
 
-def get_runner_url(runner_version=None):
-    if runner_version is None:
-        runner_version = __version__
-    return f"https://gist.githubusercontent.com/robusta-lab/6b809d508dfc3d8d92afc92c7bbbe88e/raw/robusta-{runner_version}.yaml"
+if add_custom_certificate(ADDITIONAL_CERTIFICATE):
+    typer.secho("using custom certificate", fg="green")
+
+app = typer.Typer(add_completion=False)
+app.add_typer(playbooks_commands, name="playbooks", help="Playbooks commands menu")
+app.add_typer(integrations_commands, name="integrations", help="Integrations commands menu")
+app.add_typer(auth_commands, name="auth", help="Authentication commands menu")
+app.add_typer(self_host_commands, name="self-host", help="Self-host commands menu")
 
 
 class GlobalConfig(BaseModel):
     signing_key: str = ""
     account_id: str = ""
 
 
-class PodConfigs(Dict[str, Dict[str, Dict[str, str]]]):
-    __root__: Dict[str, Dict[str, Dict[str, str]]]
-
-    @classmethod
-    def gen_config(cls, memory_size: str) -> Dict:
-        return {"resources": {"requests": {"memory": memory_size}}}
-
-
 class HelmValues(BaseModel, extra=Extra.allow):
     globalConfig: GlobalConfig
-    sinksConfig: List[
-        Union[
-            SlackSinkConfigWrapper, RobustaSinkConfigWrapper, MsTeamsSinkConfigWrapper
-        ]
-    ]
-    clusterName: str
+    sinksConfig: List[Union[SlackSinkConfigWrapper, RobustaSinkConfigWrapper, MsTeamsSinkConfigWrapper]]
+    clusterName: Optional[str] = None
+    isSmallCluster: Optional[bool] = None
     enablePrometheusStack: bool = False
     disableCloudRouting: bool = False
     enablePlatformPlaybooks: bool = False
     playbooksPersistentVolumeSize: str = None
     kubewatch: Dict = None
     grafanaRenderer: Dict = None
     runner: Dict = None
-    rsa: RSAKeyPair = None
-
-    def set_pod_configs_for_small_clusters(self):
-        self.kubewatch = PodConfigs.gen_config(FORWARDER_CONFIG_FOR_SMALL_CLUSTERS)
-        self.runner = PodConfigs.gen_config(RUNNER_CONFIG_FOR_SMALL_CLUSTERS)
-        self.grafanaRenderer = PodConfigs.gen_config(
-            GRAFANA_RENDERER_CONFIG_FOR_SMALL_CLUSTERS
-        )
-
-
-def guess_cluster_name(context):
-    with click_spinner.spinner():
-        try:
-            all_contexts, current_context = config.list_kube_config_contexts()
-            if context is not None:
-                for i in range(len(all_contexts)):
-                    if all_contexts[i].get('name') == context:
-                        return all_contexts[i].get('context').get('cluster')
-                typer.echo(f" no context exists with the name '{context}', your current context is {current_context.get('cluster')}")
-            if current_context and current_context.get("name"):
-                return current_context.get("context").get("cluster")
-        except Exception:  # this happens, for example, if you don't have a kubeconfig file
-            typer.echo("Error reading kubeconfig to generate cluster name")
-        return f"cluster_{random.randint(0, 1000000)}"
 
 
 def get_slack_channel() -> str:
     return (
         typer.prompt(
             "Which slack channel should I send notifications to? ",
             prompt_suffix="#",
@@ -122,30 +91,29 @@
     )
 
 
 def write_values_file(output_path: str, values: HelmValues):
     with open(output_path, "w") as output_file:
         yaml.safe_dump(values.dict(exclude_defaults=True), output_file, sort_keys=False)
         typer.secho(
-            f"Saved configuration to {output_path}",
-            fg="green",
-        )
-        typer.secho(
-            f"Save this file for future use. It contains your account credentials",
+            f"Saved configuration to {output_path} - save this file for future use!",
             fg="red",
         )
 
 
 @app.command()
 def gen_config(
     cluster_name: str = typer.Option(
         None,
         help="Cluster Name",
     ),
-    is_small_cluster: bool = typer.Option(None),
+    is_small_cluster: bool = typer.Option(
+        None,
+        help="Local/Small cluster",
+    ),
     slack_api_key: str = typer.Option(
         "",
         help="Slack API Key",
     ),
     slack_channel: str = typer.Option(
         "",
         help="Slack Channel",
@@ -153,54 +121,45 @@
     msteams_webhook: str = typer.Option(
         None,
         help="MsTeams webhook url",
     ),
     robusta_api_key: str = typer.Option(None),
     enable_prometheus_stack: bool = typer.Option(None),
     disable_cloud_routing: bool = typer.Option(None),
-    output_path: str = typer.Option(
-        "./generated_values.yaml", help="Output path of generated Helm values"
-    ),
+    output_path: str = typer.Option("./generated_values.yaml", help="Output path of generated Helm values"),
     debug: bool = typer.Option(False),
     context: str = typer.Option(
         None,
         help="The name of the kubeconfig context to use",
     ),
+    enable_crash_report: bool = typer.Option(None),
 ):
     """Create runtime configuration file"""
-    if cluster_name is None:
-        cluster_name = typer.prompt(
-            "Please specify a unique name for your cluster or press ENTER to use the default",
-            default=guess_cluster_name(context),
-        )
-    if is_small_cluster is None:
-        is_small_cluster = typer.confirm(
-            "Are you running a mini cluster? (Like minikube or kind)"
-        )
 
-    sinks_config: List[
-        Union[
-            SlackSinkConfigWrapper, RobustaSinkConfigWrapper, MsTeamsSinkConfigWrapper
-        ]
-    ] = []
+    # Configure sinks
+    typer.secho(
+        """Robusta reports its findings to external destinations (we call them "sinks").\nWe'll define some of them now.\n""",
+        fg=typer.colors.CYAN,
+        bold=True,
+    )
+
+    sinks_config: List[Union[SlackSinkConfigWrapper, RobustaSinkConfigWrapper, MsTeamsSinkConfigWrapper]] = []
     slack_workspace = "N/A"
     if not slack_api_key and typer.confirm(
-        "Do you want to configure slack integration? This is HIGHLY recommended.",
+        "Configure Slack integration? This is HIGHLY recommended.",
         default=True,
     ):
         slack_api_key, slack_workspace = get_slack_key()
 
     if slack_api_key and not slack_channel:
         slack_channel = get_slack_channel()
 
     slack_integration_configured = False
     if slack_api_key and slack_channel:
-        while not verify_slack_channel(
-            slack_api_key, cluster_name, slack_channel, slack_workspace, debug
-        ):
+        while not verify_slack_channel(slack_api_key, slack_channel, slack_workspace, debug):
             slack_channel = get_slack_channel()
 
         sinks_config.append(
             SlackSinkConfigWrapper(
                 slack_sink=SlackSinkParams(
                     name="main_slack_sink",
                     api_key=slack_api_key,
@@ -208,19 +167,19 @@
                 )
             )
         )
 
         slack_integration_configured = True
 
     if msteams_webhook is None and typer.confirm(
-        "Do you want to configure MsTeams integration ?",
+        "Configure MsTeams integration?",
         default=False,
     ):
         msteams_webhook = typer.prompt(
-            "Please insert your MsTeams webhook url",
+            "Please insert your MsTeams webhook url. See https://docs.robusta.dev/master/configuration/sinks/ms-teams.html",
             default=None,
         )
 
     if msteams_webhook:
         sinks_config.append(
             MsTeamsSinkConfigWrapper(
                 ms_teams_sink=MsTeamsSinkParams(
@@ -231,251 +190,208 @@
         )
 
     enable_platform_playbooks = False
     # we have a slightly different flow here than the other options so that pytest can pass robusta_api_key="" to skip
     # asking the question
     if robusta_api_key is None:
         if typer.confirm(
-            "Would you like to use Robusta UI? This is HIGHLY recommended.",
+            "Configure Robusta UI sink? This is HIGHLY recommended.",
             default=True,
         ):
-            if typer.confirm("Do you already have a Robusta account?"):
-                while True:
-                    robusta_api_key = typer.prompt(
-                        "Please insert your Robusta account token",
-                        default=None,
-                    )
-                    try:
-                        json.loads(base64.b64decode(robusta_api_key))
-                        break
-                    except Exception:
-                        typer.secho(
-                            "Sorry, invalid token format. "
-                            "The token can be found in any existing generated_values.yaml file, under the robusta_sink",
-                            fg="red",
-                        )
-
-            else:  # self registration
-                account_name = typer.prompt("Choose your account name")
-                email = typer.prompt(
-                    "Enter a Gmail/Google Workspace address. This will be used to login"
-                )
-                email = email.strip()
-                res = requests.post(
-                    f"{backend_profile.robusta_cloud_api_host}/accounts/create",
-                    json={
-                        "account_name": account_name,
-                        "email": email,
-                    },
-                )
-                if res.status_code == 201:
-                    robusta_api_key = res.json().get("token")
-                    typer.echo(
-                        "Successfully registered.\n",
-                        color="green",
-                    )
-                    typer.echo("A few more questions and we're done...\n")
-                else:
-                    typer.echo(
-                        "Sorry, something didn't work out. Please contact us at support@robusta.dev",
-                        color="red",
-                    )
-                    robusta_api_key = ""
+            robusta_api_key = get_ui_key()
         else:
             robusta_api_key = ""
 
     account_id = str(uuid.uuid4())
-    require_eula_approval = False
     if robusta_api_key:  # if Robusta ui sink is defined, take the account id from it
         token = json.loads(base64.b64decode(robusta_api_key))
         account_id = token.get("account_id", account_id)
 
-        sinks_config.append(
-            RobustaSinkConfigWrapper(
-                robusta_sink=RobustaSinkParams(
-                    name="robusta_ui_sink", token=robusta_api_key
-                )
-            )
-        )
+        # Make sure the UI sink (if enabled) is the first one. See MAIN-1088.
+        sinks_config = [
+            RobustaSinkConfigWrapper(robusta_sink=RobustaSinkParams(name="robusta_ui_sink", token=robusta_api_key))
+        ] + sinks_config
         enable_platform_playbooks = True
-        require_eula_approval = True
+        disable_cloud_routing = False
 
     slack_feedback_heads_up_message: Optional[str] = None
-    if slack_integration_configured:
+    # When using custom certificates we do not want to add the extra slack message.
+    if slack_integration_configured and not ADDITIONAL_CERTIFICATE:
         try:
             slack_feedback_heads_up_message = SlackFeedbackMessagesSender(
-                slack_api_key,
-                slack_channel,
-                account_id,
-                debug
+                slack_api_key, slack_channel, account_id, debug
             ).schedule_feedback_messages()
-        except Exception as e:
+        except Exception:
             if debug:
                 typer.secho(traceback.format_exc())
 
     if enable_prometheus_stack is None:
+        typer.echo(
+            f"""Robusta can use {typer.style("Prometheus", fg=typer.colors.YELLOW, bold=True)} as an alert source."""
+        )
+
         enable_prometheus_stack = typer.confirm(
-            "If you haven't installed Prometheus yet, Robusta can install a pre-configured Prometheus. Would you like to do so?"
+            f"""If you haven't installed it yet, Robusta can install a pre-configured {typer.style("Prometheus", fg=typer.colors.YELLOW, bold=True)}.\nWould you like to do so?"""
         )
 
     if disable_cloud_routing is None:
         disable_cloud_routing = not typer.confirm(
             "Would you like to enable two-way interactivity (e.g. fix-it buttons in Slack) via Robusta's cloud?"
         )
-        if not disable_cloud_routing:
-            require_eula_approval = True
 
-    if require_eula_approval:
-        eula_url = f"{backend_profile.robusta_cloud_api_host}/eula.html"
-        typer.echo(
-            f"Please read and approve our End User License Agreement: {eula_url}"
-        )
-        eula_approved = typer.confirm("Do you accept our End User License Agreement?")
-        if not eula_approved:
-            typer.echo("End User License Agreement rejected. Installation aborted.")
-            return
+    handle_eula(account_id, robusta_api_key, not disable_cloud_routing)
 
-        try:
-            requests.get(f"{eula_url}?account_id={account_id}")
-        except Exception:
-            typer.echo(f"\nEula approval failed: {eula_url}")
+    if enable_crash_report is None:
+        enable_crash_report = typer.confirm(
+            "Last question! Would you like to help us improve Robusta by sending exception reports?"
+        )
 
     signing_key = str(uuid.uuid4()).replace("_", "")
 
     values = HelmValues(
         clusterName=cluster_name,
+        isSmallCluster=is_small_cluster,
         globalConfig=GlobalConfig(signing_key=signing_key, account_id=account_id),
         sinksConfig=sinks_config,
         enablePrometheusStack=enable_prometheus_stack,
         disableCloudRouting=disable_cloud_routing,
         enablePlatformPlaybooks=enable_platform_playbooks,
-        rsa=gen_rsa_pair()
     )
 
-    if is_small_cluster:
-        values.set_pod_configs_for_small_clusters()
-        values.playbooksPersistentVolumeSize = "128Mi"
+    values.runner = {}
+    values.runner["sendAdditionalTelemetry"] = enable_crash_report
 
     if backend_profile.custom_profile:
-        if not values.runner:
-            values.runner = {}
         values.runner["additional_env_vars"] = [
             {
                 "name": "RELAY_EXTERNAL_ACTIONS_URL",
                 "value": backend_profile.robusta_relay_external_actions_url,
             },
             {
                 "name": "WEBSOCKET_RELAY_ADDRESS",
                 "value": backend_profile.robusta_relay_ws_address,
             },
             {"name": "ROBUSTA_UI_DOMAIN", "value": backend_profile.robusta_ui_domain},
             {
                 "name": "ROBUSTA_TELEMETRY_ENDPOINT",
-                "value": backend_profile.robusta_telemetry_endpoint
-            }
+                "value": backend_profile.robusta_telemetry_endpoint,
+            },
         ]
 
+    if is_small_cluster:
+        setattr(values, "kube-prometheus-stack", {})
+        kube_stack = getattr(values, "kube-prometheus-stack")
+        kube_stack["prometheus"] = {
+            "prometheusSpec": {"resources": {"requests": {"memory": "300Mi"}, "limits": {"memory": "300Mi"}}},
+        }
+
     write_values_file(output_path, values)
 
     if robusta_api_key:
         typer.secho(
-            f"Finish the Helm install and then login to Robusta UI at {backend_profile.robusta_ui_domain}\n",
+            f"Finish installing with Helm (see the Robusta docs). Then login to Robusta UI at {backend_profile.robusta_ui_domain}\n",
+            fg="green",
+        )
+    else:
+        typer.secho(
+            "Finish installing with Helm (see the Robusta docs). By the way, you're missing out on the UI! See https://home.robusta.dev/ui/\n",
             fg="green",
         )
 
     if slack_feedback_heads_up_message:
         typer.secho(slack_feedback_heads_up_message)
 
 
 @app.command()
-def update_config(
-    existing_values: str = typer.Option(
-        ...,
-        help="Existing values.yaml file name. You can run `helm get values` to get it from the cluster.",
-    ),
-):
-    """
-        Update an existing values.yaml file.
-        Add RSA key-pair if it doesn't exist
-        Add a signing key if it doesn't exist, or replace with a valid one if the key has an invalid format
-    """
-    with open(existing_values, "r") as existing_values_file:
-        values: HelmValues = HelmValues(**yaml.safe_load(existing_values_file))
-        if not values.rsa:
-            typer.secho("Generating RSA key-pair", fg="green")
-            values.rsa = gen_rsa_pair()
-
-        if not values.globalConfig.signing_key:
-            typer.secho("Generating signing key", fg="green")
-            values.globalConfig.signing_key = str(uuid.uuid4())
-
-        try:
-            uuid.UUID(values.globalConfig.signing_key)
-        except:
-            typer.secho("Invalid signing key. Generating a new one", fg="green")
-            values.globalConfig.signing_key = str(uuid.uuid4())
-
-        write_values_file("updated_values.yaml", values)
-        typer.secho("Run `helm upgrade robusta -f ./updated_values.yaml`", fg="green")
-
-
-@app.command()
-def playground():
-    """Open a python playground - useful when writing playbooks"""
-    typer.echo(
-        "this command is temporarily disabled due to recent changes to python:3.8-slim"
-    )
-    # exec_in_robusta_runner("socat readline unix-connect:/tmp/manhole-1")
-
-
-@app.command()
 def version():
     """Show the version of the local robusta-cli"""
     if __version__ == "0.0.0":
-        typer.echo("running with development version from git")
+        typer.echo("running with development version from git (0.0.0)")
     else:
         typer.echo(f"version {__version__}")
 
 
 @app.command()
 def demo():
     """Deliberately deploy a crashing pod to kubernetes so you can test robusta's response"""
     CRASHPOD_YAML = "https://gist.githubusercontent.com/robusta-lab/283609047306dc1f05cf59806ade30b6/raw/crashpod.yaml"
     log_title("Deploying a crashing pod to kubernetes...")
     subprocess.check_call(f"kubectl apply -f {CRASHPOD_YAML}", shell=True)
-    log_title(
-        "In ~30 seconds you should receive a slack notification on a crashing pod"
-    )
+    log_title("In ~30 seconds you should receive a slack notification on a crashing pod")
     time.sleep(60)
-    subprocess.check_call(f"kubectl delete deployment crashpod", shell=True)
+    subprocess.check_call("kubectl delete deployment crashpod", shell=True)
     log_title("Done!")
 
 
 @app.command()
 def logs(
     namespace: str = typer.Option(
         None,
         help="Namespace",
     ),
     f: bool = typer.Option(False, "-f", show_default=False, help="Stream runner logs"),
-    since: str = typer.Option(
-        None, help="Only return logs newer than a relative duration like 5s, 2m, or 3h."
-    ),
+    since: str = typer.Option(None, help="Only return logs newer than a relative duration like 5s, 2m, or 3h."),
     tail: int = typer.Option(None, help="Lines of recent log file to display."),
-    context: str = typer.Option(
-        None,
-        help="The name of the kubeconfig context to use"
-    ),
+    context: str = typer.Option(None, help="The name of the kubeconfig context to use"),
+    resource_name: str = typer.Option(None, help="Robusta Runner deployment or pod name"),
 ):
     """Fetch Robusta runner logs"""
     stream = "-f" if f else ""
     since = f"--since={since}" if since else ""
     tail = f"--tail={tail}" if tail else ""
     context = f"--context={context}" if context else ""
-    subprocess.check_call(
-        f"kubectl logs {stream} {namespace_to_kubectl(namespace)} deployment/robusta-runner -c runner {since} {tail} {context}",
-        shell=True,
-    )
+    resource_name = resource_name if resource_name else get_runner_pod(namespace)
+
+    if not resource_name:
+        return
+
+    try:
+        subprocess.check_call(
+            f"kubectl logs {stream} {namespace_to_kubectl(namespace)} {resource_name} -c runner {since} {tail} {context}",
+            shell=True,
+        )
+    except Exception:
+        log_title("Error fetching logs. Did you forget to specify --namespace?", color="red")
+
+
+@app.command()
+def demo_alert(
+    alertmanager_url: str = typer.Option(
+        None,
+        help="Alertmanager in cluster url. "
+        "By default, Robusta will auto-discover the AlertManager running in your cluster. "
+        "Use this parameter to override the AlertManager url."
+        "For example: http://alertmanager.monitoring.svc.cluster.local:9093",
+    ),
+    namespaces: List[str] = typer.Option(
+        ["robusta", "default"],
+        help="List of namespaces, to select the alert pod from",
+    ),
+    alert: str = typer.Option(
+        "KubePodNotReady",
+        help="Created alert name",
+    ),
+    labels: str = typer.Option(
+        None,
+        help="Additional alert labels. Comma separated list. For example: env=prod,team=infra ",
+    ),
+    kube_config: str = typer.Option(None, help="Kube config file path override."),
+    image: str = typer.Option("curlimages/curl", help="Docker image with curl support."),
+):
+    """
+    Create a demo alert on AlertManager.
+    The alert pod is selected randomly from the pods in the current namespace
+    """
+    try:
+        pod_name, namespace = create_demo_alert(alertmanager_url, namespaces, alert, labels, kube_config, image)
+        typer.secho(
+            f"Created Alertmanager alert: alert-name: {alert} pod: {pod_name} "
+            f"namespace: {namespace}",
+            fg="green",
+        )
+        typer.echo("\n")
+    except AlertManagerException as e:
+        typer.secho(e.message, fg="red")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `robusta-cli-0.9.9/src/robusta/cli/playbooks_cmd.py` & `robusta_cli-1.0a0/robusta_cli/playbooks_cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,59 @@
 import base64
 import json
 import os
 import subprocess
 import tempfile
 import time
 import traceback
-import click_spinner
-import click
-from typing import List, Optional, Dict
-
-import yaml
+from typing import Dict, List, Optional
 
+import click
+import click_spinner
 import typer
+import yaml
 
-from ..cli.utils import (
-    log_title,
-    fetch_runner_logs,
+from robusta_cli.utils import (
+    PLAYBOOKS_DIR,
+    _build_exec_command,
     exec_in_robusta_runner,
-    namespace_to_kubectl,
-    PLAYBOOKS_DIR, get_package_name,
+    fetch_runner_logs,
+    get_package_name,
+    get_runner_pod,
+    log_title,
+    namespace_to_kubectl
 )
 
 PLAYBOOKS_MOUNT_LOCATION = "/etc/robusta/playbooks/storage"
 
-NAMESPACE_EXPLANATION = (
-    "Installation namespace. If none use the namespace currently active with kubectl."
-)
+NAMESPACE_EXPLANATION = "Installation namespace. If none use the namespace currently active with kubectl."
 CONFIG_SECRET_NAME = "robusta-playbooks-config-secret"
 
-app = typer.Typer()
-
-
-def get_runner_pod(namespace: str) -> Optional[str]:
-    pods = subprocess.check_output(
-        f'kubectl get pods {namespace_to_kubectl(namespace)} --selector="robustaComponent=runner"',
-        shell=True,
-    )
-    text = pods.decode("utf-8")
-    if not text:
-        return None
-
-    lines = text.split("\n")
-    if len(lines) < 2:
-        return None
-    return lines[1].split(" ")[0]
+app = typer.Typer(add_completion=False)
 
 
 def __validate_playbooks_dir(playbooks_dir: str) -> bool:
     files = os.listdir(playbooks_dir)
     if "pyproject.toml" not in files:
         typer.secho("Illegal playbooks package. missing pyproject.toml", fg="red")
         return False
 
     package_name = get_package_name(os.path.join(playbooks_dir))
     if not package_name:
-        typer.secho("Illegal pyproject.toml. `name` attribute not defined in pyproject.toml", fg="red")
+        typer.secho(
+            "Illegal pyproject.toml. `name` attribute not defined in pyproject.toml",
+            fg="red",
+        )
         return False
 
     if package_name not in files:
-        typer.secho(f"Playbooks directory missing or does not match playbooks package name {package_name}", fg="red")
+        typer.secho(
+            f"Playbooks directory missing or does not match playbooks package name {package_name}",
+            fg="red",
+        )
         return False
 
     return True
 
 
 @app.command()
 def push(
@@ -76,15 +67,18 @@
     ),
 ):
     """Load custom playbooks code"""
     log_title("Uploading playbooks code...")
     with fetch_runner_logs(namespace):
         runner_pod = get_runner_pod(namespace)
         if not runner_pod:
-            log_title(f"Runner pod not found in the {namespace} namespace. If robusta is installed in a different namespace, use the --namespace flag.", color="red")
+            log_title(
+                f"Runner pod not found in the {namespace} namespace. If robusta is installed in a different namespace, use the --namespace flag.",
+                color="red",
+            )
             return
 
         subprocess.check_call(
             f"kubectl exec -it {namespace_to_kubectl(namespace)} {runner_pod} -c runner "
             f"-- bash -c 'mkdir -p {PLAYBOOKS_MOUNT_LOCATION}'",
             shell=True,
         )
@@ -94,17 +88,15 @@
             return
 
         subprocess.check_call(
             f"kubectl cp {namespace_to_kubectl(namespace)} {abs_path} "
             f"{runner_pod}:{PLAYBOOKS_MOUNT_LOCATION}/{dir_name} -c runner",
             shell=True,
         )
-        time.sleep(
-            5
-        )  # wait five seconds for the runner to actually reload the playbooks
+        time.sleep(5)  # wait five seconds for the runner to actually reload the playbooks
     log_title("Loaded custom playbooks code!")
 
 
 @app.command()
 def configure(
     config_file: str = typer.Argument(
         ...,
@@ -120,21 +112,19 @@
     with fetch_runner_logs(namespace):
         subprocess.check_call(
             f"kubectl create secret generic {namespace_to_kubectl(namespace)} {CONFIG_SECRET_NAME} "
             f"--from-file active_playbooks.yaml={config_file} --type=Opaque -o yaml --dry-run | kubectl apply -f -",
             shell=True,
         )
         subprocess.check_call(
-            f'kubectl annotate pods {namespace_to_kubectl(namespace)} -l robustaComponent=runner '
+            f"kubectl annotate pods {namespace_to_kubectl(namespace)} -l robustaComponent=runner "
             f'--overwrite "playbooks-last-modified={time.time()}"',
             shell=True,
         )
-        time.sleep(
-            5
-        )  # wait five seconds for the runner to actually reload the playbooks
+        time.sleep(5)  # wait five seconds for the runner to actually reload the playbooks
     log_title("Deployed playbooks!")
 
 
 def get_playbooks_config(namespace: str):
     configmap_content = subprocess.check_output(
         f"kubectl get secret {namespace_to_kubectl(namespace)} {CONFIG_SECRET_NAME} -o yaml",
         shell=True,
@@ -162,51 +152,56 @@
         playbooks_directory = os.path.join(os.getcwd(), PLAYBOOKS_DIR)
 
     log_title(f"Pulling playbooks into {playbooks_directory} ")
 
     try:
         runner_pod = get_runner_pod(namespace)
         if not runner_pod:
-            log_title("Runner pod not found.", color="red")
             return
 
         subprocess.check_call(
             f"kubectl cp {namespace_to_kubectl(namespace)} "
             f"{runner_pod}:{PLAYBOOKS_MOUNT_LOCATION}/ -c runner {playbooks_directory}",
             shell=True,
         )
-    except Exception as e:
+    except Exception:
         typer.echo(f"Failed to pull deployed playbooks {traceback.format_exc()}")
 
 
 @app.command("list-dirs")
 def list_dirs(
     namespace: str = typer.Option(
         None,
         help=NAMESPACE_EXPLANATION,
     ),
 ):
     """List stored playbooks directories"""
-    log_title(f"Listing playbooks directories ")
+    log_title("Listing playbooks directories ")
 
     try:
         runner_pod = get_runner_pod(namespace)
         if not runner_pod:
-            log_title("Runner pod not found.", color="red")
             return
 
         ls_res = subprocess.check_output(
             f"kubectl exec -it {namespace_to_kubectl(namespace)} {runner_pod} -c runner "
             f"-- bash -c 'ls {PLAYBOOKS_MOUNT_LOCATION}'",
             shell=True,
+            stderr=subprocess.STDOUT,
         )
 
         log_title(f"Stored playbooks directories: \n { ls_res.decode('utf-8')}")
 
-    except Exception as e:
+    except subprocess.CalledProcessError as e:
+        if "no such file or directory" in str(e.output).lower():
+            log_title(f"Could not find any stored playbooks.")
+            return
+
+        typer.echo(f"Failed to list deployed playbooks {traceback.format_exc()}")
+    except Exception:
         typer.echo(f"Failed to list deployed playbooks {traceback.format_exc()}")
 
 
 @app.command()
 def delete(
     playbooks_directory: str = typer.Argument(
         ...,
@@ -223,51 +218,56 @@
         return
 
     log_title(f"Deleting playbooks directory {playbooks_directory} ")
 
     try:
         runner_pod = get_runner_pod(namespace)
         if not runner_pod:
-            log_title("Runner pod not found.", color="red")
             return
 
         path_to_delete = os.path.join(PLAYBOOKS_MOUNT_LOCATION, playbooks_directory)
         subprocess.check_call(
             f"kubectl exec -it {namespace_to_kubectl(namespace)} {runner_pod} -c runner "
             f"-- bash -c 'rm -rf {path_to_delete}'",
             shell=True,
         )
 
-    except Exception as e:
+    except Exception:
         typer.echo(f"Failed to delete deployed playbooks {traceback.format_exc()}")
 
 
 def print_yaml_if_not_none(key: str, json_dict: dict):
     if json_dict.get(key):
         json = {}
         json[key] = json_dict.get(key)
         typer.echo(f"{yaml.dump(json)}")
 
 
+# not named list as that would shadow the builtin list function
 @app.command("list")
 def list_(
     namespace: str = typer.Option(
         None,
         help=NAMESPACE_EXPLANATION,
     ),
-):  # not named list as that would shadow the builtin list function
+):  
     """list current active playbooks"""
-    typer.echo(f"Getting deployed playbooks list...")
+    # first we fetch the runner pod, as if the namespace is invalid we want an error message
+    runner_pod = get_runner_pod(namespace)
+    if not runner_pod:
+        return
+    
+    typer.echo("Getting deployed playbooks list...")
     with click_spinner.spinner():
         playbooks_config = get_playbooks_config(namespace)
 
     active_playbooks_file = playbooks_config["data"]["active_playbooks.yaml"]
     active_playbooks_yaml = yaml.safe_load(active_playbooks_file)
     for playbook in active_playbooks_yaml["active_playbooks"]:
-        typer.secho(f"--------------------------------------", fg="blue")
+        typer.secho("--------------------------------------", fg="blue")
         print_yaml_if_not_none("sinks", playbook)
         print_yaml_if_not_none("triggers", playbook)
         print_yaml_if_not_none("actions", playbook)
 
 
 @app.command()
 def edit_config(
@@ -291,26 +291,27 @@
         with tempfile.NamedTemporaryFile(delete=False) as f:
             f.write(edited_result.encode())
             f.flush()
             fname = f.name
         configure(config_file=fname, namespace=namespace)
 
 
-def _post_in_runner_pod(namespace: str, api_path: str, req_body: Dict, req_name: str):
+def _post_in_runner_pod(namespace: str, api_path: str, req_body: Dict, req_name: str, dry_run: bool = False):
     with fetch_runner_logs(namespace=namespace):
         cmd = (
             f"curl -X POST http://localhost:5000/api/{api_path} "
             f"-H 'Content-Type: application/json' "
             f"-d '{json.dumps(req_body)}'"
         )
         exec_in_robusta_runner(
             cmd,
             namespace=namespace,
             tries=3,
             error_msg=f"Cannot {req_name} - usually this means Robusta just started. Will try again",
+            dry_run=dry_run,
         )
         typer.echo("\n")
 
 
 @app.command()
 def trigger(
     action_name: str,
@@ -319,36 +320,67 @@
         help="data to send to action (can be used multiple times)",
         metavar="key=value",
     ),
     namespace: str = typer.Option(
         None,
         help="Robusta namespace",
     ),
+    dry_run: bool = typer.Option(
+        False,
+        help="Don't actually run the trigger, just print a command that can be used to trigger",
+    ),
 ):
     """trigger a manually run playbook"""
     log_title("Triggering action...")
     action_params = {}
     for p in param:
         (key, val) = p.split("=")
         action_params[key] = val
     # action_params = " ".join([f"-F '{p}'" for p in param])
     req_body = {"action_name": action_name, "action_params": action_params}
 
-    _post_in_runner_pod(namespace=namespace, api_path="trigger", req_body=req_body, req_name="trigger action")
+    cmd = (
+        f"curl -X POST http://localhost:5000/api/trigger "
+        f"-H 'Content-Type: application/json' "
+        f"-d '{json.dumps(req_body)}'"
+    )
+
+    if dry_run:
+        typer.echo("For a local runner:")
+        typer.echo(cmd)
+        typer.echo("For your cluster:")
+        typer.echo(" ".join(_build_exec_command(cmd, namespace)))
+        return
+
+    with fetch_runner_logs(namespace=namespace):
+        exec_in_robusta_runner(
+            cmd,
+            namespace=namespace,
+            tries=3,
+            error_msg=f"Cannot trigger playbook - usually this means Robusta just started. Will try again",
+            dry_run=False,  # dry_run handled separately above
+        )
+        typer.echo("\n")
+
     log_title("Done!")
 
 
 @app.command()
 def reload(
-        namespace: str = typer.Option(
-            None,
-            help="Robusta namespace",
-        ),
+    namespace: str = typer.Option(
+        None,
+        help="Robusta namespace",
+    ),
 ):
     """reload playbooks configuration"""
     log_title("Reloading playbooks...")
-    _post_in_runner_pod(namespace=namespace, api_path="playbooks/reload", req_body={}, req_name="reload playbooks")
+    _post_in_runner_pod(
+        namespace=namespace,
+        api_path="playbooks/reload",
+        req_body={},
+        req_name="reload playbooks",
+    )
     log_title("Done!")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `robusta-cli-0.9.9/src/robusta/cli/slack_feedback_message.py` & `robusta_cli-1.0a0/robusta_cli/slack_feedback_message.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
-from slack_sdk import WebClient
-from typing import Optional, List
-from pydantic import BaseModel
-
 import urllib.request
+from typing import List, Optional
+
+from pydantic import BaseModel
+from slack_sdk import WebClient
 
 REMOTE_FEEDBACK_MESSAGE_ADDRESS = "https://docs.robusta.dev/extra/feedback_messages.json"
 
 
 class SlackFeedbackMessage(BaseModel):
     minutes_from_now: int
     title: str
@@ -31,60 +31,56 @@
         slack_feedback_config: SlackFeedbackConfig = SlackFeedbackConfig.parse_raw(raw_feedback_messages)
         if len(slack_feedback_config.messages) == 0:
             return None
         for feedback_message in slack_feedback_config.messages:
             self._schedule_message(
                 feedback_message.minutes_from_now,
                 self._replace_account_id(feedback_message.title),
-                list(map(self._replace_account_id, feedback_message.other_sections)))
+                list(map(self._replace_account_id, feedback_message.other_sections)),
+            )
         return slack_feedback_config.heads_up_message
 
     def _replace_account_id(self, text: str):
-        return text.replace('$ACCOUNT_ID', self.account_id)
+        return text.replace("$ACCOUNT_ID", self.account_id)
 
     @staticmethod
     def _get_feedback_config_from_remote() -> str:
         with urllib.request.urlopen(REMOTE_FEEDBACK_MESSAGE_ADDRESS) as response:
             return response.read()
 
-    def _schedule_message(
-            self,
-            minutes_from_now: int,
-            title: str,
-            other_sections: List[str]
-    ):
+    def _schedule_message(self, minutes_from_now: int, title: str, other_sections: List[str]):
         slack_client = WebClient(token=self.slack_api_key)
 
         schedule_datetime = datetime.datetime.now() + datetime.timedelta(minutes=minutes_from_now)
-        schedule_timestamp = schedule_datetime.strftime('%s')
+        schedule_timestamp = schedule_datetime.strftime("%s")
 
         slack_client.chat_scheduleMessage(
             channel=self.channel_name,
             post_at=schedule_timestamp,
             text="Your feedback is important",
             blocks=self._gen_robusta_slack_message(title, other_sections),
             display_as_bot=True,
             unfurl_links=True,
-            unfurl_media=True
+            unfurl_media=True,
         )
 
     @staticmethod
     def _gen_robusta_slack_message(title: str, other_sections: List[str]):
         blocks = [
             {
                 "type": "header",
                 "text": {
                     "type": "plain_text",
                     "text": title,
                     "emoji": True,
                 },
             },
         ]
-        additional_blocks = [{
-            "type": "section",
-            "text": {
-                "type": "mrkdwn",
-                "text": message
-            },
-        } for message in other_sections]
+        additional_blocks = [
+            {
+                "type": "section",
+                "text": {"type": "mrkdwn", "text": message},
+            }
+            for message in other_sections
+        ]
         blocks.extend(additional_blocks)
         return blocks
```

### Comparing `robusta-cli-0.9.9/src/robusta/cli/slack_verification.py` & `robusta_cli-1.0a0/robusta_cli/slack_verification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 import traceback
+from urllib.error import URLError
+
+import certifi
+import ssl
+import os
 import typer
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
 SLACK_WELCOME_MESSAGE_TITLE = ":large_green_circle: INFO - Welcome to Robusta"
-SLACK_WELCOME_MESSAGE_HEADER_WITH_CLUSTER_NAME = (
-    "You have signed up for Slack Monitoring on cluster: '{}'."
-)
+SLACK_WELCOME_MESSAGE_HEADER = "You've just signed up for Slack monitoring! "
 SLACK_WELCOME_THANK_YOU_MESSAGE = "Thank you for using Robusta.dev"
 SLACK_WELCOME_SUPPORT_MESSAGE = (
     "If you have any questions or feedback feel free to write us at "
     "<mailto:support@robusta.dev|support@robusta.dev> "
 )
 
 
 def verify_slack_channel(
     slack_api_key: str,
-    cluster_name: str,
     channel_name: str,
     workspace: str,
     debug: bool,
 ) -> bool:
     try:
-        output_welcome_message_blocks = __gen_robusta_test_welcome_message(cluster_name)
-        slack_client = WebClient(token=slack_api_key)
+        output_welcome_message_blocks = __gen_robusta_test_welcome_message()
+
+        ssl_context = None
+        if os.environ.get("CERTIFICATE", ""):
+            try:
+                ssl_context = ssl.create_default_context(cafile=certifi.where())
+            except Exception as e:
+                typer.secho(
+                    f"Failed to use custom certificate. {e}",
+                    fg=typer.colors.RED,
+                )
+        slack_client = WebClient(token=slack_api_key, ssl=ssl_context)
         slack_client.chat_postMessage(
             channel=channel_name,
             text="Welcome to Robusta",
             blocks=output_welcome_message_blocks,
             display_as_bot=True,
             unfurl_links=True,
             unfurl_media=True,
@@ -35,45 +47,53 @@
         return True
     except SlackApiError as e:
         if e.response.data["error"] == "channel_not_found":
             channel_name_styled = typer.style(channel_name, fg=typer.colors.RED)
             typer.secho(
                 f"The channel {channel_name_styled} was not found on Slack workspace {workspace}.\n"
                 f"Please verify that the channel exists.\n"
-                f"If this is a private channel, verify the Robusta app was added to the channel."
-                f"(See https://docs.robusta.dev/master/catalog/sinks/slack.html#sending-robusta-notifications-to-a-private-channel)"
+                f"If this is a private channel, verify the Robusta app was added to the channel. "
+                f"(See https://docs.robusta.dev/master/configuration/sinks/slack.html#using-private-channels)"
             )
+        else:
+            typer.secho(f"Unknown Slack error: {e.response.data['error']}")
         return False
-    except Exception as e:
+    except URLError:
+        typer.secho(
+            "SSL certificate issue. See https://docs.robusta.dev/master/help.html\n"
+            "Use --debug for more info.",
+            fg=typer.colors.RED,
+        )
+        exit(1)
+    except Exception:
         if debug:
             typer.secho(traceback.format_exc())
     typer.secho(
-        f"There was an unknown exception setting up Slack, please contact Robusta support.",
+        "There was an unknown exception setting up Slack, use --debug for more info.\n"
+        "Please contact support@robusta.dev",
         fg=typer.colors.RED,
     )
     return False
 
 
-def __gen_robusta_test_welcome_message(cluster_name: str):
+def __gen_robusta_test_welcome_message():
     return [
         {
             "type": "header",
             "text": {
                 "type": "plain_text",
                 "text": SLACK_WELCOME_MESSAGE_TITLE,
                 "emoji": True,
             },
         },
         {
             "type": "header",
             "text": {
                 "type": "plain_text",
-                "text": SLACK_WELCOME_MESSAGE_HEADER_WITH_CLUSTER_NAME.format(
-                    cluster_name
-                ),
+                "text": SLACK_WELCOME_MESSAGE_HEADER,
                 "emoji": True,
             },
         },
         {
             "type": "section",
             "text": {"type": "mrkdwn", "text": SLACK_WELCOME_THANK_YOU_MESSAGE},
         },
```

### Comparing `robusta-cli-0.9.9/src/robusta/cli/utils.py` & `robusta_cli-1.0a0/robusta_cli/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
+import shlex
 import subprocess
 import time
 from contextlib import contextmanager
-from typing import Optional
+from typing import List, Optional
 
 import click_spinner
+import requests
 import toml
 import typer
-import requests
 from dpath.util import get
 
 PLAYBOOKS_DIR = "playbooks/"
 
 
 def namespace_to_kubectl(namespace: Optional[str]):
     if namespace is None:
@@ -22,39 +23,54 @@
 
 def exec_in_robusta_runner(
     cmd,
     namespace: Optional[str],
     tries=1,
     time_between_attempts=10,
     error_msg="error running cmd",
+    dry_run: bool = False,
 ):
-    exec_cmd = [
-        "kubectl",
-        "exec",
-        "-it",
-        "deployment/robusta-runner",
-        "-c",
-        "runner",
-    ]
-    if namespace is not None:
-        exec_cmd += ["-n", namespace]
+    exec_cmd = _build_exec_command(cmd, namespace)
 
-    exec_cmd += ["--", "bash", "-c", cmd]
+    if dry_run:
+        typer.echo(f"Run the following command:\n {shlex.join(exec_cmd)}")
+        return
 
     typer.echo(f"running cmd: {cmd}")
 
     for _ in range(tries - 1):
         try:
             return subprocess.check_call(exec_cmd)
-        except Exception as e:
+        except Exception:
             typer.secho(f"error: {error_msg}", fg="red")
             time.sleep(time_between_attempts)
     return subprocess.check_call(cmd)
 
 
+def exec_in_robusta_runner_output(command: str, namespace: Optional[str]) -> Optional[bytes]:
+    exec_cmd = _build_exec_command(command, namespace)
+    result = subprocess.check_output(exec_cmd)
+    return result
+
+
+def _build_exec_command(command: str, namespace: Optional[str]) -> List[str]:
+    exec_cmd = [
+        "kubectl",
+        "exec",
+        "-it",
+        get_runner_pod(namespace),
+        "-c",
+        "runner",
+    ]
+    if namespace is not None:
+        exec_cmd += ["-n", namespace]
+    exec_cmd += ["--", "bash", "-c", command]
+    return exec_cmd
+
+
 def download_file(url, local_path):
     with click_spinner.spinner():
         response = requests.get(url)
         response.raise_for_status()
     with open(local_path, "wb") as f:
         f.write(response.content)
 
@@ -65,43 +81,66 @@
     typer.echo("=" * 70)
 
 
 def replace_in_file(path, original, replacement):
     with open(path) as r:
         text = r.read()
         if original not in text:
-            raise Exception(
-                f"Cannot replace text {original} in file {path} because it was not found"
-            )
+            raise Exception(f"Cannot replace text {original} in file {path} because it was not found")
         text = text.replace(original, replacement)
     with open(path, "w") as w:
         w.write(text)
 
 
+def host_for_params(component, domain, scheme="https"):
+    return f"{scheme}://{component}.{domain}"
+
+
 @contextmanager
 def fetch_runner_logs(namespace: Optional[str], all_logs=False):
     start = time.time()
     try:
         yield
     finally:
         log_title("Fetching logs...")
         try:
             if all_logs:
                 subprocess.check_call(
-                    f"kubectl logs {namespace_to_kubectl(namespace)} deployment/robusta-runner -c runner",
+                    f"kubectl logs {namespace_to_kubectl(namespace)} {get_runner_pod(namespace)} -c runner",
                     shell=True,
                 )
             else:
                 subprocess.check_call(
-                    f"kubectl logs {namespace_to_kubectl(namespace)} deployment/robusta-runner -c runner --since={int(time.time() - start + 1)}s",
+                    f"kubectl logs {namespace_to_kubectl(namespace)} {get_runner_pod(namespace)} -c runner --since={int(time.time() - start + 1)}s",
                     shell=True,
                 )
-        except:
+        except Exception:
             log_title("Cannot fetch logs. robusta-runner not found", color="red")
             return
 
 
 def get_package_name(playbooks_dir: str) -> str:
     with open(os.path.join(playbooks_dir, "pyproject.toml"), "r") as pyproj_toml:
         data = pyproj_toml.read()
         parsed = toml.loads(data)
         return get(parsed, "tool/poetry/name", default="")
+
+
+def get_runner_pod(namespace: Optional[str]) -> str:
+    output = subprocess.run(
+        f"kubectl get pods {namespace_to_kubectl(namespace)} "
+        f'--selector="robustaComponent=runner" '
+        f"--field-selector=status.phase==Running "
+        f"--no-headers "
+        f'-o custom-columns=":metadata.name"',
+        shell=True,
+        text=True,
+        capture_output=True,
+    ).stdout.strip()
+
+    if not output:
+        typer.secho(
+            f"Could not find robusta pod in namespace {namespace}. Are you missing the --namespace flag correctly?",
+            fg="red",
+        )
+
+    return output
```


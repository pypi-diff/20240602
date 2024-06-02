# Comparing `tmp/pyroblack-2.3.71.tar.gz` & `tmp/pyroblack-2.3.72.tar.gz`

## Comparing `pyroblack-2.3.71.tar` & `pyroblack-2.3.72.tar`

### file list

```diff
@@ -1,586 +1,586 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyroblack-2.3.71/MANIFEST.in
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyroblack-2.3.71/Makefile
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pyroblack-2.3.71/build-docs.sh
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/__init__.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/api/__init__.py
--rw-r--r--   0        0        0    23145 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/api/compiler.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/api/source/auth_key.tl
--rw-r--r--   0        0        0   210861 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/api/source/main_api.tl
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/api/source/sys_msgs.tl
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/api/template/combinator.txt
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/api/template/type.txt
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/__init__.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/compiler.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/sort.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0        0        0    29324 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/template/class.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyroblack-2.3.71/compiler/errors/template/sub_class.txt
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/__init__.py
--rw-r--r--   0        0        0    48685 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/client.py
--rw-r--r--   0        0        0    19150 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   209155 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/emoji.py
--rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/file_id.py
--rw-r--r--   0        0        0    28954 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/filters.py
--rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/mime_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/py.typed
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/sync.py
--rw-r--r--   0        0        0    17418 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/utils.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/business_schedule.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/client_platform.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/listerner_types.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/profile_color.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/reaction_type.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/reply_color.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/stories_privacy_rules.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/story_privacy.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/errors/pyromod/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/errors/pyromod/listener_stopped.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/errors/pyromod/listener_timeout.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/bot_business_connect_handler.py
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/bot_business_message_handler.py
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/conversation_handler.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/deleted_bot_business_messages_handler.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/edited_bot_business_message_handler.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/pre_checkout_query_handler.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/story_handler.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/helpers/__init__.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/helpers/helpers.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/answer_pre_checkout_query.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/get_bot_info.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/get_collectible_item_info.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/set_bot_info.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/join_folder.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/leave_folder.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0    10011 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/toggle_folder_tags.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/toggle_forum_topics.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/toggle_join_to_send.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/chats/update_color.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_bot_business_connect.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_bot_business_message.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_deleted_bot_business_messages.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_edited_bot_business_message.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_pre_checkout_query.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_story.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    13345 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_available_effects.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_scheduled_messages.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/get_stickers.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/send_web_page.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/view_messages.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/payments/__init__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/payments/check_giftcode.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/phone/__init__.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/phone/get_call_members.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/__init__.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/ask.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/get_listener_matching_with_data.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/listen.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/register_next_step_handler.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/remove_listerner.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/stop_listener.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/stop_listening.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/wait_for_callback_query.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/pyromod/wait_for_message.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/stickers/get_sticker_set.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/check_username.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/delete_stories.py
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/edit_story.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/export_story_link.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/forward_story.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_all_stories.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_peer_stories.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_stories.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_stories_history.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/send_story.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/update_birthday.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/update_personal_chat.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/run.py
--rwxr-xr-x   0        0        0     1592 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/run_sync.py
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/nav/__init__.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/nav/pagination.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/parser/html.py
--rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/parser/utils.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/auth.py
--rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/session.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/list.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/object.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/update.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_business_connection.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_info.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    12925 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/collectible_item_info.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/inline_keyboard_button_buy.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/payment_info.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/pre_checkout_query.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/request_peer_type_user.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/requested_chats.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/shipping_address.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/successful_payment.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media_area.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media_area_channel_post.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_message_content/input_reply_to_message.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_message_content/input_reply_to_story.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/available_effect.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/checked_gift_code.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/exported_story_link.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/giveaway_launched.py
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/giveaway_result.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/media_area.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/media_area_channel_post.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/media_area_coordinates.py
--rw-r--r--   0        0        0   217568 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/message_invoice.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/message_story.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/reaction_count.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/reaction_type.py
--rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/stories_privacy_rules.py
--rw-r--r--   0        0        0    76319 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/story_deleted.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/story_forward_header.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/story_skipped.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/story_views.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/web_page_empty.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/messages_and_media/web_page_preview.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/pyromod/__init__.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/pyromod/identifier.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/pyromod/listener.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/birthday.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/business_info.py
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/business_message.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/business_recipients.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/business_weekly_open.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/business_working_hours.py
--rw-r--r--   0        0        0    44237 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0        0        0    22989 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0    10248 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/group_call_member.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pyroblack-2.3.71/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyroblack-2.3.71/COPYING
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyroblack-2.3.71/COPYING.lesser
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pyroblack-2.3.71/NOTICE
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.71/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pyroblack-2.3.71/hatch_build.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pyroblack-2.3.71/pyproject.toml
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 pyroblack-2.3.71/PKG-INFO
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyroblack-2.3.72/MANIFEST.in
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyroblack-2.3.72/Makefile
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pyroblack-2.3.72/build-docs.sh
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/api/__init__.py
+-rw-r--r--   0        0        0    23145 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/api/compiler.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/api/source/auth_key.tl
+-rw-r--r--   0        0        0   210861 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/api/source/main_api.tl
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/api/source/sys_msgs.tl
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/api/template/combinator.txt
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/api/template/type.txt
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/__init__.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/compiler.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/sort.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0        0        0    29324 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/template/class.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyroblack-2.3.72/compiler/errors/template/sub_class.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/__init__.py
+-rw-r--r--   0        0        0    48685 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/client.py
+-rw-r--r--   0        0        0    19150 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   209155 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/emoji.py
+-rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/file_id.py
+-rw-r--r--   0        0        0    28954 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/filters.py
+-rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/mime_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/py.typed
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/sync.py
+-rw-r--r--   0        0        0    17418 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/utils.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/business_schedule.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/client_platform.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/listerner_types.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/profile_color.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/reaction_type.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/reply_color.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/stories_privacy_rules.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/story_privacy.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/errors/pyromod/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/errors/pyromod/listener_stopped.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/errors/pyromod/listener_timeout.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/bot_business_connect_handler.py
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/bot_business_message_handler.py
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/conversation_handler.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/deleted_bot_business_messages_handler.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/edited_bot_business_message_handler.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/pre_checkout_query_handler.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/story_handler.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/helpers/__init__.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/helpers/helpers.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/answer_pre_checkout_query.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/get_bot_info.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/get_collectible_item_info.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/set_bot_info.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/join_folder.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/leave_folder.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0    10011 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/toggle_folder_tags.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/toggle_forum_topics.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/toggle_join_to_send.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/chats/update_color.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_bot_business_connect.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_bot_business_message.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_deleted_bot_business_messages.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_edited_bot_business_message.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_pre_checkout_query.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_story.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    13345 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_available_effects.py
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_scheduled_messages.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/get_stickers.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/send_web_page.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/view_messages.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/payments/__init__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/payments/check_giftcode.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/phone/__init__.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/phone/get_call_members.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/__init__.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/ask.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/get_listener_matching_with_data.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/listen.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/register_next_step_handler.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/remove_listerner.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/stop_listener.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/stop_listening.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/wait_for_callback_query.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/pyromod/wait_for_message.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/stickers/get_sticker_set.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/check_username.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/delete_stories.py
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/edit_story.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/export_story_link.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/forward_story.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_all_stories.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_peer_stories.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_stories.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_stories_history.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/send_story.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/update_birthday.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/update_personal_chat.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/run.py
+-rwxr-xr-x   0        0        0     1592 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/run_sync.py
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/nav/__init__.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/nav/pagination.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/auth.py
+-rw-r--r--   0        0        0    15767 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/session.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/list.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/update.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_business_connection.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_info.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    12925 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/collectible_item_info.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/inline_keyboard_button_buy.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/payment_info.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/pre_checkout_query.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/request_peer_type_user.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/requested_chats.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/shipping_address.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/successful_payment.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media_area.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media_area_channel_post.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_message_content/input_reply_to_message.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_message_content/input_reply_to_story.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/available_effect.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/checked_gift_code.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/exported_story_link.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/giveaway_launched.py
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/giveaway_result.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/media_area.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/media_area_channel_post.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/media_area_coordinates.py
+-rw-r--r--   0        0        0   217568 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/message_invoice.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/message_story.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/reaction_count.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/reaction_type.py
+-rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/stories_privacy_rules.py
+-rw-r--r--   0        0        0    76319 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/story_deleted.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/story_forward_header.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/story_skipped.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/story_views.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/web_page_empty.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/messages_and_media/web_page_preview.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/pyromod/__init__.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/pyromod/identifier.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/pyromod/listener.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/birthday.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/business_info.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/business_message.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/business_recipients.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/business_weekly_open.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/business_working_hours.py
+-rw-r--r--   0        0        0    44237 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0        0        0    22989 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0    10248 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/group_call_member.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pyroblack-2.3.72/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyroblack-2.3.72/COPYING
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyroblack-2.3.72/COPYING.lesser
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pyroblack-2.3.72/NOTICE
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.72/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pyroblack-2.3.72/hatch_build.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pyroblack-2.3.72/pyproject.toml
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 pyroblack-2.3.72/PKG-INFO
```

### Comparing `pyroblack-2.3.71/Makefile` & `pyroblack-2.3.72/Makefile`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/build-docs.sh` & `pyroblack-2.3.72/build-docs.sh`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/__init__.py` & `pyroblack-2.3.72/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/api/__init__.py` & `pyroblack-2.3.72/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/api/compiler.py` & `pyroblack-2.3.72/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/api/source/auth_key.tl` & `pyroblack-2.3.72/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/api/source/main_api.tl` & `pyroblack-2.3.72/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/api/source/sys_msgs.tl` & `pyroblack-2.3.72/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/api/template/combinator.txt` & `pyroblack-2.3.72/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/api/template/type.txt` & `pyroblack-2.3.72/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/__init__.py` & `pyroblack-2.3.72/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/compiler.py` & `pyroblack-2.3.72/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/sort.py` & `pyroblack-2.3.72/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyroblack-2.3.72/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyroblack-2.3.72/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/source/403_FORBIDDEN.tsv` & `pyroblack-2.3.72/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyroblack-2.3.72/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/source/420_FLOOD.tsv` & `pyroblack-2.3.72/compiler/errors/source/420_FLOOD.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyroblack-2.3.72/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/__init__.py` & `pyroblack-2.3.72/pyrogram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with pyroblack.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "pyroblack"
-__version__ = "2.3.71"
+__version__ = "2.3.72"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "#  Copyright (C) 2024-present eyMarv <https://github.com/eyMarv>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyroblack-2.3.71/pyrogram/client.py` & `pyroblack-2.3.72/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/dispatcher.py` & `pyroblack-2.3.72/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/emoji.py` & `pyroblack-2.3.72/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/file_id.py` & `pyroblack-2.3.72/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/filters.py` & `pyroblack-2.3.72/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/mime_types.py` & `pyroblack-2.3.72/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/sync.py` & `pyroblack-2.3.72/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/utils.py` & `pyroblack-2.3.72/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/__init__.py` & `pyroblack-2.3.72/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/connection.py` & `pyroblack-2.3.72/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/__init__.py` & `pyroblack-2.3.72/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/tcp/__init__.py` & `pyroblack-2.3.72/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp.py` & `pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_full.py` & `pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyroblack-2.3.72/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/crypto/__init__.py` & `pyroblack-2.3.72/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/crypto/aes.py` & `pyroblack-2.3.72/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/crypto/mtproto.py` & `pyroblack-2.3.72/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/crypto/prime.py` & `pyroblack-2.3.72/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/crypto/rsa.py` & `pyroblack-2.3.72/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/__init__.py` & `pyroblack-2.3.72/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/auto_name.py` & `pyroblack-2.3.72/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/business_schedule.py` & `pyroblack-2.3.72/pyrogram/enums/business_schedule.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/chat_action.py` & `pyroblack-2.3.72/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/chat_event_action.py` & `pyroblack-2.3.72/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/chat_member_status.py` & `pyroblack-2.3.72/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/chat_members_filter.py` & `pyroblack-2.3.72/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/chat_type.py` & `pyroblack-2.3.72/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/client_platform.py` & `pyroblack-2.3.72/pyrogram/enums/client_platform.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/listerner_types.py` & `pyroblack-2.3.72/pyrogram/enums/listerner_types.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/message_entity_type.py` & `pyroblack-2.3.72/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/message_media_type.py` & `pyroblack-2.3.72/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/message_service_type.py` & `pyroblack-2.3.72/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/messages_filter.py` & `pyroblack-2.3.72/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/next_code_type.py` & `pyroblack-2.3.72/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/parse_mode.py` & `pyroblack-2.3.72/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/poll_type.py` & `pyroblack-2.3.72/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/profile_color.py` & `pyroblack-2.3.72/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/reaction_type.py` & `pyroblack-2.3.72/pyrogram/enums/reaction_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/reply_color.py` & `pyroblack-2.3.72/pyrogram/enums/reply_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/sent_code_type.py` & `pyroblack-2.3.72/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/stories_privacy_rules.py` & `pyroblack-2.3.72/pyrogram/enums/stories_privacy_rules.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/story_privacy.py` & `pyroblack-2.3.72/pyrogram/enums/story_privacy.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/enums/user_status.py` & `pyroblack-2.3.72/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/errors/__init__.py` & `pyroblack-2.3.72/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/errors/rpc_error.py` & `pyroblack-2.3.72/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/__init__.py` & `pyroblack-2.3.72/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/bot_business_connect_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/bot_business_connect_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/bot_business_message_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/bot_business_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/callback_query_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/chat_join_request_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/chat_member_updated_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/chosen_inline_result_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/conversation_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/deleted_bot_business_messages_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/deleted_bot_business_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/deleted_messages_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/disconnect_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/edited_bot_business_message_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/edited_bot_business_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/edited_message_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/handler.py` & `pyroblack-2.3.72/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/inline_query_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/message_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/message_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,26 +59,29 @@
         Checks if the message has a matching listener.
 
         :param client: The Client object to check with.
         :param message: The Message object to check with.
         :return: A tuple of whether the message has a matching listener and its filters does match with the Message
         and the matching listener;
         """
+        chat = message.chat
+        chat_id = chat.id if chat else None
+        chat_username = chat.username if chat else None
         from_user = message.from_user
         from_user_id = from_user.id if from_user else None
         from_user_username = from_user.username if from_user else None
 
         message_id = getattr(message, "id", getattr(message, "message_id", None))
 
         if not message.chat:
             return False, None
 
         data = Identifier(
             message_id=message_id,
-            chat_id=[message.chat.id, message.chat.username],
+            chat_id=[chat_id, chat_username],
             from_user_id=[from_user_id, from_user_username],
         )
 
         listener = client.get_listener_matching_with_data(
             data, pyrogram.enums.ListenerTypes.MESSAGE
         )
 
@@ -103,18 +106,16 @@
         Checks if the message has a matching listener or handler and its filters does match with the Message.
 
         :param client: Client object to check with.
         :param message: Message object to check with.
         :return: Whether the message has a matching listener or handler and its filters does match with the Message.
         """
         listener_does_match = (
-            (await self.check_if_has_matching_listener(client, message))[0]
-            if message.chat is not None and message.from_user is not None
-            else False
-        )
+            await self.check_if_has_matching_listener(client, message)
+        )[0]
 
         if callable(self.filters):
             if iscoroutinefunction(self.filters.__call__):
                 handler_does_match = await self.filters(client, message)
             else:
                 handler_does_match = await client.loop.run_in_executor(
                     None, self.filters, client, message
@@ -133,19 +134,17 @@
         Resolves the future or calls the callback of the listener if the message has a matching listener.
 
         :param client: Client object to resolve or call with.
         :param message: Message object to resolve or call with.
         :param args: Arguments to call the callback with.
         :return: None
         """
-        listener_does_match, listener = (
-            await self.check_if_has_matching_listener(client, message)
-            if message.chat is not None and message.from_user is not None
-            else False
-        ), None
+        listener_does_match, listener = await self.check_if_has_matching_listener(
+            client, message
+        )
 
         if listener and listener_does_match:
             client.remove_listener(listener)
 
             if listener.future and not listener.future.done():
                 listener.future.set_result(message)
```

### Comparing `pyroblack-2.3.71/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/message_reaction_updated_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/poll_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/pre_checkout_query_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/pre_checkout_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/raw_update_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/story_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/story_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/handlers/user_status_handler.py` & `pyroblack-2.3.72/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/helpers/__init__.py` & `pyroblack-2.3.72/pyrogram/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/helpers/helpers.py` & `pyroblack-2.3.72/pyrogram/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/advanced/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/advanced/invoke.py` & `pyroblack-2.3.72/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/advanced/resolve_peer.py` & `pyroblack-2.3.72/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/advanced/save_file.py` & `pyroblack-2.3.72/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/accept_terms_of_service.py` & `pyroblack-2.3.72/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/check_password.py` & `pyroblack-2.3.72/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/connect.py` & `pyroblack-2.3.72/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/disconnect.py` & `pyroblack-2.3.72/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/get_password_hint.py` & `pyroblack-2.3.72/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/initialize.py` & `pyroblack-2.3.72/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/log_out.py` & `pyroblack-2.3.72/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/recover_password.py` & `pyroblack-2.3.72/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/resend_code.py` & `pyroblack-2.3.72/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/send_code.py` & `pyroblack-2.3.72/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/send_recovery_code.py` & `pyroblack-2.3.72/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/sign_in.py` & `pyroblack-2.3.72/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/sign_in_bot.py` & `pyroblack-2.3.72/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/sign_up.py` & `pyroblack-2.3.72/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/auth/terminate.py` & `pyroblack-2.3.72/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/answer_callback_query.py` & `pyroblack-2.3.72/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/answer_inline_query.py` & `pyroblack-2.3.72/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/answer_pre_checkout_query.py` & `pyroblack-2.3.72/pyrogram/methods/bots/answer_pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/answer_web_app_query.py` & `pyroblack-2.3.72/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/delete_bot_commands.py` & `pyroblack-2.3.72/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/get_bot_commands.py` & `pyroblack-2.3.72/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyroblack-2.3.72/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/get_bot_info.py` & `pyroblack-2.3.72/pyrogram/methods/bots/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/get_chat_menu_button.py` & `pyroblack-2.3.72/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/get_collectible_item_info.py` & `pyroblack-2.3.72/pyrogram/methods/bots/get_collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/get_game_high_scores.py` & `pyroblack-2.3.72/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/get_inline_bot_results.py` & `pyroblack-2.3.72/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/request_callback_answer.py` & `pyroblack-2.3.72/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/send_game.py` & `pyroblack-2.3.72/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/send_inline_bot_result.py` & `pyroblack-2.3.72/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/set_bot_commands.py` & `pyroblack-2.3.72/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyroblack-2.3.72/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/set_bot_info.py` & `pyroblack-2.3.72/pyrogram/methods/bots/set_bot_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/set_chat_menu_button.py` & `pyroblack-2.3.72/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/bots/set_game_score.py` & `pyroblack-2.3.72/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/add_chat_members.py` & `pyroblack-2.3.72/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/archive_chats.py` & `pyroblack-2.3.72/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/ban_chat_member.py` & `pyroblack-2.3.72/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/close_forum_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/close_general_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/create_channel.py` & `pyroblack-2.3.72/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/create_forum_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/create_group.py` & `pyroblack-2.3.72/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/create_supergroup.py` & `pyroblack-2.3.72/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/delete_channel.py` & `pyroblack-2.3.72/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/delete_chat_photo.py` & `pyroblack-2.3.72/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/delete_forum_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/delete_supergroup.py` & `pyroblack-2.3.72/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/delete_user_history.py` & `pyroblack-2.3.72/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/edit_forum_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/edit_general_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_chat.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_chat_event_log.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_chat_member.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_chat_members.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_chat_members_count.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_chat_online_count.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_dialogs.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_dialogs_count.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_forum_topics.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_forum_topics_by_id.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_nearby_chats.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/get_send_as_chats.py` & `pyroblack-2.3.72/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/hide_general_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/join_chat.py` & `pyroblack-2.3.72/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/join_folder.py` & `pyroblack-2.3.72/pyrogram/methods/chats/join_folder.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/leave_chat.py` & `pyroblack-2.3.72/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/leave_folder.py` & `pyroblack-2.3.72/pyrogram/methods/chats/leave_folder.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/mark_chat_unread.py` & `pyroblack-2.3.72/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/pin_chat_message.py` & `pyroblack-2.3.72/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/promote_chat_member.py` & `pyroblack-2.3.72/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/reopen_forum_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/reopen_general_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/restrict_chat_member.py` & `pyroblack-2.3.72/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_administrator_title.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_chat_description.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_chat_permissions.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_chat_photo.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_chat_protected_content.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_chat_title.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_chat_username.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_send_as_chat.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/set_slow_mode.py` & `pyroblack-2.3.72/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/toggle_folder_tags.py` & `pyroblack-2.3.72/pyrogram/methods/chats/toggle_folder_tags.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/toggle_forum_topics.py` & `pyroblack-2.3.72/pyrogram/methods/chats/toggle_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/toggle_join_to_send.py` & `pyroblack-2.3.72/pyrogram/methods/chats/toggle_join_to_send.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/unarchive_chats.py` & `pyroblack-2.3.72/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/unban_chat_member.py` & `pyroblack-2.3.72/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/unhide_general_topic.py` & `pyroblack-2.3.72/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyroblack-2.3.72/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/unpin_chat_message.py` & `pyroblack-2.3.72/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/chats/update_color.py` & `pyroblack-2.3.72/pyrogram/methods/chats/update_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/contacts/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/contacts/add_contact.py` & `pyroblack-2.3.72/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/contacts/delete_contacts.py` & `pyroblack-2.3.72/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/contacts/get_contacts.py` & `pyroblack-2.3.72/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/contacts/get_contacts_count.py` & `pyroblack-2.3.72/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/contacts/import_contacts.py` & `pyroblack-2.3.72/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_bot_business_connect.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_bot_business_connect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_bot_business_message.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_bot_business_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_callback_query.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_chat_join_request.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_deleted_bot_business_messages.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_deleted_bot_business_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_deleted_messages.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_disconnect.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_edited_bot_business_message.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_edited_bot_business_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_edited_message.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_inline_query.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_message.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_poll.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_pre_checkout_query.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_raw_update.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_story.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/decorators/on_user_status.py` & `pyroblack-2.3.72/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyroblack-2.3.72/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/copy_media_group.py` & `pyroblack-2.3.72/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/copy_message.py` & `pyroblack-2.3.72/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/delete_messages.py` & `pyroblack-2.3.72/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/download_media.py` & `pyroblack-2.3.72/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_caption.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_media.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_inline_text.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_message_caption.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_message_media.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/edit_message_text.py` & `pyroblack-2.3.72/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/forward_messages.py` & `pyroblack-2.3.72/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_available_effects.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_available_effects.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_chat_history.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_chat_history_count.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_discussion_message.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_discussion_replies.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_media_group.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_messages.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_scheduled_messages.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_scheduled_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/get_stickers.py` & `pyroblack-2.3.72/pyrogram/methods/messages/get_stickers.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/inline_session.py` & `pyroblack-2.3.72/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/read_chat_history.py` & `pyroblack-2.3.72/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/retract_vote.py` & `pyroblack-2.3.72/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/search_global.py` & `pyroblack-2.3.72/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/search_global_count.py` & `pyroblack-2.3.72/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/search_messages.py` & `pyroblack-2.3.72/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/search_messages_count.py` & `pyroblack-2.3.72/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_animation.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_audio.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_cached_media.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_chat_action.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_contact.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_dice.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_document.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_location.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_media_group.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_message.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_photo.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_poll.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_reaction.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_sticker.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_venue.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_video.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_video_note.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_voice.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/send_web_page.py` & `pyroblack-2.3.72/pyrogram/methods/messages/send_web_page.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/stop_poll.py` & `pyroblack-2.3.72/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/stream_media.py` & `pyroblack-2.3.72/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/view_messages.py` & `pyroblack-2.3.72/pyrogram/methods/messages/view_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/messages/vote_poll.py` & `pyroblack-2.3.72/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/password/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/password/change_cloud_password.py` & `pyroblack-2.3.72/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/password/enable_cloud_password.py` & `pyroblack-2.3.72/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/password/remove_cloud_password.py` & `pyroblack-2.3.72/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/payments/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/payments/check_giftcode.py` & `pyroblack-2.3.72/pyrogram/methods/payments/check_giftcode.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/phone/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/phone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/phone/get_call_members.py` & `pyroblack-2.3.72/pyrogram/methods/phone/get_call_members.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/ask.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/ask.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/get_listener_matching_with_data.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/get_listener_matching_with_data.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/listen.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/listen.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/register_next_step_handler.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/register_next_step_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/remove_listerner.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/remove_listerner.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/stop_listener.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/stop_listener.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/stop_listening.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/stop_listening.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/wait_for_callback_query.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/pyromod/wait_for_message.py` & `pyroblack-2.3.72/pyrogram/methods/pyromod/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/stickers/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/stickers/add_sticker_to_set.py` & `pyroblack-2.3.72/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/stickers/create_sticker_set.py` & `pyroblack-2.3.72/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/stickers/get_sticker_set.py` & `pyroblack-2.3.72/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/block_user.py` & `pyroblack-2.3.72/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/check_username.py` & `pyroblack-2.3.72/pyrogram/methods/users/check_username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/delete_profile_photos.py` & `pyroblack-2.3.72/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/delete_stories.py` & `pyroblack-2.3.72/pyrogram/methods/users/delete_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/edit_story.py` & `pyroblack-2.3.72/pyrogram/methods/users/edit_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/export_story_link.py` & `pyroblack-2.3.72/pyrogram/methods/users/export_story_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/forward_story.py` & `pyroblack-2.3.72/pyrogram/methods/users/forward_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_all_stories.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_all_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_chat_photos.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_chat_photos_count.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_common_chats.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_me.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_peer_stories.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_peer_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_stories.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_stories_history.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_stories_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/get_users.py` & `pyroblack-2.3.72/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/send_story.py` & `pyroblack-2.3.72/pyrogram/methods/users/send_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/set_emoji_status.py` & `pyroblack-2.3.72/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/set_profile_photo.py` & `pyroblack-2.3.72/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/set_username.py` & `pyroblack-2.3.72/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/unblock_user.py` & `pyroblack-2.3.72/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/update_birthday.py` & `pyroblack-2.3.72/pyrogram/methods/users/update_birthday.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/update_personal_chat.py` & `pyroblack-2.3.72/pyrogram/methods/users/update_personal_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/users/update_profile.py` & `pyroblack-2.3.72/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/__init__.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/add_handler.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/compose.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/export_session_string.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/idle.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/remove_handler.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/restart.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/run.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/run_sync.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/run_sync.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/start.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/stop.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/methods/utilities/stop_transmission.py` & `pyroblack-2.3.72/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/nav/__init__.py` & `pyroblack-2.3.72/pyrogram/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/nav/pagination.py` & `pyroblack-2.3.72/pyrogram/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/parser/__init__.py` & `pyroblack-2.3.72/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/parser/html.py` & `pyroblack-2.3.72/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/parser/markdown.py` & `pyroblack-2.3.72/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/parser/parser.py` & `pyroblack-2.3.72/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/parser/utils.py` & `pyroblack-2.3.72/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/__init__.py` & `pyroblack-2.3.72/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/__init__.py` & `pyroblack-2.3.72/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/future_salt.py` & `pyroblack-2.3.72/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/future_salts.py` & `pyroblack-2.3.72/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/gzip_packed.py` & `pyroblack-2.3.72/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/list.py` & `pyroblack-2.3.72/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/message.py` & `pyroblack-2.3.72/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/msg_container.py` & `pyroblack-2.3.72/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/tl_object.py` & `pyroblack-2.3.72/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/primitives/__init__.py` & `pyroblack-2.3.72/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/primitives/bool.py` & `pyroblack-2.3.72/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/primitives/bytes.py` & `pyroblack-2.3.72/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/primitives/double.py` & `pyroblack-2.3.72/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/primitives/int.py` & `pyroblack-2.3.72/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/primitives/string.py` & `pyroblack-2.3.72/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/raw/core/primitives/vector.py` & `pyroblack-2.3.72/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/session/__init__.py` & `pyroblack-2.3.72/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/session/auth.py` & `pyroblack-2.3.72/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/session/session.py` & `pyroblack-2.3.72/pyrogram/session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with pyroblack.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 import bisect
 import logging
 import os
+from datetime import datetime, timedelta
 from hashlib import sha1
 from io import BytesIO
 
 from pyrogram.raw.all import layer
 
 import pyrogram
 from pyrogram import raw
@@ -56,15 +57,16 @@
 class Session:
     START_TIMEOUT = 2
     WAIT_TIMEOUT = 15
     SLEEP_THRESHOLD = 10
     MAX_RETRIES = 10
     ACKS_THRESHOLD = 10
     PING_INTERVAL = 5
-    STORED_MSG_IDS_MAX_SIZE = 500
+    STORED_MSG_IDS_MAX_SIZE = 1000 * 2
+    RECONNECT_THRESHOLD = timedelta(seconds=10)
 
     TRANSPORT_ERRORS = {
         404: "auth key not found",
         429: "transport flood",
         444: "invalid DC",
     }
 
@@ -104,14 +106,16 @@
 
         self.recv_task = None
 
         self.is_started = asyncio.Event()
 
         self.loop = asyncio.get_event_loop()
 
+        self.last_reconnect_attempt = None
+
     async def start(self):
         while True:
             self.connection = Connection(
                 self.dc_id,
                 self.test_mode,
                 self.client.ipv6,
                 self.client.alt_port,
@@ -193,14 +197,23 @@
                 await self.client.disconnect_handler(self.client)
             except Exception as e:
                 log.exception(e)
 
         log.info("Session stopped")
 
     async def restart(self):
+        now = datetime.now()
+        if (
+            self.last_reconnect_attempt
+            and now - self.last_reconnect_attempt < self.RECONNECT_THRESHOLD
+        ):
+            log.info("Reconnecting too frequently, sleeping for a while")
+            await asyncio.sleep(5)
+
+        self.last_reconnect_attempt = now
         await self.stop()
         await self.start()
 
     async def handle_packet(self, packet):
         data = await self.loop.run_in_executor(
             pyrogram.crypto_executor,
             mtproto.unpack,
@@ -441,15 +454,15 @@
         ):
             inner_query = query.query
         else:
             inner_query = query
 
         query_name = ".".join(inner_query.QUALNAME.split(".")[1:])
 
-        while True:
+        while retries > 0:
             try:
                 return await self.send(query, timeout=timeout)
             except (FloodWait, FloodPremiumWait) as e:
                 amount = e.value
 
                 if amount > sleep_threshold >= 0:
                     raise
@@ -459,24 +472,25 @@
                     self.client.name,
                     amount,
                     query_name,
                 )
 
                 await asyncio.sleep(amount)
             except (OSError, InternalServerError, ServiceUnavailable) as e:
+                retries -= 1
                 if retries == 0:
                     self.client.updates_invoke_error = e
-                    raise e from None
+                    raise e
 
                 (log.warning if retries < 2 else log.info)(
                     '[%s] Retrying "%s" due to: %s',
-                    Session.MAX_RETRIES - retries + 1,
+                    Session.MAX_RETRIES - retries,
                     query_name,
                     str(e) or repr(e),
                 )
 
                 await asyncio.sleep(0.5)
-
-                return await self.invoke(query, retries - 1, timeout)
             except Exception as e:
                 self.client.updates_invoke_error = e
                 raise
+
+        raise TimeoutError("Exceeded maximum number of retries")
```

### Comparing `pyroblack-2.3.71/pyrogram/session/internals/__init__.py` & `pyroblack-2.3.72/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/session/internals/data_center.py` & `pyroblack-2.3.72/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/session/internals/msg_factory.py` & `pyroblack-2.3.72/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/session/internals/msg_id.py` & `pyroblack-2.3.72/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/session/internals/seq_no.py` & `pyroblack-2.3.72/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/storage/__init__.py` & `pyroblack-2.3.72/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/storage/file_storage.py` & `pyroblack-2.3.72/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/storage/memory_storage.py` & `pyroblack-2.3.72/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/storage/sqlite_storage.py` & `pyroblack-2.3.72/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/storage/storage.py` & `pyroblack-2.3.72/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/__init__.py` & `pyroblack-2.3.72/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/list.py` & `pyroblack-2.3.72/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/object.py` & `pyroblack-2.3.72/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/update.py` & `pyroblack-2.3.72/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/authorization/__init__.py` & `pyroblack-2.3.72/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/authorization/sent_code.py` & `pyroblack-2.3.72/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/authorization/terms_of_service.py` & `pyroblack-2.3.72/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/__init__.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_business_connection.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_business_connection.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/bot_info.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/bot_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/collectible_item_info.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/inline_keyboard_button_buy.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/inline_keyboard_button_buy.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,22 @@
 
     Parameters:
         text (``str``):
             Text of the button. If none of the optional fields are used, it will be sent as a message when
             the button is pressed.
     """
 
-    def __init__(self, text: str):
+    def __init__(
+        self,
+        text: str
+    ):
         super().__init__()
 
         self.text = str(text)
 
     @staticmethod
     def read(b):
-        return InlineKeyboardButtonBuy(text=b.text)
+        return InlineKeyboardButtonBuy(
+            text=b.text
+        )
 
     # TODO: Implement write method
```

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,20 +28,15 @@
     """An inline keyboard that appears right next to the message it belongs to.
 
     Parameters:
         inline_keyboard (List of List of :obj:`~pyrogram.types.InlineKeyboardButton`):
             List of button rows, each represented by a List of InlineKeyboardButton objects.
     """
 
-    def __init__(
-        self,
-        inline_keyboard: List[
-            List[Union["types.InlineKeyboardButton", "types.InlineKeyboardButtonBuy"]]
-        ],
-    ):
+    def __init__(self, inline_keyboard: List[List[Union["types.InlineKeyboardButton", "types.InlineKeyboardButtonBuy"]]]):
         super().__init__()
 
         self.inline_keyboard = inline_keyboard
 
     @staticmethod
     def read(o):
         inline_keyboard = []
```

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/login_url.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/payment_info.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/payment_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/pre_checkout_query.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/request_peer_type_user.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/request_peer_type_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/requested_chats.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/requested_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/shipping_address.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/shipping_address.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/successful_payment.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/successful_payment.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyroblack-2.3.72/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/__init__.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyroblack-2.3.72/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/__init__.py` & `pyroblack-2.3.72/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media_animation.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media_area.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media_area.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media_area_channel_post.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media_area_channel_post.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media_audio.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media_document.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media_photo.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_media_video.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_media/input_phone_contact.py` & `pyroblack-2.3.72/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_message_content/__init__.py` & `pyroblack-2.3.72/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_message_content/input_message_content.py` & `pyroblack-2.3.72/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_message_content/input_reply_to_message.py` & `pyroblack-2.3.72/pyrogram/types/input_message_content/input_reply_to_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_message_content/input_reply_to_story.py` & `pyroblack-2.3.72/pyrogram/types/input_message_content/input_reply_to_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/input_message_content/input_text_message_content.py` & `pyroblack-2.3.72/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/__init__.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .media_area_coordinates import MediaAreaCoordinates
 from .message import Message
 from .message_entity import MessageEntity
 from .message_reaction_count_updated import MessageReactionCountUpdated
 from .message_reaction_updated import MessageReactionUpdated
 from .message_reactions import MessageReactions
 from .message_story import MessageStory
+from .message_invoice import MessageInvoice
 from .photo import Photo
 from .poll import Poll
 from .poll_option import PollOption
 from .reaction import Reaction
 from .reaction_count import ReactionCount
 from .reaction_type import ReactionType
 from .sticker import Sticker
```

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/animation.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/audio.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/available_effect.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/available_effect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/checked_gift_code.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/checked_gift_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/contact.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/dice.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/document.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/exported_story_link.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/exported_story_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/game.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/gift_code.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/gift_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/giveaway.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/giveaway_launched.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/giveaway_launched.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/giveaway_result.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/giveaway_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/location.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/media_area.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/media_area.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/media_area_channel_post.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/media_area_channel_post.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/media_area_coordinates.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/media_area_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/message.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/message_entity.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/message_invoice.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/message_invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             The message_id of the message sent to the chat when the invoice is paid.
     """
 
     def __init__(
         self,
         *,
         title: str,
-        description: str,
+        description :  str,
         currency: str,
         total_amount: int,
         start_parameter: str,
         shipping_address_requested: bool = None,
         test: bool = None,
         receipt_message_id: int = None,
         # TODO: Implement photo, extended_media parameters
@@ -72,18 +72,20 @@
         self.total_amount = total_amount
         self.start_parameter = start_parameter
         self.shipping_address_requested = shipping_address_requested
         self.test = test
         self.receipt_message_id = receipt_message_id
 
     @staticmethod
-    def _parse(message_invoice: "raw.types.MessageMediaInvoice") -> "MessageInvoice":
+    def _parse(
+        message_invoice: "raw.types.MessageMediaInvoice"
+    ) -> "MessageInvoice":
         return MessageInvoice(
             title=message_invoice.title,
             description=message_invoice.description,
             currency=message_invoice.currency,
             total_amount=message_invoice.total_amount,
             start_parameter=message_invoice.start_param,
             shipping_address_requested=message_invoice.shipping_address_requested,
             test=message_invoice.test,
-            receipt_message_id=message_invoice.receipt_msg_id,
+            receipt_message_id=message_invoice.receipt_msg_id
         )
```

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/message_reactions.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/message_story.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/message_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/photo.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/poll.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/poll_option.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/reaction.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/reaction_count.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/reaction_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/reaction_type.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/reaction_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/sticker.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/stickerset.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/stories_privacy_rules.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/stories_privacy_rules.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/story.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/story_deleted.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/story_deleted.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/story_forward_header.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/story_forward_header.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/story_skipped.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/story_skipped.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/story_views.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/story_views.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/thumbnail.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/venue.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/video.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/video_note.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/voice.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/web_app_data.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/web_page.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/web_page_empty.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/web_page_empty.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/messages_and_media/web_page_preview.py` & `pyroblack-2.3.72/pyrogram/types/messages_and_media/web_page_preview.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/pyromod/identifier.py` & `pyroblack-2.3.72/pyrogram/types/pyromod/identifier.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/pyromod/listener.py` & `pyroblack-2.3.72/pyrogram/types/pyromod/listener.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/__init__.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/birthday.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/birthday.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/business_info.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/business_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/business_message.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/business_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/business_recipients.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/business_recipients.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/business_weekly_open.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/business_weekly_open.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/business_working_hours.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/business_working_hours.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_color.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_event.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_join_request.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_joiner.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_member.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_permissions.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_photo.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_preview.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_privileges.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/chat_reactions.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/dialog.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/emoji_status.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_closed.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_created.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_edited.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/group_call_member.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/group_call_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/peer_channel.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/peer_user.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/restriction.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/user.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/username.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyrogram/types/user_and_chats/video_chat_started.py` & `pyroblack-2.3.72/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/.gitignore` & `pyroblack-2.3.72/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/COPYING` & `pyroblack-2.3.72/COPYING`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/COPYING.lesser` & `pyroblack-2.3.72/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/NOTICE` & `pyroblack-2.3.72/NOTICE`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/README.md` & `pyroblack-2.3.72/README.md`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/hatch_build.py` & `pyroblack-2.3.72/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/pyproject.toml` & `pyroblack-2.3.72/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.71/PKG-INFO` & `pyroblack-2.3.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyroblack
-Version: 2.3.71
+Version: 2.3.72
 Summary: Pyrogram, but black. Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Project-URL: Tracker, https://github.com/eyMarv/pyroblack/issues
 Project-URL: Community, https://t.me/OpenFileZ
 Project-URL: Source, https://github.com/eyMarv/pyroblack
 Project-URL: Documentation, https://eyMarv.github.io/pyroblack-docs
 Author-email: eyMarv <eyMarv07@gmail.com>
 License-Expression: LGPL-3.0-or-later
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pyroblack Version: 2.3.71 Summary: Pyrogram, but
+Metadata-Version: 2.3 Name: pyroblack Version: 2.3.72 Summary: Pyrogram, but
 black. Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Project-URL: Tracker, https://github.com/eyMarv/
 pyroblack/issues Project-URL: Community, https://t.me/OpenFileZ Project-URL:
 Source, https://github.com/eyMarv/pyroblack Project-URL: Documentation, https:/
 /eyMarv.github.io/pyroblack-docs Author-email: eyMarv
 gmail.com> License-Expression: LGPL-3.0-or-later License-File: COPYING License-
 File: COPYING.lesser License-File: NOTICE Keywords: black bsxcs telegram chat
```


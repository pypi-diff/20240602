# Comparing `tmp/aiotraq-0.1.1.tar.gz` & `tmp/aiotraq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotraq-0.1.1.tar", max compression
+gzip compressed data, was "aiotraq-0.1.2.tar", max compression
```

## Comparing `aiotraq-0.1.1.tar` & `aiotraq-0.1.2.tar`

### file list

```diff
@@ -1,323 +1,323 @@
--rw-r--r--   0        0        0     4247 2024-05-17 23:04:46.687845 aiotraq-0.1.1/README.md
--rw-r--r--   0        0        0      150 2024-05-15 23:06:18.975610 aiotraq-0.1.1/aiotraq/__init__.py
--rw-r--r--   0        0        0       45 2024-05-15 23:06:18.975906 aiotraq-0.1.1/aiotraq/api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.976100 aiotraq-0.1.1/aiotraq/api/activity/__init__.py
--rw-r--r--   0        0        0     6751 2024-05-15 23:06:18.976301 aiotraq-0.1.1/aiotraq/api/activity/get_activity_timeline.py
--rw-r--r--   0        0        0     3710 2024-05-15 23:06:18.976529 aiotraq-0.1.1/aiotraq/api/activity/get_online_users.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.976731 aiotraq-0.1.1/aiotraq/api/authentication/__init__.py
--rw-r--r--   0        0        0     4158 2024-05-15 23:06:18.976926 aiotraq-0.1.1/aiotraq/api/authentication/get_my_external_accounts.py
--rw-r--r--   0        0        0     3978 2024-05-15 23:06:18.977221 aiotraq-0.1.1/aiotraq/api/authentication/get_my_sessions.py
--rw-r--r--   0        0        0     3520 2024-05-15 23:06:18.977445 aiotraq-0.1.1/aiotraq/api/authentication/link_external_account.py
--rw-r--r--   0        0        0     3424 2024-05-15 23:06:18.977706 aiotraq-0.1.1/aiotraq/api/authentication/login.py
--rw-r--r--   0        0        0     3020 2024-05-15 23:06:18.977928 aiotraq-0.1.1/aiotraq/api/authentication/logout.py
--rw-r--r--   0        0        0     2775 2024-05-15 23:06:18.978115 aiotraq-0.1.1/aiotraq/api/authentication/revoke_my_session.py
--rw-r--r--   0        0        0     3149 2024-05-15 23:06:18.978287 aiotraq-0.1.1/aiotraq/api/authentication/unlink_external_account.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.978514 aiotraq-0.1.1/aiotraq/api/bot/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-15 23:06:18.978758 aiotraq-0.1.1/aiotraq/api/bot/activate_bot.py
--rw-r--r--   0        0        0     3371 2024-05-15 23:06:18.978975 aiotraq-0.1.1/aiotraq/api/bot/change_bot_icon.py
--rw-r--r--   0        0        0     5609 2024-05-15 23:06:18.979216 aiotraq-0.1.1/aiotraq/api/bot/connect_bot_ws.py
--rw-r--r--   0        0        0     5089 2024-05-15 23:06:18.979405 aiotraq-0.1.1/aiotraq/api/bot/create_bot.py
--rw-r--r--   0        0        0     2626 2024-05-15 23:06:18.979557 aiotraq-0.1.1/aiotraq/api/bot/delete_bot.py
--rw-r--r--   0        0        0     3499 2024-05-15 23:06:18.979724 aiotraq-0.1.1/aiotraq/api/bot/edit_bot.py
--rw-r--r--   0        0        0     5904 2024-05-15 23:06:18.979881 aiotraq-0.1.1/aiotraq/api/bot/get_bot.py
--rw-r--r--   0        0        0     4081 2024-05-15 23:06:18.980032 aiotraq-0.1.1/aiotraq/api/bot/get_bot_icon.py
--rw-r--r--   0        0        0     5835 2024-05-15 23:06:18.980192 aiotraq-0.1.1/aiotraq/api/bot/get_bot_logs.py
--rw-r--r--   0        0        0     4650 2024-05-15 23:06:18.980348 aiotraq-0.1.1/aiotraq/api/bot/get_bots.py
--rw-r--r--   0        0        0     4609 2024-05-15 23:06:18.980564 aiotraq-0.1.1/aiotraq/api/bot/get_channel_bots.py
--rw-r--r--   0        0        0     2681 2024-05-15 23:06:18.980721 aiotraq-0.1.1/aiotraq/api/bot/inactivate_bot.py
--rw-r--r--   0        0        0     3646 2024-05-15 23:06:18.980905 aiotraq-0.1.1/aiotraq/api/bot/let_bot_join_channel.py
--rw-r--r--   0        0        0     3416 2024-05-15 23:06:18.981054 aiotraq-0.1.1/aiotraq/api/bot/let_bot_leave_channel.py
--rw-r--r--   0        0        0     4558 2024-05-15 23:06:18.981216 aiotraq-0.1.1/aiotraq/api/bot/reissue_bot.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.981398 aiotraq-0.1.1/aiotraq/api/channel/__init__.py
--rw-r--r--   0        0        0     4974 2024-05-15 23:06:18.981566 aiotraq-0.1.1/aiotraq/api/channel/create_channel.py
--rw-r--r--   0        0        0     3685 2024-05-15 23:06:18.981725 aiotraq-0.1.1/aiotraq/api/channel/edit_channel.py
--rw-r--r--   0        0        0     3761 2024-05-15 23:06:18.981932 aiotraq-0.1.1/aiotraq/api/channel/edit_channel_subscribers.py
--rw-r--r--   0        0        0     3428 2024-05-15 23:06:18.982147 aiotraq-0.1.1/aiotraq/api/channel/edit_channel_topic.py
--rw-r--r--   0        0        0     4138 2024-05-15 23:06:18.982293 aiotraq-0.1.1/aiotraq/api/channel/get_channel.py
--rw-r--r--   0        0        0     9367 2024-05-17 02:20:00.184727 aiotraq-0.1.1/aiotraq/api/channel/get_channel_events.py
--rw-r--r--   0        0        0     4628 2024-05-15 23:06:18.982580 aiotraq-0.1.1/aiotraq/api/channel/get_channel_pins.py
--rw-r--r--   0        0        0     4258 2024-05-15 23:06:18.982767 aiotraq-0.1.1/aiotraq/api/channel/get_channel_stats.py
--rw-r--r--   0        0        0     4548 2024-05-15 23:06:18.982905 aiotraq-0.1.1/aiotraq/api/channel/get_channel_subscribers.py
--rw-r--r--   0        0        0     4258 2024-05-15 23:06:18.983060 aiotraq-0.1.1/aiotraq/api/channel/get_channel_topic.py
--rw-r--r--   0        0        0     4606 2024-05-15 23:06:18.983250 aiotraq-0.1.1/aiotraq/api/channel/get_channel_viewers.py
--rw-r--r--   0        0        0     4341 2024-05-15 23:06:18.983572 aiotraq-0.1.1/aiotraq/api/channel/get_channels.py
--rw-r--r--   0        0        0     9238 2024-05-15 23:06:18.983879 aiotraq-0.1.1/aiotraq/api/channel/get_messages.py
--rw-r--r--   0        0        0     3759 2024-05-15 23:06:18.984075 aiotraq-0.1.1/aiotraq/api/channel/set_channel_subscribers.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.984249 aiotraq-0.1.1/aiotraq/api/clip/__init__.py
--rw-r--r--   0        0        0     5531 2024-05-15 23:06:18.984424 aiotraq-0.1.1/aiotraq/api/clip/clip_message.py
--rw-r--r--   0        0        0     5001 2024-05-15 23:06:18.984633 aiotraq-0.1.1/aiotraq/api/clip/create_clip_folder.py
--rw-r--r--   0        0        0     2575 2024-05-15 23:06:18.984864 aiotraq-0.1.1/aiotraq/api/clip/delete_clip_folder.py
--rw-r--r--   0        0        0     3252 2024-05-15 23:06:18.985019 aiotraq-0.1.1/aiotraq/api/clip/edit_clip_folder.py
--rw-r--r--   0        0        0     4236 2024-05-15 23:06:18.985160 aiotraq-0.1.1/aiotraq/api/clip/get_clip_folder.py
--rw-r--r--   0        0        0     3947 2024-05-15 23:06:18.985361 aiotraq-0.1.1/aiotraq/api/clip/get_clip_folders.py
--rw-r--r--   0        0        0     7051 2024-05-15 23:06:18.985556 aiotraq-0.1.1/aiotraq/api/clip/get_clips.py
--rw-r--r--   0        0        0     3066 2024-05-15 23:06:18.985746 aiotraq-0.1.1/aiotraq/api/clip/unclip_message.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.985907 aiotraq-0.1.1/aiotraq/api/file/__init__.py
--rw-r--r--   0        0        0     2697 2024-05-15 23:06:18.986117 aiotraq-0.1.1/aiotraq/api/file/delete_file.py
--rw-r--r--   0        0        0     4993 2024-05-15 23:06:18.986291 aiotraq-0.1.1/aiotraq/api/file/get_file.py
--rw-r--r--   0        0        0     4504 2024-05-15 23:06:18.986590 aiotraq-0.1.1/aiotraq/api/file/get_file_meta.py
--rw-r--r--   0        0        0    10079 2024-05-15 23:06:18.986786 aiotraq-0.1.1/aiotraq/api/file/get_files.py
--rw-r--r--   0        0        0     5492 2024-05-15 23:06:18.987107 aiotraq-0.1.1/aiotraq/api/file/get_thumbnail_image.py
--rw-r--r--   0        0        0     5239 2024-05-15 23:06:18.987526 aiotraq-0.1.1/aiotraq/api/file/post_file.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.987769 aiotraq-0.1.1/aiotraq/api/group/__init__.py
--rw-r--r--   0        0        0     3381 2024-05-15 23:06:18.987948 aiotraq-0.1.1/aiotraq/api/group/add_user_group_admin.py
--rw-r--r--   0        0        0     3360 2024-05-15 23:06:18.988107 aiotraq-0.1.1/aiotraq/api/group/add_user_group_member.py
--rw-r--r--   0        0        0     3386 2024-05-15 23:06:18.988258 aiotraq-0.1.1/aiotraq/api/group/change_user_group_icon.py
--rw-r--r--   0        0        0     5114 2024-05-15 23:06:18.988423 aiotraq-0.1.1/aiotraq/api/group/create_user_group.py
--rw-r--r--   0        0        0     2780 2024-05-15 23:06:18.988603 aiotraq-0.1.1/aiotraq/api/group/delete_user_group.py
--rw-r--r--   0        0        0     3498 2024-05-15 23:06:18.988742 aiotraq-0.1.1/aiotraq/api/group/edit_user_group.py
--rw-r--r--   0        0        0     3692 2024-05-15 23:06:18.988946 aiotraq-0.1.1/aiotraq/api/group/edit_user_group_member.py
--rw-r--r--   0        0        0     4175 2024-05-15 23:06:18.989151 aiotraq-0.1.1/aiotraq/api/group/get_user_group.py
--rw-r--r--   0        0        0     4141 2024-05-15 23:06:18.989286 aiotraq-0.1.1/aiotraq/api/group/get_user_group_admins.py
--rw-r--r--   0        0        0     4559 2024-05-15 23:06:18.989550 aiotraq-0.1.1/aiotraq/api/group/get_user_group_members.py
--rw-r--r--   0        0        0     3844 2024-05-15 23:06:18.989822 aiotraq-0.1.1/aiotraq/api/group/get_user_groups.py
--rw-r--r--   0        0        0     3260 2024-05-15 23:06:18.990025 aiotraq-0.1.1/aiotraq/api/group/remove_user_group_admin.py
--rw-r--r--   0        0        0     3222 2024-05-15 23:06:18.990238 aiotraq-0.1.1/aiotraq/api/group/remove_user_group_member.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.990444 aiotraq-0.1.1/aiotraq/api/me/__init__.py
--rw-r--r--   0        0        0     3241 2024-05-15 23:06:18.990629 aiotraq-0.1.1/aiotraq/api/me/add_my_star.py
--rw-r--r--   0        0        0     4621 2024-05-15 23:06:18.990876 aiotraq-0.1.1/aiotraq/api/me/add_my_user_tag.py
--rw-r--r--   0        0        0     2948 2024-05-15 23:06:18.991013 aiotraq-0.1.1/aiotraq/api/me/change_my_icon.py
--rw-r--r--   0        0        0     3037 2024-05-15 23:06:18.991173 aiotraq-0.1.1/aiotraq/api/me/change_my_notify_citation.py
--rw-r--r--   0        0        0     2979 2024-05-15 23:06:18.991334 aiotraq-0.1.1/aiotraq/api/me/change_my_password.py
--rw-r--r--   0        0        0     2889 2024-05-15 23:06:18.991528 aiotraq-0.1.1/aiotraq/api/me/edit_me.py
--rw-r--r--   0        0        0     3553 2024-05-15 23:06:18.991848 aiotraq-0.1.1/aiotraq/api/me/get_me.py
--rw-r--r--   0        0        0     3978 2024-05-15 23:06:18.992061 aiotraq-0.1.1/aiotraq/api/me/get_my_channel_subscriptions.py
--rw-r--r--   0        0        0     3691 2024-05-15 23:06:18.992215 aiotraq-0.1.1/aiotraq/api/me/get_my_icon.py
--rw-r--r--   0        0        0     3751 2024-05-15 23:06:18.992421 aiotraq-0.1.1/aiotraq/api/me/get_my_notify_citation.py
--rw-r--r--   0        0        0     4455 2024-05-15 23:06:18.992664 aiotraq-0.1.1/aiotraq/api/me/get_my_qr_code.py
--rw-r--r--   0        0        0     3620 2024-05-15 23:06:18.992812 aiotraq-0.1.1/aiotraq/api/me/get_my_stars.py
--rw-r--r--   0        0        0     3917 2024-05-15 23:06:18.993008 aiotraq-0.1.1/aiotraq/api/me/get_my_unread_channels.py
--rw-r--r--   0        0        0     3813 2024-05-15 23:06:18.993174 aiotraq-0.1.1/aiotraq/api/me/get_my_user_tags.py
--rw-r--r--   0        0        0     4025 2024-05-15 23:06:18.993391 aiotraq-0.1.1/aiotraq/api/me/get_my_view_states.py
--rw-r--r--   0        0        0     3818 2024-05-15 23:06:18.993604 aiotraq-0.1.1/aiotraq/api/me/get_oidc_user_info.py
--rw-r--r--   0        0        0     3465 2024-05-15 23:06:18.993763 aiotraq-0.1.1/aiotraq/api/me/get_user_settings.py
--rw-r--r--   0        0        0     2515 2024-05-15 23:06:18.994114 aiotraq-0.1.1/aiotraq/api/me/read_channel.py
--rw-r--r--   0        0        0     2903 2024-05-15 23:06:18.994392 aiotraq-0.1.1/aiotraq/api/me/register_fcm_device.py
--rw-r--r--   0        0        0     2634 2024-05-15 23:06:18.994572 aiotraq-0.1.1/aiotraq/api/me/remove_my_star.py
--rw-r--r--   0        0        0     3425 2024-05-15 23:06:18.994746 aiotraq-0.1.1/aiotraq/api/me/set_channel_subscribe_level.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.994936 aiotraq-0.1.1/aiotraq/api/message/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-15 23:06:18.995089 aiotraq-0.1.1/aiotraq/api/message/add_message_stamp.py
--rw-r--r--   0        0        0     5062 2024-05-15 23:06:18.995279 aiotraq-0.1.1/aiotraq/api/message/create_pin.py
--rw-r--r--   0        0        0     3156 2024-05-15 23:06:18.995466 aiotraq-0.1.1/aiotraq/api/message/delete_message.py
--rw-r--r--   0        0        0     3590 2024-05-15 23:06:18.995658 aiotraq-0.1.1/aiotraq/api/message/edit_message.py
--rw-r--r--   0        0        0     9362 2024-05-15 23:06:18.995869 aiotraq-0.1.1/aiotraq/api/message/get_direct_messages.py
--rw-r--r--   0        0        0     4078 2024-05-15 23:06:18.996018 aiotraq-0.1.1/aiotraq/api/message/get_message.py
--rw-r--r--   0        0        0     4542 2024-05-15 23:06:18.996169 aiotraq-0.1.1/aiotraq/api/message/get_message_clips.py
--rw-r--r--   0        0        0     4700 2024-05-15 23:06:18.996337 aiotraq-0.1.1/aiotraq/api/message/get_message_stamps.py
--rw-r--r--   0        0        0     4194 2024-05-15 23:06:18.996494 aiotraq-0.1.1/aiotraq/api/message/get_pin.py
--rw-r--r--   0        0        0     5098 2024-05-15 23:06:18.996643 aiotraq-0.1.1/aiotraq/api/message/post_direct_message.py
--rw-r--r--   0        0        0     5867 2024-05-15 23:06:18.996780 aiotraq-0.1.1/aiotraq/api/message/post_message.py
--rw-r--r--   0        0        0     2812 2024-05-15 23:06:18.997010 aiotraq-0.1.1/aiotraq/api/message/remove_message_stamp.py
--rw-r--r--   0        0        0     2642 2024-05-15 23:06:18.997224 aiotraq-0.1.1/aiotraq/api/message/remove_pin.py
--rw-r--r--   0        0        0    12982 2024-05-15 23:06:18.997433 aiotraq-0.1.1/aiotraq/api/message/search_messages.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.997628 aiotraq-0.1.1/aiotraq/api/notification/__init__.py
--rw-r--r--   0        0        0    21754 2024-05-15 23:06:18.997903 aiotraq-0.1.1/aiotraq/api/notification/ws.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:18.998175 aiotraq-0.1.1/aiotraq/api/oauth2/__init__.py
--rw-r--r--   0        0        0     4690 2024-05-15 23:06:18.998451 aiotraq-0.1.1/aiotraq/api/oauth2/create_client.py
--rw-r--r--   0        0        0     2989 2024-05-15 23:06:18.998772 aiotraq-0.1.1/aiotraq/api/oauth2/delete_client.py
--rw-r--r--   0        0        0     3769 2024-05-15 23:06:18.998964 aiotraq-0.1.1/aiotraq/api/oauth2/edit_client.py
--rw-r--r--   0        0        0     6375 2024-05-15 23:06:18.999172 aiotraq-0.1.1/aiotraq/api/oauth2/get_client.py
--rw-r--r--   0        0        0     5081 2024-05-15 23:06:18.999336 aiotraq-0.1.1/aiotraq/api/oauth2/get_clients.py
--rw-r--r--   0        0        0     4044 2024-05-15 23:06:18.999564 aiotraq-0.1.1/aiotraq/api/oauth2/get_my_tokens.py
--rw-r--r--   0        0        0     5788 2024-05-15 23:06:18.999750 aiotraq-0.1.1/aiotraq/api/oauth2/get_o_auth_2_authorize.py
--rw-r--r--   0        0        0     2887 2024-05-15 23:06:18.999945 aiotraq-0.1.1/aiotraq/api/oauth2/post_o_auth_2_authorize.py
--rw-r--r--   0        0        0     2791 2024-05-15 23:06:19.000147 aiotraq-0.1.1/aiotraq/api/oauth2/post_o_auth_2_authorize_decide.py
--rw-r--r--   0        0        0     4539 2024-05-15 23:06:19.000344 aiotraq-0.1.1/aiotraq/api/oauth2/post_o_auth_2_token.py
--rw-r--r--   0        0        0     2592 2024-05-15 23:06:19.000527 aiotraq-0.1.1/aiotraq/api/oauth2/revoke_my_token.py
--rw-r--r--   0        0        0     2840 2024-05-15 23:06:19.000708 aiotraq-0.1.1/aiotraq/api/oauth2/revoke_o_auth_2_token.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:19.000910 aiotraq-0.1.1/aiotraq/api/ogp/__init__.py
--rw-r--r--   0        0        0     2779 2024-05-15 23:06:19.001085 aiotraq-0.1.1/aiotraq/api/ogp/delete_ogp_cache.py
--rw-r--r--   0        0        0     4740 2024-05-15 23:06:19.001313 aiotraq-0.1.1/aiotraq/api/ogp/get_ogp.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:19.001569 aiotraq-0.1.1/aiotraq/api/public/__init__.py
--rw-r--r--   0        0        0     4107 2024-05-15 23:06:19.001772 aiotraq-0.1.1/aiotraq/api/public/get_public_user_icon.py
--rw-r--r--   0        0        0     3545 2024-05-15 23:06:19.001942 aiotraq-0.1.1/aiotraq/api/public/get_server_version.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:19.002116 aiotraq-0.1.1/aiotraq/api/stamp/__init__.py
--rw-r--r--   0        0        0     3119 2024-05-15 23:06:19.002304 aiotraq-0.1.1/aiotraq/api/stamp/change_stamp_image.py
--rw-r--r--   0        0        0     4596 2024-05-15 23:06:19.002568 aiotraq-0.1.1/aiotraq/api/stamp/create_stamp.py
--rw-r--r--   0        0        0     4683 2024-05-15 23:06:19.002744 aiotraq-0.1.1/aiotraq/api/stamp/create_stamp_palette.py
--rw-r--r--   0        0        0     2702 2024-05-15 23:06:19.002904 aiotraq-0.1.1/aiotraq/api/stamp/delete_stamp.py
--rw-r--r--   0        0        0     2802 2024-05-15 23:06:19.003064 aiotraq-0.1.1/aiotraq/api/stamp/delete_stamp_palette.py
--rw-r--r--   0        0        0     3273 2024-05-15 23:06:19.003274 aiotraq-0.1.1/aiotraq/api/stamp/edit_stamp.py
--rw-r--r--   0        0        0     3647 2024-05-15 23:06:19.003418 aiotraq-0.1.1/aiotraq/api/stamp/edit_stamp_palette.py
--rw-r--r--   0        0        0     5145 2024-05-15 23:06:19.003578 aiotraq-0.1.1/aiotraq/api/stamp/get_my_stamp_history.py
--rw-r--r--   0        0        0     4050 2024-05-15 23:06:19.003716 aiotraq-0.1.1/aiotraq/api/stamp/get_stamp.py
--rw-r--r--   0        0        0     4044 2024-05-15 23:06:19.003977 aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_image.py
--rw-r--r--   0        0        0     4258 2024-05-15 23:06:19.004160 aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_palette.py
--rw-r--r--   0        0        0     3999 2024-05-15 23:06:19.004326 aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_palettes.py
--rw-r--r--   0        0        0     4170 2024-05-15 23:06:19.004493 aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_stats.py
--rw-r--r--   0        0        0     5462 2024-05-15 23:06:19.004729 aiotraq-0.1.1/aiotraq/api/stamp/get_stamps.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:19.004894 aiotraq-0.1.1/aiotraq/api/user/__init__.py
--rw-r--r--   0        0        0     5563 2024-05-15 23:06:19.005039 aiotraq-0.1.1/aiotraq/api/user/add_user_tag.py
--rw-r--r--   0        0        0     3394 2024-05-15 23:06:19.005236 aiotraq-0.1.1/aiotraq/api/user/change_user_icon.py
--rw-r--r--   0        0        0     3369 2024-05-15 23:06:19.005508 aiotraq-0.1.1/aiotraq/api/user/change_user_password.py
--rw-r--r--   0        0        0     4806 2024-05-15 23:06:19.005754 aiotraq-0.1.1/aiotraq/api/user/create_user.py
--rw-r--r--   0        0        0     3259 2024-05-15 23:06:19.006020 aiotraq-0.1.1/aiotraq/api/user/edit_user.py
--rw-r--r--   0        0        0     3441 2024-05-15 23:06:19.006194 aiotraq-0.1.1/aiotraq/api/user/edit_user_tag.py
--rw-r--r--   0        0        0     4145 2024-05-15 23:06:19.006353 aiotraq-0.1.1/aiotraq/api/user/get_user.py
--rw-r--r--   0        0        0     4771 2024-05-15 23:06:19.006571 aiotraq-0.1.1/aiotraq/api/user/get_user_dm_channel.py
--rw-r--r--   0        0        0     4136 2024-05-15 23:06:19.006767 aiotraq-0.1.1/aiotraq/api/user/get_user_icon.py
--rw-r--r--   0        0        0     4138 2024-05-15 23:06:19.006994 aiotraq-0.1.1/aiotraq/api/user/get_user_stats.py
--rw-r--r--   0        0        0     4420 2024-05-15 23:06:19.007186 aiotraq-0.1.1/aiotraq/api/user/get_user_tags.py
--rw-r--r--   0        0        0     6344 2024-05-15 23:06:19.007414 aiotraq-0.1.1/aiotraq/api/user/get_users.py
--rw-r--r--   0        0        0     2848 2024-05-15 23:06:19.007620 aiotraq-0.1.1/aiotraq/api/user/remove_user_tag.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:19.007886 aiotraq-0.1.1/aiotraq/api/user_tag/__init__.py
--rw-r--r--   0        0        0     3142 2024-05-15 23:06:19.008056 aiotraq-0.1.1/aiotraq/api/user_tag/edit_my_user_tag.py
--rw-r--r--   0        0        0     3938 2024-05-15 23:06:19.008208 aiotraq-0.1.1/aiotraq/api/user_tag/get_tag.py
--rw-r--r--   0        0        0     2606 2024-05-15 23:06:19.008355 aiotraq-0.1.1/aiotraq/api/user_tag/remove_my_user_tag.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:19.008596 aiotraq-0.1.1/aiotraq/api/webhook/__init__.py
--rw-r--r--   0        0        0     3228 2024-05-15 23:06:19.008804 aiotraq-0.1.1/aiotraq/api/webhook/change_webhook_icon.py
--rw-r--r--   0        0        0     4747 2024-05-15 23:06:19.008963 aiotraq-0.1.1/aiotraq/api/webhook/create_webhook.py
--rw-r--r--   0        0        0     2675 2024-05-15 23:06:19.009290 aiotraq-0.1.1/aiotraq/api/webhook/delete_webhook.py
--rw-r--r--   0        0        0     3134 2024-05-15 23:06:19.009641 aiotraq-0.1.1/aiotraq/api/webhook/edit_webhook.py
--rw-r--r--   0        0        0     4074 2024-05-15 23:06:19.009855 aiotraq-0.1.1/aiotraq/api/webhook/get_webhook.py
--rw-r--r--   0        0        0     4117 2024-05-15 23:06:19.010206 aiotraq-0.1.1/aiotraq/api/webhook/get_webhook_icon.py
--rw-r--r--   0        0        0     9399 2024-05-15 23:06:19.010576 aiotraq-0.1.1/aiotraq/api/webhook/get_webhook_messages.py
--rw-r--r--   0        0        0     4854 2024-05-15 23:06:19.010955 aiotraq-0.1.1/aiotraq/api/webhook/get_webhooks.py
--rw-r--r--   0        0        0        0 2024-05-15 23:06:19.011345 aiotraq-0.1.1/aiotraq/api/webrtc/__init__.py
--rw-r--r--   0        0        0     3904 2024-05-15 23:06:19.011625 aiotraq-0.1.1/aiotraq/api/webrtc/get_web_rtc_state.py
--rw-r--r--   0        0        0     4850 2024-05-15 23:06:19.011829 aiotraq-0.1.1/aiotraq/api/webrtc/post_web_rtc_authenticate.py
--rw-r--r--   0        0        0    12417 2024-05-15 23:06:19.012145 aiotraq-0.1.1/aiotraq/client.py
--rw-r--r--   0        0        0      546 2024-05-15 23:06:19.012477 aiotraq-0.1.1/aiotraq/errors.py
--rw-r--r--   0        0        0    10121 2024-05-15 23:06:19.012949 aiotraq-0.1.1/aiotraq/models/__init__.py
--rw-r--r--   0        0        0     2549 2024-05-17 02:14:41.797977 aiotraq-0.1.1/aiotraq/models/active_o_auth_2_token.py
--rw-r--r--   0        0        0     2707 2024-05-15 23:06:19.013437 aiotraq-0.1.1/aiotraq/models/activity_timeline_message.py
--rw-r--r--   0        0        0     3575 2024-05-15 23:06:19.013623 aiotraq-0.1.1/aiotraq/models/bot.py
--rw-r--r--   0        0        0     4691 2024-05-15 23:06:19.013832 aiotraq-0.1.1/aiotraq/models/bot_detail.py
--rw-r--r--   0        0        0     3003 2024-05-15 23:06:19.014046 aiotraq-0.1.1/aiotraq/models/bot_event_log.py
--rw-r--r--   0        0        0      175 2024-05-15 23:06:19.014232 aiotraq-0.1.1/aiotraq/models/bot_event_result.py
--rw-r--r--   0        0        0      158 2024-05-15 23:06:19.014437 aiotraq-0.1.1/aiotraq/models/bot_mode.py
--rw-r--r--   0        0        0      162 2024-05-15 23:06:19.014653 aiotraq-0.1.1/aiotraq/models/bot_state.py
--rw-r--r--   0        0        0     1838 2024-05-15 23:06:19.014914 aiotraq-0.1.1/aiotraq/models/bot_tokens.py
--rw-r--r--   0        0        0     1634 2024-05-15 23:06:19.015107 aiotraq-0.1.1/aiotraq/models/bot_user.py
--rw-r--r--   0        0        0     1997 2024-05-15 23:06:19.015291 aiotraq-0.1.1/aiotraq/models/change_stamp_image_body.py
--rw-r--r--   0        0        0     2915 2024-05-15 23:06:19.015511 aiotraq-0.1.1/aiotraq/models/channel.py
--rw-r--r--   0        0        0     8026 2024-05-15 23:06:19.015722 aiotraq-0.1.1/aiotraq/models/channel_event.py
--rw-r--r--   0        0        0      463 2024-05-15 23:06:19.015897 aiotraq-0.1.1/aiotraq/models/channel_event_type.py
--rw-r--r--   0        0        0     2732 2024-05-15 23:06:19.016089 aiotraq-0.1.1/aiotraq/models/channel_list.py
--rw-r--r--   0        0        0     3364 2024-05-15 23:06:19.016292 aiotraq-0.1.1/aiotraq/models/channel_stats.py
--rw-r--r--   0        0        0     1962 2024-05-15 23:06:19.016635 aiotraq-0.1.1/aiotraq/models/channel_stats_stamp.py
--rw-r--r--   0        0        0     1742 2024-05-15 23:06:19.016854 aiotraq-0.1.1/aiotraq/models/channel_stats_user.py
--rw-r--r--   0        0        0      175 2024-05-15 23:06:19.017014 aiotraq-0.1.1/aiotraq/models/channel_subscribe_level.py
--rw-r--r--   0        0        0     1473 2024-05-15 23:06:19.017210 aiotraq-0.1.1/aiotraq/models/channel_topic.py
--rw-r--r--   0        0        0      193 2024-05-15 23:06:19.017412 aiotraq-0.1.1/aiotraq/models/channel_view_state.py
--rw-r--r--   0        0        0     2094 2024-05-15 23:06:19.017604 aiotraq-0.1.1/aiotraq/models/channel_viewer.py
--rw-r--r--   0        0        0     1750 2024-05-15 23:06:19.017826 aiotraq-0.1.1/aiotraq/models/child_created_event.py
--rw-r--r--   0        0        0     2343 2024-05-15 23:06:19.017992 aiotraq-0.1.1/aiotraq/models/clip_folder.py
--rw-r--r--   0        0        0     2005 2024-05-15 23:06:19.018237 aiotraq-0.1.1/aiotraq/models/clipped_message.py
--rw-r--r--   0        0        0     1647 2024-05-15 23:06:19.018427 aiotraq-0.1.1/aiotraq/models/dm_channel.py
--rw-r--r--   0        0        0     2081 2024-05-15 23:06:19.018592 aiotraq-0.1.1/aiotraq/models/external_provider_user.py
--rw-r--r--   0        0        0     5748 2024-05-15 23:06:19.018777 aiotraq-0.1.1/aiotraq/models/file_info.py
--rw-r--r--   0        0        0     2216 2024-05-15 23:06:19.019006 aiotraq-0.1.1/aiotraq/models/file_info_thumbnail_type_0.py
--rw-r--r--   0        0        0     1795 2024-05-15 23:06:19.019187 aiotraq-0.1.1/aiotraq/models/forced_notification_changed_event.py
--rw-r--r--   0        0        0      160 2024-05-15 23:06:19.019372 aiotraq-0.1.1/aiotraq/models/get_channel_events_order.py
--rw-r--r--   0        0        0      152 2024-05-15 23:06:19.019553 aiotraq-0.1.1/aiotraq/models/get_clips_order.py
--rw-r--r--   0        0        0      161 2024-05-15 23:06:19.019816 aiotraq-0.1.1/aiotraq/models/get_direct_messages_order.py
--rw-r--r--   0        0        0      152 2024-05-15 23:06:19.020012 aiotraq-0.1.1/aiotraq/models/get_files_order.py
--rw-r--r--   0        0        0      155 2024-05-15 23:06:19.020185 aiotraq-0.1.1/aiotraq/models/get_messages_order.py
--rw-r--r--   0        0        0     1603 2024-05-15 23:06:19.020363 aiotraq-0.1.1/aiotraq/models/get_notify_citation.py
--rw-r--r--   0        0        0      168 2024-05-15 23:06:19.020520 aiotraq-0.1.1/aiotraq/models/get_stamps_type.py
--rw-r--r--   0        0        0      162 2024-05-15 23:06:19.020682 aiotraq-0.1.1/aiotraq/models/get_webhook_messages_order.py
--rw-r--r--   0        0        0     1763 2024-05-15 23:06:19.020867 aiotraq-0.1.1/aiotraq/models/login_session.py
--rw-r--r--   0        0        0     3946 2024-05-15 23:06:19.021035 aiotraq-0.1.1/aiotraq/models/message.py
--rw-r--r--   0        0        0     1870 2024-05-15 23:06:19.021259 aiotraq-0.1.1/aiotraq/models/message_clip.py
--rw-r--r--   0        0        0     1810 2024-05-15 23:06:19.021452 aiotraq-0.1.1/aiotraq/models/message_pin.py
--rw-r--r--   0        0        0     2518 2024-05-15 23:06:19.021609 aiotraq-0.1.1/aiotraq/models/message_stamp.py
--rw-r--r--   0        0        0     2010 2024-05-15 23:06:19.021783 aiotraq-0.1.1/aiotraq/models/my_channel_view_state.py
--rw-r--r--   0        0        0     6243 2024-05-15 23:06:19.021962 aiotraq-0.1.1/aiotraq/models/my_user_detail.py
--rw-r--r--   0        0        0     1896 2024-05-15 23:06:19.022122 aiotraq-0.1.1/aiotraq/models/name_changed_event.py
--rw-r--r--   0        0        0     4639 2024-05-15 23:06:19.022275 aiotraq-0.1.1/aiotraq/models/o_auth_2_authorization.py
--rw-r--r--   0        0        0     2650 2024-05-15 23:06:19.022494 aiotraq-0.1.1/aiotraq/models/o_auth_2_client.py
--rw-r--r--   0        0        0     3132 2024-05-15 23:06:19.022770 aiotraq-0.1.1/aiotraq/models/o_auth_2_client_detail.py
--rw-r--r--   0        0        0     1479 2024-05-15 23:06:19.022949 aiotraq-0.1.1/aiotraq/models/o_auth_2_decide.py
--rw-r--r--   0        0        0      135 2024-05-15 23:06:19.023110 aiotraq-0.1.1/aiotraq/models/o_auth_2_prompt.py
--rw-r--r--   0        0        0      179 2024-05-15 23:06:19.023274 aiotraq-0.1.1/aiotraq/models/o_auth_2_response_type.py
--rw-r--r--   0        0        0     1565 2024-05-15 23:06:19.023478 aiotraq-0.1.1/aiotraq/models/o_auth_2_revoke.py
--rw-r--r--   0        0        0      230 2024-05-15 23:06:19.023651 aiotraq-0.1.1/aiotraq/models/o_auth_2_scope.py
--rw-r--r--   0        0        0     2863 2024-05-15 23:06:19.023865 aiotraq-0.1.1/aiotraq/models/o_auth_2_token.py
--rw-r--r--   0        0        0     2978 2024-05-15 23:06:19.024023 aiotraq-0.1.1/aiotraq/models/ogp.py
--rw-r--r--   0        0        0     3066 2024-05-15 23:06:19.024221 aiotraq-0.1.1/aiotraq/models/ogp_media.py
--rw-r--r--   0        0        0     5719 2024-05-15 23:06:19.024394 aiotraq-0.1.1/aiotraq/models/oidc_traq_user_info.py
--rw-r--r--   0        0        0     3202 2024-05-15 23:06:19.024558 aiotraq-0.1.1/aiotraq/models/oidc_user_info.py
--rw-r--r--   0        0        0     1914 2024-05-15 23:06:19.024713 aiotraq-0.1.1/aiotraq/models/parent_changed_event.py
--rw-r--r--   0        0        0     4054 2024-05-15 23:06:19.024904 aiotraq-0.1.1/aiotraq/models/patch_bot_request.py
--rw-r--r--   0        0        0     2468 2024-05-15 23:06:19.025060 aiotraq-0.1.1/aiotraq/models/patch_channel_request.py
--rw-r--r--   0        0        0     2190 2024-05-15 23:06:19.025218 aiotraq-0.1.1/aiotraq/models/patch_channel_subscribers_request.py
--rw-r--r--   0        0        0     2598 2024-05-15 23:06:19.025379 aiotraq-0.1.1/aiotraq/models/patch_client_request.py
--rw-r--r--   0        0        0     1941 2024-05-15 23:06:19.025572 aiotraq-0.1.1/aiotraq/models/patch_clip_folder_request.py
--rw-r--r--   0        0        0     1563 2024-05-15 23:06:19.025736 aiotraq-0.1.1/aiotraq/models/patch_group_member_request.py
--rw-r--r--   0        0        0     2679 2024-05-15 23:06:19.025888 aiotraq-0.1.1/aiotraq/models/patch_me_request.py
--rw-r--r--   0        0        0     2375 2024-05-15 23:06:19.026055 aiotraq-0.1.1/aiotraq/models/patch_stamp_palette_request.py
--rw-r--r--   0        0        0     1895 2024-05-15 23:06:19.026204 aiotraq-0.1.1/aiotraq/models/patch_stamp_request.py
--rw-r--r--   0        0        0     2188 2024-05-15 23:06:19.026436 aiotraq-0.1.1/aiotraq/models/patch_user_group_request.py
--rw-r--r--   0        0        0     2912 2024-05-15 23:06:19.026604 aiotraq-0.1.1/aiotraq/models/patch_user_request.py
--rw-r--r--   0        0        0     1584 2024-05-15 23:06:19.026846 aiotraq-0.1.1/aiotraq/models/patch_user_tag_request.py
--rw-r--r--   0        0        0     2821 2024-05-15 23:06:19.027048 aiotraq-0.1.1/aiotraq/models/patch_webhook_request.py
--rw-r--r--   0        0        0     2151 2024-05-15 23:06:19.027200 aiotraq-0.1.1/aiotraq/models/pin.py
--rw-r--r--   0        0        0     1718 2024-05-15 23:06:19.027355 aiotraq-0.1.1/aiotraq/models/pin_added_event.py
--rw-r--r--   0        0        0     1728 2024-05-15 23:06:19.027544 aiotraq-0.1.1/aiotraq/models/pin_removed_event.py
--rw-r--r--   0        0        0     1609 2024-05-15 23:06:19.027683 aiotraq-0.1.1/aiotraq/models/post_bot_action_join_request.py
--rw-r--r--   0        0        0     1614 2024-05-15 23:06:19.027831 aiotraq-0.1.1/aiotraq/models/post_bot_action_leave_request.py
--rw-r--r--   0        0        0     2706 2024-05-15 23:06:19.027975 aiotraq-0.1.1/aiotraq/models/post_bot_request.py
--rw-r--r--   0        0        0     2013 2024-05-15 23:06:19.028141 aiotraq-0.1.1/aiotraq/models/post_channel_request.py
--rw-r--r--   0        0        0     2531 2024-05-15 23:06:19.028385 aiotraq-0.1.1/aiotraq/models/post_client_request.py
--rw-r--r--   0        0        0     1623 2024-05-15 23:06:19.028599 aiotraq-0.1.1/aiotraq/models/post_clip_folder_message_request.py
--rw-r--r--   0        0        0     1755 2024-05-15 23:06:19.028757 aiotraq-0.1.1/aiotraq/models/post_clip_folder_request.py
--rw-r--r--   0        0        0     2458 2024-05-15 23:06:19.028927 aiotraq-0.1.1/aiotraq/models/post_file_request.py
--rw-r--r--   0        0        0     1653 2024-05-15 23:06:19.029092 aiotraq-0.1.1/aiotraq/models/post_link_external_account.py
--rw-r--r--   0        0        0     1688 2024-05-15 23:06:19.029242 aiotraq-0.1.1/aiotraq/models/post_login_request.py
--rw-r--r--   0        0        0     1911 2024-05-15 23:06:19.029445 aiotraq-0.1.1/aiotraq/models/post_message_request.py
--rw-r--r--   0        0        0     1540 2024-05-15 23:06:19.029660 aiotraq-0.1.1/aiotraq/models/post_message_stamp_request.py
--rw-r--r--   0        0        0     1612 2024-05-15 23:06:19.029824 aiotraq-0.1.1/aiotraq/models/post_my_fcm_device_request.py
--rw-r--r--   0        0        0     4102 2024-05-15 23:06:19.030002 aiotraq-0.1.1/aiotraq/models/post_o_auth_2_token.py
--rw-r--r--   0        0        0     2007 2024-05-15 23:06:19.030153 aiotraq-0.1.1/aiotraq/models/post_stamp_palette_request.py
--rw-r--r--   0        0        0     2313 2024-05-15 23:06:19.030347 aiotraq-0.1.1/aiotraq/models/post_stamp_request.py
--rw-r--r--   0        0        0     1549 2024-05-15 23:06:19.030669 aiotraq-0.1.1/aiotraq/models/post_star_request.py
--rw-r--r--   0        0        0     1665 2024-05-15 23:06:19.030823 aiotraq-0.1.1/aiotraq/models/post_unlink_external_account.py
--rw-r--r--   0        0        0     1513 2024-05-15 23:06:19.030967 aiotraq-0.1.1/aiotraq/models/post_user_group_admin.py
--rw-r--r--   0        0        0     1915 2024-05-15 23:06:19.031123 aiotraq-0.1.1/aiotraq/models/post_user_group_request.py
--rw-r--r--   0        0        0     1815 2024-05-15 23:06:19.031333 aiotraq-0.1.1/aiotraq/models/post_user_request.py
--rw-r--r--   0        0        0     1504 2024-05-15 23:06:19.031481 aiotraq-0.1.1/aiotraq/models/post_user_tag_request.py
--rw-r--r--   0        0        0     1584 2024-05-15 23:06:19.031685 aiotraq-0.1.1/aiotraq/models/post_web_rtc_authenticate_request.py
--rw-r--r--   0        0        0     2173 2024-05-15 23:06:19.031891 aiotraq-0.1.1/aiotraq/models/post_webhook_request.py
--rw-r--r--   0        0        0     1840 2024-05-15 23:06:19.032113 aiotraq-0.1.1/aiotraq/models/put_channel_subscribe_level_request.py
--rw-r--r--   0        0        0     1623 2024-05-15 23:06:19.032266 aiotraq-0.1.1/aiotraq/models/put_channel_subscribers_request.py
--rw-r--r--   0        0        0     1550 2024-05-15 23:06:19.032418 aiotraq-0.1.1/aiotraq/models/put_channel_topic_request.py
--rw-r--r--   0        0        0     1816 2024-05-15 23:06:19.032600 aiotraq-0.1.1/aiotraq/models/put_my_password_request.py
--rw-r--r--   0        0        0     1690 2024-05-15 23:06:19.032763 aiotraq-0.1.1/aiotraq/models/put_notify_citation_request.py
--rw-r--r--   0        0        0     2027 2024-05-15 23:06:19.032955 aiotraq-0.1.1/aiotraq/models/put_user_icon_request.py
--rw-r--r--   0        0        0     1630 2024-05-15 23:06:19.033122 aiotraq-0.1.1/aiotraq/models/put_user_password_request.py
--rw-r--r--   0        0        0     2274 2024-05-15 23:06:19.033295 aiotraq-0.1.1/aiotraq/models/search_messages_message_search_result.py
--rw-r--r--   0        0        0      233 2024-05-15 23:06:19.033515 aiotraq-0.1.1/aiotraq/models/search_messages_sort.py
--rw-r--r--   0        0        0     2766 2024-05-15 23:06:19.033648 aiotraq-0.1.1/aiotraq/models/stamp.py
--rw-r--r--   0        0        0     1841 2024-05-15 23:06:19.033781 aiotraq-0.1.1/aiotraq/models/stamp_history_entry.py
--rw-r--r--   0        0        0     2915 2024-05-15 23:06:19.033940 aiotraq-0.1.1/aiotraq/models/stamp_palette.py
--rw-r--r--   0        0        0     1829 2024-05-15 23:06:19.034077 aiotraq-0.1.1/aiotraq/models/stamp_stats.py
--rw-r--r--   0        0        0     3122 2024-05-15 23:06:19.034219 aiotraq-0.1.1/aiotraq/models/stamp_with_thumbnail.py
--rw-r--r--   0        0        0     1958 2024-05-15 23:06:19.034350 aiotraq-0.1.1/aiotraq/models/subscribers_changed_event.py
--rw-r--r--   0        0        0     1771 2024-05-15 23:06:19.034505 aiotraq-0.1.1/aiotraq/models/tag.py
--rw-r--r--   0        0        0     2272 2024-05-15 23:06:19.034717 aiotraq-0.1.1/aiotraq/models/thumbnail_info.py
--rw-r--r--   0        0        0      164 2024-05-15 23:06:19.035073 aiotraq-0.1.1/aiotraq/models/thumbnail_type.py
--rw-r--r--   0        0        0     1883 2024-05-15 23:06:19.035331 aiotraq-0.1.1/aiotraq/models/topic_changed_event.py
--rw-r--r--   0        0        0     2941 2024-05-15 23:06:19.035617 aiotraq-0.1.1/aiotraq/models/unread_channel.py
--rw-r--r--   0        0        0     2880 2024-05-15 23:06:19.035867 aiotraq-0.1.1/aiotraq/models/user.py
--rw-r--r--   0        0        0      170 2024-05-15 23:06:19.036070 aiotraq-0.1.1/aiotraq/models/user_account_state.py
--rw-r--r--   0        0        0     5543 2024-05-15 23:06:19.036349 aiotraq-0.1.1/aiotraq/models/user_detail.py
--rw-r--r--   0        0        0     3691 2024-05-15 23:06:19.036557 aiotraq-0.1.1/aiotraq/models/user_group.py
--rw-r--r--   0        0        0     1639 2024-05-15 23:06:19.036913 aiotraq-0.1.1/aiotraq/models/user_group_member.py
--rw-r--r--   0        0        0     3487 2024-05-15 23:06:19.037102 aiotraq-0.1.1/aiotraq/models/user_permission.py
--rw-r--r--   0        0        0     1743 2024-05-15 23:06:19.037266 aiotraq-0.1.1/aiotraq/models/user_settings.py
--rw-r--r--   0        0        0     2660 2024-05-15 23:06:19.037434 aiotraq-0.1.1/aiotraq/models/user_stats.py
--rw-r--r--   0        0        0     1941 2024-05-15 23:06:19.037580 aiotraq-0.1.1/aiotraq/models/user_stats_stamp.py
--rw-r--r--   0        0        0     1981 2024-05-15 23:06:19.037737 aiotraq-0.1.1/aiotraq/models/user_subscribe_state.py
--rw-r--r--   0        0        0     2417 2024-05-15 23:06:19.037880 aiotraq-0.1.1/aiotraq/models/user_tag.py
--rw-r--r--   0        0        0     2072 2024-05-15 23:06:19.038059 aiotraq-0.1.1/aiotraq/models/version.py
--rw-r--r--   0        0        0     1915 2024-05-15 23:06:19.038338 aiotraq-0.1.1/aiotraq/models/version_flags.py
--rw-r--r--   0        0        0     1790 2024-05-15 23:06:19.038610 aiotraq-0.1.1/aiotraq/models/visibility_changed_event.py
--rw-r--r--   0        0        0     2140 2024-05-15 23:06:19.038849 aiotraq-0.1.1/aiotraq/models/web_rtc_authenticate_result.py
--rw-r--r--   0        0        0     2542 2024-05-15 23:06:19.039082 aiotraq-0.1.1/aiotraq/models/web_rtc_user_state.py
--rw-r--r--   0        0        0     1745 2024-05-15 23:06:19.039255 aiotraq-0.1.1/aiotraq/models/web_rtc_user_state_sessions_item.py
--rw-r--r--   0        0        0     3327 2024-05-15 23:06:19.039406 aiotraq-0.1.1/aiotraq/models/webhook.py
--rw-r--r--   0        0        0       25 2024-05-15 23:06:19.039557 aiotraq-0.1.1/aiotraq/py.typed
--rw-r--r--   0        0        0      985 2024-05-15 23:06:19.039752 aiotraq-0.1.1/aiotraq/types.py
--rw-r--r--   0        0        0      894 2024-05-17 23:17:16.738611 aiotraq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5136 1970-01-01 00:00:00.000000 aiotraq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4393 2024-06-02 10:06:15.283745 aiotraq-0.1.2/README.md
+-rw-r--r--   0        0        0      150 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/__init__.py
+-rw-r--r--   0        0        0       45 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/activity/__init__.py
+-rw-r--r--   0        0        0     6751 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/activity/get_activity_timeline.py
+-rw-r--r--   0        0        0     3710 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/activity/get_online_users.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/__init__.py
+-rw-r--r--   0        0        0     4158 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/get_my_external_accounts.py
+-rw-r--r--   0        0        0     3978 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/get_my_sessions.py
+-rw-r--r--   0        0        0     3520 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/link_external_account.py
+-rw-r--r--   0        0        0     3424 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/login.py
+-rw-r--r--   0        0        0     3020 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/logout.py
+-rw-r--r--   0        0        0     2775 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/revoke_my_session.py
+-rw-r--r--   0        0        0     3149 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/authentication/unlink_external_account.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/__init__.py
+-rw-r--r--   0        0        0     2675 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/activate_bot.py
+-rw-r--r--   0        0        0     3371 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/change_bot_icon.py
+-rw-r--r--   0        0        0     5609 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/connect_bot_ws.py
+-rw-r--r--   0        0        0     5089 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/create_bot.py
+-rw-r--r--   0        0        0     2626 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/delete_bot.py
+-rw-r--r--   0        0        0     3499 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/edit_bot.py
+-rw-r--r--   0        0        0     5904 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/get_bot.py
+-rw-r--r--   0        0        0     4081 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/get_bot_icon.py
+-rw-r--r--   0        0        0     5835 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/get_bot_logs.py
+-rw-r--r--   0        0        0     4650 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/get_bots.py
+-rw-r--r--   0        0        0     4609 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/get_channel_bots.py
+-rw-r--r--   0        0        0     2681 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/inactivate_bot.py
+-rw-r--r--   0        0        0     3646 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/let_bot_join_channel.py
+-rw-r--r--   0        0        0     3416 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/let_bot_leave_channel.py
+-rw-r--r--   0        0        0     4558 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/bot/reissue_bot.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/__init__.py
+-rw-r--r--   0        0        0     4974 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/create_channel.py
+-rw-r--r--   0        0        0     3685 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/edit_channel.py
+-rw-r--r--   0        0        0     3761 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/edit_channel_subscribers.py
+-rw-r--r--   0        0        0     3428 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/edit_channel_topic.py
+-rw-r--r--   0        0        0     4138 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channel.py
+-rw-r--r--   0        0        0     9367 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channel_events.py
+-rw-r--r--   0        0        0     4628 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channel_pins.py
+-rw-r--r--   0        0        0     4258 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channel_stats.py
+-rw-r--r--   0        0        0     4548 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channel_subscribers.py
+-rw-r--r--   0        0        0     4258 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channel_topic.py
+-rw-r--r--   0        0        0     4606 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channel_viewers.py
+-rw-r--r--   0        0        0     4341 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_channels.py
+-rw-r--r--   0        0        0     9238 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/get_messages.py
+-rw-r--r--   0        0        0     3759 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/channel/set_channel_subscribers.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/__init__.py
+-rw-r--r--   0        0        0     5531 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/clip_message.py
+-rw-r--r--   0        0        0     5001 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/create_clip_folder.py
+-rw-r--r--   0        0        0     2575 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/delete_clip_folder.py
+-rw-r--r--   0        0        0     3252 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/edit_clip_folder.py
+-rw-r--r--   0        0        0     4236 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/get_clip_folder.py
+-rw-r--r--   0        0        0     3947 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/get_clip_folders.py
+-rw-r--r--   0        0        0     7051 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/get_clips.py
+-rw-r--r--   0        0        0     3066 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/clip/unclip_message.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/file/__init__.py
+-rw-r--r--   0        0        0     2697 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/file/delete_file.py
+-rw-r--r--   0        0        0     4993 2024-06-02 10:06:15.283745 aiotraq-0.1.2/aiotraq/api/file/get_file.py
+-rw-r--r--   0        0        0     4504 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/file/get_file_meta.py
+-rw-r--r--   0        0        0    10079 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/file/get_files.py
+-rw-r--r--   0        0        0     5492 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/file/get_thumbnail_image.py
+-rw-r--r--   0        0        0     5239 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/file/post_file.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/__init__.py
+-rw-r--r--   0        0        0     3381 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/add_user_group_admin.py
+-rw-r--r--   0        0        0     3360 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/add_user_group_member.py
+-rw-r--r--   0        0        0     3386 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/change_user_group_icon.py
+-rw-r--r--   0        0        0     5114 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/create_user_group.py
+-rw-r--r--   0        0        0     2780 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/delete_user_group.py
+-rw-r--r--   0        0        0     3498 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/edit_user_group.py
+-rw-r--r--   0        0        0     3692 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/edit_user_group_member.py
+-rw-r--r--   0        0        0     4175 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/get_user_group.py
+-rw-r--r--   0        0        0     4141 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/get_user_group_admins.py
+-rw-r--r--   0        0        0     4559 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/get_user_group_members.py
+-rw-r--r--   0        0        0     3844 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/get_user_groups.py
+-rw-r--r--   0        0        0     3260 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/remove_user_group_admin.py
+-rw-r--r--   0        0        0     3222 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/group/remove_user_group_member.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/__init__.py
+-rw-r--r--   0        0        0     3241 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/add_my_star.py
+-rw-r--r--   0        0        0     4621 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/add_my_user_tag.py
+-rw-r--r--   0        0        0     2948 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/change_my_icon.py
+-rw-r--r--   0        0        0     3037 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/change_my_notify_citation.py
+-rw-r--r--   0        0        0     2979 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/change_my_password.py
+-rw-r--r--   0        0        0     2889 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/edit_me.py
+-rw-r--r--   0        0        0     3553 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_me.py
+-rw-r--r--   0        0        0     3978 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_channel_subscriptions.py
+-rw-r--r--   0        0        0     3691 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_icon.py
+-rw-r--r--   0        0        0     3751 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_notify_citation.py
+-rw-r--r--   0        0        0     4455 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_qr_code.py
+-rw-r--r--   0        0        0     3620 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_stars.py
+-rw-r--r--   0        0        0     3917 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_unread_channels.py
+-rw-r--r--   0        0        0     3813 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_user_tags.py
+-rw-r--r--   0        0        0     4025 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_my_view_states.py
+-rw-r--r--   0        0        0     3818 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_oidc_user_info.py
+-rw-r--r--   0        0        0     3465 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/get_user_settings.py
+-rw-r--r--   0        0        0     2515 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/read_channel.py
+-rw-r--r--   0        0        0     2903 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/register_fcm_device.py
+-rw-r--r--   0        0        0     2634 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/remove_my_star.py
+-rw-r--r--   0        0        0     3425 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/me/set_channel_subscribe_level.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/__init__.py
+-rw-r--r--   0        0        0     3387 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/add_message_stamp.py
+-rw-r--r--   0        0        0     5062 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/create_pin.py
+-rw-r--r--   0        0        0     3156 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/delete_message.py
+-rw-r--r--   0        0        0     3590 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/edit_message.py
+-rw-r--r--   0        0        0     9362 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/get_direct_messages.py
+-rw-r--r--   0        0        0     4078 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/get_message.py
+-rw-r--r--   0        0        0     4542 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/get_message_clips.py
+-rw-r--r--   0        0        0     4700 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/get_message_stamps.py
+-rw-r--r--   0        0        0     4194 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/get_pin.py
+-rw-r--r--   0        0        0     5098 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/post_direct_message.py
+-rw-r--r--   0        0        0     5867 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/post_message.py
+-rw-r--r--   0        0        0     2812 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/remove_message_stamp.py
+-rw-r--r--   0        0        0     2642 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/remove_pin.py
+-rw-r--r--   0        0        0    12982 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/message/search_messages.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/notification/__init__.py
+-rw-r--r--   0        0        0    21754 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/notification/ws.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/__init__.py
+-rw-r--r--   0        0        0     4690 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/create_client.py
+-rw-r--r--   0        0        0     2989 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/delete_client.py
+-rw-r--r--   0        0        0     3769 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/edit_client.py
+-rw-r--r--   0        0        0     6375 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/get_client.py
+-rw-r--r--   0        0        0     5081 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/get_clients.py
+-rw-r--r--   0        0        0     4044 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/get_my_tokens.py
+-rw-r--r--   0        0        0     5788 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/get_o_auth_2_authorize.py
+-rw-r--r--   0        0        0     2887 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/post_o_auth_2_authorize.py
+-rw-r--r--   0        0        0     2791 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/post_o_auth_2_authorize_decide.py
+-rw-r--r--   0        0        0     4539 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/post_o_auth_2_token.py
+-rw-r--r--   0        0        0     2592 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/revoke_my_token.py
+-rw-r--r--   0        0        0     2840 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/oauth2/revoke_o_auth_2_token.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/ogp/__init__.py
+-rw-r--r--   0        0        0     2779 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/ogp/delete_ogp_cache.py
+-rw-r--r--   0        0        0     4740 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/ogp/get_ogp.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/public/__init__.py
+-rw-r--r--   0        0        0     4107 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/public/get_public_user_icon.py
+-rw-r--r--   0        0        0     3545 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/public/get_server_version.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/__init__.py
+-rw-r--r--   0        0        0     3119 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/change_stamp_image.py
+-rw-r--r--   0        0        0     4596 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/create_stamp.py
+-rw-r--r--   0        0        0     4683 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/create_stamp_palette.py
+-rw-r--r--   0        0        0     2702 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/delete_stamp.py
+-rw-r--r--   0        0        0     2802 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/delete_stamp_palette.py
+-rw-r--r--   0        0        0     3273 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/edit_stamp.py
+-rw-r--r--   0        0        0     3647 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/edit_stamp_palette.py
+-rw-r--r--   0        0        0     5145 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/get_my_stamp_history.py
+-rw-r--r--   0        0        0     4050 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/get_stamp.py
+-rw-r--r--   0        0        0     4044 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_image.py
+-rw-r--r--   0        0        0     4258 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_palette.py
+-rw-r--r--   0        0        0     3999 2024-06-02 10:06:15.287746 aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_palettes.py
+-rw-r--r--   0        0        0     4170 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_stats.py
+-rw-r--r--   0        0        0     5462 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/stamp/get_stamps.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/__init__.py
+-rw-r--r--   0        0        0     5563 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/add_user_tag.py
+-rw-r--r--   0        0        0     3394 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/change_user_icon.py
+-rw-r--r--   0        0        0     3369 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/change_user_password.py
+-rw-r--r--   0        0        0     4806 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/create_user.py
+-rw-r--r--   0        0        0     3259 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/edit_user.py
+-rw-r--r--   0        0        0     3441 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/edit_user_tag.py
+-rw-r--r--   0        0        0     4145 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/get_user.py
+-rw-r--r--   0        0        0     4771 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/get_user_dm_channel.py
+-rw-r--r--   0        0        0     4136 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/get_user_icon.py
+-rw-r--r--   0        0        0     4138 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/get_user_stats.py
+-rw-r--r--   0        0        0     4420 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/get_user_tags.py
+-rw-r--r--   0        0        0     6344 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/get_users.py
+-rw-r--r--   0        0        0     2848 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user/remove_user_tag.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user_tag/__init__.py
+-rw-r--r--   0        0        0     3142 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user_tag/edit_my_user_tag.py
+-rw-r--r--   0        0        0     3938 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user_tag/get_tag.py
+-rw-r--r--   0        0        0     2606 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/user_tag/remove_my_user_tag.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/__init__.py
+-rw-r--r--   0        0        0     3228 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/change_webhook_icon.py
+-rw-r--r--   0        0        0     4747 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/create_webhook.py
+-rw-r--r--   0        0        0     2675 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/delete_webhook.py
+-rw-r--r--   0        0        0     3134 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/edit_webhook.py
+-rw-r--r--   0        0        0     4074 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/get_webhook.py
+-rw-r--r--   0        0        0     4117 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/get_webhook_icon.py
+-rw-r--r--   0        0        0     9399 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/get_webhook_messages.py
+-rw-r--r--   0        0        0     4854 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webhook/get_webhooks.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webrtc/__init__.py
+-rw-r--r--   0        0        0     3904 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webrtc/get_web_rtc_state.py
+-rw-r--r--   0        0        0     4850 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/api/webrtc/post_web_rtc_authenticate.py
+-rw-r--r--   0        0        0    12417 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/client.py
+-rw-r--r--   0        0        0      546 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/errors.py
+-rw-r--r--   0        0        0    10121 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/__init__.py
+-rw-r--r--   0        0        0     2549 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/active_o_auth_2_token.py
+-rw-r--r--   0        0        0     2707 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/activity_timeline_message.py
+-rw-r--r--   0        0        0     3575 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot.py
+-rw-r--r--   0        0        0     4691 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot_detail.py
+-rw-r--r--   0        0        0     3003 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot_event_log.py
+-rw-r--r--   0        0        0      175 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot_event_result.py
+-rw-r--r--   0        0        0      158 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot_mode.py
+-rw-r--r--   0        0        0      162 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot_state.py
+-rw-r--r--   0        0        0     1838 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot_tokens.py
+-rw-r--r--   0        0        0     1634 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/bot_user.py
+-rw-r--r--   0        0        0     1997 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/change_stamp_image_body.py
+-rw-r--r--   0        0        0     2915 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel.py
+-rw-r--r--   0        0        0     8026 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_event.py
+-rw-r--r--   0        0        0      463 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_event_type.py
+-rw-r--r--   0        0        0     2732 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_list.py
+-rw-r--r--   0        0        0     3364 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_stats.py
+-rw-r--r--   0        0        0     1962 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_stats_stamp.py
+-rw-r--r--   0        0        0     1742 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_stats_user.py
+-rw-r--r--   0        0        0      175 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_subscribe_level.py
+-rw-r--r--   0        0        0     1473 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_topic.py
+-rw-r--r--   0        0        0      193 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_view_state.py
+-rw-r--r--   0        0        0     2094 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/channel_viewer.py
+-rw-r--r--   0        0        0     1750 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/child_created_event.py
+-rw-r--r--   0        0        0     2343 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/clip_folder.py
+-rw-r--r--   0        0        0     2005 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/clipped_message.py
+-rw-r--r--   0        0        0     1647 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/dm_channel.py
+-rw-r--r--   0        0        0     2081 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/external_provider_user.py
+-rw-r--r--   0        0        0     5748 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/file_info.py
+-rw-r--r--   0        0        0     2216 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/file_info_thumbnail_type_0.py
+-rw-r--r--   0        0        0     1795 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/forced_notification_changed_event.py
+-rw-r--r--   0        0        0      160 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_channel_events_order.py
+-rw-r--r--   0        0        0      152 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_clips_order.py
+-rw-r--r--   0        0        0      161 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_direct_messages_order.py
+-rw-r--r--   0        0        0      152 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_files_order.py
+-rw-r--r--   0        0        0      155 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_messages_order.py
+-rw-r--r--   0        0        0     1603 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_notify_citation.py
+-rw-r--r--   0        0        0      168 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_stamps_type.py
+-rw-r--r--   0        0        0      162 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/get_webhook_messages_order.py
+-rw-r--r--   0        0        0     1763 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/login_session.py
+-rw-r--r--   0        0        0     3946 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/message.py
+-rw-r--r--   0        0        0     1870 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/message_clip.py
+-rw-r--r--   0        0        0     1810 2024-06-02 10:06:15.291746 aiotraq-0.1.2/aiotraq/models/message_pin.py
+-rw-r--r--   0        0        0     2518 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/message_stamp.py
+-rw-r--r--   0        0        0     2010 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/my_channel_view_state.py
+-rw-r--r--   0        0        0     6243 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/my_user_detail.py
+-rw-r--r--   0        0        0     1896 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/name_changed_event.py
+-rw-r--r--   0        0        0     4639 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_authorization.py
+-rw-r--r--   0        0        0     2650 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_client.py
+-rw-r--r--   0        0        0     3132 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_client_detail.py
+-rw-r--r--   0        0        0     1479 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_decide.py
+-rw-r--r--   0        0        0      135 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_prompt.py
+-rw-r--r--   0        0        0      179 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_response_type.py
+-rw-r--r--   0        0        0     1565 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_revoke.py
+-rw-r--r--   0        0        0      230 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_scope.py
+-rw-r--r--   0        0        0     2863 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/o_auth_2_token.py
+-rw-r--r--   0        0        0     2978 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/ogp.py
+-rw-r--r--   0        0        0     3066 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/ogp_media.py
+-rw-r--r--   0        0        0     5719 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/oidc_traq_user_info.py
+-rw-r--r--   0        0        0     3202 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/oidc_user_info.py
+-rw-r--r--   0        0        0     1914 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/parent_changed_event.py
+-rw-r--r--   0        0        0     4054 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_bot_request.py
+-rw-r--r--   0        0        0     2468 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_channel_request.py
+-rw-r--r--   0        0        0     2190 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_channel_subscribers_request.py
+-rw-r--r--   0        0        0     2598 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_client_request.py
+-rw-r--r--   0        0        0     1941 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_clip_folder_request.py
+-rw-r--r--   0        0        0     1563 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_group_member_request.py
+-rw-r--r--   0        0        0     2679 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_me_request.py
+-rw-r--r--   0        0        0     2375 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_stamp_palette_request.py
+-rw-r--r--   0        0        0     1895 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_stamp_request.py
+-rw-r--r--   0        0        0     2188 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_user_group_request.py
+-rw-r--r--   0        0        0     2912 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_user_request.py
+-rw-r--r--   0        0        0     1584 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_user_tag_request.py
+-rw-r--r--   0        0        0     2821 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/patch_webhook_request.py
+-rw-r--r--   0        0        0     2151 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/pin.py
+-rw-r--r--   0        0        0     1718 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/pin_added_event.py
+-rw-r--r--   0        0        0     1728 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/pin_removed_event.py
+-rw-r--r--   0        0        0     1609 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_bot_action_join_request.py
+-rw-r--r--   0        0        0     1614 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_bot_action_leave_request.py
+-rw-r--r--   0        0        0     2706 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_bot_request.py
+-rw-r--r--   0        0        0     2013 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_channel_request.py
+-rw-r--r--   0        0        0     2531 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_client_request.py
+-rw-r--r--   0        0        0     1623 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_clip_folder_message_request.py
+-rw-r--r--   0        0        0     1755 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_clip_folder_request.py
+-rw-r--r--   0        0        0     2458 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_file_request.py
+-rw-r--r--   0        0        0     1653 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_link_external_account.py
+-rw-r--r--   0        0        0     1688 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_login_request.py
+-rw-r--r--   0        0        0     1911 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_message_request.py
+-rw-r--r--   0        0        0     1540 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_message_stamp_request.py
+-rw-r--r--   0        0        0     1612 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_my_fcm_device_request.py
+-rw-r--r--   0        0        0     4102 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_o_auth_2_token.py
+-rw-r--r--   0        0        0     2007 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_stamp_palette_request.py
+-rw-r--r--   0        0        0     2313 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_stamp_request.py
+-rw-r--r--   0        0        0     1549 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_star_request.py
+-rw-r--r--   0        0        0     1665 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_unlink_external_account.py
+-rw-r--r--   0        0        0     1513 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_user_group_admin.py
+-rw-r--r--   0        0        0     1915 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_user_group_request.py
+-rw-r--r--   0        0        0     1815 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_user_request.py
+-rw-r--r--   0        0        0     1504 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_user_tag_request.py
+-rw-r--r--   0        0        0     1584 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_web_rtc_authenticate_request.py
+-rw-r--r--   0        0        0     2173 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/post_webhook_request.py
+-rw-r--r--   0        0        0     1840 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/put_channel_subscribe_level_request.py
+-rw-r--r--   0        0        0     1623 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/put_channel_subscribers_request.py
+-rw-r--r--   0        0        0     1550 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/put_channel_topic_request.py
+-rw-r--r--   0        0        0     1816 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/put_my_password_request.py
+-rw-r--r--   0        0        0     1690 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/put_notify_citation_request.py
+-rw-r--r--   0        0        0     2027 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/put_user_icon_request.py
+-rw-r--r--   0        0        0     1630 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/put_user_password_request.py
+-rw-r--r--   0        0        0     2274 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/search_messages_message_search_result.py
+-rw-r--r--   0        0        0      233 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/search_messages_sort.py
+-rw-r--r--   0        0        0     2766 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/stamp.py
+-rw-r--r--   0        0        0     1841 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/stamp_history_entry.py
+-rw-r--r--   0        0        0     2915 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/stamp_palette.py
+-rw-r--r--   0        0        0     1829 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/stamp_stats.py
+-rw-r--r--   0        0        0     3122 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/stamp_with_thumbnail.py
+-rw-r--r--   0        0        0     1958 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/subscribers_changed_event.py
+-rw-r--r--   0        0        0     1771 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/tag.py
+-rw-r--r--   0        0        0     2272 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/thumbnail_info.py
+-rw-r--r--   0        0        0      164 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/thumbnail_type.py
+-rw-r--r--   0        0        0     1883 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/topic_changed_event.py
+-rw-r--r--   0        0        0     2941 2024-06-02 10:06:15.295746 aiotraq-0.1.2/aiotraq/models/unread_channel.py
+-rw-r--r--   0        0        0     2880 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user.py
+-rw-r--r--   0        0        0      170 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_account_state.py
+-rw-r--r--   0        0        0     5543 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_detail.py
+-rw-r--r--   0        0        0     3691 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_group.py
+-rw-r--r--   0        0        0     1639 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_group_member.py
+-rw-r--r--   0        0        0     3487 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_permission.py
+-rw-r--r--   0        0        0     1743 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_settings.py
+-rw-r--r--   0        0        0     2660 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_stats.py
+-rw-r--r--   0        0        0     1941 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_stats_stamp.py
+-rw-r--r--   0        0        0     1981 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_subscribe_state.py
+-rw-r--r--   0        0        0     2417 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/user_tag.py
+-rw-r--r--   0        0        0     2072 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/version.py
+-rw-r--r--   0        0        0     1915 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/version_flags.py
+-rw-r--r--   0        0        0     1790 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/visibility_changed_event.py
+-rw-r--r--   0        0        0     2140 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/web_rtc_authenticate_result.py
+-rw-r--r--   0        0        0     2542 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/web_rtc_user_state.py
+-rw-r--r--   0        0        0     1745 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/web_rtc_user_state_sessions_item.py
+-rw-r--r--   0        0        0     3327 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/models/webhook.py
+-rw-r--r--   0        0        0       25 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/py.typed
+-rw-r--r--   0        0        0      985 2024-06-02 10:06:15.299746 aiotraq-0.1.2/aiotraq/types.py
+-rw-r--r--   0        0        0     1130 2024-06-02 10:06:15.299746 aiotraq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 aiotraq-0.1.2/PKG-INFO
```

### Comparing `aiotraq-0.1.1/README.md` & `aiotraq-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # aiotraq
 
 Async ready traQ API Client for Python
 
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/aiotraq)](https://pypi.org/project/aiotraq/)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
+[![CI](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml/badge.svg)](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml)
 
 ## Installation
 
 ```bash
 pip install aiotraq
 ```
```

### Comparing `aiotraq-0.1.1/aiotraq/api/activity/get_activity_timeline.py` & `aiotraq-0.1.2/aiotraq/api/activity/get_activity_timeline.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/activity/get_online_users.py` & `aiotraq-0.1.2/aiotraq/api/activity/get_online_users.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/authentication/get_my_external_accounts.py` & `aiotraq-0.1.2/aiotraq/api/authentication/get_my_external_accounts.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/authentication/get_my_sessions.py` & `aiotraq-0.1.2/aiotraq/api/authentication/get_my_sessions.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/authentication/link_external_account.py` & `aiotraq-0.1.2/aiotraq/api/authentication/link_external_account.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/authentication/login.py` & `aiotraq-0.1.2/aiotraq/api/authentication/login.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/authentication/logout.py` & `aiotraq-0.1.2/aiotraq/api/authentication/logout.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/authentication/revoke_my_session.py` & `aiotraq-0.1.2/aiotraq/api/authentication/revoke_my_session.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/authentication/unlink_external_account.py` & `aiotraq-0.1.2/aiotraq/api/authentication/unlink_external_account.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/activate_bot.py` & `aiotraq-0.1.2/aiotraq/api/bot/activate_bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/change_bot_icon.py` & `aiotraq-0.1.2/aiotraq/api/bot/change_bot_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/connect_bot_ws.py` & `aiotraq-0.1.2/aiotraq/api/bot/connect_bot_ws.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/create_bot.py` & `aiotraq-0.1.2/aiotraq/api/bot/create_bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/delete_bot.py` & `aiotraq-0.1.2/aiotraq/api/bot/delete_bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/edit_bot.py` & `aiotraq-0.1.2/aiotraq/api/bot/edit_bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/get_bot.py` & `aiotraq-0.1.2/aiotraq/api/bot/get_bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/get_bot_icon.py` & `aiotraq-0.1.2/aiotraq/api/bot/get_bot_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/get_bot_logs.py` & `aiotraq-0.1.2/aiotraq/api/bot/get_bot_logs.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/get_bots.py` & `aiotraq-0.1.2/aiotraq/api/bot/get_bots.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/get_channel_bots.py` & `aiotraq-0.1.2/aiotraq/api/bot/get_channel_bots.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/inactivate_bot.py` & `aiotraq-0.1.2/aiotraq/api/bot/inactivate_bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/let_bot_join_channel.py` & `aiotraq-0.1.2/aiotraq/api/bot/let_bot_join_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/let_bot_leave_channel.py` & `aiotraq-0.1.2/aiotraq/api/bot/let_bot_leave_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/bot/reissue_bot.py` & `aiotraq-0.1.2/aiotraq/api/bot/reissue_bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/create_channel.py` & `aiotraq-0.1.2/aiotraq/api/channel/create_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/edit_channel.py` & `aiotraq-0.1.2/aiotraq/api/channel/edit_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/edit_channel_subscribers.py` & `aiotraq-0.1.2/aiotraq/api/channel/edit_channel_subscribers.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/edit_channel_topic.py` & `aiotraq-0.1.2/aiotraq/api/channel/edit_channel_topic.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channel.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channel_events.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channel_events.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channel_pins.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channel_pins.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channel_stats.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channel_stats.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channel_subscribers.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channel_subscribers.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channel_topic.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channel_topic.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channel_viewers.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channel_viewers.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_channels.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_channels.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/get_messages.py` & `aiotraq-0.1.2/aiotraq/api/channel/get_messages.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/channel/set_channel_subscribers.py` & `aiotraq-0.1.2/aiotraq/api/channel/set_channel_subscribers.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/clip_message.py` & `aiotraq-0.1.2/aiotraq/api/clip/clip_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/create_clip_folder.py` & `aiotraq-0.1.2/aiotraq/api/clip/create_clip_folder.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/delete_clip_folder.py` & `aiotraq-0.1.2/aiotraq/api/clip/delete_clip_folder.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/edit_clip_folder.py` & `aiotraq-0.1.2/aiotraq/api/clip/edit_clip_folder.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/get_clip_folder.py` & `aiotraq-0.1.2/aiotraq/api/clip/get_clip_folder.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/get_clip_folders.py` & `aiotraq-0.1.2/aiotraq/api/clip/get_clip_folders.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/get_clips.py` & `aiotraq-0.1.2/aiotraq/api/clip/get_clips.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/clip/unclip_message.py` & `aiotraq-0.1.2/aiotraq/api/clip/unclip_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/file/delete_file.py` & `aiotraq-0.1.2/aiotraq/api/file/delete_file.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/file/get_file.py` & `aiotraq-0.1.2/aiotraq/api/file/get_file.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/file/get_file_meta.py` & `aiotraq-0.1.2/aiotraq/api/file/get_file_meta.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/file/get_files.py` & `aiotraq-0.1.2/aiotraq/api/file/get_files.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/file/get_thumbnail_image.py` & `aiotraq-0.1.2/aiotraq/api/file/get_thumbnail_image.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/file/post_file.py` & `aiotraq-0.1.2/aiotraq/api/file/post_file.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/add_user_group_admin.py` & `aiotraq-0.1.2/aiotraq/api/group/add_user_group_admin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/add_user_group_member.py` & `aiotraq-0.1.2/aiotraq/api/group/add_user_group_member.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/change_user_group_icon.py` & `aiotraq-0.1.2/aiotraq/api/group/change_user_group_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/create_user_group.py` & `aiotraq-0.1.2/aiotraq/api/group/create_user_group.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/delete_user_group.py` & `aiotraq-0.1.2/aiotraq/api/group/delete_user_group.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/edit_user_group.py` & `aiotraq-0.1.2/aiotraq/api/group/edit_user_group.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/edit_user_group_member.py` & `aiotraq-0.1.2/aiotraq/api/group/edit_user_group_member.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/get_user_group.py` & `aiotraq-0.1.2/aiotraq/api/group/get_user_group.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/get_user_group_admins.py` & `aiotraq-0.1.2/aiotraq/api/group/get_user_group_admins.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/get_user_group_members.py` & `aiotraq-0.1.2/aiotraq/api/group/get_user_group_members.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/get_user_groups.py` & `aiotraq-0.1.2/aiotraq/api/group/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/remove_user_group_admin.py` & `aiotraq-0.1.2/aiotraq/api/group/remove_user_group_admin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/group/remove_user_group_member.py` & `aiotraq-0.1.2/aiotraq/api/group/remove_user_group_member.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/add_my_star.py` & `aiotraq-0.1.2/aiotraq/api/me/add_my_star.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/add_my_user_tag.py` & `aiotraq-0.1.2/aiotraq/api/me/add_my_user_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/change_my_icon.py` & `aiotraq-0.1.2/aiotraq/api/me/change_my_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/change_my_notify_citation.py` & `aiotraq-0.1.2/aiotraq/api/me/change_my_notify_citation.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/change_my_password.py` & `aiotraq-0.1.2/aiotraq/api/me/change_my_password.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/edit_me.py` & `aiotraq-0.1.2/aiotraq/api/me/edit_me.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_me.py` & `aiotraq-0.1.2/aiotraq/api/me/get_me.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_channel_subscriptions.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_channel_subscriptions.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_icon.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_notify_citation.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_notify_citation.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_qr_code.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_qr_code.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_stars.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_stars.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_unread_channels.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_unread_channels.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_user_tags.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_user_tags.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_my_view_states.py` & `aiotraq-0.1.2/aiotraq/api/me/get_my_view_states.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_oidc_user_info.py` & `aiotraq-0.1.2/aiotraq/api/me/get_oidc_user_info.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/get_user_settings.py` & `aiotraq-0.1.2/aiotraq/api/me/get_user_settings.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/read_channel.py` & `aiotraq-0.1.2/aiotraq/api/me/read_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/register_fcm_device.py` & `aiotraq-0.1.2/aiotraq/api/me/register_fcm_device.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/remove_my_star.py` & `aiotraq-0.1.2/aiotraq/api/me/remove_my_star.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/me/set_channel_subscribe_level.py` & `aiotraq-0.1.2/aiotraq/api/me/set_channel_subscribe_level.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/add_message_stamp.py` & `aiotraq-0.1.2/aiotraq/api/message/add_message_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/create_pin.py` & `aiotraq-0.1.2/aiotraq/api/message/create_pin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/delete_message.py` & `aiotraq-0.1.2/aiotraq/api/message/delete_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/edit_message.py` & `aiotraq-0.1.2/aiotraq/api/message/edit_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/get_direct_messages.py` & `aiotraq-0.1.2/aiotraq/api/message/get_direct_messages.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/get_message.py` & `aiotraq-0.1.2/aiotraq/api/message/get_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/get_message_clips.py` & `aiotraq-0.1.2/aiotraq/api/message/get_message_clips.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/get_message_stamps.py` & `aiotraq-0.1.2/aiotraq/api/message/get_message_stamps.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/get_pin.py` & `aiotraq-0.1.2/aiotraq/api/message/get_pin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/post_direct_message.py` & `aiotraq-0.1.2/aiotraq/api/message/post_direct_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/post_message.py` & `aiotraq-0.1.2/aiotraq/api/message/post_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/remove_message_stamp.py` & `aiotraq-0.1.2/aiotraq/api/message/remove_message_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/remove_pin.py` & `aiotraq-0.1.2/aiotraq/api/message/remove_pin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/message/search_messages.py` & `aiotraq-0.1.2/aiotraq/api/message/search_messages.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/notification/ws.py` & `aiotraq-0.1.2/aiotraq/api/notification/ws.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/create_client.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/create_client.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/delete_client.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/delete_client.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/edit_client.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/edit_client.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/get_client.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/get_client.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/get_clients.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/get_clients.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/get_my_tokens.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/get_my_tokens.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/get_o_auth_2_authorize.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/get_o_auth_2_authorize.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/post_o_auth_2_authorize.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/post_o_auth_2_authorize.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/post_o_auth_2_authorize_decide.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/post_o_auth_2_authorize_decide.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/post_o_auth_2_token.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/post_o_auth_2_token.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/revoke_my_token.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/revoke_my_token.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/oauth2/revoke_o_auth_2_token.py` & `aiotraq-0.1.2/aiotraq/api/oauth2/revoke_o_auth_2_token.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/ogp/delete_ogp_cache.py` & `aiotraq-0.1.2/aiotraq/api/ogp/delete_ogp_cache.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/ogp/get_ogp.py` & `aiotraq-0.1.2/aiotraq/api/ogp/get_ogp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/public/get_public_user_icon.py` & `aiotraq-0.1.2/aiotraq/api/public/get_public_user_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/public/get_server_version.py` & `aiotraq-0.1.2/aiotraq/api/public/get_server_version.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/change_stamp_image.py` & `aiotraq-0.1.2/aiotraq/api/stamp/change_stamp_image.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/create_stamp.py` & `aiotraq-0.1.2/aiotraq/api/stamp/create_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/create_stamp_palette.py` & `aiotraq-0.1.2/aiotraq/api/stamp/create_stamp_palette.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/delete_stamp.py` & `aiotraq-0.1.2/aiotraq/api/stamp/delete_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/delete_stamp_palette.py` & `aiotraq-0.1.2/aiotraq/api/stamp/delete_stamp_palette.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/edit_stamp.py` & `aiotraq-0.1.2/aiotraq/api/stamp/edit_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/edit_stamp_palette.py` & `aiotraq-0.1.2/aiotraq/api/stamp/edit_stamp_palette.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/get_my_stamp_history.py` & `aiotraq-0.1.2/aiotraq/api/stamp/get_my_stamp_history.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/get_stamp.py` & `aiotraq-0.1.2/aiotraq/api/stamp/get_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_image.py` & `aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_image.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_palette.py` & `aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_palette.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_palettes.py` & `aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_palettes.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/get_stamp_stats.py` & `aiotraq-0.1.2/aiotraq/api/stamp/get_stamp_stats.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/stamp/get_stamps.py` & `aiotraq-0.1.2/aiotraq/api/stamp/get_stamps.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/add_user_tag.py` & `aiotraq-0.1.2/aiotraq/api/user/add_user_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/change_user_icon.py` & `aiotraq-0.1.2/aiotraq/api/user/change_user_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/change_user_password.py` & `aiotraq-0.1.2/aiotraq/api/user/change_user_password.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/create_user.py` & `aiotraq-0.1.2/aiotraq/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/edit_user.py` & `aiotraq-0.1.2/aiotraq/api/user/edit_user.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/edit_user_tag.py` & `aiotraq-0.1.2/aiotraq/api/user/edit_user_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/get_user.py` & `aiotraq-0.1.2/aiotraq/api/user/get_user.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/get_user_dm_channel.py` & `aiotraq-0.1.2/aiotraq/api/user/get_user_dm_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/get_user_icon.py` & `aiotraq-0.1.2/aiotraq/api/user/get_user_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/get_user_stats.py` & `aiotraq-0.1.2/aiotraq/api/user/get_user_stats.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/get_user_tags.py` & `aiotraq-0.1.2/aiotraq/api/user/get_user_tags.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/get_users.py` & `aiotraq-0.1.2/aiotraq/api/user/get_users.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user/remove_user_tag.py` & `aiotraq-0.1.2/aiotraq/api/user/remove_user_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user_tag/edit_my_user_tag.py` & `aiotraq-0.1.2/aiotraq/api/user_tag/edit_my_user_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user_tag/get_tag.py` & `aiotraq-0.1.2/aiotraq/api/user_tag/get_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/user_tag/remove_my_user_tag.py` & `aiotraq-0.1.2/aiotraq/api/user_tag/remove_my_user_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/change_webhook_icon.py` & `aiotraq-0.1.2/aiotraq/api/webhook/change_webhook_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/create_webhook.py` & `aiotraq-0.1.2/aiotraq/api/webhook/create_webhook.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/delete_webhook.py` & `aiotraq-0.1.2/aiotraq/api/webhook/delete_webhook.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/edit_webhook.py` & `aiotraq-0.1.2/aiotraq/api/webhook/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/get_webhook.py` & `aiotraq-0.1.2/aiotraq/api/webhook/get_webhook.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/get_webhook_icon.py` & `aiotraq-0.1.2/aiotraq/api/webhook/get_webhook_icon.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/get_webhook_messages.py` & `aiotraq-0.1.2/aiotraq/api/webhook/get_webhook_messages.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webhook/get_webhooks.py` & `aiotraq-0.1.2/aiotraq/api/webhook/get_webhooks.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webrtc/get_web_rtc_state.py` & `aiotraq-0.1.2/aiotraq/api/webrtc/get_web_rtc_state.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/api/webrtc/post_web_rtc_authenticate.py` & `aiotraq-0.1.2/aiotraq/api/webrtc/post_web_rtc_authenticate.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/client.py` & `aiotraq-0.1.2/aiotraq/client.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/errors.py` & `aiotraq-0.1.2/aiotraq/errors.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/__init__.py` & `aiotraq-0.1.2/aiotraq/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/active_o_auth_2_token.py` & `aiotraq-0.1.2/aiotraq/models/active_o_auth_2_token.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/activity_timeline_message.py` & `aiotraq-0.1.2/aiotraq/models/activity_timeline_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/bot.py` & `aiotraq-0.1.2/aiotraq/models/bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/bot_detail.py` & `aiotraq-0.1.2/aiotraq/models/bot_detail.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/bot_event_log.py` & `aiotraq-0.1.2/aiotraq/models/bot_event_log.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/bot_tokens.py` & `aiotraq-0.1.2/aiotraq/models/bot_tokens.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/bot_user.py` & `aiotraq-0.1.2/aiotraq/models/bot_user.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/change_stamp_image_body.py` & `aiotraq-0.1.2/aiotraq/models/change_stamp_image_body.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel.py` & `aiotraq-0.1.2/aiotraq/models/channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel_event.py` & `aiotraq-0.1.2/aiotraq/models/channel_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel_list.py` & `aiotraq-0.1.2/aiotraq/models/channel_list.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel_stats.py` & `aiotraq-0.1.2/aiotraq/models/channel_stats.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel_stats_stamp.py` & `aiotraq-0.1.2/aiotraq/models/channel_stats_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel_stats_user.py` & `aiotraq-0.1.2/aiotraq/models/channel_stats_user.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel_topic.py` & `aiotraq-0.1.2/aiotraq/models/channel_topic.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/channel_viewer.py` & `aiotraq-0.1.2/aiotraq/models/channel_viewer.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/child_created_event.py` & `aiotraq-0.1.2/aiotraq/models/child_created_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/clip_folder.py` & `aiotraq-0.1.2/aiotraq/models/clip_folder.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/clipped_message.py` & `aiotraq-0.1.2/aiotraq/models/clipped_message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/dm_channel.py` & `aiotraq-0.1.2/aiotraq/models/dm_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/external_provider_user.py` & `aiotraq-0.1.2/aiotraq/models/external_provider_user.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/file_info.py` & `aiotraq-0.1.2/aiotraq/models/file_info.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/file_info_thumbnail_type_0.py` & `aiotraq-0.1.2/aiotraq/models/file_info_thumbnail_type_0.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/forced_notification_changed_event.py` & `aiotraq-0.1.2/aiotraq/models/forced_notification_changed_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/get_notify_citation.py` & `aiotraq-0.1.2/aiotraq/models/get_notify_citation.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/login_session.py` & `aiotraq-0.1.2/aiotraq/models/login_session.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/message.py` & `aiotraq-0.1.2/aiotraq/models/message.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/message_clip.py` & `aiotraq-0.1.2/aiotraq/models/message_clip.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/message_pin.py` & `aiotraq-0.1.2/aiotraq/models/message_pin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/message_stamp.py` & `aiotraq-0.1.2/aiotraq/models/message_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/my_channel_view_state.py` & `aiotraq-0.1.2/aiotraq/models/my_channel_view_state.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/my_user_detail.py` & `aiotraq-0.1.2/aiotraq/models/my_user_detail.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/name_changed_event.py` & `aiotraq-0.1.2/aiotraq/models/name_changed_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/o_auth_2_authorization.py` & `aiotraq-0.1.2/aiotraq/models/o_auth_2_authorization.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/o_auth_2_client.py` & `aiotraq-0.1.2/aiotraq/models/o_auth_2_client.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/o_auth_2_client_detail.py` & `aiotraq-0.1.2/aiotraq/models/o_auth_2_client_detail.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/o_auth_2_decide.py` & `aiotraq-0.1.2/aiotraq/models/o_auth_2_decide.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/o_auth_2_revoke.py` & `aiotraq-0.1.2/aiotraq/models/o_auth_2_revoke.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/o_auth_2_token.py` & `aiotraq-0.1.2/aiotraq/models/o_auth_2_token.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/ogp.py` & `aiotraq-0.1.2/aiotraq/models/ogp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/ogp_media.py` & `aiotraq-0.1.2/aiotraq/models/ogp_media.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/oidc_traq_user_info.py` & `aiotraq-0.1.2/aiotraq/models/oidc_traq_user_info.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/oidc_user_info.py` & `aiotraq-0.1.2/aiotraq/models/oidc_user_info.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/parent_changed_event.py` & `aiotraq-0.1.2/aiotraq/models/parent_changed_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_bot_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_bot_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_channel_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_channel_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_channel_subscribers_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_channel_subscribers_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_client_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_client_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_clip_folder_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_clip_folder_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_group_member_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_group_member_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_me_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_me_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_stamp_palette_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_stamp_palette_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_stamp_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_stamp_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_user_group_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_user_group_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_user_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_user_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_user_tag_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_user_tag_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/patch_webhook_request.py` & `aiotraq-0.1.2/aiotraq/models/patch_webhook_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/pin.py` & `aiotraq-0.1.2/aiotraq/models/pin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/pin_added_event.py` & `aiotraq-0.1.2/aiotraq/models/pin_added_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/pin_removed_event.py` & `aiotraq-0.1.2/aiotraq/models/pin_removed_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_bot_action_join_request.py` & `aiotraq-0.1.2/aiotraq/models/post_bot_action_join_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_bot_action_leave_request.py` & `aiotraq-0.1.2/aiotraq/models/post_bot_action_leave_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_bot_request.py` & `aiotraq-0.1.2/aiotraq/models/post_bot_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_channel_request.py` & `aiotraq-0.1.2/aiotraq/models/post_channel_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_client_request.py` & `aiotraq-0.1.2/aiotraq/models/post_client_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_clip_folder_message_request.py` & `aiotraq-0.1.2/aiotraq/models/post_clip_folder_message_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_clip_folder_request.py` & `aiotraq-0.1.2/aiotraq/models/post_clip_folder_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_file_request.py` & `aiotraq-0.1.2/aiotraq/models/post_file_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_link_external_account.py` & `aiotraq-0.1.2/aiotraq/models/post_link_external_account.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_login_request.py` & `aiotraq-0.1.2/aiotraq/models/post_login_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_message_request.py` & `aiotraq-0.1.2/aiotraq/models/post_message_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_message_stamp_request.py` & `aiotraq-0.1.2/aiotraq/models/post_message_stamp_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_my_fcm_device_request.py` & `aiotraq-0.1.2/aiotraq/models/post_my_fcm_device_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_o_auth_2_token.py` & `aiotraq-0.1.2/aiotraq/models/post_o_auth_2_token.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_stamp_palette_request.py` & `aiotraq-0.1.2/aiotraq/models/post_stamp_palette_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_stamp_request.py` & `aiotraq-0.1.2/aiotraq/models/post_stamp_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_star_request.py` & `aiotraq-0.1.2/aiotraq/models/post_star_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_unlink_external_account.py` & `aiotraq-0.1.2/aiotraq/models/post_unlink_external_account.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_user_group_admin.py` & `aiotraq-0.1.2/aiotraq/models/post_user_group_admin.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_user_group_request.py` & `aiotraq-0.1.2/aiotraq/models/post_user_group_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_user_request.py` & `aiotraq-0.1.2/aiotraq/models/post_user_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_user_tag_request.py` & `aiotraq-0.1.2/aiotraq/models/post_user_tag_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_web_rtc_authenticate_request.py` & `aiotraq-0.1.2/aiotraq/models/post_web_rtc_authenticate_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/post_webhook_request.py` & `aiotraq-0.1.2/aiotraq/models/post_webhook_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/put_channel_subscribe_level_request.py` & `aiotraq-0.1.2/aiotraq/models/put_channel_subscribe_level_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/put_channel_subscribers_request.py` & `aiotraq-0.1.2/aiotraq/models/put_channel_subscribers_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/put_channel_topic_request.py` & `aiotraq-0.1.2/aiotraq/models/put_channel_topic_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/put_my_password_request.py` & `aiotraq-0.1.2/aiotraq/models/put_my_password_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/put_notify_citation_request.py` & `aiotraq-0.1.2/aiotraq/models/put_notify_citation_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/put_user_icon_request.py` & `aiotraq-0.1.2/aiotraq/models/put_user_icon_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/put_user_password_request.py` & `aiotraq-0.1.2/aiotraq/models/put_user_password_request.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/search_messages_message_search_result.py` & `aiotraq-0.1.2/aiotraq/models/search_messages_message_search_result.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/stamp.py` & `aiotraq-0.1.2/aiotraq/models/stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/stamp_history_entry.py` & `aiotraq-0.1.2/aiotraq/models/stamp_history_entry.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/stamp_palette.py` & `aiotraq-0.1.2/aiotraq/models/stamp_palette.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/stamp_stats.py` & `aiotraq-0.1.2/aiotraq/models/stamp_stats.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/stamp_with_thumbnail.py` & `aiotraq-0.1.2/aiotraq/models/stamp_with_thumbnail.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/subscribers_changed_event.py` & `aiotraq-0.1.2/aiotraq/models/subscribers_changed_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/tag.py` & `aiotraq-0.1.2/aiotraq/models/tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/thumbnail_info.py` & `aiotraq-0.1.2/aiotraq/models/thumbnail_info.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/topic_changed_event.py` & `aiotraq-0.1.2/aiotraq/models/topic_changed_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/unread_channel.py` & `aiotraq-0.1.2/aiotraq/models/unread_channel.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user.py` & `aiotraq-0.1.2/aiotraq/models/user.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_detail.py` & `aiotraq-0.1.2/aiotraq/models/user_detail.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_group.py` & `aiotraq-0.1.2/aiotraq/models/user_group.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_group_member.py` & `aiotraq-0.1.2/aiotraq/models/user_group_member.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_permission.py` & `aiotraq-0.1.2/aiotraq/models/user_permission.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_settings.py` & `aiotraq-0.1.2/aiotraq/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_stats.py` & `aiotraq-0.1.2/aiotraq/models/user_stats.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_stats_stamp.py` & `aiotraq-0.1.2/aiotraq/models/user_stats_stamp.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_subscribe_state.py` & `aiotraq-0.1.2/aiotraq/models/user_subscribe_state.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/user_tag.py` & `aiotraq-0.1.2/aiotraq/models/user_tag.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/version.py` & `aiotraq-0.1.2/aiotraq/models/version.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/version_flags.py` & `aiotraq-0.1.2/aiotraq/models/version_flags.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/visibility_changed_event.py` & `aiotraq-0.1.2/aiotraq/models/visibility_changed_event.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/web_rtc_authenticate_result.py` & `aiotraq-0.1.2/aiotraq/models/web_rtc_authenticate_result.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/web_rtc_user_state.py` & `aiotraq-0.1.2/aiotraq/models/web_rtc_user_state.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/web_rtc_user_state_sessions_item.py` & `aiotraq-0.1.2/aiotraq/models/web_rtc_user_state_sessions_item.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/models/webhook.py` & `aiotraq-0.1.2/aiotraq/models/webhook.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/aiotraq/types.py` & `aiotraq-0.1.2/aiotraq/types.py`

 * *Files identical despite different names*

### Comparing `aiotraq-0.1.1/pyproject.toml` & `aiotraq-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiotraq"
-version = "0.1.1"
+version = "0.1.2"
 description = "Async ready traQ API Client"
 authors = ["toshi00"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "aiotraq" }]
 include = ["aiotraq/py.typed"]
 repository = "https://github.com/toshi-pono/aiotraq"
@@ -19,19 +19,30 @@
 python = ">=3.8,<4.0"
 httpx = ">=0.20.0,<0.28.0"
 attrs = ">=21.3.0"
 python-dateutil = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 types-python-dateutil = "^2.8.0"
+mypy = "^1.10.0"
+ruff = "^0.4.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.mypy]
+show_error_context = true
+show_column_numbers = true
+ignore_missing_imports = true
+disallow_untyped_defs = true
+no_implicit_optional = true
+warn_return_any = false
+check_untyped_defs = true
+
 
 [tool.ruff]
 exclude = [".venv", "venv", "__pycache__", ".git"]
 
 line-length = 120
 indent-width = 4
```

### Comparing `aiotraq-0.1.1/PKG-INFO` & `aiotraq-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotraq
-Version: 0.1.1
+Version: 0.1.2
 Summary: Async ready traQ API Client
 Home-page: https://github.com/toshi-pono/aiotraq
 License: MIT
 Keywords: traQ,API,async,httpx
 Author: toshi00
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,16 +21,17 @@
 Project-URL: Source Code, https://github.com/toshi-pono/aiotraq/tree/main/libs/aiotraq
 Description-Content-Type: text/markdown
 
 # aiotraq
 
 Async ready traQ API Client for Python
 
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/aiotraq)](https://pypi.org/project/aiotraq/)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
+[![CI](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml/badge.svg)](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml)
 
 ## Installation
 
 ```bash
 pip install aiotraq
 ```
```


# Comparing `tmp/discord_typings-0.8.0.tar.gz` & `tmp/discord_typings-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_typings-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "discord_typings-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `discord_typings-0.8.0.tar` & `discord_typings-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0      172 2024-01-22 22:53:15.151029 discord_typings-0.8.0/.flake8
--rw-r--r--   0        0        0      486 2024-01-22 22:53:30.239519 discord_typings-0.8.0/.github/workflows/import.yml
--rw-r--r--   0        0        0     1369 2024-01-22 22:53:30.251479 discord_typings-0.8.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1077 2024-01-22 22:53:15.159002 discord_typings-0.8.0/.gitignore
--rw-r--r--   0        0        0       61 2024-01-22 22:53:15.167973 discord_typings-0.8.0/.isort.cfg
--rw-r--r--   0        0        0     1102 2024-01-22 22:53:15.175946 discord_typings-0.8.0/LICENSE
--rw-r--r--   0        0        0     4858 2024-01-22 22:53:15.198869 discord_typings-0.8.0/README.md
--rw-r--r--   0        0        0     1243 2024-03-21 23:16:54.001405 discord_typings-0.8.0/discord_typings/__init__.py
--rw-r--r--   0        0        0    38225 2024-03-21 23:16:54.002401 discord_typings-0.8.0/discord_typings/_gateway.py
--rw-r--r--   0        0        0    11994 2024-03-21 23:17:28.127199 discord_typings-0.8.0/discord_typings/_interactions/_commands.py
--rw-r--r--   0        0        0     5361 2024-03-21 23:16:53.509415 discord_typings-0.8.0/discord_typings/_interactions/_components.py
--rw-r--r--   0        0        0    12176 2024-03-21 23:18:46.916533 discord_typings-0.8.0/discord_typings/_interactions/_receiving.py
--rw-r--r--   0        0        0      791 2024-03-21 23:16:54.004395 discord_typings-0.8.0/discord_typings/_monetization/_entitlements.py
--rw-r--r--   0        0        0     1596 2024-01-22 22:53:30.928213 discord_typings-0.8.0/discord_typings/_oauth.py
--rw-r--r--   0        0        0     1558 2024-03-21 22:04:38.235190 discord_typings-0.8.0/discord_typings/_reference.py
--rw-r--r--   0        0        0     3023 2024-03-21 23:19:56.968095 discord_typings-0.8.0/discord_typings/_resources/_application.py
--rw-r--r--   0        0        0     3121 2024-01-22 22:53:31.166416 discord_typings-0.8.0/discord_typings/_resources/_audit_log.py
--rw-r--r--   0        0        0     5514 2024-03-21 22:05:25.813780 discord_typings-0.8.0/discord_typings/_resources/_auto_moderation.py
--rw-r--r--   0        0        0    17777 2024-03-24 15:47:25.916614 discord_typings-0.8.0/discord_typings/_resources/_channel.py
--rw-r--r--   0        0        0      570 2024-01-22 22:53:31.202296 discord_typings-0.8.0/discord_typings/_resources/_emoji.py
--rw-r--r--   0        0        0    12963 2024-03-24 15:47:26.253848 discord_typings-0.8.0/discord_typings/_resources/_guild.py
--rw-r--r--   0        0        0     3102 2024-01-22 22:53:31.224223 discord_typings-0.8.0/discord_typings/_resources/_guild_scheduled_events.py
--rw-r--r--   0        0        0      615 2024-01-22 22:53:31.234190 discord_typings-0.8.0/discord_typings/_resources/_guild_template.py
--rw-r--r--   0        0        0     1722 2024-01-22 22:53:31.244156 discord_typings-0.8.0/discord_typings/_resources/_invite.py
--rw-r--r--   0        0        0      982 2024-01-22 22:53:31.253126 discord_typings-0.8.0/discord_typings/_resources/_role_connection_metadata.py
--rw-r--r--   0        0        0      802 2024-01-22 22:53:31.262096 discord_typings-0.8.0/discord_typings/_resources/_stage_instance.py
--rw-r--r--   0        0        0     1712 2024-01-22 22:53:31.272063 discord_typings-0.8.0/discord_typings/_resources/_sticker.py
--rw-r--r--   0        0        0     2471 2024-01-22 22:53:31.282030 discord_typings-0.8.0/discord_typings/_resources/_user.py
--rw-r--r--   0        0        0      975 2024-01-22 22:53:31.293989 discord_typings-0.8.0/discord_typings/_resources/_voice.py
--rw-r--r--   0        0        0      984 2024-01-22 22:53:31.305949 discord_typings-0.8.0/discord_typings/_resources/_webhook.py
--rw-r--r--   0        0        0        0 2024-01-22 22:53:30.904294 discord_typings-0.8.0/discord_typings/py.typed
--rw-r--r--   0        0        0     1709 2024-03-24 15:51:45.379700 discord_typings-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6139 1970-01-01 00:00:00.000000 discord_typings-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      172 2024-01-22 22:53:15.151029 discord_typings-0.9.0/.flake8
+-rw-r--r--   0        0        0      486 2024-01-22 22:53:30.239519 discord_typings-0.9.0/.github/workflows/import.yml
+-rw-r--r--   0        0        0     1369 2024-01-22 22:53:30.251479 discord_typings-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1077 2024-01-22 22:53:15.159002 discord_typings-0.9.0/.gitignore
+-rw-r--r--   0        0        0       61 2024-01-22 22:53:15.167973 discord_typings-0.9.0/.isort.cfg
+-rw-r--r--   0        0        0     1102 2024-01-22 22:53:15.175946 discord_typings-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4858 2024-01-22 22:53:15.198869 discord_typings-0.9.0/README.md
+-rw-r--r--   0        0        0     1312 2024-06-02 19:02:51.719414 discord_typings-0.9.0/discord_typings/__init__.py
+-rw-r--r--   0        0        0    39507 2024-06-02 19:02:51.719414 discord_typings-0.9.0/discord_typings/_gateway.py
+-rw-r--r--   0        0        0    11994 2024-04-01 22:52:30.320200 discord_typings-0.9.0/discord_typings/_interactions/_commands.py
+-rw-r--r--   0        0        0     5361 2024-04-01 22:52:30.321196 discord_typings-0.9.0/discord_typings/_interactions/_components.py
+-rw-r--r--   0        0        0    12287 2024-06-02 19:02:51.719414 discord_typings-0.9.0/discord_typings/_interactions/_receiving.py
+-rw-r--r--   0        0        0      889 2024-06-02 19:02:51.719414 discord_typings-0.9.0/discord_typings/_monetization/_entitlements.py
+-rw-r--r--   0        0        0      542 2024-06-02 19:02:51.720915 discord_typings-0.9.0/discord_typings/_monetization/_skus.py
+-rw-r--r--   0        0        0     1596 2024-01-22 22:53:30.928213 discord_typings-0.9.0/discord_typings/_oauth.py
+-rw-r--r--   0        0        0     1558 2024-04-01 22:52:30.321196 discord_typings-0.9.0/discord_typings/_reference.py
+-rw-r--r--   0        0        0     3023 2024-04-01 22:52:30.321196 discord_typings-0.9.0/discord_typings/_resources/_application.py
+-rw-r--r--   0        0        0     3167 2024-06-02 19:02:51.720915 discord_typings-0.9.0/discord_typings/_resources/_audit_log.py
+-rw-r--r--   0        0        0     6072 2024-06-02 19:02:51.720915 discord_typings-0.9.0/discord_typings/_resources/_auto_moderation.py
+-rw-r--r--   0        0        0    18288 2024-06-02 19:02:51.720915 discord_typings-0.9.0/discord_typings/_resources/_channel.py
+-rw-r--r--   0        0        0      570 2024-01-22 22:53:31.202296 discord_typings-0.9.0/discord_typings/_resources/_emoji.py
+-rw-r--r--   0        0        0    13311 2024-06-02 19:02:51.721935 discord_typings-0.9.0/discord_typings/_resources/_guild.py
+-rw-r--r--   0        0        0     3102 2024-01-22 22:53:31.224223 discord_typings-0.9.0/discord_typings/_resources/_guild_scheduled_events.py
+-rw-r--r--   0        0        0      615 2024-01-22 22:53:31.234190 discord_typings-0.9.0/discord_typings/_resources/_guild_template.py
+-rw-r--r--   0        0        0     1906 2024-06-02 19:02:51.721935 discord_typings-0.9.0/discord_typings/_resources/_invite.py
+-rw-r--r--   0        0        0     2060 2024-06-02 19:02:51.721935 discord_typings-0.9.0/discord_typings/_resources/_poll.py
+-rw-r--r--   0        0        0      982 2024-01-22 22:53:31.253126 discord_typings-0.9.0/discord_typings/_resources/_role_connection_metadata.py
+-rw-r--r--   0        0        0      802 2024-01-22 22:53:31.262096 discord_typings-0.9.0/discord_typings/_resources/_stage_instance.py
+-rw-r--r--   0        0        0     1712 2024-01-22 22:53:31.272063 discord_typings-0.9.0/discord_typings/_resources/_sticker.py
+-rw-r--r--   0        0        0     2771 2024-06-02 19:02:51.721935 discord_typings-0.9.0/discord_typings/_resources/_user.py
+-rw-r--r--   0        0        0      975 2024-01-22 22:53:31.293989 discord_typings-0.9.0/discord_typings/_resources/_voice.py
+-rw-r--r--   0        0        0      984 2024-01-22 22:53:31.305949 discord_typings-0.9.0/discord_typings/_resources/_webhook.py
+-rw-r--r--   0        0        0        0 2024-01-22 22:53:30.904294 discord_typings-0.9.0/discord_typings/py.typed
+-rw-r--r--   0        0        0     1709 2024-06-02 19:04:43.374924 discord_typings-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6139 1970-01-01 00:00:00.000000 discord_typings-0.9.0/PKG-INFO
```

### Comparing `discord_typings-0.8.0/.github/workflows/lint.yml` & `discord_typings-0.9.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/.gitignore` & `discord_typings-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/LICENSE` & `discord_typings-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/README.md` & `discord_typings-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/__init__.py` & `discord_typings-0.9.0/discord_typings/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 # User needs to be imported before channel, due to UserMentionData subclass
 from ._resources._user import *
 
 from ._interactions._commands import *
 from ._interactions._components import *
 from ._interactions._receiving import *
 from ._monetization._entitlements import *
+from ._monetization._skus import *
 from ._oauth import *
 from ._reference import *
 from ._resources._application import *
 from ._resources._audit_log import *
 from ._resources._auto_moderation import *
 from ._resources._channel import *
 from ._resources._emoji import *
 from ._resources._guild import *
 from ._resources._guild_scheduled_events import *
 from ._resources._guild_template import *
 from ._resources._invite import *
+from ._resources._poll import *
 from ._resources._role_connection_metadata import *
 from ._resources._stage_instance import *
 from ._resources._sticker import *
 from ._resources._voice import *
 from ._resources._webhook import *
 
 # Gateway imports several other things, so it is imported last
```

### Comparing `discord_typings-0.8.0/discord_typings/_gateway.py` & `discord_typings-0.9.0/discord_typings/_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,18 @@
     'InteractionCreateEvent',
     'StageInstanceCreateData',
     'StageInstanceCreateEvent',
     'StageInstanceUpdateData',
     'StageInstanceUpdateEvent',
     'StageInstanceDeleteData',
     'StageInstanceDeleteEvent',
+    'MessagePollVoteAddData',
+    'MessagePollVoteAddEvent',
+    'MessagePollVoteRemoveData',
+    'MessagePollVoteRemoveEvent',
     'DispatchEvent',
     'GatewayCommand',
     'GatewayEvent',
 )
 
 
 _D = TypeVar('_D', bound='Mapping[str, Any]')
@@ -663,15 +667,18 @@
 GuildDeleteData: TypeAlias = 'discord_typings.UnavailableGuildData'
 GuildDeleteEvent = GenericDispatchEvent[Literal['GUILD_DELETE'], 'GuildDeleteData']
 
 
 # https://discord.com/developers/docs/topics/gateway-events#guild-audit-log-entry-create
 
 
-GuildAuditLogEntryCreateData: TypeAlias = 'discord_typings.AuditLogEntryData'
+class GuildAuditLogEntryCreateData(discord_typings.AuditLogEntryData):
+    guild_id: 'discord_typings.Snowflake'  # Extra field
+
+
 GuildAuditLogEntryCreateEvent = GenericDispatchEvent[
     Literal['GUILD_AUDIT_LOG_ENTRY_CREATE'],
     GuildAuditLogEntryCreateData
 ]
 
 
 # https://discord.com/developers/docs/topics/gateway-events#guild-ban-add
@@ -1051,14 +1058,17 @@
     user_id: 'discord_typings.Snowflake'
     channel_id: 'discord_typings.Snowflake'
     message_id: 'discord_typings.Snowflake'
     guild_id: NotRequired['discord_typings.Snowflake']
     member: NotRequired['discord_typings.GuildMemberData']
     emoji: 'discord_typings.EmojiData'
     message_author_id: NotRequired['discord_typings.Snowflake']
+    burst: bool
+    burst_colors: NotRequired[List[str]]
+    type: 'discord_typings.ReactionTypes'
 
 
 MessageReactionAddEvent = GenericDispatchEvent[
     Literal['MESSAGE_REACTION_ADD'], MessageReactionAddData
 ]
 
 
@@ -1067,14 +1077,16 @@
 
 class MessageReactionRemoveData(TypedDict):
     user_id: 'discord_typings.Snowflake'
     channel_id: 'discord_typings.Snowflake'
     message_id: 'discord_typings.Snowflake'
     guild_id: NotRequired['discord_typings.Snowflake']
     emoji: 'discord_typings.EmojiData'
+    burst: bool
+    type: 'discord_typings.ReactionTypes'
 
 
 MessageReactionRemoveEvent = GenericDispatchEvent[
     Literal['MESSAGE_REACTION_REMOVE'], MessageReactionRemoveData
 ]
 
 
@@ -1297,14 +1309,46 @@
 
 StageInstanceDeleteData: TypeAlias = 'discord_typings.StageInstanceData'
 StageInstanceDeleteEvent = GenericDispatchEvent[
     Literal['STAGE_INSTANCE_DELETE'], StageInstanceDeleteData
 ]
 
 
+# https://discord.com/developers/docs/topics/gateway-events#message-poll-vote-add
+
+
+class MessagePollVoteAddData(TypedDict):
+    user_id: 'discord_typings.Snowflake'
+    channel_id: 'discord_typings.Snowflake'
+    message_id: 'discord_typings.Snowflake'
+    guild_id: NotRequired['discord_typings.Snowflake']
+    answer_id: int
+
+
+MessagePollVoteAddEvent = GenericDispatchEvent[
+    Literal['MESSAGE_POLL_VOTE_ADD'], MessagePollVoteAddData
+]
+
+
+# https://discord.com/developers/docs/topics/gateway-events#message-poll-vote-remove
+
+
+class MessagePollVoteRemoveData(TypedDict):
+    user_id: 'discord_typings.Snowflake'
+    channel_id: 'discord_typings.Snowflake'
+    message_id: 'discord_typings.Snowflake'
+    guild_id: NotRequired['discord_typings.Snowflake']
+    answer_id: int
+
+
+MessagePollVoteRemoveEvent = GenericDispatchEvent[
+    Literal['MESSAGE_POLL_VOTE_REMOVE'], MessagePollVoteRemoveData
+]
+
+
 # Generalized unions for the typings in this file
 
 
 DispatchEvent = GenericDispatchEvent[str, Dict[str, Any]]
 
 
 GatewayCommand = Union[
```

### Comparing `discord_typings-0.8.0/discord_typings/_interactions/_commands.py` & `discord_typings-0.9.0/discord_typings/_interactions/_commands.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_interactions/_components.py` & `discord_typings-0.9.0/discord_typings/_interactions/_components.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_interactions/_receiving.py` & `discord_typings-0.9.0/discord_typings/_interactions/_receiving.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     version: int
 
 
 class _GuildInteractionData(TypedDict):
     id: 'discord_typings.Snowflake'
     application_id: 'discord_typings.Snowflake'
     guild_id: 'discord_typings.Snowflake'
+    guild: 'discord_typings.PartialGuildData'
     channel: 'discord_typings.PartialChannelData'
     channel_id: 'discord_typings.Snowflake'
     member: 'discord_typings.GuildMemberData'
     token: str
     version: int
     app_permissions: str
     locale: 'discord_typings.Locales'
@@ -381,14 +382,15 @@
     tts: NotRequired[bool]
     content: NotRequired[str]
     embeds: NotRequired[List['discord_typings.EmbedData']]
     allowed_mentions: NotRequired['discord_typings.AllowedMentionsData']
     flags: NotRequired[int]
     components: NotRequired[List['discord_typings.ComponentData']]
     attachments: NotRequired[List['discord_typings.PartialAttachmentData']]
+    poll: NotRequired['discord_typings.PollCreateRequestData']
 
 
 class InteractionAutocompleteCallbackData(TypedDict, Generic[_T]):
     choices: List['discord_typings.CommandOptionChoiceData[_T]']
 
 
 class InteractionModalCallbackData(TypedDict):
```

### Comparing `discord_typings-0.8.0/discord_typings/_monetization/_entitlements.py` & `discord_typings-0.9.0/discord_typings/_monetization/_entitlements.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,13 +17,23 @@
     application_id: 'discord_typings.Snowflake'
     user_id: NotRequired['discord_typings.Snowflake']
     type: 'discord_typings.EntitlementTypes'
     deleted: bool
     starts_at: NotRequired[str]
     ends_at: NotRequired[str]
     guild_id: NotRequired['discord_typings.Snowflake']
+    consumed: NotRequired[bool]
 
 
 # https://discord.com/developers/docs/monetization/entitlements#entitlement-object-entitlement-types
 
 
-EntitlementTypes = Literal[8]
+EntitlementTypes = Literal[
+    1,
+    2,
+    3,
+    4,
+    5,
+    6,
+    7,
+    8,
+]
```

### Comparing `discord_typings-0.8.0/discord_typings/_oauth.py` & `discord_typings-0.9.0/discord_typings/_oauth.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_reference.py` & `discord_typings-0.9.0/discord_typings/_reference.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_application.py` & `discord_typings-0.9.0/discord_typings/_resources/_application.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_audit_log.py` & `discord_typings-0.9.0/discord_typings/_resources/_audit_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,15 +63,17 @@
     72, 73, 74, 75,
     80, 81, 82, 83, 84, 85,
     90, 91, 92,
     100, 101, 102,
     110, 111, 112,
     121,
     140, 141, 142, 143, 144, 145,
-    150, 151
+    150, 151,
+    163, 164, 165, 166, 167,
+    190, 191,
 ]
 
 
 # https://discord.com/developers/docs/resources/audit-log#audit-log-entry-object-optional-audit-entry-info
 
 
 class OptionalAuditLogEntryData(TypedDict):
```

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_auto_moderation.py` & `discord_typings-0.9.0/discord_typings/_resources/_auto_moderation.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import discord_typings
 
 __all__ = (
     'KeywordAutoModerationRuleData',
     'SpamAutoModerationRuleData',
     'KeywordPresetAutoModerationRuleData',
     'MentionSpamAutoModerationRuleData',
+    'MemberProfileAutoModerationRuleData',
     'AutoModerationRuleData',
     'AutoModerationTriggerTypes',
     'KeywordAutoModerationTriggerMetadata',
     'KeywordPresetAutoModerationTriggerMetadataData',
     'MentionSpamAutoModerationTriggerMetadataData',
+    'MemberProfileAutoModerationTriggerMetadataData',
     'EmptyAutoModerationTriggerMetadataData',
     'AutoModerationTriggerMetadataData',
     'AutoModerationKeywordPresetTypes',
     'AutoModerationEventTypes',
     'BlockMessageAutoModerationActionData',
     'SendAlertMessageAutoModerationActionData',
     'TimeoutAutoModerationActionData',
@@ -61,24 +63,30 @@
 
 
 class MentionSpamAutoModerationRuleData(_AutoModerationRuleData):
     trigger_type: Literal[5]
     trigger_metadata: 'discord_typings.MentionSpamAutoModerationTriggerMetadataData'
 
 
+class MemberProfileAutoModerationRuleData(_AutoModerationRuleData):
+    trigger_type: Literal[6]
+    trigger_metadata: 'discord_typings.MemberProfileAutoModerationTriggerMetadataData'
+
+
 AutoModerationRuleData = Union[
     KeywordAutoModerationRuleData, KeywordPresetAutoModerationRuleData,
-    SpamAutoModerationRuleData, MentionSpamAutoModerationRuleData
+    SpamAutoModerationRuleData, MentionSpamAutoModerationRuleData,
+    MemberProfileAutoModerationRuleData
 ]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-rule-object-trigger-types
 
 
-AutoModerationTriggerTypes = Literal[1, 2, 3, 4]
+AutoModerationTriggerTypes = Literal[1, 2, 3, 4, 5, 6]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-rule-object-trigger-metadata
 
 
 class KeywordAutoModerationTriggerMetadata(TypedDict):
     keyword_filter: List[str]
@@ -93,36 +101,44 @@
 
 
 class MentionSpamAutoModerationTriggerMetadataData(TypedDict):
     mention_total_limit: int
     mention_raid_protection_enabled: bool
 
 
+class MemberProfileAutoModerationTriggerMetadataData(TypedDict):
+    keyword_filter: List[str]
+    regex_patterns: List[str]
+
+    allow_list: List[str]
+
+
 class EmptyAutoModerationTriggerMetadataData(TypedDict):
     ...
 
 
 AutoModerationTriggerMetadataData = Union[
     KeywordAutoModerationTriggerMetadata,
     KeywordPresetAutoModerationTriggerMetadataData,
     MentionSpamAutoModerationTriggerMetadataData,
+    MemberProfileAutoModerationTriggerMetadataData,
     EmptyAutoModerationTriggerMetadataData,
 ]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-rule-object-keyword-preset-types
 
 
 AutoModerationKeywordPresetTypes = Literal[1, 2, 3]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-rule-object-event-types
 
 
-AutoModerationEventTypes = Literal[1]
+AutoModerationEventTypes = Literal[1, 2]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-action-object-auto-moderation-action-structure
 
 
 class BlockMessageAutoModerationActionData(TypedDict):
     type: Literal[1]
@@ -144,15 +160,15 @@
     TimeoutAutoModerationActionData
 ]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-action-object-action-types
 
 
-AutoModerationActionTypes = Literal[1, 2, 3]
+AutoModerationActionTypes = Literal[1, 2, 3, 4]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-action-object-action-metadata
 
 
 class BlockmessageAutoModerationActionMetadataData(TypedDict):
     custom_message: NotRequired[str]
```

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_channel.py` & `discord_typings-0.9.0/discord_typings/_resources/_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     'ForumLayoutTypes',
     'MessageData',
     'UserMentionData',
     'MessageTypes',
     'MessageActivityData',
     'MessageActivityTypes',
     'MessageInteractionMetadataData',
+    'MessageCallData',
     'MessageReferenceData',
     'FollowedChannelData',
     'MessageReactionData',
     'ReactionCountDetailsData',
     'PermissionOverwriteData',
     'ThreadMetadataData',
     'ThreadMemberData',
@@ -44,14 +45,15 @@
     'EmbedFooterData',
     'EmbedFieldData',
     'PartialAttachmentData',
     'AttachmentData',
     'ChannelMentionData',
     'AllowedMentionsData',
     'RoleSubscriptionData',
+    'ReactionTypes',
     'HasMoreListThreadsData',
 )
 
 
 # https://discord.com/developers/docs/resources/channel#channel-object-channel-structure
 
 
@@ -269,14 +271,16 @@
     interaction: NotRequired['discord_typings.MessageInteractionData']
     thread: NotRequired['discord_typings.ThreadChannelData']
     components: NotRequired[List['discord_typings.ComponentData']]
     sticker_items: NotRequired[List['discord_typings.StickerItemData']]
     position: NotRequired[int]
     role_subscription_data: NotRequired['discord_typings.RoleSubscriptionData']
     resolved: NotRequired['discord_typings.ResolvedInteractionDataData']
+    poll: NotRequired['discord_typings.PollCreateRequestData']
+    call: NotRequired['discord_typings.MessageCallData']
 
 
 class _GuildMessageData(_ChannelMessageData):
     guild_id: 'discord_typings.Snowflake'
     member: 'discord_typings.GuildMemberData'
 
 
@@ -312,24 +316,32 @@
 
 # https://discord.com/developers/docs/resources/channel#message-interaction-metadata-object
 
 
 class MessageInteractionMetadataData(TypedDict):
     id: 'discord_typings.Snowflake'
     type: 'discord_typings.InteractionTypes'
-    user_id: 'discord_typings.Snowflake'
+    user: 'discord_typings.UserData'
     authorizing_integration_owners: Dict[
         'discord_typings.ApplicationIntegrationTypes',
         'discord_typings.Snowflake'
     ]
     original_response_message_id: NotRequired['discord_typings.Snowflake']
     interacted_message_id: NotRequired['discord_typings.Snowflake']
     triggering_interaction_metadata: NotRequired['MessageInteractionMetadataData']
 
 
+# https://discord.com/developers/docs/resources/channel#message-call-object
+
+
+class MessageCallData(TypedDict):
+    participants: List['discord_typings.Snowflake']
+    ended_timestamp: NotRequired[Optional[str]]
+
+
 # https://discord.com/developers/docs/resources/channel#message-reference-object-message-reference-structure
 
 
 class MessageReferenceData(TypedDict):
     message_id: NotRequired['discord_typings.Snowflake']
     # Note: This will always be sent when receiving a message reference.
     channel_id: NotRequired['discord_typings.Snowflake']
@@ -553,14 +565,20 @@
 class RoleSubscriptionData(TypedDict):
     role_subscription_listing_id: 'discord_typings.Snowflake'
     tier_name: str
     total_months_subscribed: int
     is_renewal: bool
 
 
+# https://discord.com/developers/docs/resources/channel#get-reactions-reaction-types
+
+
+ReactionTypes = Literal[0, 1]
+
+
 # https://discord.com/developers/docs/resources/channel#list-public-archived-threads-response-body
 
 
 class HasMoreListThreadsData(TypedDict):
     threads: List[ThreadChannelData]
     members: List[ThreadMemberData]
     has_more: bool
```

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_emoji.py` & `discord_typings-0.9.0/discord_typings/_resources/_emoji.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_guild.py` & `discord_typings-0.9.0/discord_typings/_resources/_guild.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     'GuildOnboardingData',
     'GuildOnboardingPromptsData',
     'GuildOnboardingPromptOptionData',
     'GuildOnboardingModes',
     'GuildOnboardingPromptTypes',
     'ChannelPositionData',
     'ListThreadsData',
+    'BulkBanData',
     'RolePositionData',
     'RoleData',
     'RoleTagsData',
     'PartialGuildData',
 )
 
 
@@ -231,14 +232,15 @@
     premium_since: NotRequired[Optional[str]]
     deaf: bool
     mute: bool
     flags: int
     pending: NotRequired[bool]
     permissions: NotRequired[str]
     communication_disabled_until: NotRequired[Optional[str]]
+    avatar_decoration_data: NotRequired[Optional['discord_typings.AvatarDecorationDataData']]
 
 
 # https://discord.com/developers/docs/resources/guild#integration-object-integration-structure
 
 
 class StreamingIntegrationData(TypedDict):
     id: 'discord_typings.Snowflake'
@@ -390,14 +392,22 @@
 
 
 class ListThreadsData(TypedDict):
     threads: List['discord_typings.ThreadChannelData']
     members: List['discord_typings.ThreadMemberData']
 
 
+# https://discord.com/developers/docs/resources/guild#bulk-guild-ban-bulk-ban-response
+
+
+class BulkBanData(TypedDict):
+    banned_users: List['discord_typings.Snowflake']
+    failed_users: List['discord_typings.Snowflake']
+
+
 # https://discord.com/developers/docs/resources/guild#modify-guild-role-positions-json-params
 
 
 class RolePositionData(TypedDict):
     id: 'discord_typings.Snowflake'
     position: NotRequired[Optional[int]]
```

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_guild_scheduled_events.py` & `discord_typings-0.9.0/discord_typings/_resources/_guild_scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_guild_template.py` & `discord_typings-0.9.0/discord_typings/_resources/_guild_template.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_invite.py` & `discord_typings-0.9.0/discord_typings/_resources/_invite.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,46 @@
 
 from typing_extensions import Literal, NotRequired, TypedDict
 
 import discord_typings
 
 __all__ = (
     'InviteData',
+    'InviteTypes',
     'InviteTargetTypes',
     'InviteMetadata',
     'InviteStageInstanceData',
 )
 
 
 # https://discord.com/developers/docs/resources/invite#invite-object-invite-structure
 
 
 class InviteData(TypedDict):
+    type: 'discord_typings.InviteTypes'
     code: str
     guild: NotRequired['discord_typings.PartialGuildData']
     channel: Optional['discord_typings.PartialChannelData']
     inviter: NotRequired['discord_typings.UserData']
     target_type: NotRequired['discord_typings.InviteTargetTypes']
     target_user: NotRequired['discord_typings.UserData']
     target_application: NotRequired['discord_typings.ApplicationData']
     approximate_presence_count: NotRequired[int]
     approximate_member_count: NotRequired[int]
     expires_at: NotRequired[Optional[str]]
     stage_instance: NotRequired['discord_typings.InviteStageInstanceData']
     guild_scheduled_event: NotRequired['discord_typings.GuildScheduledEventData']
 
 
+# https://discord.com/developers/docs/resources/invite#invite-object-invite-types
+
+
+InviteTypes = Literal[0, 1, 2]
+
+
 # https://discord.com/developers/docs/resources/invite#invite-object-invite-target-types
 
 
 InviteTargetTypes = Literal[1, 2]
 
 
 # https://discord.com/developers/docs/resources/invite#invite-metadata-object-invite-metadata-structure
```

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_role_connection_metadata.py` & `discord_typings-0.9.0/discord_typings/_resources/_role_connection_metadata.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_stage_instance.py` & `discord_typings-0.9.0/discord_typings/_resources/_stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_sticker.py` & `discord_typings-0.9.0/discord_typings/_resources/_sticker.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_user.py` & `discord_typings-0.9.0/discord_typings/_resources/_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, List, Optional, Union
 
 from typing_extensions import Literal, NotRequired, TypedDict
 
 __all__ = (
     'UserData',
     'UserPremiumTypes',
+    'AvatarDecorationDataData',
     'ConnectionData',
     'ConnectionTypes',
     'ConnectionVisibilityTypes',
     'ApplicationRoleConnectionData',
 )
 
 import discord_typings
@@ -29,23 +30,31 @@
     accent_color: NotRequired[Optional[int]]
     locale: NotRequired['discord_typings.Locales']
     verified: NotRequired[bool]
     email: NotRequired[Optional[str]]
     flags: NotRequired[int]
     premium_type: NotRequired['discord_typings.UserPremiumTypes']
     public_flags: NotRequired[int]
-    avatar_decoration: NotRequired[Optional[str]]
+    avatar_decoration_data: NotRequired[Optional['discord_typings.AvatarDecorationDataData']]
 
 
 # https://discord.com/developers/docs/resources/user#user-object-premium-types
 
 
 UserPremiumTypes = Literal[0, 1, 2, 3]
 
 
+# https://discord.com/developers/docs/resources/user#avatar-decoration-data-object
+
+
+class AvatarDecorationDataData(TypedDict):
+    asset: str
+    sku_id: 'discord_typings.Snowflake'
+
+
 # https://discord.com/developers/docs/resources/user#connection-object
 
 
 class ConnectionData(TypedDict):
     id: str
     name: str
     type: 'discord_typings.ConnectionTypes'
@@ -59,14 +68,16 @@
 
 
 # https://discord.com/developers/docs/resources/user#connection-object-services
 
 
 ConnectionTypes = Literal[
     'battlenet',
+    'bungie',
+    'domain',
     'ebay',
     'epicgames',
     'facebook',
     'github',
     'instagram',
     'leagueoflegends',
     'paypal',
```

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_voice.py` & `discord_typings-0.9.0/discord_typings/_resources/_voice.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/discord_typings/_resources/_webhook.py` & `discord_typings-0.9.0/discord_typings/_resources/_webhook.py`

 * *Files identical despite different names*

### Comparing `discord_typings-0.8.0/pyproject.toml` & `discord_typings-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "discord-typings"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python typings of all payloads that Discord sends as TypedDicts"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [{name = "Bluenix", email = "bluenixdev@gmail.com"}]
 
 keywords = [
```

### Comparing `discord_typings-0.8.0/PKG-INFO` & `discord_typings-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-typings
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python typings of all payloads that Discord sends as TypedDicts
 Keywords: discord,discord-api,discord-api-wrapper,python-3,typing
 Author-email: Bluenix <bluenixdev@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


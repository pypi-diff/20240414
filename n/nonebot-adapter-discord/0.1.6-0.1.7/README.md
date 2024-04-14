# Comparing `tmp/nonebot_adapter_discord-0.1.6.tar.gz` & `tmp/nonebot_adapter_discord-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_discord-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_adapter_discord-0.1.7.tar", max compression
```

## Comparing `nonebot_adapter_discord-0.1.6.tar` & `nonebot_adapter_discord-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7812 2024-03-25 14:15:16.707135 nonebot_adapter_discord-0.1.6/README.md
--rw-r--r--   0        0        0      230 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/__init__.py
--rw-r--r--   0        0        0    17184 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/adapter.py
--rw-r--r--   0        0        0      134 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/__init__.py
--rw-r--r--   0        0        0       25 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/client.py
--rw-r--r--   0        0        0    59455 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/client.pyi
--rw-r--r--   0        0        0   118064 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/handle.py
--rw-r--r--   0        0        0   110503 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/model.py
--rw-r--r--   0        0        0     1337 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/request.py
--rw-r--r--   0        0        0    45279 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/types.py
--rw-r--r--   0        0        0     3719 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/utils.py
--rw-r--r--   0        0        0     7958 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/bot.py
--rw-r--r--   0        0        0      461 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/commands/__init__.py
--rw-r--r--   0        0        0    17690 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/commands/matcher.py
--rw-r--r--   0        0        0     4965 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/commands/params.py
--rw-r--r--   0        0        0     2973 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/commands/storage.py
--rw-r--r--   0        0        0     2267 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/config.py
--rw-r--r--   0        0        0    32425 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/event.py
--rw-r--r--   0        0        0     1928 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/exception.py
--rw-r--r--   0        0        0    14781 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/message.py
--rw-r--r--   0        0        0     2013 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/payload.py
--rw-r--r--   0        0        0     1596 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/utils.py
--rw-r--r--   0        0        0     1268 2024-03-25 14:15:16.711135 nonebot_adapter_discord-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     8670 1970-01-01 00:00:00.000000 nonebot_adapter_discord-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     7812 2024-04-14 16:03:13.779344 nonebot_adapter_discord-0.1.7/README.md
+-rw-r--r--   0        0        0      230 2024-04-14 16:03:13.779344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/__init__.py
+-rw-r--r--   0        0        0    17184 2024-04-14 16:03:13.779344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/adapter.py
+-rw-r--r--   0        0        0      134 2024-04-14 16:03:13.779344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-14 16:03:13.779344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/client.py
+-rw-r--r--   0        0        0    59455 2024-04-14 16:03:13.779344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/client.pyi
+-rw-r--r--   0        0        0   118064 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/handle.py
+-rw-r--r--   0        0        0   110590 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/model.py
+-rw-r--r--   0        0        0     1337 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/request.py
+-rw-r--r--   0        0        0    45279 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/types.py
+-rw-r--r--   0        0        0     3719 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/utils.py
+-rw-r--r--   0        0        0     7958 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/bot.py
+-rw-r--r--   0        0        0      461 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/commands/__init__.py
+-rw-r--r--   0        0        0    17690 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/commands/matcher.py
+-rw-r--r--   0        0        0     4965 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/commands/params.py
+-rw-r--r--   0        0        0     2975 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/commands/storage.py
+-rw-r--r--   0        0        0     2267 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/config.py
+-rw-r--r--   0        0        0    32587 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/event.py
+-rw-r--r--   0        0        0     1928 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/exception.py
+-rw-r--r--   0        0        0    14765 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/message.py
+-rw-r--r--   0        0        0     2013 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/payload.py
+-rw-r--r--   0        0        0     1596 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/utils.py
+-rw-r--r--   0        0        0     1268 2024-04-14 16:03:13.783344 nonebot_adapter_discord-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     8670 1970-01-01 00:00:00.000000 nonebot_adapter_discord-0.1.7/PKG-INFO
```

### Comparing `nonebot_adapter_discord-0.1.6/README.md` & `nonebot_adapter_discord-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/adapter.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/client.pyi` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/handle.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/model.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2214,26 +2214,28 @@
     """User
 
     see https://discord.com/developers/docs/resources/user#user-object"""
 
     id: Snowflake
     username: str
     discriminator: str
+    global_name: Optional[str]
     avatar: Optional[str] = Field(...)
     bot: Missing[bool] = UNSET
     system: Missing[bool] = UNSET
     mfa_enabled: Missing[bool] = UNSET
     banner: MissingOrNullable[str] = UNSET
     accent_color: MissingOrNullable[int] = UNSET
     locale: Missing[str] = UNSET
     verified: Missing[bool] = UNSET
     email: MissingOrNullable[str] = UNSET
     flags: Missing[int] = UNSET
     premium_type: Missing[PremiumType] = UNSET
     public_flags: Missing[UserFlags] = UNSET
+    avatar_decoration: MissingOrNullable[str] = UNSET
 
 
 class Connection(BaseModel):
     """Connection
 
     see https://discord.com/developers/docs/resources/user#connection-object"""
 
@@ -2648,17 +2650,17 @@
     joined_at: Missing[str] = UNSET
     large: Missing[bool] = UNSET
     member_count: Missing[int] = UNSET
     voice_states: Missing[List["VoiceState"]] = UNSET
     members: Missing[List["GuildMember"]] = UNSET
     channels: Missing[List["Channel"]] = UNSET
     threads: Missing[List["Channel"]] = UNSET
-    presences: Missing[
-        List["PresenceUpdate"]
-    ] = UNSET  # partial presence update objects
+    presences: Missing[List["PresenceUpdate"]] = (
+        UNSET  # partial presence update objects
+    )
     stage_instances: Missing[List["StageInstance"]] = UNSET
     guild_scheduled_events: Missing[List["GuildScheduledEvent"]] = UNSET
 
 
 class GuildUpdate(Guild):
     """Guild Update Event Fields
```

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/request.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/types.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/api/utils.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/bot.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/commands/matcher.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/commands/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/commands/params.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/commands/params.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/commands/storage.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/commands/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from ..utils import model_dump
 
 if TYPE_CHECKING:
     from .matcher import ApplicationCommandConfig
 
 _application_command_storage: Dict[str, "ApplicationCommandConfig"] = {}
 
-OPTION_KEY: Literal[
+OPTION_KEY: Literal["_discord_application_command_options"] = (
     "_discord_application_command_options"
-] = "_discord_application_command_options"
+)
 
 
 async def sync_application_command(bot: Bot):
     commands_global: List[ApplicationCommandCreate] = []
     commands_guild: Dict[Snowflake, List[ApplicationCommandCreate]] = defaultdict(List)
     if "*" in bot.bot_info.application_commands:
         if "*" in bot.bot_info.application_commands["*"]:
```

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/config.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/event.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,14 +620,20 @@
 class InteractionCreateEvent(NoticeEvent, InteractionCreate):
     """Interaction create event
 
     see https://discord.com/developers/docs/topics/gateway-events#interaction-create"""
 
     __type__ = EventType.INTERACTION_CREATE
 
+    @override
+    def get_user_id(self) -> str:
+        if not self.user:
+            raise ValueError("Event has no context!")
+        return str(self.user.id)
+
 
 class PingInteractionEvent(InteractionCreateEvent):
     type: Literal[InteractionType.PING]
     data: Literal[UNSET] = UNSET
 
 
 class ApplicationCommandInteractionEvent(InteractionCreateEvent):
```

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/exception.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/message.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,26 +138,24 @@
     ) -> "TimestampSegment":
         if isinstance(timestamp, datetime.datetime):
             timestamp = int(timestamp.timestamp())
         return TimestampSegment("timestamp", {"timestamp": timestamp, "style": style})
 
     @staticmethod
     @overload
-    def reference(reference: MessageReference) -> "ReferenceSegment":
-        ...
+    def reference(reference: MessageReference) -> "ReferenceSegment": ...
 
     @staticmethod
     @overload
     def reference(
         reference: SnowflakeType,
         channel_id: Optional[SnowflakeType] = None,
         guild_id: Optional[SnowflakeType] = None,
         fail_if_not_exists: Optional[bool] = None,
-    ) -> "ReferenceSegment":
-        ...
+    ) -> "ReferenceSegment": ...
 
     @staticmethod
     def reference(
         reference: Union[SnowflakeType, MessageReference],
         channel_id: Optional[SnowflakeType] = None,
         guild_id: Optional[SnowflakeType] = None,
         fail_if_not_exists: Optional[bool] = None,
```

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/payload.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/payload.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/nonebot/adapters/discord/utils.py` & `nonebot_adapter_discord-0.1.7/nonebot/adapters/discord/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_discord-0.1.6/pyproject.toml` & `nonebot_adapter_discord-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-discord"
-version = "0.1.6"
+version = "0.1.7"
 description = "Discord adapter for nonebot2"
 authors = ["CMHopeSunshine <277073121@qq.com>", "yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/adapter-discord"
 repository = "https://github.com/nonebot/adapter-discord"
 documentation = "https://github.com/nonebot/adapter-discord"
```

### Comparing `nonebot_adapter_discord-0.1.6/PKG-INFO` & `nonebot_adapter_discord-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-discord
-Version: 0.1.6
+Version: 0.1.7
 Summary: Discord adapter for nonebot2
 Home-page: https://github.com/nonebot/adapter-discord
 License: MIT
 Keywords: nonebot,discord,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-discord Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-discord Version: 0.1.7 Summary:
 Discord adapter for nonebot2 Home-page: https://github.com/nonebot/adapter-
 discord License: MIT Keywords: nonebot,discord,bot Author: CMHopeSunshine
 Author-email: 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```


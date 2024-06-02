# Comparing `tmp/rlbot-1.9.5.tar.gz` & `tmp/rlbot-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rlbot-1.9.5.tar", last modified: Sun Jan  6 02:22:35 2019, max compression
+gzip compressed data, was "dist\rlbot-1.9.6.tar", last modified: Sun Jan  6 17:41:50 2019, max compression
```

## Comparing `rlbot-1.9.5.tar` & `rlbot-1.9.6.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/flatbuffers/
--rw-rw-rw-   0        0        0    24651 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/builder.py
--rw-rw-rw-   0        0        0     2423 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/compat.py
--rw-rw-rw-   0        0        0     1595 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/encode.py
--rw-rw-rw-   0        0        0     4136 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/number_types.py
--rw-rw-rw-   0        0        0     1207 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/packer.py
--rw-rw-rw-   0        0        0     4837 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/table.py
--rw-rw-rw-   0        0        0     1022 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/util.py
--rw-rw-rw-   0        0        0      715 2019-01-06 02:22:34.000000 rlbot-1.9.5/flatbuffers/__init__.py
--rw-rw-rw-   0        0        0     1629 2019-01-06 02:22:35.000000 rlbot-1.9.5/PKG-INFO
--rw-rw-rw-   0        0        0      943 2019-01-06 02:22:34.000000 rlbot-1.9.5/README.md
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/agents/
--rw-rw-rw-   0        0        0    15708 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/base_agent.py
--rw-rw-rw-   0        0        0     3503 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/base_dotnet_agent.py
--rw-rw-rw-   0        0        0     2136 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/base_flatbuffer_agent.py
--rw-rw-rw-   0        0        0      276 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/base_independent_agent.py
--rw-rw-rw-   0        0        0     4143 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/base_java_agent.py
--rw-rw-rw-   0        0        0     1455 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/base_subprocess_agent.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/agents/human/
--rw-rw-rw-   0        0        0     2061 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/human/controller_input.py
--rw-rw-rw-   0        0        0      453 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/human/human_bot.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/human/__init__.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/agents/__init__.py
--rw-rw-rw-   0        0        0     1094 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/base_extension.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/botmanager/
--rw-rw-rw-   0        0        0     1034 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/agent_metadata.py
--rw-rw-rw-   0        0        0      830 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/bot_helper_process.py
--rw-rw-rw-   0        0        0    11187 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/bot_manager.py
--rw-rw-rw-   0        0        0     1763 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/bot_manager_flatbuffer.py
--rw-rw-rw-   0        0        0     1150 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/bot_manager_independent.py
--rw-rw-rw-   0        0        0     3244 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/bot_manager_struct.py
--rw-rw-rw-   0        0        0     2571 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/helper_process_manager.py
--rw-rw-rw-   0        0        0      793 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/helper_process_request.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/botmanager/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/dll/
--rwxrwxrwx   0        0        0   152576 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/dll/BallPrediction.exe
--rw-rw-rw-   0        0        0   199680 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/dll/RLBot_Core.dll
--rw-rw-rw-   0        0        0   125440 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/dll/RLBot_Core_Interface.dll
--rw-rw-rw-   0        0        0    96256 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/dll/RLBot_Core_Interface_32.dll
--rwxrwxrwx   0        0        0  1165312 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/dll/RLBot_Injector.exe
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/gui/
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/gui/design/
--rw-rw-rw-   0        0        0     7962 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/agent_customisation.py
--rw-rw-rw-   0        0        0     5393 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/agent_customisation.ui
--rw-rw-rw-   0        0        0    31979 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/car_customisation.py
--rw-rw-rw-   0        0        0    28622 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/car_customisation.ui
--rw-rw-rw-   0        0        0    12504 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/mutator_customisation.py
--rw-rw-rw-   0        0        0     8685 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/mutator_customisation.ui
--rw-rw-rw-   0        0        0    33290 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/qt_gui.py
--rw-rw-rw-   0        0        0    32341 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/qt_gui.ui
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/design/__init__.py
--rw-rw-rw-   0        0        0     4524 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/gui_agent.py
--rw-rw-rw-   0        0        0     1156 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/index_manager.py
--rw-rw-rw-   0        0        0     4283 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/mutator_editor.py
--rw-rw-rw-   0        0        0     4715 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/presets.py
--rw-rw-rw-   0        0        0    22527 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/preset_editors.py
--rw-rw-rw-   0        0        0    36381 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/qt_root.py
--rw-rw-rw-   0        0        0    68088 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/rocket_league_items.json
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/img/
--rw-rw-rw-   0        0        0     5452 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/img/rlbot_icon.png
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/matchconfig/
--rw-rw-rw-   0        0        0     5340 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/matchconfig/match_config.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/matchconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/messages/
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/messages/flat/
--rw-rw-rw-   0        0        0     2147 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/BallInfo.py
--rw-rw-rw-   0        0        0     1801 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/BallPrediction.py
--rw-rw-rw-   0        0        0     1225 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/BallRigidBodyState.py
--rw-rw-rw-   0        0        0      536 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Bool.py
--rw-rw-rw-   0        0        0     1416 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/BoostPad.py
--rw-rw-rw-   0        0        0     1454 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/BoostPadState.py
--rw-rw-rw-   0        0        0     1795 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Color.py
--rw-rw-rw-   0        0        0     3774 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/ControllerState.py
--rw-rw-rw-   0        0        0     1179 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DesiredBallState.py
--rw-rw-rw-   0        0        0     1146 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DesiredBoostState.py
--rw-rw-rw-   0        0        0     2626 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DesiredCarState.py
--rw-rw-rw-   0        0        0     1672 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DesiredGameInfoState.py
--rw-rw-rw-   0        0        0     3723 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DesiredGameState.py
--rw-rw-rw-   0        0        0     2801 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DesiredPhysics.py
--rw-rw-rw-   0        0        0     1786 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DropShotBallInfo.py
--rw-rw-rw-   0        0        0     1003 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/DropshotTile.py
--rw-rw-rw-   0        0        0     2414 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/FieldInfo.py
--rw-rw-rw-   0        0        0      546 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Float.py
--rw-rw-rw-   0        0        0     4426 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/GameInfo.py
--rw-rw-rw-   0        0        0     4554 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/GameTickPacket.py
--rw-rw-rw-   0        0        0     1878 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/GoalInfo.py
--rw-rw-rw-   0        0        0     2499 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Physics.py
--rw-rw-rw-   0        0        0     5129 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/PlayerInfo.py
--rw-rw-rw-   0        0        0     1530 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/PlayerInput.py
--rw-rw-rw-   0        0        0     1903 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/PlayerRigidBodyState.py
--rw-rw-rw-   0        0        0     1713 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/PredictionSlice.py
--rw-rw-rw-   0        0        0     1391 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Quaternion.py
--rw-rw-rw-   0        0        0     1793 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/QuickChat.py
--rw-rw-rw-   0        0        0     2285 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/QuickChatSelection.py
--rw-rw-rw-   0        0        0     1939 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/RenderGroup.py
--rw-rw-rw-   0        0        0     4146 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/RenderMessage.py
--rw-rw-rw-   0        0        0      297 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/RenderType.py
--rw-rw-rw-   0        0        0     3178 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/RigidBodyState.py
--rw-rw-rw-   0        0        0     2163 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/RigidBodyTick.py
--rw-rw-rw-   0        0        0     1054 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Rotator.py
--rw-rw-rw-   0        0        0     2018 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/RotatorPartial.py
--rw-rw-rw-   0        0        0     2946 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/ScoreInfo.py
--rw-rw-rw-   0        0        0      340 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/TileState.py
--rw-rw-rw-   0        0        0     1623 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/TinyBall.py
--rw-rw-rw-   0        0        0     2112 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/TinyPacket.py
--rw-rw-rw-   0        0        0     3506 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/TinyPlayer.py
--rw-rw-rw-   0        0        0     2428 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Touch.py
--rw-rw-rw-   0        0        0      937 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Vector3.py
--rw-rw-rw-   0        0        0     1982 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/Vector3Partial.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/flat/__init__.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/messages/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/parsing/
--rw-rw-rw-   0        0        0    12414 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/parsing/agent_config_parser.py
--rw-rw-rw-   0        0        0    12252 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/parsing/custom_config.py
--rw-rw-rw-   0        0        0      812 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/parsing/directory_scanner.py
--rw-rw-rw-   0        0        0      285 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/parsing/incrementing_integer.py
--rw-rw-rw-   0        0        0    10085 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/parsing/match_settings_config_parser.py
--rw-rw-rw-   0        0        0     3629 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/parsing/rlbot_config_parser.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/parsing/__init__.py
--rw-rw-rw-   0        0        0      520 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/runner.py
--rw-rw-rw-   0        0        0    13787 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/setup_manager.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/training/
--rw-rw-rw-   0        0        0     2403 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/training/status_rendering.py
--rw-rw-rw-   0        0        0     8782 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/training/training.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/training/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/utils/
--rw-rw-rw-   0        0        0     3688 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/class_importer.py
--rw-rw-rw-   0        0        0     1013 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/file_util.py
--rw-rw-rw-   0        0        0    14541 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/game_state_util.py
--rw-rw-rw-   0        0        0     3924 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/item_id_parser.py
--rw-rw-rw-   0        0        0     1181 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/logging_utils.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/utils/prediction/
--rw-rw-rw-   0        0        0   322724 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/prediction/dropshot.dat
--rw-rw-rw-   0        0        0  2473968 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/prediction/hoops.dat
--rw-rw-rw-   0        0        0      584 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/prediction/prediction_util.py
--rw-rw-rw-   0        0        0  1186446 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/prediction/soccar.dat
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/prediction/__init__.py
--rw-rw-rw-   0        0        0     3252 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/process_configuration.py
--rw-rw-rw-   0        0        0      993 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/public_utils.py
--rw-rw-rw-   0        0        0      720 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/python_version_check.py
--rw-rw-rw-   0        0        0     1145 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/rate_limiter.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/utils/rendering/
--rw-rw-rw-   0        0        0    14432 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/rendering/rendering_manager.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/rendering/__init__.py
--rw-rw-rw-   0        0        0     3912 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/rlbot_exception.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot/utils/structures/
--rw-rw-rw-   0        0        0      366 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/ball_prediction_struct.py
--rw-rw-rw-   0        0        0      409 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/bot_input_struct.py
--rw-rw-rw-   0        0        0     8198 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/game_data_struct.py
--rw-rw-rw-   0        0        0    13696 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/game_interface.py
--rw-rw-rw-   0        0        0     1351 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/game_status.py
--rw-rw-rw-   0        0        0     8655 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/legacy_data_v3.py
--rw-rw-rw-   0        0        0     5002 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/quick_chats.py
--rw-rw-rw-   0        0        0     1107 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/rigid_body_struct.py
--rw-rw-rw-   0        0        0     2926 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/start_match_structures.py
--rw-rw-rw-   0        0        0      952 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/struct.py
--rw-rw-rw-   0        0        0     1010 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/utils.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/structures/__init__.py
--rw-rw-rw-   0        0        0        0 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/utils/__init__.py
--rw-rw-rw-   0        0        0    10840 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/version.py
--rw-rw-rw-   0        0        0       34 2019-01-06 02:22:34.000000 rlbot-1.9.5/rlbot/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot.egg-info/
--rw-rw-rw-   0        0        0        1 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1629 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       25 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0     4932 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       18 2019-01-06 02:22:35.000000 rlbot-1.9.5/rlbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-01-06 02:22:35.000000 rlbot-1.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1159 2019-01-06 02:22:34.000000 rlbot-1.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:50.000000 rlbot-1.9.6/
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/flatbuffers/
+-rw-rw-rw-   0        0        0    24651 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/builder.py
+-rw-rw-rw-   0        0        0     2423 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/compat.py
+-rw-rw-rw-   0        0        0     1595 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/encode.py
+-rw-rw-rw-   0        0        0     4136 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/number_types.py
+-rw-rw-rw-   0        0        0     1207 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/packer.py
+-rw-rw-rw-   0        0        0     4837 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/table.py
+-rw-rw-rw-   0        0        0     1022 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/util.py
+-rw-rw-rw-   0        0        0      715 2019-01-06 17:41:48.000000 rlbot-1.9.6/flatbuffers/__init__.py
+-rw-rw-rw-   0        0        0     1629 2019-01-06 17:41:50.000000 rlbot-1.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2019-01-06 17:41:48.000000 rlbot-1.9.6/README.md
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/agents/
+-rw-rw-rw-   0        0        0    15708 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/base_agent.py
+-rw-rw-rw-   0        0        0     3503 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/base_dotnet_agent.py
+-rw-rw-rw-   0        0        0     2136 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/base_flatbuffer_agent.py
+-rw-rw-rw-   0        0        0      276 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/base_independent_agent.py
+-rw-rw-rw-   0        0        0     4143 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/base_java_agent.py
+-rw-rw-rw-   0        0        0     1455 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/base_subprocess_agent.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/agents/human/
+-rw-rw-rw-   0        0        0     2061 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/human/controller_input.py
+-rw-rw-rw-   0        0        0      453 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/human/human_bot.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/human/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/agents/__init__.py
+-rw-rw-rw-   0        0        0     1094 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/base_extension.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/botmanager/
+-rw-rw-rw-   0        0        0     1034 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/agent_metadata.py
+-rw-rw-rw-   0        0        0      830 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/bot_helper_process.py
+-rw-rw-rw-   0        0        0    11187 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/bot_manager.py
+-rw-rw-rw-   0        0        0     1763 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/bot_manager_flatbuffer.py
+-rw-rw-rw-   0        0        0     1150 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/bot_manager_independent.py
+-rw-rw-rw-   0        0        0     3244 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/bot_manager_struct.py
+-rw-rw-rw-   0        0        0     2571 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/helper_process_manager.py
+-rw-rw-rw-   0        0        0      793 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/helper_process_request.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/botmanager/__init__.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/dll/
+-rwxrwxrwx   0        0        0   152576 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/dll/BallPrediction.exe
+-rw-rw-rw-   0        0        0   199680 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/dll/RLBot_Core.dll
+-rw-rw-rw-   0        0        0   125440 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/dll/RLBot_Core_Interface.dll
+-rw-rw-rw-   0        0        0    96256 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/dll/RLBot_Core_Interface_32.dll
+-rwxrwxrwx   0        0        0  1165312 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/dll/RLBot_Injector.exe
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/gui/
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/gui/design/
+-rw-rw-rw-   0        0        0     7962 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/agent_customisation.py
+-rw-rw-rw-   0        0        0     5393 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/agent_customisation.ui
+-rw-rw-rw-   0        0        0    31979 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/car_customisation.py
+-rw-rw-rw-   0        0        0    28622 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/car_customisation.ui
+-rw-rw-rw-   0        0        0    12504 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/mutator_customisation.py
+-rw-rw-rw-   0        0        0     8685 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/mutator_customisation.ui
+-rw-rw-rw-   0        0        0    33290 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/qt_gui.py
+-rw-rw-rw-   0        0        0    32341 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/qt_gui.ui
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/design/__init__.py
+-rw-rw-rw-   0        0        0     4524 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/gui_agent.py
+-rw-rw-rw-   0        0        0     1156 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/index_manager.py
+-rw-rw-rw-   0        0        0     4283 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/mutator_editor.py
+-rw-rw-rw-   0        0        0     4715 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/presets.py
+-rw-rw-rw-   0        0        0    22527 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/preset_editors.py
+-rw-rw-rw-   0        0        0    36385 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/qt_root.py
+-rw-rw-rw-   0        0        0    68088 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/rocket_league_items.json
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/img/
+-rw-rw-rw-   0        0        0     5452 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/img/rlbot_icon.png
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/matchconfig/
+-rw-rw-rw-   0        0        0     5340 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/matchconfig/match_config.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/matchconfig/__init__.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/messages/
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/messages/flat/
+-rw-rw-rw-   0        0        0     2147 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/BallInfo.py
+-rw-rw-rw-   0        0        0     1801 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/BallPrediction.py
+-rw-rw-rw-   0        0        0     1225 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/BallRigidBodyState.py
+-rw-rw-rw-   0        0        0      536 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Bool.py
+-rw-rw-rw-   0        0        0     1416 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/BoostPad.py
+-rw-rw-rw-   0        0        0     1454 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/BoostPadState.py
+-rw-rw-rw-   0        0        0     1795 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Color.py
+-rw-rw-rw-   0        0        0     3774 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/ControllerState.py
+-rw-rw-rw-   0        0        0     1179 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DesiredBallState.py
+-rw-rw-rw-   0        0        0     1146 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DesiredBoostState.py
+-rw-rw-rw-   0        0        0     2626 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DesiredCarState.py
+-rw-rw-rw-   0        0        0     1672 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DesiredGameInfoState.py
+-rw-rw-rw-   0        0        0     3723 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DesiredGameState.py
+-rw-rw-rw-   0        0        0     2801 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DesiredPhysics.py
+-rw-rw-rw-   0        0        0     1786 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DropShotBallInfo.py
+-rw-rw-rw-   0        0        0     1003 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/DropshotTile.py
+-rw-rw-rw-   0        0        0     2414 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/FieldInfo.py
+-rw-rw-rw-   0        0        0      546 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Float.py
+-rw-rw-rw-   0        0        0     4426 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/GameInfo.py
+-rw-rw-rw-   0        0        0     4554 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/GameTickPacket.py
+-rw-rw-rw-   0        0        0     1878 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/GoalInfo.py
+-rw-rw-rw-   0        0        0     2499 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Physics.py
+-rw-rw-rw-   0        0        0     5129 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/PlayerInfo.py
+-rw-rw-rw-   0        0        0     1530 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/PlayerInput.py
+-rw-rw-rw-   0        0        0     1903 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/PlayerRigidBodyState.py
+-rw-rw-rw-   0        0        0     1713 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/PredictionSlice.py
+-rw-rw-rw-   0        0        0     1391 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Quaternion.py
+-rw-rw-rw-   0        0        0     1793 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/QuickChat.py
+-rw-rw-rw-   0        0        0     2285 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/QuickChatSelection.py
+-rw-rw-rw-   0        0        0     1939 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/RenderGroup.py
+-rw-rw-rw-   0        0        0     4146 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/RenderMessage.py
+-rw-rw-rw-   0        0        0      297 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/RenderType.py
+-rw-rw-rw-   0        0        0     3178 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/RigidBodyState.py
+-rw-rw-rw-   0        0        0     2163 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/RigidBodyTick.py
+-rw-rw-rw-   0        0        0     1054 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Rotator.py
+-rw-rw-rw-   0        0        0     2018 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/RotatorPartial.py
+-rw-rw-rw-   0        0        0     2946 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/ScoreInfo.py
+-rw-rw-rw-   0        0        0      340 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/TileState.py
+-rw-rw-rw-   0        0        0     1623 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/TinyBall.py
+-rw-rw-rw-   0        0        0     2112 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/TinyPacket.py
+-rw-rw-rw-   0        0        0     3506 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/TinyPlayer.py
+-rw-rw-rw-   0        0        0     2428 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Touch.py
+-rw-rw-rw-   0        0        0      937 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Vector3.py
+-rw-rw-rw-   0        0        0     1982 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/Vector3Partial.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/flat/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/messages/__init__.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:50.000000 rlbot-1.9.6/rlbot/parsing/
+-rw-rw-rw-   0        0        0    12414 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/parsing/agent_config_parser.py
+-rw-rw-rw-   0        0        0    12252 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/parsing/custom_config.py
+-rw-rw-rw-   0        0        0      812 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/parsing/directory_scanner.py
+-rw-rw-rw-   0        0        0      285 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/parsing/incrementing_integer.py
+-rw-rw-rw-   0        0        0    10085 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/parsing/match_settings_config_parser.py
+-rw-rw-rw-   0        0        0     3629 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/parsing/rlbot_config_parser.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/parsing/__init__.py
+-rw-rw-rw-   0        0        0      520 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/runner.py
+-rw-rw-rw-   0        0        0    13787 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/setup_manager.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:50.000000 rlbot-1.9.6/rlbot/training/
+-rw-rw-rw-   0        0        0     2403 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/training/status_rendering.py
+-rw-rw-rw-   0        0        0     8782 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/training/training.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/training/__init__.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:50.000000 rlbot-1.9.6/rlbot/utils/
+-rw-rw-rw-   0        0        0     3688 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/class_importer.py
+-rw-rw-rw-   0        0        0     1013 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/file_util.py
+-rw-rw-rw-   0        0        0    14541 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/game_state_util.py
+-rw-rw-rw-   0        0        0     3924 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/item_id_parser.py
+-rw-rw-rw-   0        0        0     1181 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/logging_utils.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:50.000000 rlbot-1.9.6/rlbot/utils/prediction/
+-rw-rw-rw-   0        0        0   322724 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/prediction/dropshot.dat
+-rw-rw-rw-   0        0        0  2473968 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/prediction/hoops.dat
+-rw-rw-rw-   0        0        0      584 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/prediction/prediction_util.py
+-rw-rw-rw-   0        0        0  1186446 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/prediction/soccar.dat
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/prediction/__init__.py
+-rw-rw-rw-   0        0        0     3252 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/process_configuration.py
+-rw-rw-rw-   0        0        0      993 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/public_utils.py
+-rw-rw-rw-   0        0        0      720 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/python_version_check.py
+-rw-rw-rw-   0        0        0     1145 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/rate_limiter.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:50.000000 rlbot-1.9.6/rlbot/utils/rendering/
+-rw-rw-rw-   0        0        0    14432 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/rendering/rendering_manager.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/rendering/__init__.py
+-rw-rw-rw-   0        0        0     3912 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/rlbot_exception.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:50.000000 rlbot-1.9.6/rlbot/utils/structures/
+-rw-rw-rw-   0        0        0      366 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/ball_prediction_struct.py
+-rw-rw-rw-   0        0        0      409 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/bot_input_struct.py
+-rw-rw-rw-   0        0        0     8198 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/game_data_struct.py
+-rw-rw-rw-   0        0        0    13696 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/game_interface.py
+-rw-rw-rw-   0        0        0     1351 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/game_status.py
+-rw-rw-rw-   0        0        0     8655 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/legacy_data_v3.py
+-rw-rw-rw-   0        0        0     5002 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/quick_chats.py
+-rw-rw-rw-   0        0        0     1107 2019-01-06 17:41:48.000000 rlbot-1.9.6/rlbot/utils/structures/rigid_body_struct.py
+-rw-rw-rw-   0        0        0     2926 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/utils/structures/start_match_structures.py
+-rw-rw-rw-   0        0        0      952 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/utils/structures/struct.py
+-rw-rw-rw-   0        0        0     1010 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/utils/structures/utils.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/utils/structures/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/utils/__init__.py
+-rw-rw-rw-   0        0        0    10768 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/version.py
+-rw-rw-rw-   0        0        0       34 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot/__init__.py
+drwxrwxrwx   0        0        0        0 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1629 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     4932 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       18 2019-01-06 17:41:49.000000 rlbot-1.9.6/rlbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2019-01-06 17:41:50.000000 rlbot-1.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1159 2019-01-06 17:41:49.000000 rlbot-1.9.6/setup.py
```

### Comparing `rlbot-1.9.5/flatbuffers/builder.py` & `rlbot-1.9.6/flatbuffers/builder.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/flatbuffers/compat.py` & `rlbot-1.9.6/flatbuffers/compat.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/flatbuffers/encode.py` & `rlbot-1.9.6/flatbuffers/encode.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/flatbuffers/number_types.py` & `rlbot-1.9.6/flatbuffers/number_types.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/flatbuffers/packer.py` & `rlbot-1.9.6/flatbuffers/packer.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/flatbuffers/table.py` & `rlbot-1.9.6/flatbuffers/table.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/flatbuffers/util.py` & `rlbot-1.9.6/flatbuffers/util.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/flatbuffers/__init__.py` & `rlbot-1.9.6/flatbuffers/__init__.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/PKG-INFO` & `rlbot-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlbot
-Version: 1.9.5
+Version: 1.9.6
 Summary: A framework for writing custom Rocket League bots that run offline.
 Home-page: https://github.com/RLBot/RLBot
 Author: RLBot Community
 Author-email: rlbotofficial@gmail.com
 License: UNKNOWN
 Description: # RLBot
```

### Comparing `rlbot-1.9.5/README.md` & `rlbot-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/agents/base_agent.py` & `rlbot-1.9.6/rlbot/agents/base_agent.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/agents/base_dotnet_agent.py` & `rlbot-1.9.6/rlbot/agents/base_dotnet_agent.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/agents/base_flatbuffer_agent.py` & `rlbot-1.9.6/rlbot/agents/base_flatbuffer_agent.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/agents/base_java_agent.py` & `rlbot-1.9.6/rlbot/agents/base_java_agent.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/agents/base_subprocess_agent.py` & `rlbot-1.9.6/rlbot/agents/base_subprocess_agent.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/agents/human/controller_input.py` & `rlbot-1.9.6/rlbot/agents/human/controller_input.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/base_extension.py` & `rlbot-1.9.6/rlbot/base_extension.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/agent_metadata.py` & `rlbot-1.9.6/rlbot/botmanager/agent_metadata.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/bot_helper_process.py` & `rlbot-1.9.6/rlbot/botmanager/bot_helper_process.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/bot_manager.py` & `rlbot-1.9.6/rlbot/botmanager/bot_manager.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/bot_manager_flatbuffer.py` & `rlbot-1.9.6/rlbot/botmanager/bot_manager_flatbuffer.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/bot_manager_independent.py` & `rlbot-1.9.6/rlbot/botmanager/bot_manager_independent.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/bot_manager_struct.py` & `rlbot-1.9.6/rlbot/botmanager/bot_manager_struct.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/helper_process_manager.py` & `rlbot-1.9.6/rlbot/botmanager/helper_process_manager.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/botmanager/helper_process_request.py` & `rlbot-1.9.6/rlbot/botmanager/helper_process_request.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/dll/BallPrediction.exe` & `rlbot-1.9.6/rlbot/dll/BallPrediction.exe`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/dll/RLBot_Core.dll` & `rlbot-1.9.6/rlbot/dll/RLBot_Core.dll`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/dll/RLBot_Core_Interface.dll` & `rlbot-1.9.6/rlbot/dll/RLBot_Core_Interface.dll`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/dll/RLBot_Core_Interface_32.dll` & `rlbot-1.9.6/rlbot/dll/RLBot_Core_Interface_32.dll`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/dll/RLBot_Injector.exe` & `rlbot-1.9.6/rlbot/dll/RLBot_Injector.exe`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/agent_customisation.py` & `rlbot-1.9.6/rlbot/gui/design/agent_customisation.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/agent_customisation.ui` & `rlbot-1.9.6/rlbot/gui/design/agent_customisation.ui`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/car_customisation.py` & `rlbot-1.9.6/rlbot/gui/design/car_customisation.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/car_customisation.ui` & `rlbot-1.9.6/rlbot/gui/design/car_customisation.ui`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/mutator_customisation.py` & `rlbot-1.9.6/rlbot/gui/design/mutator_customisation.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/mutator_customisation.ui` & `rlbot-1.9.6/rlbot/gui/design/mutator_customisation.ui`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/qt_gui.py` & `rlbot-1.9.6/rlbot/gui/design/qt_gui.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/design/qt_gui.ui` & `rlbot-1.9.6/rlbot/gui/design/qt_gui.ui`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/gui_agent.py` & `rlbot-1.9.6/rlbot/gui/gui_agent.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/index_manager.py` & `rlbot-1.9.6/rlbot/gui/index_manager.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/mutator_editor.py` & `rlbot-1.9.6/rlbot/gui/mutator_editor.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/presets.py` & `rlbot-1.9.6/rlbot/gui/presets.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/preset_editors.py` & `rlbot-1.9.6/rlbot/gui/preset_editors.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/gui/qt_root.py` & `rlbot-1.9.6/rlbot/gui/qt_root.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         self.cfg_autosave_checkbutton.setDisabled(True)
         if self.overall_config is None:
             self.overall_config = create_bot_config_layout()
         GUIAgent.overall_config = self.overall_config
         self.overall_config.init_indices(10)
         self.overall_config_path = ""
         self.load_agents()
-        self.load_bot_directory(".")
+        # self.load_bot_directory(".")
         self.update_teams_listwidgets()
         if not self.overall_config_path:
             self.cfg_file_path_lineedit.setStyleSheet("border: 1px solid red;")
             self.cfg_file_path_lineedit.setText("Please load a configuration file")
             self.blue_plus_toolbutton.setEnabled(False)
             self.orange_plus_toolbutton.setEnabled(False)
             self.run_button.setEnabled(False)
@@ -399,15 +399,15 @@
             if not raw_parser.has_section(section):
                 self.popup_message(f"Config file is missing the section {section}, not loading it!",
                                    "Invalid Config File", QMessageBox.Warning)
                 return
         self.overall_config_path = config_path
         self.overall_config.parse_file(raw_parser, 10, config_directory=os.path.dirname(self.overall_config_path))
         self.load_agents()
-        self.load_bot_directory(".")
+        # self.load_bot_directory(".")
         self.update_teams_listwidgets()
         self.cfg_file_path_lineedit.setText(self.overall_config_path)
         self.cfg_file_path_lineedit.setStyleSheet("")
         self.run_button.setEnabled(True)
         self.update_team_settings()
         self.car_customisation.update_presets_widgets()
         self.agent_customisation.update_presets_widgets()
```

### Comparing `rlbot-1.9.5/rlbot/gui/rocket_league_items.json` & `rlbot-1.9.6/rlbot/gui/rocket_league_items.json`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/img/rlbot_icon.png` & `rlbot-1.9.6/rlbot/img/rlbot_icon.png`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/matchconfig/match_config.py` & `rlbot-1.9.6/rlbot/matchconfig/match_config.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/BallInfo.py` & `rlbot-1.9.6/rlbot/messages/flat/BallInfo.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/BallPrediction.py` & `rlbot-1.9.6/rlbot/messages/flat/BallPrediction.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/BallRigidBodyState.py` & `rlbot-1.9.6/rlbot/messages/flat/BallRigidBodyState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Bool.py` & `rlbot-1.9.6/rlbot/messages/flat/Bool.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/BoostPad.py` & `rlbot-1.9.6/rlbot/messages/flat/BoostPad.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/BoostPadState.py` & `rlbot-1.9.6/rlbot/messages/flat/BoostPadState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Color.py` & `rlbot-1.9.6/rlbot/messages/flat/Color.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/ControllerState.py` & `rlbot-1.9.6/rlbot/messages/flat/ControllerState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DesiredBallState.py` & `rlbot-1.9.6/rlbot/messages/flat/DesiredBallState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DesiredBoostState.py` & `rlbot-1.9.6/rlbot/messages/flat/DesiredBoostState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DesiredCarState.py` & `rlbot-1.9.6/rlbot/messages/flat/DesiredCarState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DesiredGameInfoState.py` & `rlbot-1.9.6/rlbot/messages/flat/DesiredGameInfoState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DesiredGameState.py` & `rlbot-1.9.6/rlbot/messages/flat/DesiredGameState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DesiredPhysics.py` & `rlbot-1.9.6/rlbot/messages/flat/DesiredPhysics.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DropShotBallInfo.py` & `rlbot-1.9.6/rlbot/messages/flat/DropShotBallInfo.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/DropshotTile.py` & `rlbot-1.9.6/rlbot/messages/flat/DropshotTile.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/FieldInfo.py` & `rlbot-1.9.6/rlbot/messages/flat/FieldInfo.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Float.py` & `rlbot-1.9.6/rlbot/messages/flat/Float.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/GameInfo.py` & `rlbot-1.9.6/rlbot/messages/flat/GameInfo.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/GameTickPacket.py` & `rlbot-1.9.6/rlbot/messages/flat/GameTickPacket.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/GoalInfo.py` & `rlbot-1.9.6/rlbot/messages/flat/GoalInfo.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Physics.py` & `rlbot-1.9.6/rlbot/messages/flat/Physics.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/PlayerInfo.py` & `rlbot-1.9.6/rlbot/messages/flat/PlayerInfo.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/PlayerInput.py` & `rlbot-1.9.6/rlbot/messages/flat/PlayerInput.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/PlayerRigidBodyState.py` & `rlbot-1.9.6/rlbot/messages/flat/PlayerRigidBodyState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/PredictionSlice.py` & `rlbot-1.9.6/rlbot/messages/flat/PredictionSlice.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Quaternion.py` & `rlbot-1.9.6/rlbot/messages/flat/Quaternion.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/QuickChat.py` & `rlbot-1.9.6/rlbot/messages/flat/QuickChat.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/QuickChatSelection.py` & `rlbot-1.9.6/rlbot/messages/flat/QuickChatSelection.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/RenderGroup.py` & `rlbot-1.9.6/rlbot/messages/flat/RenderGroup.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/RenderMessage.py` & `rlbot-1.9.6/rlbot/messages/flat/RenderMessage.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/RigidBodyState.py` & `rlbot-1.9.6/rlbot/messages/flat/RigidBodyState.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/RigidBodyTick.py` & `rlbot-1.9.6/rlbot/messages/flat/RigidBodyTick.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Rotator.py` & `rlbot-1.9.6/rlbot/messages/flat/Rotator.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/RotatorPartial.py` & `rlbot-1.9.6/rlbot/messages/flat/RotatorPartial.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/ScoreInfo.py` & `rlbot-1.9.6/rlbot/messages/flat/ScoreInfo.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/TinyBall.py` & `rlbot-1.9.6/rlbot/messages/flat/TinyBall.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/TinyPacket.py` & `rlbot-1.9.6/rlbot/messages/flat/TinyPacket.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/TinyPlayer.py` & `rlbot-1.9.6/rlbot/messages/flat/TinyPlayer.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Touch.py` & `rlbot-1.9.6/rlbot/messages/flat/Touch.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Vector3.py` & `rlbot-1.9.6/rlbot/messages/flat/Vector3.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/messages/flat/Vector3Partial.py` & `rlbot-1.9.6/rlbot/messages/flat/Vector3Partial.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/parsing/agent_config_parser.py` & `rlbot-1.9.6/rlbot/parsing/agent_config_parser.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/parsing/custom_config.py` & `rlbot-1.9.6/rlbot/parsing/custom_config.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/parsing/directory_scanner.py` & `rlbot-1.9.6/rlbot/parsing/directory_scanner.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/parsing/match_settings_config_parser.py` & `rlbot-1.9.6/rlbot/parsing/match_settings_config_parser.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/parsing/rlbot_config_parser.py` & `rlbot-1.9.6/rlbot/parsing/rlbot_config_parser.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/runner.py` & `rlbot-1.9.6/rlbot/runner.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/setup_manager.py` & `rlbot-1.9.6/rlbot/setup_manager.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/training/status_rendering.py` & `rlbot-1.9.6/rlbot/training/status_rendering.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/training/training.py` & `rlbot-1.9.6/rlbot/training/training.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/class_importer.py` & `rlbot-1.9.6/rlbot/utils/class_importer.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/file_util.py` & `rlbot-1.9.6/rlbot/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/game_state_util.py` & `rlbot-1.9.6/rlbot/utils/game_state_util.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/item_id_parser.py` & `rlbot-1.9.6/rlbot/utils/item_id_parser.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/logging_utils.py` & `rlbot-1.9.6/rlbot/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/prediction/dropshot.dat` & `rlbot-1.9.6/rlbot/utils/prediction/dropshot.dat`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/prediction/hoops.dat` & `rlbot-1.9.6/rlbot/utils/prediction/hoops.dat`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/prediction/prediction_util.py` & `rlbot-1.9.6/rlbot/utils/prediction/prediction_util.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/prediction/soccar.dat` & `rlbot-1.9.6/rlbot/utils/prediction/soccar.dat`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/process_configuration.py` & `rlbot-1.9.6/rlbot/utils/process_configuration.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/public_utils.py` & `rlbot-1.9.6/rlbot/utils/public_utils.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/python_version_check.py` & `rlbot-1.9.6/rlbot/utils/python_version_check.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/rate_limiter.py` & `rlbot-1.9.6/rlbot/utils/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/rendering/rendering_manager.py` & `rlbot-1.9.6/rlbot/utils/rendering/rendering_manager.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/rlbot_exception.py` & `rlbot-1.9.6/rlbot/utils/rlbot_exception.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/game_data_struct.py` & `rlbot-1.9.6/rlbot/utils/structures/game_data_struct.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/game_interface.py` & `rlbot-1.9.6/rlbot/utils/structures/game_interface.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/game_status.py` & `rlbot-1.9.6/rlbot/utils/structures/game_status.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/legacy_data_v3.py` & `rlbot-1.9.6/rlbot/utils/structures/legacy_data_v3.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/quick_chats.py` & `rlbot-1.9.6/rlbot/utils/structures/quick_chats.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/rigid_body_struct.py` & `rlbot-1.9.6/rlbot/utils/structures/rigid_body_struct.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/start_match_structures.py` & `rlbot-1.9.6/rlbot/utils/structures/start_match_structures.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/struct.py` & `rlbot-1.9.6/rlbot/utils/structures/struct.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/utils/structures/utils.py` & `rlbot-1.9.6/rlbot/utils/structures/utils.py`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/rlbot/version.py` & `rlbot-1.9.6/rlbot/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
 # https://stackoverflow.com/questions/458550/standard-way-to-embed-version-into-python-package
 
-__version__ = '1.9.5'
+__version__ = '1.9.6'
 
 release_notes = {
 
-    '1.9.5': """
+    '1.9.6': """
     - *Much* faster core dll initialization! - ccman32
     - Adding support for a training mode! Check out https://github.com/RLBot/RLBotTraining - DomNomNom
     - Allow the user to change the appearance of human and party-member bot agents via the GUI - r0bbi3
     - Added game speed info to game tick packet and the ability to modify it via state setting - Marvin
     - Make the game stop capturing the mouse cursor if only bots are playing - whatisaphone
     - Various quality-of-life improvements - DomNomNom
-    - Making the GUI load all bots in the current directory - tarehart
     - Match configuration refactoring to make new GUIs easier - tarehart
     """,
 
     '1.8.3': """
     - Allow SimpleControllerState initialization. - Marvin
     - Passing more params to subprocess agents. - whatisaphone
     - Made game data structs support comparison and repr in python. - DomNomNom
```

### Comparing `rlbot-1.9.5/rlbot.egg-info/PKG-INFO` & `rlbot-1.9.6/rlbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlbot
-Version: 1.9.5
+Version: 1.9.6
 Summary: A framework for writing custom Rocket League bots that run offline.
 Home-page: https://github.com/RLBot/RLBot
 Author: RLBot Community
 Author-email: rlbotofficial@gmail.com
 License: UNKNOWN
 Description: # RLBot
```

### Comparing `rlbot-1.9.5/rlbot.egg-info/SOURCES.txt` & `rlbot-1.9.6/rlbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlbot-1.9.5/setup.py` & `rlbot-1.9.6/setup.py`

 * *Files identical despite different names*


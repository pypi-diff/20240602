# Comparing `tmp/gpt_computer_assistant-0.6.0.tar.gz` & `tmp/gpt_computer_assistant-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_computer_assistant-0.6.0.tar", last modified: Wed May 29 11:09:51 2024, max compression
+gzip compressed data, was "gpt_computer_assistant-0.6.1.tar", last modified: Sun Jun  2 02:19:21 2024, max compression
```

## Comparing `gpt_computer_assistant-0.6.0.tar` & `gpt_computer_assistant-0.6.1.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.524117 gpt_computer_assistant-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.508117 gpt_computer_assistant-0.6.0/.git/
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.512117 gpt_computer_assistant-0.6.0/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     4726 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     1649 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     1374 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     4898 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     2783 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     2308 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.512117 gpt_computer_assistant-0.6.0/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-05-29 11:09:38.000000 gpt_computer_assistant-0.6.0/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.512117 gpt_computer_assistant-0.6.0/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.508117 gpt_computer_assistant-0.6.0/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.512117 gpt_computer_assistant-0.6.0/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.508117 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.512117 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Added-different-profiles-mode
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Added-icon
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Added-input-box-and-button
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Added-just-text-mode
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Added-reset-system
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Added-send-text-with-screenshot-button
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Added-splitting-long-audios
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/Fixed-high-delay-problem
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/logs/refs/remotes/origin/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.508117 gpt_computer_assistant-0.6.0/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.516117 gpt_computer_assistant-0.6.0/.git/objects/pack/
--r--r--r--   0 runner    (1001) docker     (127)     9388 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.idx
--r--r--r--   0 runner    (1001) docker     (127)    67141 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.pack
--r--r--r--   0 runner    (1001) docker     (127)     1240 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.rev
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.508117 gpt_computer_assistant-0.6.0/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.516117 gpt_computer_assistant-0.6.0/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.508117 gpt_computer_assistant-0.6.0/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.516117 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Added-different-profiles-mode
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Added-icon
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Added-input-box-and-button
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Added-just-text-mode
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Added-reset-system
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Added-send-text-with-screenshot-button
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Added-splitting-long-audios
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/Fixed-high-delay-problem
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/remotes/origin/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.520117 gpt_computer_assistant-0.6.0/.git/refs/tags/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.1.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.1.1
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.1.2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.2.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.3.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.4.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.5.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.5.1
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.5.2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.5.3
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.5.4
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.5.5
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.5.6
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.git/refs/tags/v0.6.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.508117 gpt_computer_assistant-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.520117 gpt_computer_assistant-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.github/workflows/deploys.yml
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.github/workflows/release_generation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-29 11:09:51.524117 gpt_computer_assistant-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/bump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.520117 gpt_computer_assistant-0.6.0/gpt_computer_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.520117 gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/background.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/proccess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.520117 gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/gpt_computer_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.524117 gpt_computer_assistant-0.6.0/gpt_computer_assistant/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/gui/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/gui/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.524117 gpt_computer_assistant-0.6.0/gpt_computer_assistant/screen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/screen/shot.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.524117 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.524117 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_24.png
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_256.png
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_48.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:09:51.520117 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-29 11:09:51.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-29 11:09:51.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:09:51.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 11:09:51.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:09:51.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 11:09:51.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 11:09:51.000000 gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:09:51.524117 gpt_computer_assistant-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-29 11:09:39.000000 gpt_computer_assistant-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.848530 gpt_computer_assistant-0.6.1/.git/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.848530 gpt_computer_assistant-0.6.1/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4726 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1649 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1374 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4898 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2783 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2308 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.848530 gpt_computer_assistant-0.6.1/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.852530 gpt_computer_assistant-0.6.1/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.844530 gpt_computer_assistant-0.6.1/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.852530 gpt_computer_assistant-0.6.1/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.844530 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.852530 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Added-different-profiles-mode
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Added-icon
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Added-input-box-and-button
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Added-just-text-mode
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Added-reset-system
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Added-send-text-with-screenshot-button
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Added-splitting-long-audios
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/Fixed-high-delay-problem
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/logs/refs/remotes/origin/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.844530 gpt_computer_assistant-0.6.1/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.852530 gpt_computer_assistant-0.6.1/.git/objects/pack/
+-r--r--r--   0 runner    (1001) docker     (127)    10004 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.idx
+-r--r--r--   0 runner    (1001) docker     (127)    72953 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.pack
+-r--r--r--   0 runner    (1001) docker     (127)     1328 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.rev
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.844530 gpt_computer_assistant-0.6.1/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.852530 gpt_computer_assistant-0.6.1/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.844530 gpt_computer_assistant-0.6.1/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.852530 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Added-different-profiles-mode
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Added-icon
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Added-input-box-and-button
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Added-just-text-mode
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Added-reset-system
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Added-send-text-with-screenshot-button
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Added-splitting-long-audios
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/Fixed-high-delay-problem
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/remotes/origin/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.856530 gpt_computer_assistant-0.6.1/.git/refs/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.1.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.1.1
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.1.2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.2.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.3.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.4.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.5.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.5.1
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.5.2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.5.3
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.5.4
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.5.5
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.5.6
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.6.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.git/refs/tags/v0.6.1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.844530 gpt_computer_assistant-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.856530 gpt_computer_assistant-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.github/workflows/deploys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.github/workflows/release_generation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/bump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.856530 gpt_computer_assistant-0.6.1/gpt_computer_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.856530 gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/proccess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/gpt_computer_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/gpt_computer_assistant/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/gui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/gui/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/gpt_computer_assistant/screen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/screen/shot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_48.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:19:21.856530 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-06-02 02:19:21.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-06-02 02:19:21.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 02:19:21.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 02:19:21.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 02:19:21.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-06-02 02:19:21.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 02:19:21.000000 gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 02:19:21.860530 gpt_computer_assistant-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-06-02 02:19:12.000000 gpt_computer_assistant-0.6.1/setup.py
```

### Comparing `gpt_computer_assistant-0.6.0/.git/FETCH_HEAD` & `gpt_computer_assistant-0.6.1/.git/FETCH_HEAD`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 022602896b15b5f11ad0dae0eaf31ca8b831b4eb		branch 'Added-icon' of https://github.com/onuratakan/gpt-computer-assistant
 f95a6816826e3b6cc5a2909ef8aef549d07a84b0		branch 'Added-input-box-and-button' of https://github.com/onuratakan/gpt-computer-assistant
 6a17387dda1243d1f09a807d5a2050d671e75c67		branch 'Added-just-text-mode' of https://github.com/onuratakan/gpt-computer-assistant
 f78094740a29a0b2e1eca2342d212905402a677e		branch 'Added-reset-system' of https://github.com/onuratakan/gpt-computer-assistant
 50295c84604bda90fd953593c25f2d00e5d124f0		branch 'Added-send-text-with-screenshot-button' of https://github.com/onuratakan/gpt-computer-assistant
 ea9dc1adcbee374bf5b901a5f11a3c9737b0518e		branch 'Added-splitting-long-audios' of https://github.com/onuratakan/gpt-computer-assistant
 aa3faf3045dcf6d80fd424b210d02aee0b2476d4		branch 'Fixed-high-delay-problem' of https://github.com/onuratakan/gpt-computer-assistant
-d161139c9d8ea8ef4e2dc3d558e32ae69c16e7aa		branch 'master' of https://github.com/onuratakan/gpt-computer-assistant
+ce0c41e1bd398e7b73b0e78c5d95cd6bccca1023		branch 'master' of https://github.com/onuratakan/gpt-computer-assistant
 920866c012c25fbbe11d9f162ad26b386402190f		tag 'v0.1.0' of https://github.com/onuratakan/gpt-computer-assistant
 cb203784ebebd5e6885ae69822caa8d8cfaf4ed4		tag 'v0.1.1' of https://github.com/onuratakan/gpt-computer-assistant
 d77bb1033a9d51fb08619c8b63860e57e10a11b1		tag 'v0.1.2' of https://github.com/onuratakan/gpt-computer-assistant
 365d62393dc41c08e483d3c917da0ff85fcaae0f		tag 'v0.2.0' of https://github.com/onuratakan/gpt-computer-assistant
 d967f0e3518a5b57926ed042290d1032c14e2e5a		tag 'v0.3.0' of https://github.com/onuratakan/gpt-computer-assistant
 c7926ae60405f5b243d9b4efee3b601cd7f2626d		tag 'v0.4.0' of https://github.com/onuratakan/gpt-computer-assistant
 c4ceb708ba860a5d0efec7661978e1f48881da70		tag 'v0.5.0' of https://github.com/onuratakan/gpt-computer-assistant
 227564663235da9afcbce78c10bfbcca1f5698ed		tag 'v0.5.1' of https://github.com/onuratakan/gpt-computer-assistant
 a93ff7af535e15fb644a3da6ca21d496bc980e87		tag 'v0.5.2' of https://github.com/onuratakan/gpt-computer-assistant
 aae17c3207063f00265522ea7fcd1ef971cccc85		tag 'v0.5.3' of https://github.com/onuratakan/gpt-computer-assistant
 1723625f6ac0e9fb4a39f5b90d1cef73ac7d53bb		tag 'v0.5.4' of https://github.com/onuratakan/gpt-computer-assistant
 c7f5d1052f93504bff5527db3bb2f4a8619cd566		tag 'v0.5.5' of https://github.com/onuratakan/gpt-computer-assistant
 06a8461621130428f5d4be2642a37bcb62d7e1c4		tag 'v0.5.6' of https://github.com/onuratakan/gpt-computer-assistant
 d161139c9d8ea8ef4e2dc3d558e32ae69c16e7aa		tag 'v0.6.0' of https://github.com/onuratakan/gpt-computer-assistant
+ce0c41e1bd398e7b73b0e78c5d95cd6bccca1023		tag 'v0.6.1' of https://github.com/onuratakan/gpt-computer-assistant
```

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/commit-msg.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/fsmonitor-watchman.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/pre-commit.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/pre-push.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/pre-rebase.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/pre-receive.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/prepare-commit-msg.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/push-to-checkout.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/sendemail-validate.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/hooks/update.sample` & `gpt_computer_assistant-0.6.1/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.idx` & `gpt_computer_assistant-0.6.1/.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.idx`

 * *Files 14% similar despite different names*

```diff
@@ -1,587 +1,626 @@
 00000000: ff74 4f63 0000 0002 0000 0001 0000 0004  .tOc............
 00000010: 0000 0006 0000 0006 0000 0008 0000 0008  ................
-00000020: 0000 0009 0000 000b 0000 000b 0000 000d  ................
-00000030: 0000 000e 0000 0010 0000 0012 0000 0013  ................
-00000040: 0000 0014 0000 0015 0000 0016 0000 0017  ................
-00000050: 0000 0017 0000 0017 0000 001b 0000 001b  ................
-00000060: 0000 001e 0000 001f 0000 0021 0000 0021  ...........!...!
-00000070: 0000 0022 0000 0022 0000 0024 0000 0025  ..."..."...$...%
-00000080: 0000 0025 0000 0025 0000 0026 0000 0028  ...%...%...&...(
-00000090: 0000 0029 0000 002a 0000 002a 0000 002c  ...)...*...*...,
-000000a0: 0000 002c 0000 002d 0000 002e 0000 0030  ...,...-.......0
-000000b0: 0000 0031 0000 0031 0000 0031 0000 0032  ...1...1...1...2
-000000c0: 0000 0032 0000 0032 0000 0032 0000 0034  ...2...2...2...4
-000000d0: 0000 0036 0000 0037 0000 0039 0000 003b  ...6...7...9...;
-000000e0: 0000 003d 0000 003d 0000 003f 0000 0040  ...=...=...?...@
-000000f0: 0000 0042 0000 0043 0000 0044 0000 0046  ...B...C...D...F
-00000100: 0000 004a 0000 004d 0000 004e 0000 004e  ...J...M...N...N
-00000110: 0000 004f 0000 004f 0000 0052 0000 0055  ...O...O...R...U
-00000120: 0000 0055 0000 0055 0000 0055 0000 0056  ...U...U...U...V
-00000130: 0000 0056 0000 0056 0000 0059 0000 005c  ...V...V...Y...\
-00000140: 0000 005c 0000 005d 0000 005f 0000 005f  ...\...]..._..._
-00000150: 0000 0060 0000 0060 0000 0060 0000 0062  ...`...`...`...b
-00000160: 0000 0062 0000 0062 0000 0063 0000 0063  ...b...b...c...c
-00000170: 0000 0063 0000 0065 0000 0065 0000 0066  ...c...e...e...f
-00000180: 0000 0068 0000 006b 0000 006d 0000 006e  ...h...k...m...n
-00000190: 0000 006f 0000 006f 0000 006f 0000 006f  ...o...o...o...o
-000001a0: 0000 0070 0000 0071 0000 0074 0000 0074  ...p...q...t...t
-000001b0: 0000 0075 0000 0075 0000 0076 0000 0079  ...u...u...v...y
-000001c0: 0000 007a 0000 007d 0000 007e 0000 007f  ...z...}...~....
-000001d0: 0000 007f 0000 007f 0000 0080 0000 0082  ................
-000001e0: 0000 0083 0000 0085 0000 0086 0000 0087  ................
-000001f0: 0000 0088 0000 0088 0000 008a 0000 008c  ................
-00000200: 0000 008e 0000 008e 0000 0090 0000 0092  ................
-00000210: 0000 0093 0000 0093 0000 0095 0000 0096  ................
-00000220: 0000 0099 0000 0099 0000 009c 0000 009d  ................
-00000230: 0000 009d 0000 009d 0000 009d 0000 009e  ................
-00000240: 0000 009e 0000 00a0 0000 00a0 0000 00a1  ................
-00000250: 0000 00a3 0000 00a3 0000 00a3 0000 00a4  ................
-00000260: 0000 00a5 0000 00a5 0000 00a5 0000 00a5  ................
-00000270: 0000 00a6 0000 00a8 0000 00a9 0000 00aa  ................
-00000280: 0000 00ab 0000 00ab 0000 00ac 0000 00ad  ................
-00000290: 0000 00af 0000 00b0 0000 00b1 0000 00b3  ................
-000002a0: 0000 00b4 0000 00b5 0000 00b8 0000 00bb  ................
-000002b0: 0000 00bf 0000 00c0 0000 00c0 0000 00c1  ................
-000002c0: 0000 00c1 0000 00c2 0000 00c4 0000 00c5  ................
-000002d0: 0000 00c6 0000 00c6 0000 00c6 0000 00c7  ................
-000002e0: 0000 00c9 0000 00cb 0000 00cd 0000 00ce  ................
-000002f0: 0000 00ce 0000 00cf 0000 00d1 0000 00d1  ................
-00000300: 0000 00d3 0000 00d4 0000 00d4 0000 00d5  ................
-00000310: 0000 00d8 0000 00d8 0000 00da 0000 00db  ................
-00000320: 0000 00dc 0000 00df 0000 00e1 0000 00e2  ................
-00000330: 0000 00e4 0000 00e5 0000 00e7 0000 00e8  ................
-00000340: 0000 00e8 0000 00ea 0000 00ea 0000 00eb  ................
-00000350: 0000 00ee 0000 00ef 0000 00ef 0000 00f1  ................
-00000360: 0000 00f2 0000 00f3 0000 00f3 0000 00f4  ................
-00000370: 0000 00f5 0000 00f7 0000 00f7 0000 00f9  ................
-00000380: 0000 00fe 0000 00fe 0000 0102 0000 0104  ................
-00000390: 0000 0106 0000 0106 0000 0108 0000 010a  ................
-000003a0: 0000 010d 0000 010f 0000 0111 0000 0113  ................
-000003b0: 0000 0114 0000 0115 0000 0115 0000 0117  ................
-000003c0: 0000 0117 0000 0118 0000 0118 0000 0119  ................
-000003d0: 0000 011a 0000 011b 0000 011c 0000 011c  ................
-000003e0: 0000 011e 0000 011f 0000 0120 0000 0123  ........... ...#
-000003f0: 0000 0123 0000 0125 0000 0127 0000 0128  ...#...%...'...(
-00000400: 0000 0129 0000 0129 00dd d47f dfd7 1a8b  ...)...)........
+00000020: 0000 0009 0000 000b 0000 000b 0000 000e  ................
+00000030: 0000 000f 0000 0011 0000 0013 0000 0014  ................
+00000040: 0000 0015 0000 0016 0000 0017 0000 0018  ................
+00000050: 0000 0018 0000 0018 0000 001c 0000 001c  ................
+00000060: 0000 001f 0000 0020 0000 0023 0000 0024  ....... ...#...$
+00000070: 0000 0025 0000 0025 0000 0027 0000 0029  ...%...%...'...)
+00000080: 0000 0029 0000 0029 0000 002a 0000 002c  ...)...)...*...,
+00000090: 0000 002d 0000 002e 0000 002e 0000 0030  ...-...........0
+000000a0: 0000 0030 0000 0031 0000 0032 0000 0034  ...0...1...2...4
+000000b0: 0000 0035 0000 0035 0000 0035 0000 0036  ...5...5...5...6
+000000c0: 0000 0036 0000 0036 0000 0036 0000 0038  ...6...6...6...8
+000000d0: 0000 003a 0000 003b 0000 003d 0000 003f  ...:...;...=...?
+000000e0: 0000 0041 0000 0041 0000 0043 0000 0044  ...A...A...C...D
+000000f0: 0000 0046 0000 0047 0000 0048 0000 004a  ...F...G...H...J
+00000100: 0000 004e 0000 0051 0000 0052 0000 0052  ...N...Q...R...R
+00000110: 0000 0054 0000 0054 0000 0057 0000 005a  ...T...T...W...Z
+00000120: 0000 005a 0000 005a 0000 005a 0000 005b  ...Z...Z...Z...[
+00000130: 0000 005c 0000 005c 0000 005f 0000 0062  ...\...\..._...b
+00000140: 0000 0062 0000 0063 0000 0065 0000 0066  ...b...c...e...f
+00000150: 0000 0068 0000 0068 0000 0068 0000 006a  ...h...h...h...j
+00000160: 0000 006a 0000 006a 0000 006b 0000 006b  ...j...j...k...k
+00000170: 0000 006b 0000 006d 0000 006d 0000 006e  ...k...m...m...n
+00000180: 0000 0070 0000 0073 0000 0075 0000 0076  ...p...s...u...v
+00000190: 0000 0077 0000 0077 0000 0077 0000 0077  ...w...w...w...w
+000001a0: 0000 0078 0000 0079 0000 007c 0000 007c  ...x...y...|...|
+000001b0: 0000 007d 0000 007f 0000 0081 0000 0084  ...}............
+000001c0: 0000 0085 0000 0088 0000 0089 0000 008a  ................
+000001d0: 0000 008b 0000 008b 0000 008c 0000 008e  ................
+000001e0: 0000 008f 0000 0091 0000 0092 0000 0093  ................
+000001f0: 0000 0094 0000 0094 0000 0096 0000 0098  ................
+00000200: 0000 009b 0000 009b 0000 009d 0000 009f  ................
+00000210: 0000 00a0 0000 00a0 0000 00a2 0000 00a3  ................
+00000220: 0000 00a6 0000 00a6 0000 00a9 0000 00aa  ................
+00000230: 0000 00aa 0000 00aa 0000 00aa 0000 00ab  ................
+00000240: 0000 00ab 0000 00ad 0000 00ad 0000 00ae  ................
+00000250: 0000 00b0 0000 00b0 0000 00b0 0000 00b1  ................
+00000260: 0000 00b2 0000 00b2 0000 00b3 0000 00b5  ................
+00000270: 0000 00b6 0000 00b8 0000 00b9 0000 00ba  ................
+00000280: 0000 00bb 0000 00bb 0000 00bc 0000 00bd  ................
+00000290: 0000 00bf 0000 00c0 0000 00c1 0000 00c3  ................
+000002a0: 0000 00c4 0000 00c5 0000 00c8 0000 00cb  ................
+000002b0: 0000 00cf 0000 00d0 0000 00d0 0000 00d1  ................
+000002c0: 0000 00d1 0000 00d2 0000 00d4 0000 00d5  ................
+000002d0: 0000 00d6 0000 00d6 0000 00d6 0000 00d7  ................
+000002e0: 0000 00d9 0000 00db 0000 00dd 0000 00de  ................
+000002f0: 0000 00de 0000 00df 0000 00e1 0000 00e1  ................
+00000300: 0000 00e3 0000 00e4 0000 00e5 0000 00e6  ................
+00000310: 0000 00e9 0000 00e9 0000 00eb 0000 00ec  ................
+00000320: 0000 00ed 0000 00f0 0000 00f3 0000 00f4  ................
+00000330: 0000 00f6 0000 00f7 0000 00f9 0000 00fa  ................
+00000340: 0000 00fb 0000 00fd 0000 00fd 0000 00fe  ................
+00000350: 0000 0102 0000 0103 0000 0103 0000 0105  ................
+00000360: 0000 0106 0000 0107 0000 0107 0000 0108  ................
+00000370: 0000 0109 0000 010b 0000 010b 0000 010d  ................
+00000380: 0000 0113 0000 0113 0000 0117 0000 0119  ................
+00000390: 0000 011b 0000 011b 0000 011d 0000 0120  ............... 
+000003a0: 0000 0123 0000 0125 0000 0127 0000 0129  ...#...%...'...)
+000003b0: 0000 012a 0000 012b 0000 012b 0000 012d  ...*...+...+...-
+000003c0: 0000 012d 0000 012e 0000 012e 0000 012f  ...-.........../
+000003d0: 0000 0130 0000 0131 0000 0132 0000 0132  ...0...1...2...2
+000003e0: 0000 0134 0000 0135 0000 0136 0000 0139  ...4...5...6...9
+000003f0: 0000 0139 0000 013b 0000 013d 0000 013e  ...9...;...=...>
+00000400: 0000 013f 0000 013f 00dd d47f dfd7 1a8b  ...?...?........
 00000410: b29c 7c1e ba49 3daf 4967 93c2 0180 f89b  ..|..I=.Ig......
 00000420: e496 a0ae 013b ee5a d694 b83e 83ae fde6  .....;.Z...>....
 00000430: 01cb 31ed 14ca 49cd a7c6 7b2d dc79 6a89  ..1...I...{-.yj.
 00000440: 8f88 45d4 01f5 0b52 87ff b115 4de5 4f1d  ..E....R....M.O.
 00000450: ba3f 07ae 6cbd 1e89 0226 0289 6b15 b5f1  .?..l....&..k...
 00000460: 1ad0 dae0 eaf3 1ca8 b831 b4eb 02e2 e3ff  .........1......
 00000470: 9b9a b5a5 646b 8d52 d2fc c1c5 ab6c cffa  ....dk.R.....l..
 00000480: 0488 e2c8 7683 914c 32de aaa8 667e 7497  ....v..L2...f~t.
 00000490: f76a 04d8 04c7 bfac c732 846e 5d1e 459d  .j.......2.n].E.
 000004a0: 18b3 1b08 07e3 db6e 06a8 4616 2113 0428  .......n..F.!..(
 000004b0: f5d4 be26 42a3 7bcb 62d7 e1c4 0725 883b  ...&B.{.b....%.;
 000004c0: 4fee 1fed 28e6 bc64 a993 11c9 4684 0053  O...(..d....F..S
 000004d0: 076b 11c0 012f 9e04 a9d5 4016 1c16 ecb5  .k.../....@.....
-000004e0: 0bce f460 09a6 8b4b bcdd f77d 7431 7fd9  ...`...K...}t1..
-000004f0: e224 50d8 c445 607e 09f4 9f7d 68f4 2b0f  .$P..E`~...}h.+.
-00000500: 750e 2aba 9acb 1daa c79d 50c9 0aac 1694  u.*.......P.....
-00000510: 4d6b 28c7 fc05 9944 50df 60a7 6888 f41f  Mk(....DP.`.h...
-00000520: 0b34 c374 78ab 675c 6ad3 9730 ccf9 8af1  .4.tx.g\j..0....
-00000530: 88e7 0ff9 0b97 6447 69b2 7988 d3bb 69be  ......dGi.y...i.
-00000540: 2584 342c e189 8804 0c2e 2a86 e7d7 efbf  %.4,......*.....
-00000550: 512b cf6b 85cf 6a38 a898 0019 0c91 98ac  Q+.k..j8........
-00000560: ccb3 d1ad d56b 4496 e591 fa18 cbaf 64fc  .....kD.......d.
-00000570: 0d82 432f c2d9 3143 d515 42d0 f4ed 03b6  ..C/..1C..B.....
-00000580: 3bff 69a2 0ea0 e38a 01b8 958f fbcf 297a  ;.i...........)z
-00000590: a773 effe 3623 34d0 0fee 61e9 f377 8410  .s..6#4...a..w..
-000005a0: 9916 ff54 035f 13f5 14df 8360 1025 1521  ...T._.....`.%.!
-000005b0: c1c9 9f77 238b 4860 3be0 42ba 5823 a198  ...w#.H`;.B.X#..
-000005c0: 1129 d93b 10cf ecb6 235a 9e7f 4ab5 3cc7  .).;....#Z..J.<.
-000005d0: 24ed 056c 1427 6e10 d8a0 d752 dc35 3a7c  $..l.'n....R.5:|
-000005e0: d10a 253b c579 379a 1433 ce41 50bb b18b  ..%;.y7..3.AP...
-000005f0: f7b3 c2d6 c4b8 9b32 084c 1e7d 146c addd  .......2.L.}.l..
-00000600: 63f0 e9df a465 4491 1313 6c6e 330e 20cd  c....eD...ln3. .
-00000610: 149b 0c8c 5257 8dc6 3594 ea2a 36cb 3cfd  ....RW..5..*6.<.
-00000620: 7feb 0b17 165c 1d7d e49a 08aa f59e d43a  .....\.}.......:
-00000630: c2a9 ba68 b811 30e8 1666 45c6 e558 e949  ...h..0..fE..X.I
-00000640: 854d 6828 6bf7 a958 2a47 a2a0 16f3 c37c  .Mh(k..X*G.....|
-00000650: 7b5d 4e84 c784 5968 05df 80c6 acbf 1568  {]N...Yh.......h
-00000660: 1723 625f 6ac0 e9fb 4a39 f5b9 0d1c ef73  .#b_j...J9.....s
-00000670: ac7d 53bb 1853 d346 d7ad 03dd b20b 6093  .}S..S.F......`.
-00000680: e2c7 a1ed 8a3a 72b2 18b4 e9fc ef00 0284  .....:r.........
-00000690: d53a 8288 d7e2 7c5e 3564 58cc 1a03 eb1a  .:....|^5dX.....
-000006a0: b938 e53b cd11 68ce cc2b f86e 20aa 761b  .8.;..h..+.n .v.
-000006b0: 1cf3 c9c3 075c 1fab a1eb d396 5764 e2ec  .....\......Wd..
-000006c0: af17 751b 1cf4 502a 6173 de16 a0db 5cd2  ..u...P*as....\.
-000006d0: e32b 2cd8 0f07 83d0 1d2b bf74 d823 f98f  .+,......+.t.#..
-000006e0: c203 f082 b56e 911f fa50 492e 2044 d5a0  .....n...PI. D..
-000006f0: 9f55 22b9 616b 252c 0891 a6e8 aa7b ca64  .U".ak%,.....{.d
-00000700: 2175 1d36 f8f1 7ce9 6aaf c278 22e2 0b6f  !u.6..|.j..x"..o
-00000710: c35e 999d 21c5 7523 5cca a33e d69d 759c  .^..!.u#\..>..u.
-00000720: cecb cbcb e5c2 16a6 2275 6466 3235 da9a  ........"udf25..
-00000730: fcbc e78c 10bf bcca 1f56 98ed 2302 d30b  .........V..#...
-00000740: 1108 da08 5d35 9b7b 0054 2e6d 1846 0766  ....]5.{.T.m.F.f
-00000750: 2559 1dca 5a32 c357 c6e7 d67c 9d88 fdf9  %Y..Z2.W...|....
-00000760: 9e57 2191 25f2 e150 2c69 b4cf 1669 971b  .W!.%..P,i...i..
-00000770: 9616 8399 2ca6 6ba4 27d5 b1bf 06a5 daa9  ....,.k.'.......
-00000780: 29cb 20bf d4a1 6010 7e6c 8063 284d 716a  ). ...`.~l.c(Mqj
-00000790: b3c7 2c7c 1ec5 1fa5 23db e011 09f2 320a  ..,|....#.....2.
-000007a0: 297d ac16 0961 f0ae ea73 2374 aae4 2697  )}...a...s#t..&.
-000007b0: 5013 3328 29d2 daac 5904 9917 2e55 4126  P.3()...Y....UA&
-000007c0: d72d 43d3 0ed5 a046 2a42 2fef b908 c755  .-C....F*B/....U
-000007d0: 9dd2 f716 8efc 378b 8785 ba62 2df2 9c70  ......7....b-..p
-000007e0: 5bc4 7bc7 c268 e8c4 92b6 458e 3b67 b03b  [.{..h....E.;g.;
-000007f0: 31ce d298 ccae 493b e277 6bdb 7184 b4e3  1.....I;.wk.q...
-00000800: 6003 36da 31d7 7150 caee 8e4d ec78 f304  `.6.1.qP...M.x..
-00000810: 09f4 fe0d eab6 11c1 32d8 331c 3e6f 336e  ........2.3.>o3n
-00000820: df84 ee6e 954e 0e72 1de3 a1a4 32e8 3d4f  ...n.N.r....2.=O
-00000830: cefa 3337 032a 8247 709f 7b53 03b1 32e9  ..37.*.Gp.{S..2.
-00000840: 3370 fbd1 c498 f950 017e df7e 2c97 7834  3p.....P.~.~,.x4
-00000850: a9df 0ff3 34c0 bb3d 74e1 47d3 c9f2 0418  ....4..=t.G.....
-00000860: c0f5 1abb 06a4 6efd 34fc f02c f342 4990  ......n.4..,.BI.
-00000870: f69a a8e4 f751 2b31 0cb5 15aa 355a e6e3  .....Q+1....5Z..
-00000880: 9381 137f 02e6 af0d a71f d969 2974 9429  ...........i)t.)
-00000890: 35a8 559d 8e8f 8390 86cb bd78 32a5 9c0d  5.U........x2...
-000008a0: df0e 5bf6 360c ff80 3fc6 5590 e0d0 27f9  ..[.6...?.U...'.
-000008b0: a255 de67 569f 098d 365d 6239 3dc4 1c08  .U.gV...6]b9=...
-000008c0: e483 d3c9 17da 0ff8 5fca ae0f 3850 1419  ........_...8P..
-000008d0: 135d df9b 36fa d8bd 2e4f 612b 5be2 e775  .]..6....Oa+[..u
-000008e0: 3894 9563 e601 a524 7c22 e6bd 1f6e ad7d  8..c...$|"...n.}
-000008f0: f98e 0a8d 3911 2369 cdb9 958c 956f e5bc  ....9.#i.....o..
-00000900: a73f 34f7 4d75 2891 3a7c 49fa 26f4 32f2  .?4.Mu(.:|I.&.2.
-00000910: 91f4 f49b 21b4 804c 0f5b 1178 3afd 2ed1  ....!..L.[.x:...
-00000920: 5f67 3613 7040 b4ef f58b 1a94 f096 7bd1  _g6.p@........{.
-00000930: 3baf b2ce f39b 0d2d 3b2d ff8a 301d 54b1  ;......-;-..0.T.
-00000940: c839 2969 3c0a b25e 76cc 5ed1 1c73 b8fe  .9)i<..^v.^..s..
-00000950: a7aa 5496 ebad a7ce 3de3 3dde ee30 fce9  ..T.....=.=..0..
-00000960: 17ab 3a10 b9cb 365b 625b 9fea 3def 1c80  ..:...6[b[..=...
-00000970: d6b0 cdbc 7ded 1060 4a95 aad6 62ce bb4c  ....}..`J...b..L
-00000980: 3e52 8de3 bf3e 0e9d eed6 d86d 0033 89b7  >R...>.....m.3..
-00000990: cb85 84a3 3e5f 999b 65e4 d565 2911 1ad1  ....>_..e..e)...
-000009a0: 92bf c6de 425c af47 3e69 9a2f a996 ddb0  ....B\.G>i./....
-000009b0: f8b3 f6e1 4432 2091 56f0 2438 3eb7 bc56  ....D2 .V.$8>..V
-000009c0: e4df 97de 4168 f673 d2ad 0c87 934a 3c44  ....Ah.s.....J<D
-000009d0: 3f05 0000 f2c4 5598 557b 2475 49b2 73d1  ?.....U.U{$uI.s.
-000009e0: 1881 f3df 3f0c 6fb8 2eb9 cfd9 0542 a8dc  ....?.o......B..
-000009f0: 2572 f632 97e5 f65d 3ff6 be70 55a7 961c  %r.2...]?..pU...
-00000a00: d77e 3ebf c323 2730 223b 51c3 40e6 0d18  .~>..#'0";Q.@...
-00000a10: 6d78 d3e8 53df cf06 77ac 1884 8e9f 8e58  mx..S...w......X
-00000a20: 424a b1c4 93de ac0b 8f36 5f23 f732 fd74  BJ.......6_#.2.t
-00000a30: e86a bcad 4471 35ed 9af9 bf37 13da 009f  .j..Dq5....7....
-00000a40: 3875 d0bb 3a2a 9b74 4477 b3e9 5a6c 3a22  8u..:*.tDw..Zl:"
-00000a50: d991 37b0 0859 53a8 7d7f fe9a 44a0 9b43  ..7..YS.}...D..C
-00000a60: 62d3 2602 7ef2 17a4 e5f4 a8de fd57 8799  b.&.~........W..
-00000a70: 4508 ca52 16d7 d238 30a7 d1ec 0df7 8aa2  E..R...80.......
-00000a80: 6e33 cb40 456b 4288 e355 ea73 6090 7fee  n3.@EkB..U.s`...
-00000a90: 092b b823 35e8 8f80 4580 739d a623 49c6  .+.#5...E.s..#I.
-00000aa0: a495 ff9f c82f 8c61 61d3 7161 49cd 9536  ...../.aa.qaI..6
-00000ab0: f437 89ff c916 0caa df9a 10e4 3dee 51f4  .7..........=.Q.
-00000ac0: 4c06 bf6b 863b e410 bac2 8981 a2a3 8726  L..k.;.........&
-00000ad0: fc6c 0f08 4c76 5c8e 185b a58b 2940 0aa0  .l..Lv\..[..)@..
-00000ae0: 4159 3efb b06c b0f5 4cf1 a726 2bc2 065d  AY>..l..L..&+..]
-00000af0: 939f d8ae 1261 957e 48fb ea8b 4d72 18da  .....a.~H...Mr..
-00000b00: aa31 ae06 9d5d 620a 13c0 bbac 435b 4cbb  .1...]b.....C[L.
-00000b10: 4da8 26bd a9a8 9d63 e26d 45d1 a21c 3f63  M.&....c.mE...?c
-00000b20: 7b19 a972 4dd6 6e60 7078 e4a1 3333 8a1c  {..rM.n`px..33..
-00000b30: 03a6 d316 083d b588 4fad 480f 0c74 0a54  .....=..O.H..t.T
-00000b40: d524 976a cde9 3369 3350 4ff7 5029 5c84  .$.j..3i3PO.P)\.
-00000b50: 604b da90 fd95 3593 c25f 2d00 e5d1 24f0  `K....5.._-...$.
-00000b60: 50aa 047f d1f7 7bac ba02 28d0 d3e7 a8b3  P.....{...(.....
-00000b70: 42cb 24ec 5217 9473 2a87 4182 d35a d847  B.$.R..s*.A..Z.G
-00000b80: eca2 dd45 d091 d351 5550 24f2 3d09 12c9  ...E...QUP$.=...
-00000b90: af2c 1ea3 8653 3abb 2609 efb9 5569 91ac  .,...S:.&...Ui..
-00000ba0: f0e9 2153 612e 4b34 ac5f 4290 43e1 1c53  ..!Sa.K4._B.C..S
-00000bb0: 58ff 10c2 6e80 dcd2 39c1 c1ef 2758 9904  X...n...9...'X..
-00000bc0: 8e15 56d7 5b11 9f7b bc8c 6940 091b 70d3  ..V.[..{..i@..p.
-00000bd0: 0c1e a19c 3ae4 e1dc 5b8b 005f aff9 ea30  ....:...[.._...0
-00000be0: 8819 4373 0a5f 392f 20d5 bcca 5dd1 ad3c  ..Cs._9/ ...]..<
-00000bf0: aa9a 991f e496 20a4 421e 7c98 a062 9eb7  ...... .B.|..b..
-00000c00: 5e88 5b0b d90d a8c0 3367 3c2d fce1 34ed  ^.[.....3g<-..4.
-00000c10: 7504 b2c9 5e97 43b2 7f36 b434 170f ddb6  u...^.C..6.4....
-00000c20: de8b f4ad c7c3 dcb8 5f9c 46f3 cf03 ba61  ........_.F....a
-00000c30: f4ca be43 19f1 a8fa 32f7 6548 5fd2 113a  ...C....2.eH_..:
-00000c40: 71bb 4036 3ad5 4eec 3a29 cf70 a372 6fa9  q.@6:.N.:).p.ro.
-00000c50: 5fd2 88d5 2a65 2516 ddd6 fb0e 6952 f3b1  _...*e%.....iR..
-00000c60: 25ef 882c 6085 3683 f131 2404 c291 6881  %..,`.6..1$...h.
-00000c70: ae68 3836 18ff 2547 60d5 5ede f5c8 f65d  .h86..%G`.^....]
-00000c80: a462 0621 9f91 e867 6226 693d 61a9 6482  .b.!...gb&i=a.d.
-00000c90: 6631 eb4d cc3b 1384 57f6 8c8a 8b4e b688  f1.M.;..W....N..
-00000ca0: 62bb e9e0 94c7 f3fd 4f91 6168 8ea0 2dd5  b.......O.ah..-.
-00000cb0: af44 bbab 6662 1dd8 b841 7b21 b241 ea72  .D..fb...A{!.A.r
-00000cc0: 9afe c054 7b58 7c4d 671f 9a4b 5dc7 3eda  ...T{X|Mg..K].>.
-00000cd0: f677 a721 be3f 6fea 219e b94a 6858 aa9c  .w.!.?o.!..JhX..
-00000ce0: 032c a838 5ef6 b6ed d9e2 3227 12a5 03f8  .,.8^.....2'....
-00000cf0: 688d 76ad 3267 9e92 fe3b d2d3 d14d 43a5  h.v.2g...;...MC.
-00000d00: bd26 e0d8 68bc 17f9 ff21 04a9 d7b6 7770  .&..h....!....wp
-00000d10: 58bb 4c34 3ca7 2609 6a17 387d da12 43d1  X.L4<.&.j.8}..C.
-00000d20: f09a 807d 5a20 50d6 71e7 5c67 6cf9 c5d5  ...}Z P.q.\gl...
-00000d30: cec9 654c 1ba3 d197 a132 fe20 dda9 a243  ..eL.....2. ...C
-00000d40: 6d30 3c33 e6a8 ea6d 6c16 85fe 429f 2adc  m0<3...ml...B.*.
-00000d50: 1f64 7a5d 6ddb 754a 665f fafe da03 4d0c  .dz]m.uJf_....M.
-00000d60: 5d84 580d 643f ec79 6df8 84a4 8c4f 636a  ].X.d?.ym....Ocj
-00000d70: 7703 38fb d37a d665 9159 b384 6ea9 cb6d  w.8..z.e.Y..n..m
-00000d80: 897d 54f8 fa4d 3d05 bc22 4648 99af 89ee  .}T..M=.."FH....
-00000d90: 6f54 adf8 ddd1 87dc 2a54 da6a 9450 03ee  oT......*T.j.P..
-00000da0: f73d 45eb 6fa4 a259 671a bd66 bb93 8108  .=E.o..Yg..f....
-00000db0: 0171 0f4d 3226 266e 6ff2 3dcf 38eb 6f5f  .q.M2&&no.=.8.o_
-00000dc0: 6869 0c8a 7da1 ac79 dc64 cc71 7042 a650  hi..}..y.d.qpB.P
-00000dd0: 7bbb cd65 bc85 fb9b 8626 dd68 ea23 f250  {..e.....&.h.#.P
-00000de0: 71e3 b40d cca6 a041 4014 fd87 843a 2a1f  q......A@....:*.
-00000df0: e4ef be80 7429 0546 dae1 1066 6c3e 88fe  ....t).F...fl>..
-00000e00: 2a30 1a93 55b9 05c1 7596 fa84 bbf1 9980  *0..U...u.......
-00000e10: 7aa8 b538 db31 6853 8fbd 118a 75df 5b97  z..8.1hS....u.[.
-00000e20: 7829 e935 4376 b55b f0cc 34a3 63fd 5b23  x).5Cv.[..4.c.[#
-00000e30: 7687 73ef 949d 6014 816b fb1a 88fd e9d0  v.s...`..k......
-00000e40: 77f3 5fb6 7778 0c7a a96e 36d7 4ecd 984a  w._.wx.z.n6.N..J
-00000e50: 4d75 4aaa c916 efd9 77e2 9b0c f476 f1a5  MuJ.....w....v..
-00000e60: 0f47 6d89 819a 9312 d0c7 f5fc 784c 476d  .Gm.........xLGm
-00000e70: c42c 4136 8b6d 1ba1 b910 466e 4926 291a  .,A6.m....FnI&).
-00000e80: 7903 41eb 4499 0c1a af03 1f2f db19 87c4  y.A.D....../....
-00000e90: bf6e 3f6a 7a87 06d0 7a14 6ddd 6b94 f121  .n?jz...z.m.k..!
-00000ea0: 619d 12b0 4aa3 18dc 7c3f 8495 d70c 3139  a...J...|?....19
-00000eb0: 0533 997a 83ce 63bd c0fd 4b52 7c6e 75ab  .3.z..c...KR|nu.
-00000ec0: 8a2c 040b 00d5 9bd2 24d7 2674 59f1 007b  .,......$.&tY..{
-00000ed0: 7d9b 1542 cfe9 4310 f40d b66a f976 51a2  }..B..C....j.vQ.
-00000ee0: 9cdf 2a78 7dda 0565 2d3e 0933 f9a2 86c1  ..*x}..e->.3....
-00000ef0: c875 d077 1369 ef76 7e7b 95e1 9c5a 8c33  .u.w.i.v~{...Z.3
-00000f00: 3e77 1f41 f2ae 7ec6 1376 60e3 7edf 096b  >w.A..~..v`.~..k
-00000f10: ac95 8071 a9da 9f28 8262 1127 9fd6 cb9d  ...q...(.b.'....
-00000f20: 8028 600f 1523 6a79 58bc 0c6e 4dec cc20  .(`..#jyX..nM.. 
-00000f30: 91e9 8a84 802c 28e7 e9d9 119c 315c a80d  .....,(.....1\..
-00000f40: f1ee cfd1 670e a3ef 816a a231 16ce 8311  ....g....j.1....
-00000f50: e612 6cd1 5a69 8544 95ca b4dc 8194 4274  ..l.Zi.D......Bt
-00000f60: f6bf c49e 0e0b b67a 9c81 695c bf90 e0e7  .......z..i\....
-00000f70: 8226 9d5b 29a5 7cd3 fda0 07c6 c786 d211  .&.[).|.........
-00000f80: 19a1 ed23 84c7 4cb8 2315 0fdb bbc5 3b8f  ...#..L.#.....;.
-00000f90: 8bf4 6475 3258 0fe4 84e8 7ef0 838e 2648  ..du2X....~...&H
-00000fa0: a797 c794 924b a192 234d 3f2d 85c0 14e1  .....K..#M?-....
-00000fb0: 400b 943a 1497 8dca 028a f980 e93b c00e  @..:.........;..
-00000fc0: 862a cd05 bfd2 822b 4f12 681d 9efb a224  .*.....+O.h....$
-00000fd0: 7bbb 1807 8699 1ad6 2983 9978 a859 bca1  {.......)..x.Y..
-00000fe0: d18f 1efc 31e8 57b7 86f0 2915 7af2 7140  ....1.W...).z.q@
-00000ff0: 8ecd ef17 7a79 63e9 8346 8af9 8817 8c36  ....zyc..F.....6
-00001000: ea5d a1f9 15e1 6821 9957 6606 5f5b 6d73  .]....h!.Wf._[ms
-00001010: 88dd c31d 05ad 8f61 3568 8f09 938d bc6c  .......a5h.....l
-00001020: 8737 d3fa 88e6 6128 8ad6 c373 9f2e 7ff5  .7....a(...s....
-00001030: 914e f372 27e2 a68e 8951 b1b0 f703 7a49  .N.r'....Q....zI
-00001040: 3d27 5ab0 fec5 9f7d 7ebb 0954 8dfd 3318  ='Z....}~..T..3.
-00001050: 74ae 3d3c cb5b f773 0862 39d0 e9ee 07b7  t.=<.[.s.b9.....
-00001060: 8f8a ab00 7ddc 625f 1d2c 8c53 b11c 596c  ....}.b_.,.S..Yl
-00001070: b9e7 bfbe 8fbc 1f9d ec85 d119 83cd bda2  ................
-00001080: cca0 194f 49cb bd9d 9165 546b ddee 6246  ...OI....eTk..bF
-00001090: bd4e 8ab0 fc32 cf36 2bca cb8f 9208 66c0  .N...2.6+.....f.
-000010a0: 12c2 5fbb e11d 9f16 2ad2 6b38 6402 190f  .._.....*.k8d...
-000010b0: 920d e909 d079 46eb 3c8d 8564 b8d8 1b0b  .....yF.<..d....
-000010c0: 9f79 f6d9 95af 810d a5f3 c8a0 0053 7e76  .y...........S~v
-000010d0: ac19 d601 3180 a30e 966d 853d dfd4 03ca  ....1....m.=....
-000010e0: 6d2f c1b0 2ced a83c cf9e 34be 9a22 2ba1  m/..,..<..4.."+.
-000010f0: 2f77 7cc0 cc88 712f 2db9 abf9 69fb 44aa  /w|...q/-...i.D.
-00001100: 9b32 0284 16f4 ad2c e050 e2bc a50b 3643  .2.....,.P....6C
-00001110: bf53 d939 9bd4 414f 9100 287c c7cc b134  .S.9..AO..(|...4
-00001120: a801 69fe 6be6 f013 9c37 669c fc00 9427  ..i.k....7f....'
-00001130: 5882 a966 bc95 f449 ddb1 90aa 9d47 933c  X..f...I.....G.<
-00001140: 7bda c7e1 44c7 9988 b39f cc09 0afd 02ca  {...D...........
-00001150: 9e9b 32e6 1733 4a73 337a ba1a 8aef ff4f  ..2..3Js3z.....O
-00001160: d4ba 38a6 a0b7 1932 6868 e0e7 1536 4ced  ..8....2hh...6L.
-00001170: e59f 4db3 0591 d846 a1ac 4ed2 cfed 865b  ..M....F..N....[
-00001180: c368 7980 3a3b a1ba 531c c53d a285 ae6d  .hy.:;..S..=...m
-00001190: 645e f9a5 b7e0 055c 3d58 8af7 85e2 9dda  d^.....\=X......
-000011a0: a2bb 54fe 8acf 2a8c 6d15 0c5c 0e89 b983  ..T...*.m..\....
-000011b0: f721 ee0e a3ec 8691 03d2 e3dc 18fb 5930  .!............Y0
-000011c0: 3123 9f5c abf3 be1e a42a 39aa 0aae 12ca  1#.\.....*9.....
-000011d0: 3dfb fa82 ad50 7cce 0a2c 2df1 a591 f756  =....P|..,-....V
-000011e0: 00d9 ff2a bb7a d6ec 6aa8 2b9e 3c11 26d0  ...*.z..j.+.<.&.
-000011f0: a5a5 1843 0b76 0fc3 ce3e 0834 cf90 79db  ...C.v...>.4..y.
-00001200: cfb6 da1f a6ba a636 d0f5 3143 269b 968c  .......6..1C&...
-00001210: 58c3 6819 8b91 0bf5 a7f3 a641 d9ea 72f5  X.h........A..r.
-00001220: 1911 b41c 4f99 6ad4 7230 00a2 a841 8e57  ....O.j.r0...A.W
-00001230: a4e8 a6f2 8cec 8a95 04e5 f9e7 b4a3 1bba  ................
-00001240: a852 e343 4638 f815 4709 3243 23dc d6ef  .R.CF8..G.2C#...
-00001250: e909 0a67 a86e 13e3 567f d165 1199 e0be  ...g.n..V..e....
-00001260: 5716 6bb8 a88c a5cf a93f f7af 535e 15fb  W.k......?..S^..
-00001270: 644a 3da6 ca21 d496 bc98 0e87 a94c e1a1  dJ=..!.......L..
-00001280: b2d8 d1db da64 dce5 6418 8f74 480f 2f03  .....d..d..tH./.
-00001290: a94e d9b1 8b51 adb0 4a3e 0250 d016 41f8  .N...Q..J>.P..A.
-000012a0: 03b1 6b4a aa3f af30 45dc f6d8 0fd4 24b2  ..kJ.?.0E.....$.
-000012b0: 10d0 2aee 0b24 76d4 aa6c aa64 5ee6 6d82  ..*..$v..l.d^.m.
-000012c0: 20e4 8946 6e95 585c b428 ace8 aa96 92c2   ..Fn.X\.(......
-000012d0: 4e2c d742 be01 6017 53e0 64b3 589c 4285  N,.B..`.S.d.X.B.
-000012e0: aae1 7c32 0706 3f00 2655 22ea 7fcd 1ef9  ..|2..?.&U".....
-000012f0: 71cc cc85 ab44 4fae c380 805a f86f 23bb  q....DO....Z.o#.
-00001300: 673c 8094 1d07 b847 ad00 c606 d0e3 aa41  g<.....G.......A
-00001310: 0ff0 dd50 9938 282b 21c0 2d45 afb8 bfa3  ...P.8(+!.-E....
-00001320: 153b c2d7 9b4c ca8b 8c7d ec66 d816 979f  .;...L...}.f....
-00001330: b0e6 a5a3 137b 7fe6 8f10 77fc a0f7 95f1  .....{....w.....
-00001340: d89d d24e b0ef 7617 668e 1a3d bf36 4ce6  ...N..v.f..=.6L.
-00001350: 4b25 214b 96b1 8b22 b14e 1c10 9ef6 582a  K%!K...".N....X*
-00001360: 30f9 1b6f fc27 2af2 5418 7b7e b2cb 8072  0..o.'*.T.{~...r
-00001370: 2c6d 0e61 4ca6 4214 6f34 86a1 cb84 55c6  ,m.aL.B.o4....U.
-00001380: b525 32ad cf7e 7245 a9d3 0908 0a1c 8d5f  .%2..~rE......._
-00001390: 8269 1be1 b69f 2b64 4291 26cb db65 bdfc  .i....+dB.&..e..
-000013a0: f8fb 74d2 563a 78b4 b6d2 6cfe 0653 baba  ..t.V:x...l..S..
-000013b0: 78b0 8eef b82e be57 069f 3e84 b774 aec3  x......W..>..t..
-000013c0: 980b 1fea f8ad bdec 34b8 b5e7 49d9 f489  ........4...I...
-000013d0: b79a 7def 50be eb46 660f d51f 8165 7f26  ..}.P..Ff....e.&
-000013e0: 02a4 d2a1 b812 2b62 0dc6 fd61 6c4a 7c45  ......+b...alJ|E
-000013f0: 3259 9ffb ce82 a4ff b8ec 5c4a 53ed 4d65  2Y........\JS.Me
-00001400: 40aa 9b08 ad82 2e7f 1ae3 4c03 b96d 623a  @.........L..mb:
-00001410: 82de 0268 3fc6 762b 21a9 7d57 b65f eb5d  ...h?.v+!.}W._.]
-00001420: bbf3 07ff 3ce7 2e6c f8df 49bc 07ab 19ea  ....<..l..I.....
-00001430: c8f0 bf6b bce0 4f51 51ef c1d9 5de9 5f9a  ...k..OQQ...]._.
-00001440: 82e8 e8e5 5308 eb62 bcfb 8940 46e6 e2bb  ....S..b...@F...
-00001450: 40c0 2520 721d ec5b a4ed 4f94 be9d c361  @.% r..[..O....a
-00001460: 7df9 314c d5e8 cc20 d6fb 7d71 5b86 c3a9  }.1L... ..}q[...
-00001470: bebc 19a2 8531 46d8 6974 fc1a 5496 a8ec  .....1F.it..T...
-00001480: afc0 7001 bff7 7398 1b53 4d2d 283a eeaf  ..p...s..SM-(:..
-00001490: 4f13 5954 5412 8151 c1a3 cd27 5bed 2f28  O.YTT..Q...'[./(
-000014a0: b18d a9c9 d954 6783 4f19 51a3 c21e f4f5  .....Tg.O.Q.....
-000014b0: 0443 d7ac 44c3 311b d9f4 a3a6 0d62 5feb  .C..D.1......b_.
-000014c0: c2b5 d1ac f4af 894f 5fa8 9064 c006 b13f  .......O_..d...?
-000014d0: 1c5c d512 c2c3 39d9 8466 e36a 3512 afe2  .\....9..f.j5...
-000014e0: 7281 c649 72bc 5c43 c497 2490 7117 db59  r..Ir.\C..$.q..Y
-000014f0: 238d 10d2 8d6d 1139 0b77 a68d c4ce b708  #....m.9.w......
-00001500: ba86 0a5d 0efe c766 1978 e1f4 8881 da70  ...]...f.x.....p
-00001510: c5b9 7d08 7ae2 32f4 124b 062d 8d25 f6a6  ..}.z.2..K.-.%..
-00001520: 99db 7adc c63a 6859 9674 c77f c43f ba7a  ..z..:hY.t...?.z
-00001530: c193 52d0 a6c0 c961 c723 b47d 51d7 5a6a  ..R....a.#.}Q.Zj
-00001540: d656 299e ba5e 6a86 482a 3ba6 c792 6ae6  .V)..^j.H*;...j.
-00001550: 0405 f5b2 43d9 b4ef ee3b 601c d7f2 626d  ....C....;`...bm
-00001560: c7f5 d105 2f93 504b ff55 27db 3bb2 f4a8  ..../.PK.U'.;...
-00001570: 619c d566 c8b0 cac0 8185 4d01 38b4 9d3f  a..f......M.8..?
-00001580: 0e56 3aef ea99 2dd1 c8f0 0699 181e 53ff  .V:...-.......S.
-00001590: 0551 2a20 58d0 9910 00ff 2e75 c93f 88bc  .Q* X......u.?..
-000015a0: db0e 6cd8 f7dd 75d1 869f e4ca 33c2 b743  ..l...u.....3..C
-000015b0: ca07 1809 a41a 91c5 92ab e0b5 f94e ca2b  .............N.+
-000015c0: 43a6 d57e cafc ce98 5b49 bb24 1488 dee9  C..~....[I.$....
-000015d0: f590 0a56 2524 4985 cb20 3784 ebeb d5e6  ...V%$I.. 7.....
-000015e0: 885a e698 22ca a8d8 cfaf 4ed4 cc13 0885  .Z..".....N.....
-000015f0: cd7b cc3c 033e 10b5 a01d 51ff b760 67a4  .{.<.>....Q..`g.
-00001600: cc32 fb60 a921 776f 4ffe 97f1 a718 dbbf  .2.`.!woO.......
-00001610: 8951 20b0 cd94 0740 6aab 7801 64e2 cfdb  .Q ....@j.x.d...
-00001620: 10cb 6082 e92f 4ab2 cf74 1b81 bc74 61bc  ..`../J..t...ta.
-00001630: b592 c215 2ee6 27b3 1b80 2157 cfca 8f83  ......'...!W....
-00001640: da3c f40a c8ca 0813 f8e9 1aa6 1918 155d  .<.............]
-00001650: d161 139c 9d8e a8ef 4e2d c3d5 58e3 2ae6  .a......N-..X.*.
-00001660: 9c16 e7aa d235 4ba5 ef0d 2041 7c4b d318  .....5K... A|K..
-00001670: 5238 9ddb cf11 f5bf d240 4d7c 2381 a079  R8.......@M|#..y
-00001680: 3332 8add 2a3f 55c0 5757 a598 d2b1 291e  32..*?U.WW....).
-00001690: 883c 3f9d 5692 733d 17ec ce23 70c4 0e78  .<?.V.s=...#p..x
-000016a0: d3e9 c40d c20d b746 44a1 10c2 65ba cac2  .......FD...e...
-000016b0: c832 9d36 d516 331f 2eda 8105 de33 ec76  .2.6..3......3.v
-000016c0: 43d2 7aac 0987 e1bd d564 cd08 2d74 81d5  C.z......d..-t..
-000016d0: a8b0 406a 7431 78ee 1be1 7406 d6ed da2a  ..@jt1x...t....*
-000016e0: 8d75 6ab3 1c9e bf94 4cb0 3990 4542 2a7b  .uj.....L.9.EB*{
-000016f0: d77b b103 3a9d 51fb 0861 9c8b 6386 0e57  .{..:.Q..a..c..W
-00001700: e10a 11b1 d967 f0e3 518a 5b57 926e d042  .....g..Q.[W.n.B
-00001710: 290d 1032 c14e 2e5a daff 91bd a246 920d  )..2.N.Z.....F..
-00001720: dfef c4d4 f2f2 2860 2525 d26a db80 a150  ......(`%%.j...P
-00001730: 3755 7412 42c1 8617 a5e0 6dc5 b9a9 cee5  7Ut.B.....m.....
-00001740: db9b 66f1 c32b 9c01 349e c0e7 11a0 cb71  ..f..+..4......q
-00001750: b487 cee9 dd4f 663d 5c7c b396 1e68 d656  .....Of=\|...h.V
-00001760: ea13 8f83 1b20 2429 dd75 b6da edbd 78f3  ..... $).u....x.
-00001770: 5e08 3b4d e818 3fb2 c722 bf13 de30 f0b3  ^.;M..?.."...0..
-00001780: c514 2b03 458b ae01 58bb 69a0 0bb2 d57b  ..+.E...X.i....{
-00001790: de41 62dd 1943 3851 ae15 c7f9 1a9d 74b8  .Ab..C8Q......t.
-000017a0: 9566 4057 de4a ac57 d4b7 7be4 2a82 adf9  .f@W.J.W..{.*...
-000017b0: 755d 4eb7 11ca f8c0 de91 dcae 25aa c7d3  u]N.........%...
-000017c0: 0294 3c70 45f9 80ab 35dd cb48 dee3 c25b  ..<pE...5..H...[
-000017d0: e088 ed87 1b0b bcd8 be9f 490c 5c81 0ac2  ..........I.\...
-000017e0: e04d 74a1 48a5 3b66 0bed e3bb 1d3d 2649  .Mt.H.;f.....=&I
-000017f0: a5b9 0334 e04f 9606 19cc 7622 3f68 7115  ...4.O....v"?hq.
-00001800: d0c1 9232 42a3 6898 e09e 50a6 b199 3437  ...2B.h...P...47
-00001810: a769 501c b4e2 695a 56e2 5fed e0a4 09e6  .iP...iZV._.....
-00001820: 9964 0445 6c4e 2da8 c700 492d 811d 1f9d  .d.ElN-...I-....
-00001830: e189 ae1a 43a9 9f66 2334 f82b d815 068c  ....C..f#4.+....
-00001840: d496 7b38 e1d6 8ffc 007d e403 4742 712a  ..{8.....}..GBq*
-00001850: f72a 0352 3ef3 70fe e247 eeb0 629d c5d9  .*.R>.p..G..b...
-00001860: 881e fe68 441c 79ff ea8f 885f e285 6269  ...hD.y...._..bi
-00001870: 9fe1 a2ee 1c4f 5d4b 3232 95c2 3ae2 697b  .....O]K22..:.i{
-00001880: e4c1 4033 551e 6292 dbbc 2a4b e443 c33a  ..@3U.b...*K.C.:
-00001890: 3b04 f9ae e4e2 d206 a214 b26d 103d 53e1  ;..........m.=S.
-000018a0: be4f fcf9 57e4 27db e514 181e 2647 cc99  .O..W.'.....&G..
-000018b0: d4c6 e64b dcfc 9ec3 a325 bf94 e53e f57d  ...K.....%...>.}
-000018c0: a109 9e80 4f70 08f7 cd4e 8879 817d 364e  ....Op...N.y.}6N
-000018d0: e610 b3d7 a44e b79c be09 9d27 f245 448c  .....N.....'.ED.
-000018e0: 5ecd bf09 e69d e29b b2d1 d643 4b8b 29ae  ^..........CK.).
-000018f0: 775a d8c2 e48c 5391 e6fc 34af 4a8f 603b  wZ....S...4.J.`;
-00001900: 4cf8 40ea 342d de03 c0a8 5d82 e794 4e14  L.@.4-....]...N.
-00001910: a44e 60c6 a68b 29fc 4b31 50b7 680a aeb4  .N`...).K1P.h...
-00001920: e7dc 7a7b d3ae 99e9 e704 fd03 1de9 1dcb  ..z{............
-00001930: c5cd 116f e878 21b4 2c4c b6ca 6081 e64d  ...o.x!.,L..`..M
-00001940: b74a 7786 cf68 1fee e898 8aec 01e6 5c99  .Jw..h........\.
-00001950: 9109 5098 0230 9bc2 a781 5db8 e940 4fa4  ..P..0....]..@O.
-00001960: 7750 2176 ac80 b88b e458 3a1e a305 a5bf  wP!v.....X:.....
-00001970: e968 e86b f3d2 83f4 8e4c b483 cb8a e9a7  .h.k.....L......
-00001980: 5178 9486 ea9d c1ad cbee 374b f5b9 01a5  Qx........7K....
-00001990: f11a 3c97 37b0 518e eb87 9404 f6d7 d489  ..<.7.Q.........
-000019a0: daae 129f dba9 26f6 7f8c 7708 ed08 b5df  ......&...w.....
-000019b0: b70e 776c 72b4 3c7e 5e90 509f 9566 a32e  ..wlr.<~^.P..f..
-000019c0: ed4f a920 f22b 6acc 55c9 6d41 94d1 078b  .O. .+j.U.mA....
-000019d0: ee9b 70a5 efc3 ac6e 98c7 b60a c84a 08a2  ..p....n.....J..
-000019e0: aaa2 4a74 6617 8746 f14f 5656 1893 a634  ..Jtf..F.OVV...4
-000019f0: b60e 0239 9b6f 0e02 d871 d7e3 f24f 57b3  ...9.o...q...OW.
-00001a00: eb80 39e1 c8d3 e423 0a6a 0697 92ea b5f3  ..9....#.j......
-00001a10: f390 ef81 b1a8 96ac 8b8e c388 e189 7125  ..............q%
-00001a20: a537 24be f413 32fd c472 1eea cbd7 ccd6  .7$...2..r......
-00001a30: e5ac c6c9 90dd 2d7f f633 edd3 c761 2dcc  ......-..3...a-.
-00001a40: 4ede 3aff 172a e7a0 fb6a 1705 f69a 178a  N.:..*...j......
-00001a50: fddf a735 0b5c 5778 0399 cccc ff00 650f  ...5.\Wx......e.
-00001a60: f780 9474 0a29 a0b2 e1ec a234 2d21 2905  ...t.).....4-!).
-00001a70: 402a 677e f876 9eb1 087c 7f09 03c4 2e41  @*g~.v...|.....A
-00001a80: 52d7 637a 79b6 d343 f919 8185 c34c 1115  R.czy..C.....L..
-00001a90: 7c41 1ac3 a3d1 e9a4 4454 67d1 f95a 6816  |A......DTg..Zh.
-00001aa0: 826e 3b6c c5a2 909e f8ae f549 d07a 84b0  .n;l.......I.z..
-00001ab0: f98a 9ff7 dbca 4e98 b5ba 343a 83cd 588a  ......N...4:..X.
-00001ac0: 0d29 54a5 fb33 3acb 04fc 9d25 7ad4 3dcf  .)T..3:....%z.=.
-00001ad0: f4e3 b1c2 e1ce 95df fb90 5390 dc36 462c  ..........S..6F,
-00001ae0: fb3a f0a3 035b c1a0 923d 02ba fc56 84df  .:...[...=...V..
-00001af0: f4f8 5978 212a dbca 6f0e f241 f92c 2cf0  ..Yx!*..o..A.,,.
-00001b00: fcfc 9c8a 4db8 095a 6332 0df9 cee4 7eb8  ....M..Zc2....~.
-00001b10: 282c c2e9 fd44 8b20 6f39 aad0 8adf da5e  (,...D. o9.....^
-00001b20: 1f09 e145 8bce d71f fe68 d259 df55 0d5a  ...E.....h.Y.U.Z
-00001b30: 694b 5594 fbc4 7017 98b0 ba57 3c0e 5daa  iKU...p....W<.].
-00001b40: 9426 b1d2 3df4 1a63 c4bb 041f cfba 267d  .&..=..c......&}
-00001b50: 1788 b46a b25a 2cdf 3f67 91b8 d6d7 7a9d  ...j.Z,.?g....z.
-00001b60: 5530 8271 1336 5390 b768 d554 4a23 b09c  U0.q.6S..h.TJ#..
-00001b70: 22b0 5574 d6e2 99c5 2eb1 860a 04db b713  ".Ut............
-00001b80: cf23 151c 737c 9258 33ae c6aa 0a28 ab1a  .#..s|.X3....(..
-00001b90: c0ee 48ae fd47 cc89 ec27 31e1 0f47 3bf3  ..H..G...'1..G;.
-00001ba0: 23aa 9ebb 83f8 c87d 5312 ffa3 eb9a c438  #......}S......8
-00001bb0: 402c f3ac 6756 8645 f024 d6c8 5246 fcc0  @,..gV.E.$..RF..
-00001bc0: 374f 2e09 7b52 f34d 3461 2371 65a0 e4f2  7O..{R.M4a#qe...
-00001bd0: e34d 9b21 b5c8 f238 7fa2 f6d8 569c efaf  .M.!...8....V...
-00001be0: 112e eaef c9b8 27fd c2cd ecd0 956b 1e14  ......'......k..
-00001bf0: d8a0 76c5 492d 8bf7 c782 7136 1309 ce00  ..v.I-....q6....
-00001c00: f2be e2ff 7070 5294 5aa6 36f8 613a 8038  ....ppR.Z.6.a:.8
-00001c10: fa3b fca6 0315 132f a30b 9315 3cfa 101d  .;...../....<...
-00001c20: f60a 0874 49f3 a895 29f1 e562 fc75 b350  ...tI...)..b.u.P
-00001c30: bb13 fbb9 ca09 5e5a 2c8c 2670 609d 373d  ......^Z,.&p`.7=
-00001c40: 5177 2a4e 3f98 3a9a 84ec fd1d d38c a8d1  Qw*N?.:.........
-00001c50: 04f7 4eef e97d 11ea 94e4 d657 cbc6 8a7e  ..N..}.....W...~
-00001c60: 697d 4f1d 5529 0a01 732b 49a2 01ba 81fc  i}O.U)..s+I.....
-00001c70: a651 efa8 6250 2358 ec0d d7af 8a97 a427  .Q..bP#X.......'
-00001c80: 6d4d 55a9 38d1 2009 6695 2349 efb1 5d0e  mMU.8. .f.#I..].
-00001c90: 4fc9 7768 66bd 11c6 b565 6cca ed05 99c8  O.whf....el.....
-00001ca0: f3ca 5737 5bc7 6aca c5fe e67b d1d8 d598  ..W7[.j....{....
-00001cb0: 4357 e64a d0c2 2407 fa8d 6435 4ea7 6d6b  CW.J..$...d5N.mk
-00001cc0: 273f 0ea9 6209 bda7 8ee6 37fb 507e 3d8e  '?..b.....7.P~=.
-00001cd0: 593a 8740 08dd 9b59 14ca 5bc0 730d 45cb  Y:.@...Y..[.s.E.
-00001ce0: 1c68 c80e 42aa 568c 4259 a81f 9e19 6fe7  .h..B.V.BY....o.
-00001cf0: 148c 94f0 2f48 fc5f 93de cdd4 0b3f 7b6c  ..../H._.....?{l
-00001d00: bb2d f6ca df49 556b cf2f 05a4 908e c271  .-...IUk./.....q
-00001d10: afbc c479 951f 36f3 7047 ee9b d5e4 ece0  ...y..6.pG......
-00001d20: feae f4cf fbdd ccf5 cc05 6a9e 2f8b 42f2  ..........j./.B.
-00001d30: 1f5f ca18 e09c 1041 5ee5 3f04 c485 dbfc  ._.....A^.?.....
-00001d40: 1e63 d883 be19 3a75 b619 668d 24bd 1f12  .c....:u..f.$...
-00001d50: d6d4 a821 ee75 bfd1 838b 6d35 cf74 ee9a  ...!.u....m5.t..
-00001d60: 8214 25f2 1bde f2cd 99b2 a41f 4d57 8ce9  ..%.........MW..
-00001d70: af5c 4816 fc27 d410 f8af df30 3b33 fa1b  .\H..'.....0;3..
-00001d80: 2e6e 00ce 9568 b83c 673b 3e4c 6b88 504a  .n...h.<g;>Lk.PJ
-00001d90: b020 229e 2997 8e76 231b db3d 97f5 f4be  . ".)..v#..=....
-00001da0: 9e8d e866 7300 4011 7f6d f04b 48b6 bdfe  ...fs.@..m.KH...
-00001db0: 7315 c5ee 5dfa cd90 0e9b d730 b196 7ee7  s...]......0..~.
-00001dc0: 67a0 1e7e bd39 7464 2da8 393e f245 3e14  g..~.9td-.9>.E>.
-00001dd0: dbf2 9c95 a975 ef48 35cd f071 c7fb d20f  .....u.H5..q....
-00001de0: fe73 124a 25a0 317c 63e9 ba03 3741 c5e7  .s.J%.1|c...7A..
-00001df0: f4f7 eec9 449c 8ab6 007f f2f4 f28d 8428  ....D..........(
-00001e00: 14a1 c3b5 2d5c 0128 9d75 8d06 f55c a45f  ....-\.(.u...\._
-00001e10: 2203 529d 330b c910 a597 dff1 6ab1 1a13  ".R.3.......j...
-00001e20: 20c3 be01 b363 46e9 ab9c 6877 5def 3901   ....cF...hw].9.
-00001e30: fef3 efff a9e9 c093 0fdb e8e6 0071 c4f6  .............q..
-00001e40: 3fad 593f a411 a5fb ee7f 350f 978d 830b  ?.Y?......5.....
-00001e50: bd5e 6b33 8dbd b39c 5d6a 6b8e 2442 6a12  .^k3....]jk.$Bj.
-00001e60: aa89 132b b403 1cdc 1338 e146 bb90 c89b  ...+.....8.F....
-00001e70: 0dc5 c21d b146 8bd7 8a2f 08ea 0de2 b65f  .....F.../....._
-00001e80: b211 a7fc 852e a2ea 16ed 4d3b 9034 3a6e  ..........M;.4:n
-00001e90: f736 195a eb26 8c09 6d69 11a9 0dbd 538e  .6.Z.&..mi....S.
-00001ea0: 1d3b a937 b88d e288 d453 98ec d465 f2e0  .;.7.....S...e..
-00001eb0: f1e0 3760 76a6 b227 e793 ef4e 9b97 9a79  ..7`v..'...N...y
-00001ec0: 494e d527 6c43 936d 43b2 eb5b f5ee 0530  IN.'lC.mC..[...0
-00001ed0: bbd4 b435 6596 e541 c783 2f05 d025 6a19  ...5e..A../..%j.
-00001ee0: 677b 2478 3e35 5539 c00c 3b06 6f70 ddeb  g{$x>5U9..;.op..
-00001ef0: 58aa 76c5 f04d 19c8 5302 8af2 ed5d 801d  X.v..M..S....]..
-00001f00: 7e2a 7c7e 3c4f 72c5 6a1a 79dc 7ec5 6e92  ~*|~<Or.j.y.~.n.
-00001f10: 4763 101c 0de2 586d 99d2 c97f 63ab 660f  Gc....Xm....c.f.
-00001f20: 2d38 25d1 4bab 64f6 01de f13e 5f41 c86d  -8%.K.d....>_A.m
-00001f30: 2b26 ff96 f929 573f cd5b 07fd dd22 b101  +&...)W?.[..."..
-00001f40: cbe0 beca cb26 c754 e831 85ec e57c 2e66  .....&.T.1...|.f
-00001f50: 7fee 2ec4 ca6d 7a25 70d0 897b a104 ab2d  .....mz%p..{...-
-00001f60: 23fc dffd 6db7 d623 6e76 0029 e139 aaf6  #...m..#nv.).9..
-00001f70: df9e 26be b988 54aa 17b2 db56 cb2c 19bc  ..&...T....V.,..
-00001f80: 9bbc f8e7 ff76 0474 1983 93cf a0a5 4164  .....v.t......Ad
-00001f90: 96c8 2e24 6c40 59dd 55cc 7aec f2bf 1da9  ...$l@Y.U.z.....
-00001fa0: e4c5 e7ca f192 48e6 8a50 bd94 51c3 f578  ......H..P..Q..x
-00001fb0: d27a bb29 ca2b 00a7 c218 0cee a416 fa59  .z.).+.........Y
-00001fc0: 038a 9293 4a15 7e89 2efd 63a0 0e77 75b2  ....J.~...c..wu.
-00001fd0: 44c0 d7e1 c994 c26c 913d b412 1a45 e0a4  D......l.=...E..
-00001fe0: 0000 b4c8 0000 3d92 0000 3609 0000 3cf8  ......=...6...<.
-00001ff0: 0000 46d4 0001 0472 0001 03b8 0000 b37f  ..F....r........
-00002000: 0000 d755 0000 7932 0000 97f7 0000 9989  ...U..y2........
-00002010: 0000 73da 0001 01d4 0000 27c8 0001 03e6  ..s.......'.....
-00002020: 0000 affb 0000 875b 0000 36fd 0000 e95e  .......[..6....^
-00002030: 0000 43a0 0000 ddf6 0000 9c8d 0000 9558  ..C............X
-00002040: 0000 790a 0000 ac3e 0000 0904 0000 1e3f  ..y....>.......?
-00002050: 0000 af3e 0000 93d1 0000 d899 0000 dd5b  ...>...........[
-00002060: 0000 b341 0001 0435 0000 3a7c 0000 4774  ...A...5..:|..Gt
-00002070: 0001 03cf 0000 2ea3 0000 8b39 0000 d9df  ...........9....
-00002080: 0000 095d 0000 8464 0000 068c 0000 2631  ...]...d......&1
-00002090: 0000 3645 0000 0e58 0000 e59c 0000 e6f1  ..6E...X........
-000020a0: 0000 e9cc 0000 893a 0000 2c26 0000 b818  .......:..,&....
-000020b0: 0000 9334 0000 3fdc 0000 8911 0000 b058  ...4..?........X
-000020c0: 0000 8be9 0000 47d8 0000 0a01 0000 8a45  ......G........E
-000020d0: 0000 8a97 0000 7944 0000 6e9a 0000 2bf0  ......yD..n...+.
-000020e0: 0000 b24e 0000 e199 0000 b487 0000 ba95  ...N............
-000020f0: 0000 3fb9 0000 9970 0000 078f 0001 03a0  ..?....p........
-00002100: 0000 bac6 0000 edce 0000 9a51 0000 01f8  ...........Q....
-00002110: 0000 3387 0000 bb38 0000 e481 0000 4220  ..3....8......B 
-00002120: 0000 be66 0000 e354 0000 05b7 0000 7484  ...f...T......t.
-00002130: 0000 ae30 0000 3c3e 0000 4017 0000 33fb  ...0..<>..@...3.
-00002140: 0000 93b1 0000 91ce 0000 a5d5 0000 0930  ...............0
-00002150: 0001 05fb 0000 dd2a 0000 32d8 0000 ead7  .......*..2.....
-00002160: 0000 3d0d 0000 9b50 0000 3dc7 0000 3b82  ..=....P..=...;.
-00002170: 0000 b026 0000 9a23 0000 de97 0000 91a2  ...&...#........
-00002180: 0000 be7c 0000 a489 0000 3bf3 0000 a561  ...|......;....a
-00002190: 0000 98d9 0000 ad8f 0000 995d 0000 b1af  ...........]....
-000021a0: 0000 877c 0000 368e 0000 b0cc 0000 b4b5  ...|..6.........
-000021b0: 0000 3a3c 0000 e9a1 0000 00af 0000 36e5  ..:<..........6.
-000021c0: 0000 aa35 0000 aaaf 0000 48c3 0000 c1aa  ...5......H.....
-000021d0: 0000 a167 0001 05c5 0000 e734 0000 ab53  ...g.......4...S
-000021e0: 0000 3ac2 0000 b171 0001 058f 0000 4360  ..:....q......C`
-000021f0: 0000 4aaf 0000 b199 0000 e895 0000 03dc  ..J.............
-00002200: 0000 08b3 0000 86b1 0000 0369 0000 4333  ...........i..C3
-00002210: 0001 04ec 0000 e017 0000 3b07 0000 9742  ..........;....B
-00002220: 0000 c4da 0000 77f4 0000 2bbb 0000 eaaf  ......w...+.....
-00002230: 0000 9d04 0000 2503 0000 4d35 0000 afd3  ......%...M5....
-00002240: 0000 1ee2 0000 3439 0000 ea0e 0000 34f9  ......49......4.
-00002250: 0000 79a9 0000 937e 0000 940a 0000 0ad9  ..y....~........
-00002260: 0000 4824 0000 9a65 0000 af11 0000 24d7  ..H$...e......$.
-00002270: 0000 425e 0000 ea79 0000 c808 0000 eaff  ..B^...y........
-00002280: 0000 1e2d 0000 8340 0000 4273 0000 1e71  ...-...@..Bs...q
-00002290: 0000 2fb4 0000 e7bd 0000 d5a6 0000 d688  ../.............
-000022a0: 0000 96e5 0000 9505 0000 12c1 0000 ecae  ................
-000022b0: 0000 9130 0000 e7ea 0000 7866 0000 2491  ...0......xf..$.
-000022c0: 0000 000c 0000 47b9 0000 a5b6 0000 0e14  ......G.........
-000022d0: 0000 03a6 0000 94ae 0000 d93c 0000 e6c9  ...........<....
-000022e0: 0000 11c2 0000 331e 0000 0764 0000 05f2  ......3....d....
-000022f0: 0000 2e00 0000 0ab7 0000 e0fe 0000 0a7a  ...............z
-00002300: 0000 83ad 0000 cb33 0000 b298 0000 26aa  .......3......&.
-00002310: 0000 ce62 0000 94db 0001 0516 0000 e815  ...b............
-00002320: 0000 d18f 0000 af69 0001 0552 0000 41dd  .......i...R..A.
-00002330: 0000 2667 0000 f2aa 0000 972f 0000 ad48  ..&g......./...H
-00002340: 0000 9ba7 0000 258e 0000 2703 0000 ad1c  ......%...'.....
-00002350: 0000 36a2 0000 3457 0000 d7f7 0000 428b  ..6...4W......B.
-00002360: 0000 26e7 0000 7997 0000 fca3 0000 d497  ..&...y.........
-00002370: 0000 9837 0000 ea3c 0000 8bce 0000 7892  ...7...<......x.
-00002380: 0000 0a37 0000 abee 0000 d6b5 0000 7d1e  ...7..........}.
-00002390: 0000 470a 0000 83da 0000 a5a3 0000 e8d8  ..G.............
-000023a0: 0000 2566 0000 f188 0000 95ff 0000 413a  ..%f..........A:
-000023b0: 0000 9b0a 0000 8bb8 0000 9b91 0000 96a2  ................
-000023c0: 0000 3d75 0000 e78f 0000 d4cb 0000 3db0  ..=u..........=.
-000023d0: 0000 a242 0000 9c60 0000 3cb6 0000 40ea  ...B...`..<...@.
-000023e0: 0000 b09d 0000 9bc0 0000 7466 0000 9214  ..........tf....
-000023f0: 0000 05db 0000 4115 0000 9823 0000 8f61  ......A....#...a
-00002400: 0000 e20b 0000 2e32 0000 a8f7 0000 aaa6  .......2........
-00002410: 0000 279f 0000 90ee 0000 d4f9 0000 e559  ..'............Y
-00002420: 0000 975d 0000 023b 0000 991c 0000 7cee  ...]...;......|.
-00002430: 0000 3b47 0000 88c4 0000 e91b 0000 b276  ..;G...........v
-00002440: 0000 3000 0000 8b7c 0000 741c 0000 922d  ..0....|..t....-
-00002450: 0000 e858 0000 9fc3 0000 8f23 0000 b07e  ...X.......#...~
-00002460: 0001 03ff 0000 77c4 0001 04af 0000 3237  ......w.......27
-00002470: 0000 8363 0000 40be 0000 df7c 0000 f1b0  ...c..@....|....
-00002480: 0000 6b03 3a35 c2c6 47a5 165f 748d d8be  ..k.:5..G.._t...
-00002490: 9812 ee6b 1c39 7beb 0794 189e 5852 5213  ...k.9{.....XRR.
-000024a0: 9c0e 23dc 42c1 b072 d188 571a            ..#.B..r..W.
+000004e0: 0bce f460 0921 4f3a 3a93 2baf 34c7 d381  ...`.!O::.+.4...
+000004f0: a462 054b ed28 5999 09a6 8b4b bcdd f77d  .b.K.(Y....K...}
+00000500: 7431 7fd9 e224 50d8 c445 607e 09f4 9f7d  t1...$P..E`~...}
+00000510: 68f4 2b0f 750e 2aba 9acb 1daa c79d 50c9  h.+.u.*.......P.
+00000520: 0aac 1694 4d6b 28c7 fc05 9944 50df 60a7  ....Mk(....DP.`.
+00000530: 6888 f41f 0b34 c374 78ab 675c 6ad3 9730  h....4.tx.g\j..0
+00000540: ccf9 8af1 88e7 0ff9 0b97 6447 69b2 7988  ..........dGi.y.
+00000550: d3bb 69be 2584 342c e189 8804 0c2e 2a86  ..i.%.4,......*.
+00000560: e7d7 efbf 512b cf6b 85cf 6a38 a898 0019  ....Q+.k..j8....
+00000570: 0c91 98ac ccb3 d1ad d56b 4496 e591 fa18  .........kD.....
+00000580: cbaf 64fc 0d82 432f c2d9 3143 d515 42d0  ..d...C/..1C..B.
+00000590: f4ed 03b6 3bff 69a2 0ea0 e38a 01b8 958f  ....;.i.........
+000005a0: fbcf 297a a773 effe 3623 34d0 0fee 61e9  ..)z.s..6#4...a.
+000005b0: f377 8410 9916 ff54 035f 13f5 14df 8360  .w.....T._.....`
+000005c0: 1025 1521 c1c9 9f77 238b 4860 3be0 42ba  .%.!...w#.H`;.B.
+000005d0: 5823 a198 1129 d93b 10cf ecb6 235a 9e7f  X#...).;....#Z..
+000005e0: 4ab5 3cc7 24ed 056c 1427 6e10 d8a0 d752  J.<.$..l.'n....R
+000005f0: dc35 3a7c d10a 253b c579 379a 1433 ce41  .5:|..%;.y7..3.A
+00000600: 50bb b18b f7b3 c2d6 c4b8 9b32 084c 1e7d  P..........2.L.}
+00000610: 146c addd 63f0 e9df a465 4491 1313 6c6e  .l..c....eD...ln
+00000620: 330e 20cd 149b 0c8c 5257 8dc6 3594 ea2a  3. .....RW..5..*
+00000630: 36cb 3cfd 7feb 0b17 165c 1d7d e49a 08aa  6.<......\.}....
+00000640: f59e d43a c2a9 ba68 b811 30e8 1666 45c6  ...:...h..0..fE.
+00000650: e558 e949 854d 6828 6bf7 a958 2a47 a2a0  .X.I.Mh(k..X*G..
+00000660: 16f3 c37c 7b5d 4e84 c784 5968 05df 80c6  ...|{]N...Yh....
+00000670: acbf 1568 1723 625f 6ac0 e9fb 4a39 f5b9  ...h.#b_j...J9..
+00000680: 0d1c ef73 ac7d 53bb 1853 d346 d7ad 03dd  ...s.}S..S.F....
+00000690: b20b 6093 e2c7 a1ed 8a3a 72b2 18b4 e9fc  ..`......:r.....
+000006a0: ef00 0284 d53a 8288 d7e2 7c5e 3564 58cc  .....:....|^5dX.
+000006b0: 18e0 338c ef5d 5645 7263 d691 7a88 abda  ..3..]VErc..z...
+000006c0: 7bef 876b 1940 30d2 41bd 16e3 435a be61  {..k.@0.A...CZ.a
+000006d0: ab45 f2b9 97be 439f 1a03 eb1a b938 e53b  .E....C......8.;
+000006e0: cd11 68ce cc2b f86e 20aa 761b 1cf3 c9c3  ..h..+.n .v.....
+000006f0: 075c 1fab a1eb d396 5764 e2ec af17 751b  .\......Wd....u.
+00000700: 1cf4 502a 6173 de16 a0db 5cd2 e32b 2cd8  ..P*as....\..+,.
+00000710: 0f07 83d0 1d2b bf74 d823 f98f c203 f082  .....+.t.#......
+00000720: b56e 911f fa50 492e 1d57 2e28 5e33 47fd  .n...PI..W.(^3G.
+00000730: 3694 2ec9 53dc 7146 c51e 7dc5 2044 d5a0  6...S.qF..}. D..
+00000740: 9f55 22b9 616b 252c 0891 a6e8 aa7b ca64  .U".ak%,.....{.d
+00000750: 2175 1d36 f8f1 7ce9 6aaf c278 22e2 0b6f  !u.6..|.j..x"..o
+00000760: c35e 999d 21c5 7523 5cca a33e d69d 759c  .^..!.u#\..>..u.
+00000770: cecb cbcb e5c2 16a6 2275 6466 3235 da9a  ........"udf25..
+00000780: fcbc e78c 10bf bcca 1f56 98ed 2302 d30b  .........V..#...
+00000790: 1108 da08 5d35 9b7b 0054 2e6d 1846 0766  ....]5.{.T.m.F.f
+000007a0: 2559 1dca 5a32 c357 c6e7 d67c 9d88 fdf9  %Y..Z2.W...|....
+000007b0: 9e57 2191 25f2 e150 2c69 b4cf 1669 971b  .W!.%..P,i...i..
+000007c0: 9616 8399 2ca6 6ba4 27d5 b1bf 06a5 daa9  ....,.k.'.......
+000007d0: 29cb 20bf d4a1 6010 7e6c 8063 284d 716a  ). ...`.~l.c(Mqj
+000007e0: b3c7 2c7c 1ec5 1fa5 23db e011 09f2 320a  ..,|....#.....2.
+000007f0: 297d ac16 0961 f0ae ea73 2374 aae4 2697  )}...a...s#t..&.
+00000800: 5013 3328 29d2 daac 5904 9917 2e55 4126  P.3()...Y....UA&
+00000810: d72d 43d3 0ed5 a046 2a42 2fef b908 c755  .-C....F*B/....U
+00000820: 9dd2 f716 8efc 378b 8785 ba62 2df2 9c70  ......7....b-..p
+00000830: 5bc4 7bc7 c268 e8c4 92b6 458e 3b67 b03b  [.{..h....E.;g.;
+00000840: 31ce d298 ccae 493b e277 6bdb 7184 b4e3  1.....I;.wk.q...
+00000850: 6003 36da 31d7 7150 caee 8e4d ec78 f304  `.6.1.qP...M.x..
+00000860: 09f4 fe0d eab6 11c1 32d8 331c 3e6f 336e  ........2.3.>o3n
+00000870: df84 ee6e 954e 0e72 1de3 a1a4 32e8 3d4f  ...n.N.r....2.=O
+00000880: cefa 3337 032a 8247 709f 7b53 03b1 32e9  ..37.*.Gp.{S..2.
+00000890: 3370 fbd1 c498 f950 017e df7e 2c97 7834  3p.....P.~.~,.x4
+000008a0: a9df 0ff3 34c0 bb3d 74e1 47d3 c9f2 0418  ....4..=t.G.....
+000008b0: c0f5 1abb 06a4 6efd 34fc f02c f342 4990  ......n.4..,.BI.
+000008c0: f69a a8e4 f751 2b31 0cb5 15aa 355a e6e3  .....Q+1....5Z..
+000008d0: 9381 137f 02e6 af0d a71f d969 2974 9429  ...........i)t.)
+000008e0: 35a8 559d 8e8f 8390 86cb bd78 32a5 9c0d  5.U........x2...
+000008f0: df0e 5bf6 360c ff80 3fc6 5590 e0d0 27f9  ..[.6...?.U...'.
+00000900: a255 de67 569f 098d 365d 6239 3dc4 1c08  .U.gV...6]b9=...
+00000910: e483 d3c9 17da 0ff8 5fca ae0f 3850 1419  ........_...8P..
+00000920: 135d df9b 36fa d8bd 2e4f 612b 5be2 e775  .]..6....Oa+[..u
+00000930: 3894 9563 e601 a524 7c22 e6bd 1f6e ad7d  8..c...$|"...n.}
+00000940: f98e 0a8d 3911 2369 cdb9 958c 956f e5bc  ....9.#i.....o..
+00000950: a73f 34f7 4d75 2891 3a7c 49fa 26f4 32f2  .?4.Mu(.:|I.&.2.
+00000960: 91f4 f49b 21b4 804c 0f5b 1178 3afd 2ed1  ....!..L.[.x:...
+00000970: 5f67 3613 7040 b4ef f58b 1a94 f096 7bd1  _g6.p@........{.
+00000980: 3baf b2ce f39b 0d2d 3b2d ff8a 301d 54b1  ;......-;-..0.T.
+00000990: c839 2969 3c0a b25e 76cc 5ed1 1c73 b8fe  .9)i<..^v.^..s..
+000009a0: a7aa 5496 ebad a7ce 3de3 3dde ee30 fce9  ..T.....=.=..0..
+000009b0: 17ab 3a10 b9cb 365b 625b 9fea 3def 1c80  ..:...6[b[..=...
+000009c0: d6b0 cdbc 7ded 1060 4a95 aad6 62ce bb4c  ....}..`J...b..L
+000009d0: 3e52 8de3 bf3e 0e9d eed6 d86d 0033 89b7  >R...>.....m.3..
+000009e0: cb85 84a3 3e5f 999b 65e4 d565 2911 1ad1  ....>_..e..e)...
+000009f0: 92bf c6de 425c af47 3e69 9a2f a996 ddb0  ....B\.G>i./....
+00000a00: f8b3 f6e1 4432 2091 56f0 2438 3eb7 bc56  ....D2 .V.$8>..V
+00000a10: e4df 97de 4168 f673 d2ad 0c87 934a 3c44  ....Ah.s.....J<D
+00000a20: 3f05 0000 f2c4 5598 557b 2475 49b2 73d1  ?.....U.U{$uI.s.
+00000a30: 1881 f3df 3f0c 6fb8 2eb9 cfd9 0542 a8dc  ....?.o......B..
+00000a40: 2572 f632 97e5 f65d 3ff6 be70 55a7 961c  %r.2...]?..pU...
+00000a50: d77e 3ebf c323 2730 223b 51c3 40e6 0d18  .~>..#'0";Q.@...
+00000a60: 6d78 d3e8 53df cf06 77ac 1884 8e9f 8e58  mx..S...w......X
+00000a70: 424a b1c4 93de ac0b 8f36 5f23 f732 fd74  BJ.......6_#.2.t
+00000a80: e86a bcad 42f4 1a78 02a3 e7a7 85ab a1e8  .j..B..x........
+00000a90: 0019 ab87 e7dc 47df 4471 35ed 9af9 bf37  ......G.Dq5....7
+00000aa0: 13da 009f 3875 d0bb 3a2a 9b74 4477 b3e9  ....8u..:*.tDw..
+00000ab0: 5a6c 3a22 d991 37b0 0859 53a8 7d7f fe9a  Zl:"..7..YS.}...
+00000ac0: 44a0 9b43 62d3 2602 7ef2 17a4 e5f4 a8de  D..Cb.&.~.......
+00000ad0: fd57 8799 4508 ca52 16d7 d238 30a7 d1ec  .W..E..R...80...
+00000ae0: 0df7 8aa2 6e33 cb40 456b 4288 e355 ea73  ....n3.@EkB..U.s
+00000af0: 6090 7fee 092b b823 35e8 8f80 4580 739d  `....+.#5...E.s.
+00000b00: a623 49c6 a495 ff9f c82f 8c61 61d3 7161  .#I....../.aa.qa
+00000b10: 49cd 9536 f437 89ff c916 0caa df9a 10e4  I..6.7..........
+00000b20: 3dee 51f4 4a67 524c 5be8 c65b 1ecf d877  =.Q.JgRL[..[...w
+00000b30: 63d6 8bf7 906d 38c0 4c06 bf6b 863b e410  c....m8.L..k.;..
+00000b40: bac2 8981 a2a3 8726 fc6c 0f08 4c76 5c8e  .......&.l..Lv\.
+00000b50: 185b a58b 2940 0aa0 4159 3efb b06c b0f5  .[..)@..AY>..l..
+00000b60: 4cf1 a726 2bc2 065d 939f d8ae 1261 957e  L..&+..].....a.~
+00000b70: 48fb ea8b 4d72 18da aa31 ae06 9d5d 620a  H...Mr...1...]b.
+00000b80: 13c0 bbac 435b 4cbb 4da8 26bd a9a8 9d63  ....C[L.M.&....c
+00000b90: e26d 45d1 a21c 3f63 7b19 a972 4dd6 6e60  .mE...?c{..rM.n`
+00000ba0: 7078 e4a1 3333 8a1c 03a6 d316 083d b588  px..33.......=..
+00000bb0: 4fad 480f 0c74 0a54 d524 976a cde9 3369  O.H..t.T.$.j..3i
+00000bc0: 3350 4ff7 5029 5c84 604b da90 fd95 3593  3PO.P)\.`K....5.
+00000bd0: c25f 2d00 e5d1 24f0 50aa 047f d1f7 7bac  ._-...$.P.....{.
+00000be0: ba02 28d0 d3e7 a8b3 42cb 24ec 51cc f1c0  ..(.....B.$.Q...
+00000bf0: fb98 91d5 94f4 d278 cc0a 2bef 08ed dfe8  .......x..+.....
+00000c00: 5217 9473 2a87 4182 d35a d847 eca2 dd45  R..s*.A..Z.G...E
+00000c10: d091 d351 52fc f200 124d 29bb 17cc 4133  ...QR....M)...A3
+00000c20: f196 6130 efe2 9307 5550 24f2 3d09 12c9  ..a0....UP$.=...
+00000c30: af2c 1ea3 8653 3abb 2609 efb9 5569 91ac  .,...S:.&...Ui..
+00000c40: f0e9 2153 612e 4b34 ac5f 4290 43e1 1c53  ..!Sa.K4._B.C..S
+00000c50: 58ff 10c2 6e80 dcd2 39c1 c1ef 2758 9904  X...n...9...'X..
+00000c60: 8e15 56d7 5b11 9f7b bc8c 6940 091b 70d3  ..V.[..{..i@..p.
+00000c70: 0c1e a19c 3ae4 e1dc 5b8b 005f aff9 ea30  ....:...[.._...0
+00000c80: 8819 4373 0a5f 392f 20d5 bcca 5dd1 ad3c  ..Cs._9/ ...]..<
+00000c90: aa9a 991f e496 20a4 421e 7c98 a062 9eb7  ...... .B.|..b..
+00000ca0: 5e88 5b0b d90d a8c0 3367 3c2d fce1 34ed  ^.[.....3g<-..4.
+00000cb0: 7504 b2c9 5e97 43b2 7f36 b434 170f ddb6  u...^.C..6.4....
+00000cc0: de8b f4ad c7c3 dcb8 5f9c 46f3 cf03 ba61  ........_.F....a
+00000cd0: f4ca be43 19f1 a8fa 32f7 6548 5fd2 113a  ...C....2.eH_..:
+00000ce0: 71bb 4036 3ad5 4eec 3a29 cf70 a372 6fa9  q.@6:.N.:).p.ro.
+00000cf0: 5fd2 88d5 2a65 2516 ddd6 fb0e 6952 f3b1  _...*e%.....iR..
+00000d00: 25ef 882c 6085 3683 f131 2404 c291 6881  %..,`.6..1$...h.
+00000d10: ae68 3836 18ff 2547 60d5 5ede f5c8 f65d  .h86..%G`.^....]
+00000d20: a462 0621 9f91 e867 6226 693d 61a9 6482  .b.!...gb&i=a.d.
+00000d30: 6631 eb4d cc3b 1384 57f6 8c8a 8b4e b688  f1.M.;..W....N..
+00000d40: 62bb e9e0 94c7 f3fd 4f91 6168 8ea0 2dd5  b.......O.ah..-.
+00000d50: af44 bbab 6662 1dd8 b841 7b21 b241 ea72  .D..fb...A{!.A.r
+00000d60: 9afe c054 7b58 7c4d 671f 9a4b 5dc7 3eda  ...T{X|Mg..K].>.
+00000d70: f677 a721 be3f 6fea 219e b94a 6858 aa9c  .w.!.?o.!..JhX..
+00000d80: 032c a838 5ef6 b6ed d9e2 3227 12a5 03f8  .,.8^.....2'....
+00000d90: 688d 76ad 3267 9e92 fe3b d2d3 d14d 43a5  h.v.2g...;...MC.
+00000da0: bd26 e0d8 68bc 17f9 ff21 04a9 d7b6 7770  .&..h....!....wp
+00000db0: 58bb 4c34 3ca7 2609 6a17 387d da12 43d1  X.L4<.&.j.8}..C.
+00000dc0: f09a 807d 5a20 50d6 71e7 5c67 6bbf 7ee0  ...}Z P.q.\gk.~.
+00000dd0: cffb e074 f01b c26d 3dd1 91a6 f2da 0ff1  ...t...m=.......
+00000de0: 6bca 8820 f03e ab66 6ed0 1660 b013 96be  k.. .>.fn..`....
+00000df0: 4b9d b857 6c49 3142 bb7c 984c f364 cbbd  K..WlI1B.|.L.d..
+00000e00: a883 d209 a702 16ec 6cf9 c5d5 cec9 654c  ........l.....eL
+00000e10: 1ba3 d197 a132 fe20 dda9 a243 6d30 3c33  .....2. ...Cm0<3
+00000e20: e6a8 ea6d 6c16 85fe 429f 2adc 1f64 7a5d  ...ml...B.*..dz]
+00000e30: 6ddb 754a 665f fafe da03 4d0c 5d84 580d  m.uJf_....M.].X.
+00000e40: 643f ec79 6df8 84a4 8c4f 636a 7703 38fb  d?.ym....Ocjw.8.
+00000e50: d37a d665 9159 b384 6ea9 cb6d 897d 54f8  .z.e.Y..n..m.}T.
+00000e60: fa4d 3d05 bc22 4648 99af 89ee 6f54 adf8  .M=.."FH....oT..
+00000e70: ddd1 87dc 2a54 da6a 9450 03ee f73d 45eb  ....*T.j.P...=E.
+00000e80: 6fa4 a259 671a bd66 bb93 8108 0171 0f4d  o..Yg..f.....q.M
+00000e90: 3226 266e 6ff2 3dcf 38eb 6f5f 6869 0c8a  2&&no.=.8.o_hi..
+00000ea0: 7da1 ac79 dc64 cc71 7042 a650 7bbb cd65  }..y.d.qpB.P{..e
+00000eb0: bc85 fb9b 8626 dd68 ea23 f250 71e3 b40d  .....&.h.#.Pq...
+00000ec0: cca6 a041 4014 fd87 843a 2a1f e4ef be80  ...A@....:*.....
+00000ed0: 72b8 14fc ef6b 9c61 5718 6e7c 2a1d 9e3b  r....k.aW.n|*..;
+00000ee0: 4ad9 0721 7429 0546 dae1 1066 6c3e 88fe  J..!t).F...fl>..
+00000ef0: 2a30 1a93 55b9 05c1 7596 fa84 bbf1 9980  *0..U...u.......
+00000f00: 7aa8 b538 db31 6853 8fbd 118a 75df 5b97  z..8.1hS....u.[.
+00000f10: 7829 e935 4376 b55b f0cc 34a3 63fd 5b23  x).5Cv.[..4.c.[#
+00000f20: 7687 73ef 949d 6014 816b fb1a 88fd e9d0  v.s...`..k......
+00000f30: 77f3 5fb6 7778 0c7a a96e 36d7 4ecd 984a  w._.wx.z.n6.N..J
+00000f40: 4d75 4aaa c916 efd9 77e2 9b0c f476 f1a5  MuJ.....w....v..
+00000f50: 0f47 6d89 819a 9312 d0c7 f5fc 784c 476d  .Gm.........xLGm
+00000f60: c42c 4136 8b6d 1ba1 b910 466e 4926 291a  .,A6.m....FnI&).
+00000f70: 7903 41eb 4499 0c1a af03 1f2f db19 87c4  y.A.D....../....
+00000f80: bf6e 3f6a 7a87 06d0 7a14 6ddd 6b94 f121  .n?jz...z.m.k..!
+00000f90: 619d 12b0 4aa3 18dc 7c3f 8495 d70c 3139  a...J...|?....19
+00000fa0: 0533 997a 83ce 63bd c0fd 4b52 7c6e 75ab  .3.z..c...KR|nu.
+00000fb0: 8a2c 040b 00d5 9bd2 24d7 2674 59f1 007b  .,......$.&tY..{
+00000fc0: 7d9b 1542 cfe9 4310 f40d b66a f976 51a2  }..B..C....j.vQ.
+00000fd0: 9cdf 2a78 7dda 0565 2d3e 0933 f9a2 86c1  ..*x}..e->.3....
+00000fe0: c875 d077 1369 ef76 7e7b 95e1 9c5a 8c33  .u.w.i.v~{...Z.3
+00000ff0: 3e77 1f41 f2ae 7ec6 1376 60e3 7e8d 3110  >w.A..~..v`.~.1.
+00001000: 176e 824b 1611 0be0 b499 a1f7 572d f440  .n.K........W-.@
+00001010: 7edf 096b ac95 8071 a9da 9f28 8262 1127  ~..k...q...(.b.'
+00001020: 9fd6 cb9d 8028 600f 1523 6a79 58bc 0c6e  .....(`..#jyX..n
+00001030: 4dec cc20 91e9 8a84 802c 28e7 e9d9 119c  M.. .....,(.....
+00001040: 315c a80d f1ee cfd1 670e a3ef 816a a231  1\......g....j.1
+00001050: 16ce 8311 e612 6cd1 5a69 8544 95ca b4dc  ......l.Zi.D....
+00001060: 8194 4274 f6bf c49e 0e0b b67a 9c81 695c  ..Bt.......z..i\
+00001070: bf90 e0e7 8226 9d5b 29a5 7cd3 fda0 07c6  .....&.[).|.....
+00001080: c786 d211 19a1 ed23 84c7 4cb8 2315 0fdb  .......#..L.#...
+00001090: bbc5 3b8f 8bf4 6475 3258 0fe4 84e8 7ef0  ..;...du2X....~.
+000010a0: 838e 2648 a797 c794 924b a192 234d 3f2d  ..&H.....K..#M?-
+000010b0: 85c0 14e1 400b 943a 1497 8dca 028a f980  ....@..:........
+000010c0: e93b c00e 862a cd05 bfd2 822b 4f12 681d  .;...*.....+O.h.
+000010d0: 9efb a224 7bbb 1807 8699 1ad6 2983 9978  ...${.......)..x
+000010e0: a859 bca1 d18f 1efc 31e8 57b7 86f0 2915  .Y......1.W...).
+000010f0: 7af2 7140 8ecd ef17 7a79 63e9 8346 8af9  z.q@....zyc..F..
+00001100: 8817 8c36 ea5d a1f9 15e1 6821 9957 6606  ...6.]....h!.Wf.
+00001110: 5f5b 6d73 88dd c31d 05ad 8f61 3568 8f09  _[ms.......a5h..
+00001120: 938d bc6c 8737 d3fa 88e6 6128 8ad6 c373  ...l.7....a(...s
+00001130: 9f2e 7ff5 914e f372 27e2 a68e 8951 b1b0  .....N.r'....Q..
+00001140: f703 7a49 3d27 5ab0 fec5 9f7d 7ebb 0954  ..zI='Z....}~..T
+00001150: 8dfd 3318 74ae 3d3c cb5b f773 0862 39d0  ..3.t.=<.[.s.b9.
+00001160: e9ee 07b7 8f8a ab00 7ddc 625f 1d2c 8c53  ........}.b_.,.S
+00001170: b11c 596c b9e7 bfbe 8fbc 1f9d ec85 d119  ..Yl............
+00001180: 83cd bda2 cca0 194f 49cb bd9d 9165 546b  .......OI....eTk
+00001190: ddee 6246 bd4e 8ab0 fc32 cf36 2bca cb8f  ..bF.N...2.6+...
+000011a0: 9208 66c0 12c2 5fbb e11d 9f16 2ad2 6b38  ..f..._.....*.k8
+000011b0: 6402 190f 920d e909 d079 46eb 3c8d 8564  d........yF.<..d
+000011c0: b8d8 1b0b 9f79 f6d9 95af 810d a5f3 c8a0  .....y..........
+000011d0: 0053 7e76 ac19 d601 3180 a30e 966d 853d  .S~v....1....m.=
+000011e0: dfd4 03ca 6d2f c1b0 2ced a83c cf9e 34be  ....m/..,..<..4.
+000011f0: 9845 356f 329d 5571 eb15 3f12 2e66 d126  .E5o2.Uq..?..f.&
+00001200: e197 2026 9938 2dfc f6ad 8854 710e a0b2  .. &.8-....Tq...
+00001210: 5bbe 5c6f db9f 3fbc 99aa d962 dd92 53ab  [.\o..?....b..S.
+00001220: 12ba a95b 34c0 93fe 87d1 bb5d 9a22 2ba1  ...[4......]."+.
+00001230: 2f77 7cc0 cc88 712f 2db9 abf9 69fb 44aa  /w|...q/-...i.D.
+00001240: 9b32 0284 16f4 ad2c e050 e2bc a50b 3643  .2.....,.P....6C
+00001250: bf53 d939 9bd4 414f 9100 287c c7cc b134  .S.9..AO..(|...4
+00001260: a801 69fe 6be6 f013 9c37 669c fc00 9427  ..i.k....7f....'
+00001270: 5882 a966 bc95 f449 ddb1 90aa 9d47 933c  X..f...I.....G.<
+00001280: 7bda c7e1 44c7 9988 b39f cc09 0afd 02ca  {...D...........
+00001290: 9e9b 32e6 1733 4a73 337a ba1a 8aef ff4f  ..2..3Js3z.....O
+000012a0: d4ba 38a6 a0b7 1932 6868 e0e7 1536 4ced  ..8....2hh...6L.
+000012b0: e59f 4db3 0591 d846 a1ac 4ed2 cfed 865b  ..M....F..N....[
+000012c0: c368 7980 3a3b a1ba 531c c53d a285 ae6d  .hy.:;..S..=...m
+000012d0: 645e f9a5 b7e0 055c 3d58 8af7 85e2 9dda  d^.....\=X......
+000012e0: a2bb 54fe 8acf 2a8c 6d15 0c5c 0e89 b983  ..T...*.m..\....
+000012f0: f721 ee0e a3ec 8691 03d2 e3dc 18fb 5930  .!............Y0
+00001300: 3123 9f5c abf3 be1e a42a 39aa 0aae 12ca  1#.\.....*9.....
+00001310: 3dfb fa82 ad50 7cce 0a2c 2df1 a591 f756  =....P|..,-....V
+00001320: 00d9 ff2a bb7a d6ec 6aa8 2b9e 3c11 26d0  ...*.z..j.+.<.&.
+00001330: a5a5 1843 0b76 0fc3 ce3e 0834 cf90 79db  ...C.v...>.4..y.
+00001340: cfb6 da1f a6ba a636 d0f5 3143 269b 968c  .......6..1C&...
+00001350: 58c3 6819 8b91 0bf5 a7f3 a641 d9ea 72f5  X.h........A..r.
+00001360: 1911 b41c 4f99 6ad4 7230 00a2 a841 8e57  ....O.j.r0...A.W
+00001370: a4e8 a6f2 8cec 8a95 04e5 f9e7 b4a3 1bba  ................
+00001380: a852 e343 4638 f815 4709 3243 23dc d6ef  .R.CF8..G.2C#...
+00001390: e909 0a67 a86e 13e3 567f d165 1199 e0be  ...g.n..V..e....
+000013a0: 5716 6bb8 a88c a5cf a93f f7af 535e 15fb  W.k......?..S^..
+000013b0: 644a 3da6 ca21 d496 bc98 0e87 a94c e1a1  dJ=..!.......L..
+000013c0: b2d8 d1db da64 dce5 6418 8f74 480f 2f03  .....d..d..tH./.
+000013d0: a94e d9b1 8b51 adb0 4a3e 0250 d016 41f8  .N...Q..J>.P..A.
+000013e0: 03b1 6b4a aa3f af30 45dc f6d8 0fd4 24b2  ..kJ.?.0E.....$.
+000013f0: 10d0 2aee 0b24 76d4 aa6c aa64 5ee6 6d82  ..*..$v..l.d^.m.
+00001400: 20e4 8946 6e95 585c b428 ace8 aa96 92c2   ..Fn.X\.(......
+00001410: 4e2c d742 be01 6017 53e0 64b3 589c 4285  N,.B..`.S.d.X.B.
+00001420: aae1 7c32 0706 3f00 2655 22ea 7fcd 1ef9  ..|2..?.&U".....
+00001430: 71cc cc85 ab44 4fae c380 805a f86f 23bb  q....DO....Z.o#.
+00001440: 673c 8094 1d07 b847 ad00 c606 d0e3 aa41  g<.....G.......A
+00001450: 0ff0 dd50 9938 282b 21c0 2d45 afb8 bfa3  ...P.8(+!.-E....
+00001460: 153b c2d7 9b4c ca8b 8c7d ec66 d816 979f  .;...L...}.f....
+00001470: b0e6 a5a3 137b 7fe6 8f10 77fc a0f7 95f1  .....{....w.....
+00001480: d89d d24e b0ef 7617 668e 1a3d bf36 4ce6  ...N..v.f..=.6L.
+00001490: 4b25 214b 96b1 8b22 b14e 1c10 9ef6 582a  K%!K...".N....X*
+000014a0: 30f9 1b6f fc27 2af2 5418 7b7e b2cb 8072  0..o.'*.T.{~...r
+000014b0: 2c6d 0e61 4ca6 4214 6f34 86a1 cb84 55c6  ,m.aL.B.o4....U.
+000014c0: b525 32ad cf7e 7245 a9d3 0908 0a1c 8d5f  .%2..~rE......._
+000014d0: 8269 1be1 b69f 2b64 4291 26cb db65 bdfc  .i....+dB.&..e..
+000014e0: f8fb 74d2 563a 78b4 b6d2 6cfe 0653 baba  ..t.V:x...l..S..
+000014f0: 78b0 8eef b82e be57 069f 3e84 b774 aec3  x......W..>..t..
+00001500: 980b 1fea f8ad bdec 34b8 b5e7 49d9 f489  ........4...I...
+00001510: b79a 7def 50be eb46 660f d51f 8165 7f26  ..}.P..Ff....e.&
+00001520: 02a4 d2a1 b812 2b62 0dc6 fd61 6c4a 7c45  ......+b...alJ|E
+00001530: 3259 9ffb ce82 a4ff b8ec 5c4a 53ed 4d65  2Y........\JS.Me
+00001540: 40aa 9b08 ad82 2e7f 1ae3 4c03 b96d 623a  @.........L..mb:
+00001550: 82de 0268 3fc6 762b 21a9 7d57 b65f eb5d  ...h?.v+!.}W._.]
+00001560: bbf3 07ff 3ce7 2e6c f8df 49bc 07ab 19ea  ....<..l..I.....
+00001570: c8f0 bf6b bce0 4f51 51ef c1d9 5de9 5f9a  ...k..OQQ...]._.
+00001580: 82e8 e8e5 5308 eb62 bcfb 8940 46e6 e2bb  ....S..b...@F...
+00001590: 40c0 2520 721d ec5b a4ed 4f94 be9d c361  @.% r..[..O....a
+000015a0: 7df9 314c d5e8 cc20 d6fb 7d71 5b86 c3a9  }.1L... ..}q[...
+000015b0: bebc 19a2 8531 46d8 6974 fc1a 5496 a8ec  .....1F.it..T...
+000015c0: afc0 7001 bff7 7398 1b53 4d2d 283a eeaf  ..p...s..SM-(:..
+000015d0: 4f13 5954 5412 8151 c09f 370b b592 9bed  O.YTT..Q..7.....
+000015e0: 2109 64cf 1988 f4eb 4887 40ab c1a3 cd27  !.d.....H.@....'
+000015f0: 5bed 2f28 b18d a9c9 d954 6783 4f19 51a3  [./(.....Tg.O.Q.
+00001600: c21e f4f5 0443 d7ac 44c3 311b d9f4 a3a6  .....C..D.1.....
+00001610: 0d62 5feb c2b5 d1ac f4af 894f 5fa8 9064  .b_........O_..d
+00001620: c006 b13f 1c5c d512 c2c3 39d9 8466 e36a  ...?.\....9..f.j
+00001630: 3512 afe2 7281 c649 72bc 5c43 c497 2490  5...r..Ir.\C..$.
+00001640: 7117 db59 238d 10d2 8d6d 1139 0b77 a68d  q..Y#....m.9.w..
+00001650: c4ce b708 ba86 0a5d 0efe c766 1978 e1f4  .......]...f.x..
+00001660: 8881 da70 c5b9 7d08 7ae2 32f4 124b 062d  ...p..}.z.2..K.-
+00001670: 8d25 f6a6 99db 7adc c63a 6859 9674 c77f  .%....z..:hY.t..
+00001680: c43f ba7a c193 52d0 a6c0 c961 c723 b47d  .?.z..R....a.#.}
+00001690: 51d7 5a6a d656 299e ba5e 6a86 482a 3ba6  Q.Zj.V)..^j.H*;.
+000016a0: c792 6ae6 0405 f5b2 43d9 b4ef ee3b 601c  ..j.....C....;`.
+000016b0: d7f2 626d c7f5 d105 2f93 504b ff55 27db  ..bm..../.PK.U'.
+000016c0: 3bb2 f4a8 619c d566 c88b 336c a484 b8f1  ;...a..f..3l....
+000016d0: 1529 de47 d8e1 c4a6 8a7d 4e75 c8b0 cac0  .).G.....}Nu....
+000016e0: 8185 4d01 38b4 9d3f 0e56 3aef ea99 2dd1  ..M.8..?.V:...-.
+000016f0: c8f0 0699 181e 53ff 0551 2a20 58d0 9910  ......S..Q* X...
+00001700: 00ff 2e75 c93f 88bc db0e 6cd8 f7dd 75d1  ...u.?....l...u.
+00001710: 869f e4ca 33c2 b743 ca07 1809 a41a 91c5  ....3..C........
+00001720: 92ab e0b5 f94e ca2b 43a6 d57e cafc ce98  .....N.+C..~....
+00001730: 5b49 bb24 1488 dee9 f590 0a56 2524 4985  [I.$.......V%$I.
+00001740: cb20 3784 ebeb d5e6 885a e698 22ca a8d8  . 7......Z.."...
+00001750: cfaf 4ed4 cc13 0885 cd7b cc3c 033e 10b5  ..N......{.<.>..
+00001760: a01d 51ff b760 67a4 cc32 fb60 a921 776f  ..Q..`g..2.`.!wo
+00001770: 4ffe 97f1 a718 dbbf 8951 20b0 cd94 0740  O........Q ....@
+00001780: 6aab 7801 64e2 cfdb 10cb 6082 e92f 4ab2  j.x.d.....`../J.
+00001790: ce0c 41e1 bd39 8e7b 73b0 e78c 5d95 cd6b  ..A..9.{s...]..k
+000017a0: ccca 1023 cf74 1b81 bc74 61bc b592 c215  ...#.t...ta.....
+000017b0: 2ee6 27b3 1b80 2157 cfca 8f83 da3c f40a  ..'...!W.....<..
+000017c0: c8ca 0813 f8e9 1aa6 1918 155d d161 139c  ...........].a..
+000017d0: 9d8e a8ef 4e2d c3d5 58e3 2ae6 9c16 e7aa  ....N-..X.*.....
+000017e0: d235 4ba5 ef0d 2041 7c4b d318 5238 9ddb  .5K... A|K..R8..
+000017f0: cf11 f5bf d240 4d7c 2381 a079 3332 8add  .....@M|#..y32..
+00001800: 2a3f 55c0 5757 a598 d25a fd76 0223 424a  *?U.WW...Z.v.#BJ
+00001810: ae1f 9ac0 6bc2 f7e4 4dc8 4311 d2b1 291e  ....k...M.C...).
+00001820: 883c 3f9d 5692 733d 17ec ce23 70c4 0e78  .<?.V.s=...#p..x
+00001830: d3e9 c40d c20d b746 44a1 10c2 65ba cac2  .......FD...e...
+00001840: c832 9d36 d516 331f 2eda 8105 de33 ec76  .2.6..3......3.v
+00001850: 43d2 7aac 0987 e1bd d564 cd08 2d74 81d5  C.z......d..-t..
+00001860: a8b0 406a 7431 78ee 1be1 7406 d6ed da2a  ..@jt1x...t....*
+00001870: 8d75 6ab3 1c9e bf94 4cb0 3990 4542 2a7b  .uj.....L.9.EB*{
+00001880: d77b b103 3a9d 51fb 0861 9c8b 6386 0e57  .{..:.Q..a..c..W
+00001890: e10a 11b1 d967 f0e3 518a 5b57 926e d042  .....g..Q.[W.n.B
+000018a0: 290d 1032 c14e 2e5a daff 91bd a246 920d  )..2.N.Z.....F..
+000018b0: dfef c4d4 f2f2 2860 2525 d26a db80 a150  ......(`%%.j...P
+000018c0: 3755 7412 42c1 8617 a5e0 6dc5 b9a9 cee5  7Ut.B.....m.....
+000018d0: db9b 66f1 c32b 9c01 349e c0e7 11a0 cb71  ..f..+..4......q
+000018e0: b487 cee9 dd4f 663d 5c7c b396 1e68 d656  .....Of=\|...h.V
+000018f0: ea13 8f83 1b20 2429 dd75 b6da edbd 78f3  ..... $).u....x.
+00001900: 5e08 3b4d e818 3fb2 c722 bf13 de30 f0b3  ^.;M..?.."...0..
+00001910: c514 2b03 458b ae01 58bb 69a0 0bb2 d57b  ..+.E...X.i....{
+00001920: de41 62dd 1943 3851 ae15 c7f9 1a9d 74b8  .Ab..C8Q......t.
+00001930: 9566 4057 de4a ac57 d4b7 7be4 2a82 adf9  .f@W.J.W..{.*...
+00001940: 755d 4eb7 11ca f8c0 de91 dcae 25aa c7d3  u]N.........%...
+00001950: 0294 3c70 45f9 80ab 35dd cb48 deb3 7580  ..<pE...5..H..u.
+00001960: 1490 21e9 533a f10f 9fa5 0e29 a3ce dc64  ..!.S:.....)...d
+00001970: dee3 c25b e088 ed87 1b0b bcd8 be9f 490c  ...[..........I.
+00001980: 5c81 0ac2 e04d 74a1 48a5 3b66 0bed e3bb  \....Mt.H.;f....
+00001990: 1d3d 2649 a5b9 0334 e04f 9606 19cc 7622  .=&I...4.O....v"
+000019a0: 3f68 7115 d0c1 9232 42a3 6898 e09e 50a6  ?hq....2B.h...P.
+000019b0: b199 3437 a769 501c b4e2 695a 56e2 5fed  ..47.iP...iZV._.
+000019c0: e0a4 09e6 9964 0445 6c4e 2da8 c700 492d  .....d.ElN-...I-
+000019d0: 811d 1f9d e189 ae1a 43a9 9f66 2334 f82b  ........C..f#4.+
+000019e0: d815 068c d496 7b38 e1d6 8ffc 007d e403  ......{8.....}..
+000019f0: 4742 712a f72a 0352 3ef3 70fe e247 eeb0  GBq*.*.R>.p..G..
+00001a00: 629d c5d9 881e fe68 441c 79ff ea8f 885f  b......hD.y...._
+00001a10: e285 6269 9fe1 a2ee 1c4f 5d4b 3232 95c2  ..bi.....O]K22..
+00001a20: 3ae2 697b e4c1 4033 551e 6292 dbbc 2a4b  :.i{..@3U.b...*K
+00001a30: e443 c33a 3b04 f9ae e4e2 d206 a214 b26d  .C.:;..........m
+00001a40: 103d 53e1 be4f fcf9 57e4 27db e514 181e  .=S..O..W.'.....
+00001a50: 2647 cc99 d4c6 e64b dcfc 9ec3 a325 bf94  &G.....K.....%..
+00001a60: e53e f57d a109 9e80 4f70 08f7 cd4e 8879  .>.}....Op...N.y
+00001a70: 817d 364e e576 b2f6 0d88 e3ea 327d d3e2  .}6N.v......2}..
+00001a80: 8e65 af15 2218 d091 e610 b3d7 a44e b79c  .e.."........N..
+00001a90: be09 9d27 f245 448c 5ecd bf09 e69d e29b  ...'.ED.^.......
+00001aa0: b2d1 d643 4b8b 29ae 775a d8c2 e48c 5391  ...CK.).wZ....S.
+00001ab0: e6fc 34af 4a8f 603b 4cf8 40ea 342d de03  ..4.J.`;L.@.4-..
+00001ac0: c0a8 5d82 e794 4e14 a44e 60c6 a68b 29fc  ..]...N..N`...).
+00001ad0: 4b31 50b7 680a aeb4 e7dc 7a7b d3ae 99e9  K1P.h.....z{....
+00001ae0: e704 fd03 1de9 1dcb c5cd 116f e878 21b4  ...........o.x!.
+00001af0: 2c4c b6ca 6081 e64d b74a 7786 cf68 1fee  ,L..`..M.Jw..h..
+00001b00: e898 8aec 01e6 5c99 9109 5098 0230 9bc2  ......\...P..0..
+00001b10: a781 5db8 e940 4fa4 7750 2176 ac80 b88b  ..]..@O.wP!v....
+00001b20: e458 3a1e a305 a5bf e968 e86b f3d2 83f4  .X:......h.k....
+00001b30: 8e4c b483 cb8a e9a7 5178 9486 ea9d c1ad  .L......Qx......
+00001b40: cbee 374b f5b9 01a5 f11a 3c97 37b0 518e  ..7K......<.7.Q.
+00001b50: eb87 9404 f6d7 d489 daae 129f dba9 26f6  ..............&.
+00001b60: 7f8c 7708 ed08 b5df b70e 776c 72b4 3c7e  ..w.......wlr.<~
+00001b70: 5e90 509f 9566 a32e ed4f a920 f22b 6acc  ^.P..f...O. .+j.
+00001b80: 55c9 6d41 94d1 078b ee9b 70a5 efc3 ac6e  U.mA......p....n
+00001b90: 98c7 b60a c84a 08a2 aaa2 4a74 6617 8746  .....J....Jtf..F
+00001ba0: f14f 5656 1893 a634 b60e 0239 9b6f 0e02  .OVV...4...9.o..
+00001bb0: d871 d7e3 f24f 57b3 eb80 39e1 c8d3 e423  .q...OW...9....#
+00001bc0: 0a6a 0697 92ea b5f3 f390 ef81 b1a8 96ac  .j..............
+00001bd0: 8b8e c388 e189 7125 a537 24be f413 32fd  ......q%.7$...2.
+00001be0: c472 1eea cbd7 ccd6 e5ac c6c9 90dd 2d7f  .r............-.
+00001bf0: f633 edd3 c761 2dcc 4ede 3aff 172a e7a0  .3...a-.N.:..*..
+00001c00: fb6a 1705 f69a 178a fddf a735 0b5c 5778  .j.........5.\Wx
+00001c10: 0399 cccc ff00 650f f780 9474 0a29 a0b2  ......e....t.)..
+00001c20: e1ec a234 2d21 2905 402a 677e f876 9eb1  ...4-!).@*g~.v..
+00001c30: 087c 7f09 03c4 2e41 52d7 637a 79b6 d343  .|.....AR.czy..C
+00001c40: f919 8185 c34c 1115 7c41 1ac3 a3d1 e9a4  .....L..|A......
+00001c50: 4454 67d1 f95a 6816 826e 3b6c c5a2 909e  DTg..Zh..n;l....
+00001c60: f8ae f549 d07a 84b0 f98a 9ff7 dbca 4e98  ...I.z........N.
+00001c70: b5ba 343a 83cd 588a 0d29 54a5 fb33 3acb  ..4:..X..)T..3:.
+00001c80: 04fc 9d25 7ad4 3dcf f4e3 b1c2 e1ce 95df  ...%z.=.........
+00001c90: fb90 5390 dc36 462c fb3a f0a3 035b c1a0  ..S..6F,.:...[..
+00001ca0: 923d 02ba fc56 84df f4f8 5978 212a dbca  .=...V....Yx!*..
+00001cb0: 6f0e f241 f92c 2cf0 fcfc 9c8a 4db8 095a  o..A.,,.....M..Z
+00001cc0: 6332 0df9 cee4 7eb8 282c c2e9 fd44 8b20  c2....~.(,...D. 
+00001cd0: 6f39 aad0 8adf da5e 1f09 e145 8bce d71f  o9.....^...E....
+00001ce0: fe68 d259 df55 0d5a 694b 5594 fbc4 7017  .h.Y.U.ZiKU...p.
+00001cf0: 98b0 ba57 3c0e 5daa 9426 b1d2 3df4 1a63  ...W<.]..&..=..c
+00001d00: c4bb 041f cfba 267d 52bb cb23 b25a 2cdf  ......&}R..#.Z,.
+00001d10: 3f67 91b8 d6d7 7a9d 5530 8271 1336 5390  ?g....z.U0.q.6S.
+00001d20: 0ae1 1cc5 b768 d554 4a23 b09c 22b0 5574  .....h.TJ#..".Ut
+00001d30: d6e2 99c5 2eb1 860a 04db b713 cf23 151c  .............#..
+00001d40: 737c 9258 f165 b01c 0a28 ab1a c0ee 48ae  s|.X.e...(....H.
+00001d50: fd47 cc89 ec27 31e1 0f47 3bf3 23aa 9ebb  .G...'1..G;.#...
+00001d60: 83f8 c87d 5312 ffa3 eb9a c438 402c f3ac  ...}S......8@,..
+00001d70: 6756 8645 f024 d6c8 5246 fcc0 17c6 4361  gV.E.$..RF....Ca
+00001d80: b355 3c2a ea73 4d0b 7b52 f34d 3461 2371  .U<*.sM.{R.M4a#q
+00001d90: 65a0 e4f2 22d7 e024 e34d 9b21 b5c8 f238  e..."..$.M.!...8
+00001da0: 7fa2 f6d8 569c efaf 112e eaef c9b8 27fd  ....V.........'.
+00001db0: c2cd ecd0 956b 1e14 d8a0 76c5 492d 8bf7  .....k....v.I-..
+00001dc0: 3077 4c23 1309 ce00 f2be e2ff 7070 5294  0wL#........ppR.
+00001dd0: 5aa6 36f8 613a 8038 fa3b fca6 0315 132f  Z.6.a:.8.;...../
+00001de0: a30b 9315 3cfa 101d f60a 0874 49f3 a895  ....<......tI...
+00001df0: 29f1 e562 fc75 b350 bb13 fbb9 ca09 5e5a  )..b.u.P......^Z
+00001e00: 2c8c 2670 609d 373d 5177 2a4e 3f98 3a9a  ,.&p`.7=Qw*N?.:.
+00001e10: 84ec fd1d d38c a8d1 04f7 4eef e97d 11ea  ..........N..}..
+00001e20: 94e4 d657 cbc6 8a7e 697d 4f1d 5529 0a01  ...W...~i}O.U)..
+00001e30: 732b 49a2 01ba 81fc a651 efa8 6250 2358  s+I......Q..bP#X
+00001e40: cc6b 23b5 ec0d d7af 8a97 a427 a2b5 8c70  .k#........'...p
+00001e50: 38d1 2009 6695 2349 efb1 5d0e 4fc9 7768  8. .f.#I..].O.wh
+00001e60: d7a5 3de0 66bd 11c6 b565 6cca ed05 99c8  ..=.f....el.....
+00001e70: f3ca 5737 5bc7 6aca c5fe e67b d1d8 d598  ..W7[.j....{....
+00001e80: 4357 e64a d0c2 2407 1f35 4251 e6ea 7b48  CW.J..$..5BQ..{H
+00001e90: a8b8 befe 4ea7 6d6b 273f 0ea9 6209 bda7  ....N.mk'?..b...
+00001ea0: 8ee6 37fb 507e 3d8e 593a 8740 08dd 9b59  ..7.P~=.Y:.@...Y
+00001eb0: 14ca 5bc0 730d 45cb 1c68 c80e 42aa 568c  ..[.s.E..h..B.V.
+00001ec0: 4259 a81f 9e19 6fe7 148c 94f0 2f48 fc5f  BY....o...../H._
+00001ed0: 93de cdd4 0b3f 7b6c bb2d f6ca df49 556b  .....?{l.-...IUk
+00001ee0: cf2f 05a4 908e c271 a0e8 3cd7 7a34 b462  ./.....q..<.z4.b
+00001ef0: 10b2 9a28 afbc c479 951f 36f3 7047 ee9b  ...(...y..6.pG..
+00001f00: d5e4 ece0 feae f4cf fbdd ccf5 cc05 6a9e  ..............j.
+00001f10: 2f8b 42f2 1f5f ca18 e09c 1041 f16b 420e  /.B.._.....A.kB.
+00001f20: 5ee5 3f04 c485 dbfc 1e63 d883 be19 3a75  ^.?......c....:u
+00001f30: b619 668d 24bd 1f12 d6d4 a821 f3bd f10d  ..f.$......!....
+00001f40: 838b 6d35 cf74 ee9a 8214 25f2 1bde f2cd  ..m5.t....%.....
+00001f50: 99b2 a41f 4d57 8ce9 43cf fcb7 af5c 4816  ....MW..C....\H.
+00001f60: fc27 d410 f8af df30 3b33 fa1b 2e6e 00ce  .'.....0;3...n..
+00001f70: 9568 b83c cc3d dba7 6b88 504a b020 229e  .h.<.=..k.PJ. ".
+00001f80: 2997 8e76 231b db3d 97f5 f4be 9e8d e866  )..v#..=.......f
+00001f90: 1cf3 b13e 7f6d f04b 48b6 bdfe 7315 c5ee  ...>.m.KH...s...
+00001fa0: 5dfa cd90 0e9b d730 b196 7ee7 67a0 1e7e  ]......0..~.g..~
+00001fb0: bd39 7464 2da8 393e f245 3e14 b09d d6e2  .9td-.9>.E>.....
+00001fc0: 107b 66ee 3645 b564 dbf2 9c95 a975 ef48  .{f.6E.d.....u.H
+00001fd0: 35cd f071 c7fb d20f fe73 124a 25a0 317c  5..q.....s.J%.1|
+00001fe0: 63e9 ba03 3741 c5e7 f4f7 eec9 449c 8ab6  c...7A......D...
+00001ff0: 007f f2f4 f28d 8428 14a1 c3b5 2d5c 0128  .......(....-\.(
+00002000: 9d75 8d06 f55c a45f 2203 529d 330b c910  .u...\._".R.3...
+00002010: a597 dff1 6ab1 1a13 20c3 be01 b363 46e9  ....j... ....cF.
+00002020: ab9c 6877 5def 3901 fef3 efff a9e9 c093  ..hw].9.........
+00002030: 0fdb e8e6 0071 c4f6 3fad 593f a411 a5fb  .....q..?.Y?....
+00002040: ee7f 350f 978d 830b bd5e 6b33 8dbd b39c  ..5......^k3....
+00002050: 5d6a 6b8e 2442 6a12 aa89 132b b403 1cdc  ]jk.$Bj....+....
+00002060: 1338 e146 bb90 c89b 0dc5 c21d b146 8bd7  .8.F.........F..
+00002070: 4b93 c480 0de2 b65f b211 a7fc 8ce0 474e  K......_......GN
+00002080: 16ed 4d3b 4bca dd8c 9034 3a6e f736 195a  ..M;K....4:n.6.Z
+00002090: eb26 8c09 6d69 11a9 0dbd 538e 1d3b a937  .&..mi....S..;.7
+000020a0: b88d e288 d453 98ec d465 f2e0 f1e0 3760  .....S...e....7`
+000020b0: 76a6 b227 71d8 d2df e793 ef4e 9b97 9a79  v..'q......N...y
+000020c0: 494e d527 6c43 936d 43b2 eb5b f5ee 0530  IN.'lC.mC..[...0
+000020d0: 23f8 9e49 6596 e541 c783 2f05 cd36 8e9e  #..Ie..A../..6..
+000020e0: d025 6a19 677b 2478 3e35 5539 c00c 3b06  .%j.g{$x>5U9..;.
+000020f0: 6f70 ddeb 9ab7 4fdb 58aa 76c5 f04d 19c8  op....O.X.v..M..
+00002100: 69d9 ecd9 ed5d 801d 7e2a 7c7e 3c4f 72c5  i....]..~*|~<Or.
+00002110: 6a1a 79dc 7ec5 6e92 4763 101c 0de2 586d  j.y.~.n.Gc....Xm
+00002120: 99d2 c97f 63ab 660f 2d38 25d1 4bab 64f6  ....c.f.-8%.K.d.
+00002130: 01de f13e 5f41 c86d 03cd f091 2b26 ff96  ...>_A.m....+&..
+00002140: f929 573f cd5b 07fd dd22 b101 cbe0 beca  .)W?.[..."......
+00002150: cb26 c754 e831 85ec e57c 2e66 7fee 2ec4  .&.T.1...|.f....
+00002160: ca6d 7a25 70d0 897b 9982 2485 23fc dffd  .mz%p..{..$.#...
+00002170: 3d9b 0a7a 6db7 d623 6e76 0029 e139 aaf6  =..zm..#nv.).9..
+00002180: df9e 26be b988 54aa 369a 18b9 cb2c 19bc  ..&...T.6....,..
+00002190: 9bbc f8e7 ff76 0474 1983 93cf a0a5 4164  .....v.t......Ad
+000021a0: 96c8 2e24 e3ef 1de5 55cc 7aec f2bf 1da9  ...$....U.z.....
+000021b0: e4c5 e7ca f192 48e6 8a50 bd94 51c3 f578  ......H..P..Q..x
+000021c0: d27a bb29 ca2b 00a7 c218 0cee a416 fa59  .z.).+.........Y
+000021d0: 038a 9293 d655 840b 2efd 63a0 0e77 75b2  .....U....c..wu.
+000021e0: 44c0 d7e1 c994 c26c 913d b412 1a45 e0a4  D......l.=...E..
+000021f0: 0000 b4c8 0000 3d92 0000 3609 0000 3cf8  ......=...6...<.
+00002200: 0000 46d4 0001 1b26 0001 1a1f 0000 b37f  ..F....&........
+00002210: 0000 d7f7 0000 7932 0000 97f7 0000 f27c  ......y2.......|
+00002220: 0000 9989 0000 73da 0001 183b 0000 27c8  ......s....;..'.
+00002230: 0001 1a4d 0000 affb 0000 875b 0000 36fd  ...M.......[..6.
+00002240: 0000 f982 0000 43a0 0000 ebf2 0000 9c8d  ......C.........
+00002250: 0000 9558 0000 790a 0000 ac3e 0000 0904  ...X..y....>....
+00002260: 0000 1e3f 0000 af3e 0000 93d1 0000 d93b  ...?...>.......;
+00002270: 0000 eb57 0000 b341 0001 1a66 0000 ff4f  ...W...A...f...O
+00002280: 0001 1ae9 0000 3a7c 0000 4774 0001 1a36  ......:|..Gt...6
+00002290: 0000 fefc 0000 2ea3 0000 8b39 0000 e7db  ...........9....
+000022a0: 0000 095d 0000 8464 0000 068c 0000 2631  ...]...d......&1
+000022b0: 0000 3645 0000 0e58 0000 f57d 0000 f6d2  ..6E...X...}....
+000022c0: 0000 f9f0 0000 893a 0000 2c26 0000 b818  .......:..,&....
+000022d0: 0000 9334 0000 3fdc 0000 8911 0000 b058  ...4..?........X
+000022e0: 0000 8be9 0000 47d8 0000 0a01 0000 8a45  ......G........E
+000022f0: 0000 8a97 0000 7944 0000 6e9a 0000 2bf0  ......yD..n...+.
+00002300: 0000 b24e 0000 f2d5 0000 b487 0000 ba95  ...N............
+00002310: 0000 3fb9 0000 9970 0000 078f 0001 1a07  ..?....p........
+00002320: 0000 bac6 0001 02a4 0000 9a51 0000 01f8  ...........Q....
+00002330: 0000 3387 0000 bb38 0000 f462 0000 f347  ..3....8...b...G
+00002340: 0000 4220 0000 be66 0000 f425 0000 05b7  ..B ...f...%....
+00002350: 0000 7484 0000 ae30 0000 3c3e 0000 f39f  ..t....0..<>....
+00002360: 0000 4017 0000 33fb 0000 93b1 0000 91ce  ..@...3.........
+00002370: 0000 a5d5 0000 0930 0001 1caf 0000 eb26  .......0.......&
+00002380: 0000 32d8 0000 db1d 0000 ffad 0000 ff12  ..2.............
+00002390: 0000 3d0d 0000 9b50 0000 3dc7 0000 3b82  ..=....P..=...;.
+000023a0: 0000 b026 0000 9a23 0000 ec93 0000 91a2  ...&...#........
+000023b0: 0000 be7c 0000 a489 0000 3bf3 0000 a561  ...|......;....a
+000023c0: 0000 98d9 0000 ad8f 0000 995d 0000 b1af  ...........]....
+000023d0: 0000 877c 0000 368e 0000 b0cc 0000 b4b5  ...|..6.........
+000023e0: 0000 3a3c 0000 da81 0000 f374 0000 f006  ..:<.......t....
+000023f0: 0000 f9c5 0000 00af 0000 36e5 0000 aa35  ..........6....5
+00002400: 0000 aaaf 0000 48c3 0000 c1aa 0000 a167  ......H........g
+00002410: 0001 1c79 0000 f715 0000 feb0 0000 ab53  ...y...........S
+00002420: 0000 3ac2 0000 b171 0001 1c43 0000 4360  ..:....q...C..C`
+00002430: 0000 4aaf 0000 b199 0000 f876 0000 03dc  ..J........v....
+00002440: 0000 08b3 0000 86b1 0000 0369 0000 4333  ...........i..C3
+00002450: 0001 1ba0 0000 de4b 0000 ee13 0000 3b07  .......K......;.
+00002460: 0000 9742 0000 c4da 0000 77f4 0000 2bbb  ...B......w...+.
+00002470: 0000 ff85 0000 9d04 0000 2503 0000 4d35  ..........%...M5
+00002480: 0000 afd3 0000 1ee2 0000 3439 0000 fa32  ..........49...2
+00002490: 0000 34f9 0000 79a9 0000 937e 0000 940a  ..4...y....~....
+000024a0: 0000 0ad9 0000 4824 0000 9a65 0000 af11  ......H$...e....
+000024b0: 0000 24d7 0000 425e 0001 16aa 0000 ef95  ..$...B^........
+000024c0: 0000 fa60 0001 1a7d 0000 c808 0000 ffd5  ...`...}........
+000024d0: 0000 1e2d 0000 8340 0000 4273 0000 1e71  ...-...@..Bs...q
+000024e0: 0000 2fb4 0000 f79e 0000 d5a6 0000 d688  ../.............
+000024f0: 0000 96e5 0000 9505 0000 12c1 0001 0184  ................
+00002500: 0000 9130 0000 f7cb 0000 7866 0000 2491  ...0......xf..$.
+00002510: 0000 000c 0000 47b9 0000 a5b6 0000 0e14  ......G.........
+00002520: 0000 03a6 0000 94ae 0000 d9de 0000 f6aa  ................
+00002530: 0000 11c2 0000 331e 0000 0764 0000 05f2  ......3....d....
+00002540: 0000 2e00 0000 0ab7 0000 eefa 0000 0a7a  ...............z
+00002550: 0000 83ad 0000 cb33 0000 b298 0000 26aa  .......3......&.
+00002560: 0000 ce62 0000 94db 0001 1bca 0000 f7f6  ...b............
+00002570: 0000 d18f 0000 af69 0001 1c06 0000 41dd  .......i......A.
+00002580: 0000 f14f 0000 2667 0001 0780 0000 972f  ...O..&g......./
+00002590: 0000 ad48 0000 9ba7 0000 258e 0000 2703  ...H......%...'.
+000025a0: 0000 ad1c 0000 36a2 0000 3457 0000 d899  ......6...4W....
+000025b0: 0000 f8b9 0000 428b 0000 26e7 0000 7997  ......B...&...y.
+000025c0: 0001 1179 0000 d497 0000 9837 0000 f2a8  ...y.......7....
+000025d0: 0000 8bce 0000 7892 0000 d6b5 0000 0a37  ......x........7
+000025e0: 0000 abee 0000 d757 0000 7d1e 0000 470a  .......W..}...G.
+000025f0: 0000 e17c 0000 83da 0000 a5a3 0000 f8fc  ...|............
+00002600: 0000 2566 0001 065e 0000 95ff 0000 413a  ..%f...^......A:
+00002610: 0000 9b0a 0000 8bb8 0000 9b91 0000 96a2  ................
+00002620: 0000 3d75 0000 f770 0000 d4cb 0000 3db0  ..=u...p......=.
+00002630: 0000 a242 0000 fe99 0000 9c60 0000 3cb6  ...B.......`..<.
+00002640: 0000 40ea 0000 b09d 0000 9bc0 0000 7466  ..@...........tf
+00002650: 0000 9214 0000 05db 0000 4115 0000 9823  ..........A....#
+00002660: 0000 8f61 0000 f3ca 0000 2e32 0000 e4aa  ...a.......2....
+00002670: 0000 a8f7 0000 aaa6 0000 279f 0000 90ee  ..........'.....
+00002680: 0000 d4f9 0000 f53a 0000 975d 0000 023b  .......:...]...;
+00002690: 0000 991c 0000 7cee 0000 3b47 0000 88c4  ......|...;G....
+000026a0: 0000 f93f 0000 b276 0000 3000 0000 8b7c  ...?...v..0....|
+000026b0: 0000 741c 0000 922d 0000 f839 0000 9fc3  ..t....-...9....
+000026c0: 0000 8f23 0000 b07e 0001 1ab3 0000 77c4  ...#...~......w.
+000026d0: 0001 1b63 0000 3237 0000 8363 0000 40be  ...c..27...c..@.
+000026e0: 0000 ed78 0001 0686 0000 6b03 3571 ec17  ...x......k.5q..
+000026f0: 3ed5 ebca d60b 56dc 6699 a51d 6a18 710c  >.....V.f...j.q.
+00002700: 666c 27c3 54b5 bf6f 0cb5 721f d26f 5f9a  fl'.T..o..r..o_.
+00002710: 6f55 bc17                                oU..
```

### Comparing `gpt_computer_assistant-0.6.0/.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.pack` & `gpt_computer_assistant-0.6.1/.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.pack`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 5041 434b 0000 0002 0000 0129 910e 789c  PACK.......)..x.
+00000000: 5041 434b 0000 0002 0000 013f 910e 789c  PACK.......?..x.
 00000010: 8dcb 310e c230 0c40 d13d a7f0 8e84 1237  ..1..0.@.=.....7
 00000020: 711a 0921 0103 5c23 4e1c daa1 2d2a 2e5c  q..!..\#N...-*.\
 00000030: 9f1e 813f ffa7 ab08 74cd 166a dca3 702a  ...?....t..j..p*
 00000040: ad26 1b3c e6be 160c 111b 7598 a284 46a1  .&.<......u...F.
 00000050: 9a57 5e65 5660 2b2d 928b 44bd b8dc 556e  .W^eV`+-..D...Un
 00000060: 1df9 22e4 1903 3acf 89d8 f58c 68f2 a6c3  .."...:.....h...
 00000070: b2c2 7dd4 c7c6 7029 3a2e f31b ae8b c2e9  ..}...p):.......
@@ -3429,769 +3429,1132 @@
 0000d640: 4b33 8b52 7353 f34a 8af5 4a2a 4a18 6af2  K3.RsS.J..J*J.j.
 0000d650: 4a57 77e9 b070 335c 9d7d 49e5 ba5a 49e4  JWw..p3\.}I..ZI.
 0000d660: 4786 6aa8 dae2 d492 d202 bd82 4a86 4387  G.j.........J.C.
 0000d670: 2d6f b6a4 3dce 3215 5aff a8a8 f198 67d1  -o..=.2.Z.....g.
 0000d680: 9e18 6700 101c 5e1c ee01 8062 789c 011e  ..g...^....bx...
 0000d690: 00e1 ffe6 01e6 0190 5a14 a591 f756 00d9  ........Z....V..
 0000d6a0: ff2a bb7a d6ec 6aa8 2b9e 3c11 26d0 916e  .*.z..j.+.<.&..n
-0000d6b0: 78e9 000e de91 0e78 9c8d 8b39 0ec2 3010  x......x...9..0.
-0000d6c0: 007b bf62 7ba4 c807 b663 0921 0105 7c63  .{.b{....c.!..|c
-0000d6d0: bd5e 488a c4c8 d984 ef13 7ec0 4c3b 238d  .^H.......~.L;#.
-0000d6e0: 198a 37c1 39f3 b45c b037 da17 768e 2986  ..7.9..\.7..v.).
-0000d6f0: a32b 3622 924e 7d64 938b 7a63 e359 c01a  .+6".N}d..zc.Y..
-0000d700: f2d1 5be7 8910 f7b4 8454 a24f 444c f927  ..[......T.ODL.'
-0000d710: 7bb2 2660 50b8 ca50 1bdc 4779 ac19 2e24  {.&`P..P..Gy...$
-0000d720: 639d 17b8 5681 d319 4c34 21f5 3ad9 0407  c...V...L4!.:...
-0000d730: bda3 a84e d328 c27f 0fea 36e0 fce2 021b  ...N.(....6.....
-0000d740: b765 2f61 5ea7 bcef 9f51 06d8 7417 3aad  .e/a^....Q..t.:.
-0000d750: be74 8242 ce91 0e78 9c8d cb4d 0e82 3010  .t.B...x...M..0.
-0000d760: 40e1 7d4f 317b 13d2 ffd2 c498 a80b bdc6  @.}O1{..........
-0000d770: b433 0a0b 8a81 01af 2f47 f0ad df27 0b33  .3....../G...'.3
-0000d780: 30f9 1766 ab5f d696 88b5 8650 7324 6fb2  0..f._.....Ps$o.
-0000d790: 27a3 535f 9873 491a 83fa e0c2 4dc0 f4c1  '.S_.sI.....M...
-0000d7a0: 91f3 9112 9276 44c5 ea12 7576 6c6b 42c3  .....vD...uvlkB.
-0000d7b0: d4a3 c364 8b55 b8c9 302f f018 e5b9 15b8  ...d.U..0/......
-0000d7c0: 5619 e7b6 c26d 1638 5fc0 2413 73ca d61b  V....m.8_.$.s...
-0000d7d0: 38e9 2355 e769 1a45 f86f a0ee 03b6 3713  8.#U.i.E.o....7.
-0000d7e0: ecbc acc7 096d 9bca c1bf a30c b0eb 2e74  .....m.........t
-0000d7f0: 51fd 0034 fd42 3791 0e78 9c8d 8d41 0ec2  Q..4.B7..x...A..
-0000d800: 2010 00ef bc62 ef26 0d2c a52c 8931 510f   ....b.&.,.,.1Q.
-0000d810: fa0d a08b eda1 ada1 5bfd be3c c139 cf64  ........[..<.9.d
-0000d820: a432 03c6 1eb1 7049 4153 f6ce 8571 c4e2  .2....pIAS...q..
-0000d830: cd40 5cb2 f594 c893 4b71 40f5 8e95 5701  .@\.....Kq@...W.
-0000d840: a3d1 1987 269b 1c42 f11e 2da5 9e06 6d13  ....&..B..-...m.
-0000d850: eb1e 5374 8436 9a40 2a1e 326d 151e b33c  ..St.6.@*.2m...<
-0000d860: 8f04 d72c f3b6 ee70 db04 ce17 30ed 107c  ...,...p....0..|
-0000d870: d096 e0a4 1b2a 6fcb 328b f0df 81ba 4f71  .....*o.2.....Oq
-0000d880: 7df1 081f ae7b 3361 3d96 d4f2 ef2c 137c  }....{3a=....,.|
-0000d890: 74e7 3aa7 7e3c 0640 b391 0e78 9c8d cb4d  t.:.~<.@...x...M
-0000d8a0: 0e82 3010 40e1 7d4f 317b 1332 ed50 da26  ..0.@.}O1{.2.P.&
-0000d8b0: c644 5de8 35fa 3315 1614 0383 5e5f 8ee0  .D].5.3.....^_..
-0000d8c0: 5bbf 4f56 6640 8ec8 e423 eae4 83f5 b5a6  [.OVf@...#......
-0000d8d0: 5c4d 7031 3a47 5c2b d360 88fa 82ea 1d57  \Mp1:G\+.`.....W
-0000d8e0: 6e02 96bd b709 5309 58a2 cf48 3438 caa6  n.....S.X..H48..
-0000d8f0: d4cc 9a7a 2ece 629f 4c0e 2aee 322e 2b3c  ...z..b.L.*.2.+<
-0000d900: 2679 ee09 ae59 a6a5 6d70 5b04 ce17 d04e  &y...Y..mp[....N
-0000d910: 0fc1 79ab 039c f048 e565 9e27 11fe 1ba8  ..y....H.e.'....
-0000d920: fb18 db8b 0b7c 78dd 8e13 da3e a783 7f27  .....|x....>...'
-0000d930: 19e1 839d ed7a f503 4877 4257 910e 789c  .....z..HwBW..x.
-0000d940: 8d8b 390e c230 1000 7bbf 627b a468 6de3  ..9..0..{.b{.hm.
-0000d950: 4b42 4840 01df f0da 1b92 220e 4a36 e1fb  KBH@......".J6..
-0000d960: e409 4c33 cd8c 2ccc 50d9 628f 648b d367  ..L3..,.P.b.d..g
-0000d970: 4368 cf2e 5266 d487 c8a7 8c48 64aa 0ba4  Ch..Rf.....Hd...
-0000d980: 3e79 e126 10b8 f698 3ce5 925c c4a0 73aa  >y.&....<..\..s.
-0000d990: 39f5 2646 e38d d626 a4be fa42 a9aa bcc9  9.&F...&...B....
-0000d9a0: 302f f01c e5b5 11dc 8a8c 735b e13e 0b5c  0/........s[.>.\
-0000d9b0: aea0 83f6 2944 eb1d 9cf0 4095 799a 4611  ....)D....@.y.F.
-0000d9c0: fe7b 508f 21b7 3757 d879 598f 12da 36d1  .{P.!.7W.yY...6.
-0000d9d0: b17f 4719 60c7 ce75 56fd 00f5 c141 ea97  ..G.`..uV....A..
-0000d9e0: 4378 9c75 94c9 cea3 5614 84f7 3cc5 95b2  Cx.u....V...<...
-0000d9f0: 4964 25cc 93d4 899a c9d8 3f18 6c30 36b0  Id%.......?.l06.
-0000da00: 63b8 cc70 f165 30f6 d3c7 9dde 76ce b2a4  c..p.e0.....v...
-0000da10: da54 d577 660c 2180 3ccd d112 0d19 8113  .T.wf.!.<.......
-0000da20: b34c 9673 2e13 a0c0 a579 5664 32cc d884  .L.s.....yVd2...
-0000da30: 65f8 b490 3962 4c30 1c66 4009 89c4 09b4  e...9bL0.f@.....
-0000da40: c0d0 344b 718c 54f0 3997 fe70 3309 2ba6  ..4Kq.T.9..p3.+.
-0000da50: 592a 30b9 08e9 8c23 9265 ae10 06ee b060  Y*0....#.e.....`
-0000da60: 10d8 81ef 46e0 5b32 2739 2a93 8112 be97  ....F.[2'9*.....
-0000da70: 7d52 777f 65a8 ff07 d022 2dc8 1225 5334  }Rw.e...."-..%S4
-0000da80: d851 2c45 111f b5af e719 6260 d6f3 6149  .Q,E......b`..aI
-0000da90: c1b7 0161 3876 afef 653d 574b fa3f b672  ...a8v..e=WK.?.r
-0000daa0: 2ca7 ba04 7ffe 38d5 308f 0e38 9b67 e01f  ,.....8.0..8.g..
-0000dab0: 4d47 b906 9ef1 9f4e 0002 3ca7 7da6 2a8a  MG.....N..<.}.*.
-0000dac0: aa29 ca45 bd7c f5b7 e7ab d33c 8d4e 2ee2  .).E.|.....<.N..
-0000dad0: b2f0 41d5 298a b244 cf8b a26e c925 31ec  ..A.)..D...n.%1.
-0000dae0: 5748 f33a aa47 9a82 ebdd 8d3a 02b0 6b3d  WH.:.G.....:..k=
-0000daf0: c639 ee2b f1e8 9192 6818 59e2 d67d 7211  .9.+....h.Y..}r.
-0000db00: 689e 5683 a929 16d7 4bde 5ee3 5493 672f  h.V..)..K.^.T.g/
-0000db10: 01c9 d364 31aa 43a4 51d8 349b 2b4b 007c  ...d1.C.Q.4.+K.|
-0000db20: b866 efd9 74e4 c338 382f 6f10 587e a896  .f..t..88/o.X~..
-0000db30: c78e c1fc 33b5 8cb3 af1e bb0d ab50 6937  ....3........Pi7
-0000db40: 4ede 20ff f22b 9751 5b88 f372 1cd0 eb44  N. ..+.Q[..r...D
-0000db50: 009b ad67 d543 5115 88ee e9cd d476 767d  ...g.CQ......vv}
-0000db60: c7d7 6a56 d6e6 f9d6 39be 6315 35ec 5d18  ..jV....9.c.5.].
-0000db70: 3547 b4d7 144d 2bfa eafc da32 acc5 8bbf  5G...M+....2....
-0000db80: 3005 0104 2e41 6281 0d74 3fd1 5c10 91ce  0....Ab..t?.\...
-0000db90: b6ee 648b cf04 6176 72c3 8dec d7dc 77af  ..d...avr.....w.
-0000dba0: 8491 ce07 b369 b1a5 cb45 ca05 d3e3 d89b  .....i...E......
-0000dbb0: 0337 3803 015e 7e1f 75b6 7bf6 fc32 f3f3  .78..^~.u.{..2..
-0000dbc0: ce47 f1e3 1679 79cb 3f5b 8389 8dbb 306d  .G...yy.?[....0m
-0000dbd0: ee9e ef24 8b56 2e8c b557 d3d5 0d0d a755  ...$.V...W.....U
-0000dbe0: 37f3 d81d 9f77 9700 c70a 1ec8 327e a81c  7....w......2~..
-0000dbf0: 1b37 e48a bf98 dec8 a699 3cd9 e7f1 555b  .7........<...U[
-0000dc00: d678 df61 3e4c 3b5e 4e14 e69d 3d6e 211f  .x.a>L;^N...=n!.
-0000dc10: 25e8 3adc c912 3dee da4a 009d 79ac c157  %.:...=..J..y..W
-0000dc20: d451 b23c 85d5 1e4e e158 85ee ea22 cf65  .Q.<...N.X...".e
-0000dc30: 59e9 f2dc ae16 5f1a 27bd 682c bfc6 68d0  Y....._.'.h,..h.
-0000dc40: 63c7 4c4f 7ba3 b35a 9474 eb83 00ea a5cd  c.LO{..Z.t......
-0000dc50: ab49 c422 cc69 2f43 e81a 9ebf 2249 dcb3  .I.".i/C...."I..
-0000dc60: bb72 4d98 afa9 8998 9167 b642 8739 df71  .rM......g.B.9.q
-0000dc70: d627 a203 3f4b d61d 6fe1 895b c69e 00f4  .'..?K..o..[....
-0000dc80: 1493 defa 46b7 0d8a 7e28 2c83 15ac bad6  ....F...~(,.....
-0000dc90: e64e 71d7 6581 db95 ef96 7bc6 b572 76d8  .Nq.e.....{..rv.
-0000dca0: 7963 94d4 58ce b9b9 af74 9214 6f9f e97c  yc..X....t..o..|
-0000dcb0: da34 9d77 736a ecb8 289c dbc6 a936 a3fb  .4.wsj..(....6..
-0000dcc0: 85fc d802 bb43 17f3 7dc0 ed09 e5b0 d197  .....C..}.......
-0000dcd0: 94d3 925d 4def e2aa b59f b702 55aa 7a5f  ...]M.......U.z_
-0000dce0: 3173 25c0 1b52 e651 3e04 f5e5 96cb e649  1s%..R.Q>......I
-0000dcf0: b478 5227 c0df 695d 37c4 4f26 0c47 ff35  .xR'..i]7.O&.G.5
-0000dd00: 1184 92e7 3007 131c 7230 c36d 06cf 0f66  ....0...r0.m...f
-0000dd10: 60ca 3eff 6198 2a34 8374 9967 3480 df7f  `.>.a.*4.t.g4...
-0000dd20: 93fe 2088 7f01 b7ab 54fb ec02 854b 789c  .. .....T....Kx.
-0000dd30: dbce f19f 7142 bf90 85b9 9982 b681 b181  ....qB..........
-0000dd40: 0157 727e 6e6e 6649 49ea c464 1d4e b8e8  .Wr~nnfII..d.N..
-0000dd50: 640e 160d 462e 002e f30b be9c 0d78 9c9d  d...F........x..
-0000dd60: cbbd 0ac2 3010 00e0 3d4f 915d 90fc de25  ....0...=O.]...%
-0000dd70: 20e2 e424 7490 0e8e 97e4 520b b695 9082   ..$t.....R.....
-0000dd80: 8faf cfe0 fac1 d71b b3e4 80c1 e8e4 4c76  ..............Lv
-0000dd90: 3941 2650 4133 b892 d011 6280 5c21 e8ca  9A&PA3....b.\!..
-0000dda0: 2cde d478 ed32 63f5 452b 6f6a b45e b954  ,..x.2c.E+oj.^.T
-0000ddb0: abf7 064b b229 99ea 2880 8eb9 7800 417b  ...K.)..(...x.A{
-0000ddc0: 7f6e 4d0e ebde e478 1bef c343 9ea8 53d9  .nM....x...C..S.
-0000ddd0: 265a 155c a685 e6d7 316f cb59 6ad4 1031  &Z.\....1o.Yj..1
-0000dde0: 1a63 e541 59a5 c44f 97b9 77fe 6f8b ebfc  .c.AY..O..w.o...
-0000ddf0: 115f 2fcb 407d 980e 789c 9dcc 410a c230  ._/.@}..x...A..0
-0000de00: 1040 d17d 4e91 bd20 49a6 4918 10f1 004a  .@.}N.. I.I....J
-0000de10: 17d2 85cb c964 520b 4d2b 21bd bf9e c1ed  .....dR.M+!.....
-0000de20: 87f7 7b13 d181 0bb2 cf9e 8531 f881 6d22  ..{........1..m"
-0000de30: c816 2359 7045 9cc9 9990 dc00 ea43 4db6  ..#YpE.......CM.
-0000de40: ae6d 7410 9c2f 81d8 0896 3410 60f1 094d  .mt../....4.`..M
-0000de50: b62c 2502 71cc 1e52 5274 f4f7 def4 b81d  .,%.q..RRt......
-0000de60: 4d4f f7e9 39be f485 3ae5 7da6 cd84 db5c  MO..9...:.}....\
-0000de70: 6959 cfbc d7eb 6f69 0346 3416 f4c9 8031  iY....oi.F4....1
-0000de80: ea57 ebd2 bbfc a7d5 63d9 964a ab2e 42fd  .W......c..J..B.
-0000de90: 68a2 bee7 2945 f59d 1478 9c9d 8d3d 4ec4  h...)E...x...=N.
-0000dea0: 3010 85fb 9cc2 dd16 0832 76fc 8b10 e200  0........2v.....
-0000deb0: a02d d016 9493 f138 8996 3891 e3dc 1f53  .-.....8..8....S
-0000dec0: 7001 5ef9 f4be efd5 c22c 5488 2a22 9209  p.^......,T.*"..
-0000ded0: a043 904e b131 5a2a 1b9d 8a7a 8803 7034  .C.N.1Z*...z..p4
-0000dee0: 08da 763b 16ce 5524 4a14 c8a3 8ea3 8760  ..v;..U$J......`
-0000def0: d00e 8382 9802 316b c7a3 575e 1129 0e7f  ......1k..W^.)..
-0000df00: 7b44 968e dac6 811d 1280 b2c6 28c5 e812  {D..........(...
-0000df10: 45c9 2938 492d de74 78d6 792b e29a cf22  E.)8I-.tx.y+..."
-0000df20: 6eef b7cf eb97 78c1 8a71 9b30 837d 9b56  n.....x..q.0.}.V
-0000df30: 5cbe 9f68 5b5f 8574 d206 e70d 68f1 0003  \..h[_.t....h...
-0000df40: 40d7 da75 a995 ff47 771f 5c26 1663 c14c  @..u...Gw.\&.c.L
-0000df50: b3b8 ac78 34d3 456c 49cc b5ee c773 df4f  ...x4.ElI....s.O
-0000df60: 4b9d cff1 17ef b776 d0bc 77cc fdb4 d747  K......v..w....G
-0000df70: 3c8e e5a8 986b f703 295b 6641 9c0d 789c  <....k..)[fA..x.
-0000df80: 9dcb b10a c230 1080 e13d 4f91 5d90 4b42  .....0...=O.].KB
-0000df90: 2f77 20e2 e424 7490 0e8e d75c 520b b695  /w ..$t....\R...
-0000dfa0: 9082 8faf cfe0 fa7f fcad e66c 8954 5370  ...........l.TSp
-0000dfb0: 0a9d 2815 74a1 43a2 02cc 8174 4c98 2886  ..(.t.C....tL.(.
-0000dfc0: a8a1 8879 4bcd 6bb3 31eb 4f71 94c4 1d41  ...yK.k.1.Oq...A
-0000dfd0: 74c2 2a5c 3c91 47ef 9c8f 5c14 d3c8 6a64  t.*\<.G...\...jd
-0000dfe0: 6fcf adda 7edd ab1d 6ec3 bd7f d893 34d1  o...~...n.....4.
-0000dff0: 6d92 15f0 322d 32bf 8e69 5bce d645 871c  m...2-2..i[..E..
-0000e000: a903 6f0f 1000 ccaf 2e73 6bf9 bfdb 5ce7  ..o......sk...\.
-0000e010: 8ff9 0223 6840 689d 1478 9c9d 903d 4ec4  ...#h@h..x...=N.
-0000e020: 3014 84fb 9cc2 dd16 08e2 bfe7 1f84 1007  0...............
-0000e030: 006d 81b6 a07c b69f 9368 8913 39ce fd31  .m...|...h..9..1
-0000e040: 0517 40d3 8de6 9b91 a655 2216 2271 9d41  ..@......U"."q.A
-0000e050: 80a0 1c45 f290 c843 f6e8 24b9 2e00 c51d  ...E...C..$.....
-0000e060: 0523 871d 2b95 c602 4850 1253 cc96 acd4  .#..+...HP.S....
-0000e070: 803e 29ee b9e3 28a2 4b90 9d34 5e04 127f  .>)...(.K..4^...
-0000e080: 79f4 2a67 8b19 1490 801c 8cd6 a812 9a88  y.*g............
-0000e090: 5224 ed4d 88de 7172 76c0 b3cd 5b65 d772  R$.M..qrv...[e.r
-0000e0a0: 5676 7bbf 7d5e bfd8 0b36 4cdb 8485 9bb7  Vv{.}^...6L.....
-0000e0b0: 69c5 e5fb 296e eb2b 1356 186f 9dd2 923d  i...)n.+.V.o...=
-0000e0c0: 70c5 f9d0 dd75 698d fe47 0f1f 54a7 7e44  p....ui..G..T.~D
-0000e0d0: c512 6776 59f1 e84d 17b6 6536 b7b6 1fcf  ..gvY..M..e6....
-0000e0e0: e338 2d6d 3ec3 2f3e 6e7d a0f7 deb1 8cd3  .8-m>./>n}......
-0000e0f0: de1e f138 96a3 6169 c30f aae2 6690 9c0d  ...8..ai....f...
-0000e100: 789c 9dcb b10a c230 1000 d03d 5f91 5d90  x......0...=_.].
-0000e110: bb24 5e1a 1071 7212 3a48 07c7 bbf4 a205  .$^..qr.:H......
-0000e120: db4a 48c1 cfd7 6f70 7df0 5a55 b531 810f  .JH...op}.ZU.1..
-0000e130: a812 424a 9091 b980 c7e2 ca28 98ba 9883  ..BJ.......(....
-0000e140: 1452 5f88 cd9b ab2e cd0a 6889 8491 a853  .R_.......h....S
-0000e150: 643f 4af1 14b2 5210 7770 1824 9160 27ce  d?J...R.wp.$.`'.
-0000e160: 19de da73 adb6 5fb6 6a87 eb70 ebef f6c8  ...s.._.j..p....
-0000e170: 8dc7 f5c1 0bd0 f931 f3f4 dae7 753e 598c  .......1....u>Y.
-0000e180: 4829 763e 80dd 8107 303f 9da7 d6f4 bf6d  H)v>....0?.....m
-0000e190: 2ed3 c77c 0100 4940 30a1 0778 9c33 3430  ...|..I@0..x.340
-0000e1a0: 3033 3151 888f cfcc cb2c 898f d72b a864  031Q.....,...+.d
-0000e1b0: 7836 f7d1 ec4d 17af 397b 776b ae2b 8fba  x6...M..9{wk.+..
-0000e1c0: 71e8 494f f044 4388 b2a4 d292 92fc 3c90  q.IO.DC.......<.
-0000e1d0: a253 ec12 9c4b a426 1e9d b4fa c1d6 9f7e  .S...K.&.......~
-0000e1e0: a7b4 9d97 5dad 832a 2ace 4ccf 4bcc 0129  ....]..**.L.K..)
-0000e1f0: ca5b 793a b7b3 36e4 c72f 5f5b d63d 4a6e  .[y:..6../_[.=Jn
-0000e200: 1e33 d777 be03 005e 4c30 2aab 1578 0133  .3.w...^L0*..x.3
-0000e210: 3100 0205 bdf4 cc92 8cd2 2486 7b8f 0f45  1.........$.{..E
-0000e220: 3fe8 78db 2ecd bde7 c6be f99e 3c31 8d5c  ?.x.........<1.\
-0000e230: 870c 0d0c cc4c 4cc0 4a32 d3f3 f28b 5219  .....LL.J2....R.
-0000e240: e6ba 4fb6 a9be 75fc a1cb f199 1d9b e79f  ..O...u.........
-0000e250: e1e4 facb 740a aaca c7d3 d9d5 2fd8 95c1  ....t......./...
-0000e260: f07a 61c0 a977 7dbe 6f2a 3eb3 707e f9c7  .za..w}.o*>.p~..
-0000e270: fb6a 9be0 41a8 125f 473f 4f37 d7e0 10bd  .j..A.._G?O7....
-0000e280: cc3c 8695 3e0f 176e ba71 f1f6 ad94 3b4f  .<..>..n.q....;O
-0000e290: 5324 fa4b 3cf8 f599 a1ca 825c 1d5d 7c5d  S$.K<......\.]|]
-0000e2a0: f572 5318 9ad4 e646 6b2e adb9 fc77 01fb  .rS....Fk....w..
-0000e2b0: b1e3 6d97 0425 17be 5586 2a4a 2acd 2dd0  ..m..%..U.*J*.-.
-0000e2c0: 2ba8 64b8 37f1 ce3a d555 c72f 334d b129  +.d.7..:.U./3M.)
-0000e2d0: 70fd d9b0 daf4 ee69 0f13 b0cf d20b 4ae2  p......i......J.
-0000e2e0: 93f3 730b 4a4b 528b e213 8b8b 338b 4b12  ..s.JKR.....3.K.
-0000e2f0: f34a 185c 16cc 764e baac c654 f749 7cc9  .J.\..vN...T.I|.
-0000e300: d32f 2bee fd0d 6f9f 0935 b328 b5b0 34b3  ./+...o..5.(..4.
-0000e310: 2835 3735 afa4 58af a4a2 8481 67e2 8c35  (575..X.....g..5
-0000e320: 6736 5f5c 7b35 db65 dad3 89bf 244e af4f  g6_\{5.e....$N.O
-0000e330: f903 555b 9c5a 520a 7680 acf6 fe92 1bca  ..U[.ZR.v.......
-0000e340: 3ffb 0f31 7f68 da9a 3751 fe57 80a7 1e00  ?..1.h..7Q.W....
-0000e350: e60e 9239 a114 7801 3334 3030 3331 5188  ...9..x.340031Q.
-0000e360: 8fcf cccb 2c89 8fd7 2ba8 64f8 29d9 d87a  ....,...+.d.)..z
-0000e370: d847 50b4 c651 eaf0 e28b 2f97 b884 a45f  .GP..Q..../...._
-0000e380: 3431 0002 85c4 f4d4 bc12 8696 e33e 3b94  41...........>;.
-0000e390: 45f9 6fef 3e6a dddf fd25 a5d4 2882 ff09  E.o.>j...%..(...
-0000e3a0: 54be 3425 339f e1d2 464d b90e 1bfb b961  T.4%3...FM.....a
-0000e3b0: 938a 6dc5 df9c 532e 38c2 5761 08b1 26bd  ..m...S.8.Wa..&.
-0000e3c0: a024 3e39 3fb7 a0b4 24b5 283e b1b8 38b3  .$>9?...$.(>..8.
-0000e3d0: b824 31af 0464 e921 b92f 5f59 9caf af71  .$1..d.!./_Y...q
-0000e3e0: 396c 287d f3cb e265 bc49 f1af 2186 a697  9l(}...e.I..!...
-0000e3f0: 6632 58fd d5bb 189f 6e26 5ce0 b0e5 fdd7  f2X.....n&\.....
-0000e400: 6ea9 291f a655 5f84 1a99 9393 0bd2 5fa2  n.)..U_......._.
-0000e410: c9ea 76eb a140 5a8e 5dc7 3f2d 03a9 c9a1  ..v..@Z.].?-....
-0000e420: 3b59 0f42 f417 2717 a5a6 e631 9c3f d5df  ;Y.B..'....1.?..
-0000e430: 7ccb e60b d789 531c c23f 5e4a 2d93 9410  |.....S..?^J-...
-0000e440: 8d85 1a01 7444 11d8 110a 2e57 17cc 0f55  ....tD.....W...U
-0000e450: da99 98ad aac3 3171 d98b 55d5 a752 2086  ......1q..U..R .
-0000e460: 9496 64e6 1433 2c5c e377 e9fc dbb6 e8c3  ..d..3,\.w......
-0000e470: 1995 0d56 d60b 7705 cb1c b505 00dd 567f  ...V..w.......V.
-0000e480: d0ae 0e78 0133 3430 3033 3151 888f cfcc  ...x.340031Q....
-0000e490: cb2c 898f d72b a864 4868 356b fe68 a8c2  .,...+.dHh5k.h..
-0000e4a0: 7268 6246 e3ba 0c0b 3389 ffaa ee86 1065  rhbF....3......e
-0000e4b0: 89e9 a979 2520 35b3 af38 fa4f 64d0 a839  ...y% 5..8.Od..9
-0000e4c0: 7e66 a3c9 0ac6 cc7f d9cf 3e08 c3d4 1417  ~f........>.....
-0000e4d0: 6716 9724 42d4 6df4 9311 98f7 2d42 cbe0  g..$B.m.....-B..
-0000e4e0: a774 fe1f 75ad 4f21 12d5 7550 7549 89c9  .t..u.O!..uPuI..
-0000e4f0: d9e9 45f9 a579 2920 039f 4ff1 1359 e297  ..E..y) ..O..Y..
-0000e500: 706c 59b7 e61f 6fc3 80ed 195c ebb6 4015  plY...o....\..@.
-0000e510: 2667 2496 c467 00cd cc2f aa04 295d b66b  &g$..g.../..)].k
-0000e520: 99d9 85af 86ce 6ab3 a7f5 441c ce90 ec9e  ......j...D.....
-0000e530: c8fd 15aa b4a0 283f 3939 b5b8 18a4 ecda  ......(?99......
-0000e540: db5b 5abd a559 9b65 e6ed 9fe2 b3c1 7282  .[Z..Y.e......r.
-0000e550: ab93 5635 007a 225c 7ae4 0385 4e78 9c01  ..V5.z"\z...Nx..
-0000e560: 3400 cbff db02 db02 90f7 1429 7dac 1609  4..........)}...
-0000e570: 61f0 aeea 7323 74aa e426 9750 1333 2893  a...s#t..&.P.3(.
-0000e580: 0b01 3c14 0488 e2c8 7683 914c 32de aaa8  ..<.....v..L2...
-0000e590: 667e 7497 f76a 04d8 575b 174c a114 7801  f~t..j..W[.L..x.
-0000e5a0: 3334 3030 3331 5188 8fcf cccb 2c89 8fd7  340031Q.....,...
-0000e5b0: 2ba8 6428 6b2f 7e3f 656e 8248 63f6 6fa9  +.d(k/~?en.Hc.o.
-0000e5c0: 8ebf 2f2f 947f 8edf 6662 0004 0a89 e9a9  ..//....fb......
-0000e5d0: 7925 0c4e 5e1b 8f4c beb7 86bb df2c 5ef9  y%.N^..L.....,^.
-0000e5e0: bbd1 df92 1759 7bd6 42e5 4b53 32f3 192e  .....Y{.B.KS2...
-0000e5f0: 6dd4 94eb b0b1 9f1b 36a9 d856 fccd 39e5  m.......6..V..9.
-0000e600: 8223 7c15 8610 6bd2 0b4a e293 f373 0b4a  .#|...k..J...s.J
-0000e610: 4b52 8be2 138b 8b33 8b4b 12f3 4a40 968a  KR.....3.K..J@..
-0000e620: c5c8 d63e 99c5 b1ea ebbc 2b56 8756 eeca  ...>......+V.V..
-0000e630: d821 68f0 0262 687a 6926 c382 ed92 4619  .!h..bhzi&....F.
-0000e640: 190f 9e8b 9af9 bc7d 3adf 7733 ebc4 1b6e  .......}:.w3...n
-0000e650: 5023 7372 7241 fa4b 3459 dd6e 3d14 48cb  P#srrA.K4Y.n=.H.
-0000e660: b1eb f8a7 6520 3539 7427 eb41 88fe e2e4  ....e 59t'.A....
-0000e670: a2d4 d43c 86f3 a7fa 9b6f d97c e13a 718a  ...<.....o.|.:q.
-0000e680: 43f8 c74b a965 9212 a2b1 5023 808e 2802  C..K.e....P#..(.
-0000e690: 3b42 c1e5 ea82 f9a1 4a3b 13b3 5575 3826  ;B......J;..Uu8&
-0000e6a0: 2e7b b1aa fa54 0ac4 90d2 92cc 9c62 8685  .{...T.......b..
-0000e6b0: 6bfc 2e9d 7fdb 167d 38a3 b2c1 ca7a e1ae  k......}8....z..
-0000e6c0: 6099 a3b6 00bc e182 02eb 0183 4878 9c7b  `...........Hx.{
-0000e6d0: c7f8 8e71 c22d 91b5 0cc7 d82e 3c5e e5c8  ...q.-......<^..
-0000e6e0: ffe1 6ec0 4c0b 0d6d c503 baae 00b6 a10c  ..n.L..m........
-0000e6f0: 17e4 0388 6678 9c01 3400 cbff db02 db02  ....fx..4.......
-0000e700: 90f7 1471 e3b4 0dcc a6a0 4140 14fd 8784  ...q......A@....
-0000e710: 3a2a 1fe4 efbe 8093 0b01 3c14 0aac 1694  :*........<.....
-0000e720: 4d6b 28c7 fc05 9944 50df 60a7 6888 f41f  Mk(....DP.`.h...
-0000e730: 8113 17bb ef04 8218 789c 3bc8 7490 c9dd  ........x.;.t...
-0000e740: d0c0 c0cc c444 213e 3e33 2fb3 243e 5eaf  .....D!>>3/.$>^.
-0000e750: a092 c17f ad07 3f4f 0957 c855 95e9 5967  ......?O.W.U..Yg
-0000e760: 5f1a 671a 07f8 7f37 3100 0285 c4f4 d4bc  _.g....71.......
-0000e770: 1286 d52e feeb 0e37 3444 fdc8 57de 9d6e  .......74D..W..n
-0000e780: d330 4596 7d87 fb44 f75f 0043 6f1d c7ef  .0E.}..D._.Co...
-0000e790: 0180 1e78 9c01 1f00 e0ff db02 db02 90f7  ...x............
-0000e7a0: 14a2 85ae 6d64 5ef9 a5b7 e005 5c3d 588a  ....md^.....\=X.
-0000e7b0: f785 e29d da93 0b01 5003 b70f d3ee 0180  ........P.......
-0000e7c0: 0978 9c01 1e00 e1ff c102 c102 9033 14a8  .x...........3..
-0000e7d0: 418e 57a4 e8a6 f28c ec8a 9504 e5f9 e7b4  A.W.............
-0000e7e0: a31b ba91 47fa eb1e 10ae ee01 8121 789c  ....G........!x.
-0000e7f0: 7bc7 f88e 7182 b988 d10b 5bff 73bf 8ccd  {...q.....[.s...
-0000e800: 99b5 9adc 0be6 5707 336f 347a 39d1 7b31  ......W.3o4z9.{1
-0000e810: 00c1 8a0c b3e4 038b 0a78 9c01 3400 cbff  .........x..4...
-0000e820: db02 db02 90f7 14f6 33ed d3c7 612d cc4e  ........3...a-.N
-0000e830: de3a ff17 2ae7 a0fb 6a17 0593 0b01 3c14  .:..*...j.....<.
-0000e840: e247 eeb0 629d c5d9 881e fe68 441c 79ff  .G..b......hD.y.
-0000e850: ea8f 885f c28a 1aa5 e003 801b 789c 3bc8  ..._........x.;.
-0000e860: 7490 49dd d0c0 c0cc c444 213e 3e33 2fb3  t.I......D!>>3/.
-0000e870: 243e 5eaf a092 6155 ceaa 94b8 67b9 4d0a  $>^...aU....g.M.
-0000e880: 4f3a ddf2 a646 c46c d158 f362 a3ba 1423  O:...F.l.X.b...#
-0000e890: 00a0 3712 88e4 038c 0a78 9c01 3400 cbff  ..7......x..4...
-0000e8a0: db02 db02 90f7 14be bc19 a285 3146 d869  ............1F.i
-0000e8b0: 74fc 1a54 96a8 ecaf c070 0193 0b01 3c14  t..T.....p....<.
-0000e8c0: 4508 ca52 16d7 d238 30a7 d1ec 0df7 8aa2  E..R...80.......
-0000e8d0: 6e33 cb40 8bfd 186f e403 8c4d 789c 0134  n3.@...o...Mx..4
-0000e8e0: 00cb ffdb 02db 0290 f714 cc13 0885 cd7b  ...............{
-0000e8f0: cc3c 033e 10b5 a01d 51ff b760 67a4 930b  .<.>....Q..`g...
-0000e900: 013c 140b 9764 4769 b279 88d3 bb69 be25  .<...dGi.y...i.%
-0000e910: 8434 2ce1 8988 0453 0c16 53e4 0386 4278  .4,....S..S...Bx
-0000e920: 9c01 3400 cbff db02 db02 90f7 141a 03eb  ..4.............
-0000e930: 1ab9 38e5 3bcd 1168 cecc 2bf8 6e20 aa76  ..8.;..h..+.n .v
-0000e940: 1b93 0b01 3c14 1d2b bf74 d823 f98f c203  ....<..+.t.#....
-0000e950: f082 b56e 911f fa50 492e 5f78 170d e403  ...n...PI._x....
-0000e960: 836d 789c 0134 00cb ffdb 02db 0290 f714  .mx..4..........
-0000e970: 02e2 e3ff 9b9a b5a5 646b 8d52 d2fc c1c5  ........dk.R....
-0000e980: ab6c cffa 930b 013c 143e 5f99 9b65 e4d5  .l.....<.>_..e..
-0000e990: 6529 111a d192 bfc6 de42 5caf 47f0 b71b  e).......B\.G...
-0000e9a0: 7eef 0143 789c bbcd 749b 69c2 7791 baea  ~..Cx...t.i.w...
-0000e9b0: a90f e744 f518 db95 cb3b 7e5a 5777 4cb8  ...D.....;~ZWwL.
-0000e9c0: 2ce1 f164 6ec6 0000 f026 0e2e e403 2b78  ,..dn....&....+x
-0000e9d0: 9c01 3400 cbff db02 db02 90f7 14bb f307  ..4.............
-0000e9e0: ff3c e72e 6cf8 df49 bc07 ab19 eac8 f0bf  .<..l..I........
-0000e9f0: 6b93 0b01 3c14 0488 e2c8 7683 914c 32de  k...<.....v..L2.
-0000ea00: aaa8 667e 7497 f76a 04d8 cce3 1ac3 ef01  ..f~t..j........
-0000ea10: 8279 789c 011f 00e0 ffdb 02db 0290 f714  .yx.............
-0000ea20: f98a 9ff7 dbca 4e98 b5ba 343a 83cd 588a  ......N...4:..X.
-0000ea30: 0d29 54a5 930b 0150 103d 0f27 e003 8c68  .)T....P.=.'...h
-0000ea40: 789c 3bc8 7490 49dd d0c0 c0cc c444 213e  x.;.t.I......D!>
-0000ea50: 3e33 2fb3 243e 5eaf a092 6196 92f6 42fd  >3/.$>^...a...B.
-0000ea60: f29a 0367 3a0a f575 77ae fe99 f9db 65d5  ...g:..uw.....e.
-0000ea70: 4675 2946 0095 5612 71b1 0378 9c4b 2bca  Fu)F..V.q..x.K+.
-0000ea80: cf55 d02b 2e49 2c2a 51c8 cc2d c807 5260  .U.+.I,*Q..-..R`
-0000ea90: 0e17 1757 7c7c 596a 5171 667e 5e7c bc82  ...W||YjQqf~^|..
-0000eaa0: ad82 ba81 9e99 9e81 3a17 00b2 170f a1eb  ........:.......
-0000eab0: 018b 2e78 9c7b c7f8 8e71 c22d 91bf 2edd  ...x.{...q.-....
-0000eac0: 0af9 96ab 2e74 ddbf 1527 cff9 d0b5 fbdc  .....t...'......
-0000ead0: 7579 00be e60d a9eb 0187 0e78 9c7b c7f8  uy.........x.{..
-0000eae0: 8e71 c22d 11bb ed7b c29e dc9f 7ecf 31e3  .q.-...{....~.1.
-0000eaf0: 5bf1 a5b5 3ced 93bd 6c5c 00cd 700e 1dba  [...<...l\..p...
-0000eb00: 3b78 9cbd 52bb 6edc 3010 ecf5 150b b991  ;x..R.n.0.......
-0000eb10: 8203 3f20 c015 2912 2040 0ac3 4e8a 2008  ..? ..). @..N. .
-0000eb20: e43d 6a25 11a1 489a 5cda f1df 6749 ddc3  .=j%..H.\...gI..
-0000eb30: 38b8 4a61 16a2 48cd ccee 8c76 8a7e 05a5  8.Ja..H....v.~..
-0000eb40: ac5d c1ac c147 860f 4d59 53b9 b7e8 e639  .]...G..MYS....9
-0000eb50: 6258 945e 48ff 09de 3856 e9d1 1aa6 13fa  bX.^H...8V......
-0000eb60: be9e eef1 8962 f316 3144 3a64 63f9 84d7  .....b..1D:dc...
-0000eb70: 0bf2 8033 391e e82f e9cc 3e9e 4839 24ef  ...39../..>.H9$.
-0000eb80: 8c3e 21bf 9b59 34d9 7b9b 60bf 9dba 7e3b  .>!..Y4.{.`...~;
-0000eb90: 2b72 78b0 34a0 d087 488f d944 5a45 b200  +rx.4...H..DZE..
-0000eba0: bfa0 4d74 a66d f0d2 8e14 364e 0446 9a60  ..Mt.m....6N.F.`
-0000ebb0: a6eb 1eba fe63 03b2 2271 8eee ad2e 958e  .....c.."q......
-0000ebc0: 844c 4351 1c34 5a6b dc7c a117 c5d5 8f64  .LCQ.4Zk.|.....d
-0000ebd0: bb7e b715 ed4b 186d db5e 02a9 1da8 aa9a  .~...K.m.^......
-0000ebe0: ce26 057a 8510 d140 d114 3f68 5566 2301  .&.z...@..?hUf#.
-0000ebf0: 1b3a 336e 5f78 f1ee eef3 edb7 26d4 5709  .:3n_x......&.W.
-0000ec00: 2058 b17a f920 2e6f e0a7 cfa0 51ac d4b6   X.z. .o....Q...
-0000ec10: 8117 aa7d c903 02a6 5476 f95a bb69 8a42  ...}....Tv.Z.i.B
-0000ec20: 3556 8296 adab 5938 5c69 dfbe 2ad2 eeea  5V....Y8\i..*...
-0000ec30: fd48 4947 13d8 78b7 6f3f 1deb 425a c85a  .HIG..x.o?..BZ.Z
-0000ec40: 053f 52a9 65aa fe96 0ec1 2601 daaf 2bba  .?R.e.....&...+.
-0000ec50: 3129 f8ea 4266 61f8 6c47 3810 203c a135  1)..Bfa.lG8. <.5
-0000ec60: e315 5070 13bc 888d 6774 5cf4 126d 3e7c  ..Pp....gt\..m>|
-0000ec70: e6c2 f7d3 46cc b4ab b0a3 5e88 32a5 60b8  ....F.....^.2.`.
-0000ec80: c0e0 d9f0 020f f5aa 534a f50f ea68 62ca  ........SJ...hb.
-0000ec90: 4eef 5f79 5331 bb5d d3ff d7fc bec3 48fd  N._yS1.]......H.
-0000eca0: 3aff a2df 7d9d aaa6 f907 8fbe 5167 ba26  :...}.......Qg.&
-0000ecb0: 789c 8d90 4f4b c430 10c5 effd 14a1 a714  x...OK.0........
-0000ecc0: 245d f5b6 d08b 7a58 4111 5d2f 2212 d224  $]....zXA.]/"..$
-0000ecd0: ed0e e6cf 9aa4 8722 7e77 63da ba6e a968  ......."~wc..n.h
-0000ece0: 6e99 79bf 9979 af71 5623 c54c cb77 0c0c  n.y..y.qV#.L.w..
-0000ecf0: e556 ebce 40e8 49fc 07aa a5f7 ac95 7407  .V..@.I.......t.
-0000ed00: 3e58 07d2 23d0 7beb 02da dedf 5c46 c1ed  >X..#.{.....\F..
-0000ed10: d0df a476 9f35 5fc3 48cd f86b eb6c 67c4  ...v.5_.H..k.lg.
-0000ed20: a456 4a8f 237a 6aa1 05c3 5496 8d3d eb47  .VJ.#zj...T..=.G
-0000ed30: 8c74 0194 27a2 9ea8 5686 6f4a d459 7c42  .t..'...V.oJ.Y|B
-0000ed40: 36a9 ba70 5b8f 8b75 86e2 db3b 3001 e79b  6..p[..u...;0...
-0000ed50: ebed e3dd c313 baba c84f 6693 7051 2425  .........Of.pQ$%
-0000ed60: b7c6 481e c01a 542d 1bc2 49e7 632d 8a28  ..H...T-..I.c-.(
-0000ed70: 882a 6735 3f3d 3b8f 230f 30f5 21ae 6cab  .*g5?=;.#.0.!.l.
-0000ed80: 26f7 6f0a 825c 9765 f93e dff8 910f 3ba1  &.o..\.e.>....;.
-0000ed90: 414a 1a7c a0c9 68c3 17a8 aad0 6af0 707c  AJ.|..h.....j.p|
-0000eda0: 1d61 424c 6ef1 4294 cfab 9722 4b9c 93a1  .aBLn.B...."K...
-0000edb0: 73e6 073a 9487 e0b8 92cc 0dd1 cd22 fb3d  s..:.........".=
-0000edc0: 5292 205c fc25 fbcf 859f f97d d72f b8d6  R. \.%.....}./..
-0000edd0: 0278 9ced 574b 8fdb 3610 befb 5710 3e49  .x..WK..6...W.>I
-0000ede0: cd46 4872 5cc0 c716 4d90 1712 2f7a d82e  .FHr\...M.../z..
-0000edf0: 085a a22d 66f9 1048 2a5d fdfb 0e49 917a  .Z.-f..H*]...I.z
-0000ee00: 39b1 9383 1ba0 f6c1 9686 33df 3c38 fc86  9.........3.<8..
-0000ee10: de6b 2550 5170 2e10 138d d216 fdb6 da7b  .k%PQp.........{
-0000ee20: 1931 8619 4ba4 1d16 fa95 b226 16d7 b0a8  .1..K......&....
-0000ee30: 74b7 582c 485b 3155 586b e292 a54f 165b  t.X,H[1UXk...O.[
-0000ee40: 854d 4369 594f d58c 4df0 61d9 293a 8319  .MCiYO..M.a.):..
-0000ee50: 9ca6 a5d2 5554 f532 5c11 4b56 49ef d0b2  ....UT.2\.KVI...
-0000ee60: c2b0 8324 3c01 fa37 5c13 5971 aa57 ab18  ...$<..7\.Yq.W..
-0000ee70: 4ead 29a9 983c 44db a63b 1041 a395 604f  N.)..<D..;.A..`O
-0000ee80: 4e39 6933 41e3 b306 2425 a2c3 d632 6e8a  N9i3A...$%...2n.
-0000ee90: 6a37 aac0 6a08 67be 6a3a 63a9 c046 b5b2  j7..j.g.j:c..F..
-0000eea0: c25c 95c4 3225 6fc0 5b89 436e 23e1 97d6  .\..2%o.[.Cn#...
-0000eeb0: 586c 4a4d a934 b5b2 b821 b6be 4133 01b8  XlJM.4...!..A3..
-0000eec0: aae8 1e35 5a95 d418 ec4b 9259 f248 4796  ...5Z....K.Y.HG.
-0000eed0: 9bad 6ee9 0d0a d210 80d7 dbfc 41b8 8185  ..n.........A...
-0000eee0: 4a49 7044 be52 cc04 39d0 20ce 6f57 083e  JIpD.R..9. .oW.>
-0000eef0: 07ae 7650 cb71 a99d 387c 5b28 05b8 618d  ..vP.q..8|[(..a.
-0000ef00: 0b18 6d66 7b97 1dc9 2a0f 866c bf8c e636  ..mf{...*..l...6
-0000ef10: 2c2d 705f 2d81 8f56 b187 f65f d0c7 98c9  ,-p_-..V..._....
-0000ef20: a6b5 60bb befb fcfb a75b b47e 3641 fd5e  ..`......[.~6A.^
-0000ef30: 1c31 8c01 e519 c0a0 bf25 fa60 6baa 91da  .1.......%.`k...
-0000ef40: a3a3 98af 56c9 b96a 6df0 9e8e 4f96 d06e  ....V..jm...O..n
-0000ef50: d081 5aec 4f8f 803d 838a c753 94e5 452f  ..Z.O..=...S..E/
-0000ef60: 31bd 1267 144c f3c5 b66f 66ef 4326 498e  1..g.L...of.C&I.
-0000ef70: 28ec 227a af24 cd5d 43f6 e9ce f67a 48b6  (."z.$.]C....zH.
-0000ef80: 6cb5 065f bc8b 4119 88fe 8c40 13c0 3282  l.._..A....@..2.
-0000ef90: 01dc 9785 9884 03d0 4b7f f7cf 5f3e 1425  ........K..._>.%
-0000efa0: c407 e2fb 170f 13e3 a536 7081 505f 6976  .........6p.P_iv
-0000efb0: 1c27 5f4d ccbf 9347 c929 d159 3e51 df2b  .'_M...G.).Y>Q.+
-0000efc0: 8d62 a44c 1e71 3ecd ec84 0752 5551 9af5  .b.L.q>....RUQ..
-0000efd0: bff9 b9d1 8d6d ff6c 0591 effa 97be 4e9b  .....m.l......N.
-0000efe0: fb71 591f f23e ef33 1187 4e0d 355b 74ef  .qY..>.3..N.5[t.
-0000eff0: 5421 6e4e f0d1 6806 adb9 feab 569c a2b7  T!nN..h.....V...
-0000f000: 6fdf a10f 77db 8f77 dbf5 59ed 9d0f 6775  o...w..w..Y...gu
-0000f010: cacf c3bc 01ea 308d 9286 6247 d45d 4105  ......0...bG.]A.
-0000f020: 8393 901a 5942 8733 833d 49fa d122 5445  ....YB.3.=I.."TE
-0000f030: 3926 a565 d015 f9b0 4309 c69f 93cd 6c0e  9&.e....C.....l.
-0000f040: 8d6a 30ea 194f a99c 7481 6ef2 e976 c749  .j0..O..t.n..v.I
-0000f050: d340 964a 8021 d578 3125 8128 c269 c73b  .@.J.!.x1%.(.i.;
-0000f060: f534 3177 e764 bc58 58f5 9113 26b7 de15  .41w.d.XX...&...
-0000f070: da00 d5ac 97fd 3535 31d4 7af5 71f0 49f5  ......551.z.q.I.
-0000f080: 481a 612c ccf2 1825 3891 fbd1 5730 c98e  H.a,...%8...W0..
-0000f090: 2f88 d6b0 b2e0 8a54 d9a4 b4df d675 8e66  /......T.....u.f
-0000f0a0: 50ff d40c ba66 ace4 9a66 d79a 6e1e a54f  P....f...f..n..O
-0000f0b0: 1ea6 6f61 38a5 4df6 a278 3945 3add 3ed0  ..oa8.M..x9E:.>.
-0000f0c0: 7b4d 43ab d840 4399 d2a3 0b70 47ca 471c  {MC..@C....pG.G.
-0000f0d0: 2e05 ae49 e2ed a0d8 fa27 18a9 1a22 dc0c  ...I.....'..."..
-0000f0e0: d5cc bf65 0d97 19a2 a323 c7c1 b717 69ab  ...e.....#....i.
-0000f0f0: 1f68 909f a9da cfd6 ca65 7aba 54b3 5bcc  .h.......ez.T.[.
-0000f100: 3042 5c91 4ecd f5f5 6b7f 55f2 d307 91d1  0B\.N...k.U.....
-0000f110: a42c 3c91 77aa 4556 010d 082a 7690 2b7a  .,<.w.EV...*v.+z
-0000f120: e394 0de9 907a 2cd6 632a 7324 f6fa 3d70  .....z,.c*s$..=p
-0000f130: 18ca 3ce0 8094 03ab 25df f905 c7fc b13b  ..<.....%......;
-0000f140: 601e 6e98 1721 fae8 e717 22e9 4b1c a62b  `.n..!....".K..+
-0000f150: 47a3 5f84 a3d3 d3b8 2257 aefe 0fb9 7ad8  G._....."W....z.
-0000f160: 9b29 69fb 3a79 88d3 941d feda 5f90 47d3  .)i.:y......_.G.
-0000f170: dfa0 0bd1 e679 fb76 e5cc 2b67 5e39 f3ff  .....y.v..+g^9..
-0000f180: c499 ff02 5136 db93 e002 863a 789c 7ba1  ....Q6.....:x.{.
-0000f190: 7559 6b43 2dfb e618 a142 c6cd 5f39 7458  uYkC-....B.._9tX
-0000f1a0: 802c 1ee6 cd26 028a 4c60 1600 cae7 0a31  .,...&..L`.....1
-0000f1b0: e523 2878 9cbb acf5 d770 c31e 4689 9cc4  .#(x.....p..F...
-0000f1c0: e292 f8c4 ccf8 a2d4 e282 fcbc e254 055b  .............T.[
-0000f1d0: 05bf fcbc 54ae c93b 190b 8574 14d0 a537  ....T..;...t...7
-0000f1e0: 6b31 35b2 b072 2900 c1e4 956c 87c4 d373  k15..r)....l...s
-0000f1f0: f293 1273 3094 4d8e 63d7 6256 c82f 9a9c  ...s0.M.c.bV./..
-0000f200: cb2e 2986 2e69 05d1 de28 62a5 0862 6071  ..)..i...(b..b`q
-0000f210: 414e 4e6e 7c7e 6949 4169 c9e6 ddec b798  ANNn|~iIAi......
-0000f220: a441 ca70 d9e4 28a0 b079 2b57 2c23 33c8  .A.p..(..y+W,#3.
-0000f230: 4c7b c16f f470 9231 e3e6 6ebe cd8c 930f  L{.o.p.1..n.....
-0000f240: 0888 cb42 b4e2 76dd 44ad e2e4 a2d4 d4bc  ...B..v.D.......
-0000f250: e28c fc92 f882 c492 0c4d 2e2e b016 6585  .........M....e.
-0000f260: a0d4 dcfc b254 8592 8c54 85cc dcc4 7460  .....T...T....t`
-0000f270: a0ff 6376 9c9c cc62 3a99 8945 68f2 2616  ..cv...b:..Eh.&.
-0000f280: d5c9 8eac d293 7fb1 f04c e663 d506 b24d  .........L.c...M
-0000f290: 8058 7df2 1220 5ec1 9dc9 0276 b183 e057  .X}.. ^....v...W
-0000f2a0: ba79 781e 2300 5f6c c101 b9c2 0578 9ced  .yx.#._l.....x..
-0000f2b0: 5a6d 73db 3612 feae 5f81 533e 986c 64d6  Zms.6..._.S>.ld.
-0000f2c0: 961d 5fea 19df 4cde e369 7295 2de7 7adf  .._...L..ir.-.z.
-0000f2d0: 3810 0949 a829 8205 40cb eadd fdf7 db05  8..I.)..@.......
-0000f2e0: f802 bec8 b253 a7c9 dd54 93c8 24b0 bb58  .....S...T..$..X
-0000f2f0: 3cbb 582c 169a 4bb1 2201 5db0 5407 d192  <.X,..K.".].T...
-0000f300: ea70 c995 1672 43f8 2a13 5293 ef06 7387  .p...rC.*.R...s.
-0000f310: 822a 05dd 34d5 edee 2459 6de1 c0ef feae  .*..4...$Ym.....
-0000f320: 198d ae17 52e4 695c f717 048b 9c07 8a2f  ....R.i\......./
-0000f330: 529a b459 b167 966b 2dd2 0e53 ae79 a282  R..Y.g.k-..S.y..
-0000f340: 78e6 7414 4f4b aa96 099f 95af 6aa3 ca47  x.t.OK......j..G
-0000f350: bd94 8cc6 3c5d 940d 33aa d8c9 71d5 cd57  ....<]..3...q..W
-0000f360: ac7c 9634 8dc5 aa7c 4bf3 55b6 2154 9134  .|.4...|K.U.!T.4
-0000f370: abc4 e254 6276 c323 861d 2a6e 74cc 7962  ...Tbv.#..*nt.yb
-0000f380: 9be7 8342 e16c b3a0 2b56 6abb e2b7 4c96  ...B.l..+Vj...L.
-0000f390: 1c2b aa97 9668 b2b9 d0cf 820b fd33 8f17  .+...h.......3..
-0000f3a0: 4cab 92fa e245 9625 3ca2 9a8b 7444 2e3e  L....E.%<...tD.>
-0000f3b0: 529e fecc 41bf 35bc fce3 a5b8 fd40 3722  R...A.5......@7"
-0000f3c0: d7f0 62f9 9ab2 dee5 bc92 f351 e48a bdb9  ..b........Q....
-0000f3d0: 017b 00f1 04c4 6826 f189 a1d8 9732 572d  .{....h&.....2W-
-0000f3e0: 3d5e 0959 a97c 813c 5700 1172 5cb2 085e  =^.Y.|.<W..r\..^
-0000f3f0: b3cd af7a 6a0c 074d 3fcd 7e81 c6ed 63ff  ...zj..M?.~...c.
-0000f400: c836 53f6 6bce d288 dd3d d9e9 12fe 44b9  .6S.k....=....D.
-0000f410: 2ee1 1195 fd54 c4b3 4dc0 45b0 a637 25c2  .....T..M.E..7%.
-0000f420: c5e3 e031 0144 4800 8b97 c6f3 e0e5 039d  ...1.DH.........
-0000f430: 319c e2fb 8a74 074c 1301 d0ee 50e9 35a7  1....t.L....P.5.
-0000f440: 8958 b415 2887 fac0 53f6 26e6 4d55 1c81  .X..(...S.&.MU..
-0000f450: f570 855c 2044 b8b7 e37f 1e81 00fb c924  .p.\ D.........$
-0000f460: a8e7 0dcf 4d0f 8b09 4d12 022b 4652 c999  ....M...M..+FR..
-0000f470: 1afa 83c1 a077 249c a615 a0e5 e674 40e0  .....w$......t@.
-0000f480: 53f4 457a 9331 655a 561b 9a65 3c26 6764  S.Ez.1eZV..e<&gd
-0000f490: 4fa4 b9a4 9a5e d334 5864 3a8c c42a cbc1  O....^.4Xd:..*..
-0000f4a0: e1c2 2aae 98f5 7db8 479e 102a 675c c3f8  ..*...}.G..*g\..
-0000f4b0: 1ba2 b4c4 058a a2ac d460 0d96 4a92 402d  .........`..J.@-
-0000f4c0: 5992 1c8d 8329 d3af 7229 c187 2752 444c  Y....)..r)..'RDL
-0000f4d0: a937 b768 5bae c1c6 9f14 931f 45cc 92f3  .7.h[.......E...
-0000f4e0: d75e a188 3f60 b711 cbb4 d537 83b1 41fd  .^..?`.....7..A.
-0000f4f0: 250b 790a ca84 3371 0b9a fe5d a438 b128  %.y...3q...].8.(
-0000f500: 815e 523b 87e7 388a 6ff9 6336 2721 f072  .^R;..8.o.c6'!.r
-0000f510: 1d86 9e62 c9bc 68c7 8fca 3326 3d3f a8fa  ...b..h...3&=?..
-0000f520: fdba 0b28 03c5 b495 f536 a10b e55d e8e0  ...(.....6...]..
-0000f530: ad84 9090 c014 6cfb 7bb0 0af9 3700 1dd8  ......l.{...7...
-0000f540: f7a9 a61b f553 7a25 32ec f109 e074 c956  .....Sz%2....t.V
-0000f550: e286 41a4 d2e0 fd33 2a09 8429 90ae c9da  ..A....3*..)....
-0000f560: 7010 2dc0 986b 6023 1032 b5c8 2a0d 5aaa  p.-..k`#.2..*.Z.
-0000f570: 68aa 199a 88c7 09db 43c1 1301 4699 8150  h.......C...F..P
-0000f580: d3a5 4e8b ae11 d9d3 34b9 068b 98c7 254f  ..N.....4.....%O
-0000f590: cd73 535a 9627 8a85 183d 6509 66a3 1fe1  .sSZ.'...=e.f...
-0000f5a0: f874 de86 c3c6 f570 0933 480c a3f5 f1f7  .t.....p.3H.....
-0000f5b0: f6dd 826b 3443 a380 c5c8 7a29 40bf da24  ...k4C....z)@..$
-0000f5c0: 44d8 88d3 902a 9238 cc84 e2b8 d241 a6d5  D....*.8.....A..
-0000f5d0: 4f28 cf88 7a2b 2401 fc60 0605 5e83 caa8  O(..z+$..`..^...
-0000f5e0: 858e 6d93 36ec 7685 a87b 7bef 2657 fbc7  ..m.6.v..{{.&W..
-0000f5f0: 62af 6bdd 774c ac18 2c0d eff0 e060 44cc  b.k.wL..,....`D.
-0000f600: d7b8 f832 c3bf 887f c995 3673 51fc 3713  ...2......6sQ.7.
-0000f610: bd52 c662 16d7 56aa 9ec0 7743 1e99 3998  .R.b..V...wC..9.
-0000f620: 651c 98f5 eb60 5812 0434 8edf 4200 f4f0  e....`X..4..B...
-0000f630: 253c 3c09 33d8 4d46 c56a 0d2e a630 9077  %<<.3.MF.j...0.w
-0000f640: 7832 3a3c f177 f18e 8ffb 78c7 c7a3 f1f1  x2:<.w....x.....
-0000f650: 4ede a371 1fef d178 7434 dec9 7bfc bc8f  N..q...xt4..{...
-0000f660: f7f8 f9e8 f8f9 6e9d 9ff5 4e18 9a47 f0df  ......n...N..G..
-0000f670: dfb6 020d 96a5 44bf 463d 82a8 2269 12ae  ......D.F=.."i..
-0000f680: 4d4c 45ec 6d74 b57e d111 f6ca 9217 344d  MLE.mt.~......4M
-0000f690: e69a 3a31 b11d 85d5 91be 435c 513f 21af  ..:1......C\Q?!.
-0000f6a0: c049 20f8 566b bc39 ac69 0e71 e9df a95d  .I .Vk.9.i.q...]
-0000f6b0: 4586 7abe 856c 237e cff8 62a9 bdb1 f545  E.z..l#~..b....E
-0000f6c0: 88a2 8492 3976 90a5 e921 7358 1de8 9bbb  ....9v...!sX....
-0000f6d0: 060e eb09 d51b a2d7 a4d9 a64d c16b c013  ...........M.k..
-0000f6e0: 907d a45a 7da4 72c1 53e5 c142 29fe dd83  .}.Z}.r.S..B)...
-0000f6f0: 799a d108 96b1 77e0 20e7 1027 b88b a282  y.....w. ..'....
-0000f700: 663b f586 76c9 0e47 e42e a44a f1e0 600e  f;..v..G...J..`.
-0000f710: aeae c4f6 6051 2220 f015 09ea 99bb 537b  ....`Q" ......S{
-0000f720: c37f f68f e6b2 54a6 b13e 6b22 c55d e411  ......T..>k".]..
-0000f730: 6c73 d72c 0ec0 6753 087c 5e4d f1c0 29b9  ls.,..gS.|^M..).
-0000f740: 5271 b76f 7a6a 3f00 c6a8 8e97 be88 6322  Rq.ozj?.......c"
-0000f750: c05d 24f9 744e 6013 5ba1 2d09 8084 bbd0  .]$.tN`.[.-.....
-0000f760: 762f 322c bbd6 57bf 1e2e 6bdb 1295 4bda  v/2,..W...k...K.
-0000f770: 8741 67a9 165e 6abb 3b13 b966 9b99 a012  .Ag..^j.;..f....
-0000f780: b6d2 22f7 542d 0145 73a8 22c9 580a af46  ..".T-.Es.".X..F
-0000f790: f932 53f5 dce4 d61b bed2 3279 7a38 f47b  .2S.......2yz8.{
-0000f7a0: 1da0 4754 4023 cd6f 60db ad4d 9bd0 d52c  ..GT@#.o`..M...,
-0000f7b0: a6a7 7d3b 6580 9b88 c3ed f97e 39c0 ef56  ..};e......~9..V
-0000f7c0: 7afc c594 d662 b100 2f92 2c12 124f 601e  z....b../.,..O`.
-0000f7d0: e485 2c84 b399 66ab 90e6 3117 6757 3267  ..,...f...1.gW2g
-0000f7e0: 7edb b0d5 c8a9 78c0 3cd8 ae79 34a4 7dd3  ~.....x.<..y4.}.
-0000f7f0: 5339 fa43 a7d2 1056 4dc3 5d2e e770 e282  S9.C...VM.]..p..
-0000f800: 3415 124d a0c3 2c92 1293 4a13 4ca5 a175  4..M..,...J.L..u
-0000f810: 2634 ee5e 099b 6b93 9c52 1818 fe14 41b2  &4.^..k..R....A.
-0000f820: 2690 b8e7 d482 dd74 bc3a fcb4 c242 4583  &......t.:...BE.
-0000f830: 0b7a 92d0 8841 4618 3379 c56e e134 7305  .z...AF.3y.n.4s.
-0000f840: 8705 d8ca 24d8 be9f a34a cf8e 0e2c a281  ....$....J...,..
-0000f850: ddf8 2037 dc27 2765 b276 e484 e045 2266  .. 7.''e.v...E"f
-0000f860: 3421 8de3 42d5 d93e 44d4 14f5 ac6c 6659  4!..B..>D....lfY
-0000f870: b487 0884 e764 9746 4387 20d0 3811 9ffc  .....d.FC. .8...
-0000f880: e58c 0c87 4db2 caec 2d03 5a5e c3d7 16e3  ....M...-.Z^....
-0000f890: 7704 34d0 b0a0 0dbb 5477 69df 083b 5f68  w.4.....Twi..;_h
-0000f8a0: 22ee 188f 37a7 beed c2d9 602a 31cd 4cac  "...7.....`*1.L.
-0000f8b0: f470 586b fc37 c857 c019 8a0d a624 2aa6  .pXk.7.W.....$*.
-0000f8c0: d19b 12f5 c932 c97f bd20 1cb5 00dd fe4c  .....2... .....L
-0000f8d0: 620a 5d3d c944 45df c90b 9a36 dbaa 451d  b.]=.DE....6..E.
-0000f8e0: 82da ba54 3d5b 347a 3aad 28ba 8ab5 9977  ...T=[4z:.(....w
-0000f8f0: a8e7 98bb b32d a39a 5688 c2c8 81af f7b4  .....-..V.......
-0000f900: 4423 77a8 90f2 7713 b7b5 f76d c1a3 e13d  D#w...w....m...=
-0000f910: 55e8 6558 3fdb 15c0 2f99 ce65 ba2b 8a1b  U.eX?.../..e.+..
-0000f920: 513d d1fb 0eb0 3e4f a7c7 54c7 ef62 5323  Q=....>O..T..bS#
-0000f930: 5a2c 8206 d27e 0f94 eb72 9d60 b859 6181  Z,...~...r.`.Ya.
-0000f940: 7222 b1aa 8355 4ab3 018c 08c3 e753 b77c  r"...UJ......S.|
-0000f950: e904 1f08 3ca6 bf88 2810 76ce f0cc 1c7c  ....<...(.v....|
-0000f960: 801d c83a 6c33 02f5 9509 ac00 1bee 2758  ...:l3........'X
-0000f970: 2d68 69f4 51dc b07b 2b14 b344 53b3 64b0  -hi.Q..{+..DS.d.
-0000f980: 0ae8 7564 c36e d3d1 c1df 361d d533 9fa2  ..ud.n....6..3..
-0000f990: e8d3 38e5 e569 8ca5 2f50 a71d 980d 2156  ..8..i../P....!V
-0000f9a0: 8d6c 167d 0b02 9f5a 1df1 b9d8 0937 4eeb  .l.}...Z.....7N.
-0000f9b0: a61d 671f 8858 8675 e50e 5a8e 5699 2d3c  ..g..X.u..Z.V.-<
-0000f9c0: 1b88 ec63 6ba3 2f08 30a4 5f32 9c18 d6bf  ...ck./.0._2....
-0000f9d0: bc92 3878 916a 4e13 4e15 642c e630 fb26  ..8x.jN.N.d,.0.&
-0000f9e0: a558 baa2 4ebb 39cd aa95 8043 0361 b0b4  .X..N.9....C.a..
-0000f9f0: 559f f009 4bbd 0bf3 0570 433e 713d 22cf  U...K....pC>q=".
-0000fa00: b192 104c 45c2 63cc 42fc 5ea5 4ca5 dcbb  ...LE.c.B.^.L...
-0000fa10: 28fe 54bc 25e3 846a 204c fd56 6101 0e2f  (.T.%..j L.Va../
-0000fa20: 9827 1c1e 1c98 5a94 397a db76 72bb 1f09  .'....Z.9z.vr...
-0000fa30: 9381 c162 6bf3 6c80 e787 2ecb c665 71bd  ...bk.l......eq.
-0000fa40: c72d f09d d5e5 bba6 533c 21af 255d c3ce  .-......S<!.%]..
-0000fa50: 86b5 3baa 11b0 88cb 0840 5c73 40ac 04ce  ..;......@\s@...
-0000fa60: 4249 53be 32a5 f386 0849 639e abf0 864a  BIS.2....Ic....J
-0000fa70: 4e0b a778 46be 23de 2138 12de 6804 c0eb  N..xF.#.!8..h...
-0000fa80: 39f5 c139 163b 81c0 f465 9c7c 8f48 b43c  9..9.;...e.|.H.<
-0000fa90: cdca 0449 7f3d 0029 ed11 1aa4 a539 6298  ...I.=.).....9b.
-0000faa0: c79b 24e1 1978 3e7a 4985 f47e 29ed 7b32  ..$..x>zI..~).{2
-0000fab0: 0637 77fa 367d 7db6 a1f9 522b c792 1e64  .7w.6}}...R+...d
-0000fac0: cb6a 681b da15 5e07 283c 08ff 89ee 9de8  .jh...^.(<......
-0000fad0: 3af0 2a76 ba4d d7af 68f6 5631 c6d8 104f  :.*v.M..h.V1...O
-0000fae0: 4b26 d3bb b41b e217 03a5 58a3 0a0e 6718  K&........X...g.
-0000faf0: ef57 34c1 3a79 e148 4562 4675 f33c 55e9  .W4.:y.HEbFu.<U.
-0000fb00: 8bd4 a113 75cc 04d6 3cd6 4bb3 011d 1df4  ....u...<.K.....
-0000fb10: 936e 4a52 e768 f443 9bb6 b2cd f859 273a  .nJR.h.C.....Y':
-0000fb20: b6ed d252 64bf 29a2 c6a2 a5c5 0eba 0672  ...Rd.)........r
-0000fb30: 8da6 6db6 2be4 6fb1 e01f afe5 e073 ed8c  ..m.+.o......s..
-0000fb40: 07eb ed66 3e3a 685c 3470 4512 ee5e c7fc  ...f>:h\4pE..^..
-0000fb50: 9fd9 fa0e 1b9b 02c4 d7b6 f103 4dac 45f6  ............M.E.
-0000fb60: c8f6 3d71 e859 bc95 e37f daca 21c2 f66d  ..=q.Y......!..m
-0000fb70: 5b1a 030e 4d17 1d63 3f34 683f b2f1 7b6d  [...M..c?4h?..{m
-0000fb80: fd35 61ec 3134 4217 1a9c be01 3b57 c095  .5a.14B.....;W..
-0000fb90: f11b cf3b 7916 434a 189a c4b0 38f1 a46c  ...;y.CJ....8..l
-0000fba0: 6ddf 3b77 c9c5 c57b 4550 9bc0 fc26 633e  m.;w...{EP...&c>
-0000fbb0: 9c1a 0a2b 333e 25ff aa28 ff33 6c1c 12ab  ...+3>%..(.3l...
-0000fbc0: f63b b2fc 4e7e 7846 9ad9 5499 d43a 37f8  .;..N~xF..T..:7.
-0000fbd0: 5bca 750e 054c 4264 5eb7 c8b6 ebb7 005b  [.u..LBd^......[
-0000fbe0: 68ec 6f8a 5a27 c0de 71f1 1b8b 0b8d fb2f  h.o.Z'..q....../
-0000fbf0: 4b60 c3c1 0e7e 804b 6aef 592b ab6f 01d9  K`...~.Kj.Y+.o..
-0000fc00: 9fd4 ff89 640f 92ee 6d65 7d40 da8a c07d  ....d...me}@...}
-0000fc10: 667f afdf 93d8 c561 7fd2 7105 a161 0174  f......a..q..a.t
-0000fc20: 1462 ac89 624e 1dc2 994f ef0f 3b5c 7b3e  .b..bN...O..;\{>
-0000fc30: 8583 79e7 14ed 12fc cd9c dc1f e015 0d55  ..y............U
-0000fc40: 7f6f 85ab 7dfe 40cb 698a d7e6 b610 637e  .o..}.@.i.....c~
-0000fc50: e2d2 57f8 d975 e113 839c 50d1 1b16 c229  ..W..u....P....)
-0000fc60: 74c1 ec95 4fdf b1b7 9d3f 3f9a 063d 574e  t...O....??..=WN
-0000fc70: bbc6 c75d ffd1 c6df 727b 771f 1d70 47fa  ...]....r{w..pG.
-0000fc80: 5c3d 3ab7 b883 ad23 36b7 c0cf 1d50 318d  \=:....#6....P1.
-0000fc90: 9508 1566 22cb 3377 3cfc 0c9a 9fff 020c  ...f".3w<.......
-0000fca0: 520d 1cb6 f502 789c ed58 4b6f e336 10be  R.....x..XKo.6..
-0000fcb0: eb57 10ce 2152 61e8 d64b 001f b29b b44d  .W..!Ra..K.....M
-0000fcc0: 9b87 9d35 ba47 8296 689b 8d4c 0a12 b589  ...5.G..h..L....
-0000fcd0: 51f4 bf77 48bd f890 6c2b d7d6 2791 9cf9  Q..wH...l+..'...
-0000fce0: 389c f966 3874 b02d c401 c525 db71 9221  8..f8t.-...%.q.!
-0000fcf0: 76c8 4521 d14f 4150 4fc7 a44a 9988 0b9a  v.E!.OAPO..J....
-0000fd00: 8822 f557 cba4 a094 c7e5 5ec8 01d5 1de5  .".W......^.....
-0000fd10: 32ce 0b91 24b4 2cc7 d693 3d91 78cf 4a29  2...$.,...=.x.J)
-0000fd20: 8a63 2b93 6494 14d8 5c09 8266 293f 924a  .c+.d...\..f)?.J
-0000fd30: 8a5d c582 da26 c677 58ee 0b4a 52b4 40cf  .]...&.wX..JR.@.
-0000fd40: 82d3 a0c3 af24 cbca 38dd b4a8 b5b1 ca56  .....$..8......V
-0000fd50: 9c13 b99f a392 fca0 98e4 0cbf d1e3 1c65  ...............e
-0000fd60: 82a4 fd88 2492 fd20 92e2 bfaa 5262 493f  ....$.. ....RbI?
-0000fd70: 243e 8894 6673 94d2 f135 56ba 7358 0b53  $>..fs...5V.sX.S
-0000fd80: d88c c2b6 85d8 b20c 06bb 7e70 c295 92bc  ..........~p....
-0000fd90: 51dc 5b1d 04ed d996 c795 fc39 5ec9 ef2c  Q.[........9^..,
-0000fda0: 05a4 ceb5 ab3b 4632 b19b a3d5 9f5f c4c7  .....;F2....._..
-0000fdb0: 2339 8a4a c2e0 916c 946d ab47 c6e9 7dca  #9.J...l.m.G..}.
-0000fdc0: d4d4 b22a f75f 2a29 0507 c824 2310 9e7a  ...*._*)...$#..z
-0000fdd0: f81b e169 468b 30ba 0910 fc52 ba45 1833  ...iF.0....R.E.3
-0000fde0: ce24 c661 49b3 ed1c 1d08 e3f8 9df1 54bc  .$.aI.........T.
-0000fdf0: 3742 eaa7 d6e2 2e22 108a 5f48 5652 7bd9  7B.....".._HVR{.
-0000fe00: d004 0163 648b 29c2 005f b066 9e1b db4e  ...cd.).._.f...N
-0000fe10: 52d3 15ef 6b73 fb9d 7129 4921 691a 2782  R...ks..q)I!i.'.
-0000fe20: 739a 486d 742c 38f6 24a2 4bb0 449e 9fc1  s.Hmt,8.$.K.D...
-0000fe30: d212 a358 e058 e02f e1c0 883d e36f a0e2  ...X.X./...=.o..
-0000fe40: 81f9 2217 a015 b4cc 052f 2956 ce39 9ec0  .."....../)V.9..
-0000fe50: b405 a720 8f1d 7e5c 340a 828e 3490 a2bb  ... ..~\4...4...
-0000fe60: 8cf6 9e6a c8c3 85c1 e785 e6c8 bca1 f9b1  ...j............
-0000fe70: 94f4 5007 bd5d 4805 eca2 9394 1da0 58d4  ..P..]H.......X.
-0000fe80: d340 baee 146c eb10 af27 a43e 24d8 6598  .@...l...'.>$.e.
-0000fe90: 10d9 8ba7 194b 6160 a35d a135 186a 5411  .....Ka`.].5.jT.
-0000fea0: b4a1 5b51 c08c 2294 c2e8 d02c 3d30 9283  ..[Q.."....,=0..
-0000feb0: b075 741b 599b d3c3 2efa 2217 f7d3 60fe  .ut.Y....."...`.
-0000fec0: 09a5 58b9 2974 2a9c a3e1 1fdf b209 f6b5  ..X.)t*.........
-0000fed0: c681 2fef 450a 74bc 395f cd89 2328 3933  ../.E.t.9_..#(93
-0000fee0: f656 bb4c 6ce0 2a72 ebbb eb54 affe b352  .V.Ll.*r...T...R
-0000fef0: 1709 240a ed70 773d 86e2 4c32 a8c5 61e4  ..$..pw=..L2..a.
-0000ff00: bb7f e032 a93f 54ca aef5 5708 6186 6abb  ...2.?T...W.a.j.
-0000ff10: d0e1 ee69 0557 45b1 2b17 a1e7 8779 149d  ...i.WE.+....y..
-0000ff20: dd26 d660 2e33 cfd5 367a 601d 1d54 b20d  .&.`.3..6z`..T..
-0000ff30: 9537 9d70 a70a f4ba a8c6 eb73 5ce5 a9ba  .7.p.......s\...
-0000ff40: e000 4cd2 f05a 924c 15a6 eb68 6c4b 9dff  ..L..Z.L...hlK..
-0000ff50: ee96 79c1 b80c 672f cfe8 f5fe ebcb ebdd  ..y...g/........
-0000ff60: c3f3 afe8 dbfa 65b9 bcbf 9b45 9fbd 395c  ......e....E..9\
-0000ff70: cb9a 9a79 1d79 4561 f01e 7138 322a 384a  ...y.yEa..q82*8J
-0000ff80: 96f3 05be 898e 9705 23f7 da18 cd2c f196  ........#....,..
-0000ff90: 649d cd56 a6ce 8793 733e 987d d185 a675  d..V....s>.}...u
-0000ffa0: d434 aaba ee6d 8c92 e404 bcfb 701a 97d0  .4...m......p...
-0000ffb0: 89f6 273d d103 5e80 679a 6f1e e1e4 0d36  ..'=..^.g.o....6
-0000ffc0: 9834 e3e4 6340 81eb 6804 bbe5 c344 4c83  .4..c@..h....DL.
-0000ffd0: d067 6cd6 37fa 54f4 2e91 4d9f 406b aaee  .gl.7.T...M.@k..
-0000ffe0: af12 e722 af72 17f2 0a7d 85ad 2445 a413  ...".r...}..$E..
-0000fff0: 44a9 6e34 1124 0162 bc64 2924 d416 3168  D.n4.$.b.d)$..1h
-00010000: dc5b 49d5 00c3 525e 4944 36d0 8622 9153  .[I...R^ID6..".S
-00010010: 4e58 db5f 6b4d 8236 bae7 8466 41b7 e200  NX._kM.6...fA...
-00010020: 609c a331 a9d9 69d1 36b7 1697 2c99 18c6  `..1..i.6...,...
-00010030: dff5 a1d7 4c66 349c 7d6b d667 17a8 3c89  ....Lf4.}k.g..<.
-00010040: 14d2 5d1e c395 8c6f f33c 6309 914c 703d  ..]....o.<c..Lp=
-00010050: 6d5c a303 fa75 9b1d 1a2d 7718 8d6f 9835  m\...u...-w..o.5
-00010060: 1231 49d3 ba7b 0feb fe1c ea24 78e8 f601  .1I..{.....$x...
-00010070: dd2e 1fd0 1ff4 3833 401a a7e1 da9f 8bbe  ......83@.......
-00010080: 930f 3d19 5835 df31 be40 0da2 0c5f 4388  ..=.X5.1.@..._C.
-00010090: c266 7692 c116 92a1 a94a 4c13 d185 f9c4  .fv......JL.....
-000100a0: 8048 c0d2 6c50 324e c0d5 6f46 9b99 91c3  .H..lP2N..oF....
-000100b0: 2625 37d6 dbcc de31 56dc 021f 4fb2 d9d8  &%7....1V...O...
-000100c0: d208 e715 ba4d 8187 5055 f7b4 30d8 0839  .....M..PU..0..9
-000100d0: 4625 3ad0 837a 79b6 c27a 12d7 9323 e77c  F%:..zy..z...#.|
-000100e0: d57a 4f5a c438 ef80 a677 6eff c93b e97c  .zOZ.8...wn..;.|
-000100f0: 035b 5c70 4e48 c94d 4675 59af 3356 3f59  .[\pNH.MFuY.3V?Y
-00010100: 3bb5 fe29 3b7c dcfb 5afd 77a5 aed8 849e  ;..);|..Z.w.....
-00010110: 94fa ec44 be0c 58ee 6e12 59ed fde8 83da  ...D..X.n.Y.....
-00010120: bd97 5d98 8ee1 b33b 568e 9879 52df 0dd0  ..]....;V..yR...
-00010130: f8b3 bf07 f21f 0d67 61c7 418d f075 65b5  .......ga.A..ue.
-00010140: ae00 f0ea 38e8 0aaa ab66 1f4e 600f 87f6  ....8....f.N`...
-00010150: bafd 6361 4210 da1a b4ac 55cd e2d3 a00d  ..caB.....U.....
-00010160: 169f 61a1 cef5 c6bf 1c13 6ba2 85e7 db72  ..a.......k....r
-00010170: 79a9 19d0 182f 3986 b9f6 813e 5371 0676  y..../9....>Sq.v
-00010180: ee7a a921 08fa 4113 7cea 76db 8b77 bb1b  .z.!..A.|.v..w..
-00010190: d3b6 69ca 34af 6bf5 39d4 8efd e77b 68e5  ..i.4.k.9....{h.
-000101a0: 98ee 9da6 be3f d104 fb5e 773b 612f 0093  .....?...^w;a/..
-000101b0: def4 13df f2ff 0777 3cb8 73f4 f6ae c77f  .......w<.s.....
-000101c0: cf1c 2fce 6e9c 897f 2612 c18e c1f8 ef5f  ../.n...&......_
-000101d0: be3c b3fb b13a 789c 7d53 5d6f d430 107c  .<...:x.}S]o.0.|
-000101e0: f7af 30ee 432f 281f 952a 108a 6444 250a  ..0.C/(..*..dD%.
-000101f0: 42a2 2a82 f601 5528 7293 bd9c b9c4 36de  B.*...U(r.....6.
-00010200: 35ed 81f8 eff8 9c0b a855 eff2 e087 99f1  5........U......
-00010210: eeec ac73 f4ac 0ae8 ab5b 6d2a b7a1 9535  ...s.....[m*...5
-00010220: a7ec 8817 cf0b deda 4e9b bee6 8196 c5ab  ........N.......
-00010230: 2dc2 d8d2 db91 2350 7064 ed80 5c8f ce7a  -.....#Ppd..\..z
-00010240: 9a10 c6ee 34ad b875 6016 c71e 7e04 ed61  ....4..u`...~..a
-00010250: 0443 58d2 3d1d 675c 215f ba9a f1f8 6983  .CX.=.g\!_....i.
-00010260: a486 a1d9 a990 cb48 951e 54b7 c858 2ab6  .......H..T..X*.
-00010270: 483a a346 90a2 77d4 b476 7481 c037 0a51  H:.F..w..vt..7.Q
-00010280: c7cb 8644 9e24 3fc1 a3b6 468a 93f2 4579  ...D.$?...F...Ey
-00010290: ba03 3bc0 d66b 4789 10e2 fda7 ab78 4ed4  ..;..kG......xN.
-000102a0: 604d df3c e4cb ef56 9b45 f22d 3e9f 9fbd  `M.<...V.E.->...
-000102b0: bd38 2fc7 4ee4 1ccc 9480 1429 0191 2587  .8/.N......)..%.
-000102c0: 8336 808b 2c7b ba5c 346a 280e ddd0 c645  .6..,{.\4j(....E
-000102d0: eb04 f754 8dca af3b 7b67 760e 821f a458  ...T...;{gv....X
-000102e0: 1139 acab aa8f 9185 db32 8e57 5913 bc22  .9.......2.WY.."
-000102f0: b556 a68a 1317 f3c4 c5e3 8955 884b f252  .V.........U.K.R
-00010300: 5c46 3d3f 4b17 f8f5 c7eb 2f97 5f1f 081a  \F=?K...../._...
-00010310: 1895 8e9d 62c9 cef6 ca9c bc7c d36f 916d  ....b......|.o.m
-00010320: af39 0bdd 82c1 68f3 e2c3 d50e 72aa 5dab  .9....h.....r.].
-00010330: 1e50 deec 8d9d ef61 ca78 ef20 df07 7d80  .P.....a.x. ..}.
-00010340: 8d11 0298 0382 407a c043 ed43 a7ad f896  ......@z.C.C....
-00010350: 3ff9 c2e4 6360 9245 c37e d3b8 b87f 42f9  ?...c`.E.~....B.
-00010360: 3b41 db4f c42d a21d a099 f68a a2e6 3762  ;A.O.-........7b
-00010370: 6ef9 afa3 dc37 0929 4f75 3a67 3b7f f2a9  n....7.)Ou:g;...
-00010380: f094 71fa cbfe 5b13 af25 9f5f ee2f ed1a  ..q...[..%._./..
-00010390: 544b 90ef d480 90b3 8c31 f617 ed83 3928  TK.......1....9(
-000103a0: 6c82 4c78 9c5b c8be 907d c269 4693 8d67  l.Lx.[...}.iF..g
-000103b0: ae32 0100 2059 0535 6c18 789c 5bc8 be90  .2.. Y.5l.x.[...
-000103c0: 7dc2 6946 d38d 67ae 3201 0020 5e05 366c  }.iF..g.2.. ^.6l
-000103d0: 1778 9c5b c8be 907d c269 46b3 8d67 ae32  .x.[...}.iF..g.2
-000103e0: 0100 2063 0537 6e17 789c 5bc8 be90 7dc2  .. c.7n.x.[...}.
-000103f0: 4966 333d 838d 67ae 3201 0028 2b05 95b1  If3=..g.2..(+...
-00010400: 0378 9c4b 2bca cf55 d02b 2e49 2c2a 51c8  .x.K+..U.+.I,*Q.
-00010410: cc2d c807 5260 0e17 1757 7c7c 596a 5171  .-..R`...W||YjQq
-00010420: 667e 5e7c bc82 ad82 ba81 9ea9 9e99 3a17  f~^|..........:.
-00010430: 00b2 240f a6e0 03bc 1978 9c3b c874 9049  ..$......x.;.t.I
-00010440: ddd0 c0c0 ccc4 4421 3e3e 332f b324 3e5e  ......D!>>3/.$>^
-00010450: afa0 92e1 a764 63eb 611f 41d1 1a47 a9c3  .....dc.a.A..G..
-00010460: 8b2f be5c e212 927e 71a3 ba14 2300 9379  ./.\...~q...#..y
-00010470: 11ef e003 b93e 789c 3bc8 7490 49dd d0c0  .....>x.;.t.I...
-00010480: c0cc c444 213e 3e33 2fb3 243e 5eaf a092  ...D!>>3/.$>^...
-00010490: a1c0 6959 40f5 eeb3 a97b 5a7f cf6e 53bb  ..iY@....{Z..nS.
-000104a0: 9bf1 4af9 53c0 4675 2946 00a9 d913 5ee0  ..J.S.Fu)F....^.
-000104b0: 03b9 7b78 9c3b c874 9049 ddd0 c0c0 ccc4  ..{x.;.t.I......
-000104c0: 4421 3e3e 332f b324 3e5e afa0 9261 55ce  D!>>3/.$>^...aU.
-000104d0: aa94 b867 b94d 0a4f 3add f2a6 46c4 6cd1  ...g.M.O:...F.l.
-000104e0: 58f3 62a3 ba14 2300 a037 1288 ee01 7a78  X.b...#..7....zx
-000104f0: 9c3b c874 9069 82b1 4890 f894 62ad 76c7  .;.t.i..H...b.v.
-00010500: a6cb 5137 dcdf 2cba eb7a 61e2 e5c0 89ee  ..Q7..,..za.....
-00010510: bf00 c4f6 0e95 e003 2a78 9c3b c874 9049  ........*x.;.t.I
-00010520: ddd0 c0c0 ccc4 4421 3e3e 332f b324 3e5e  ......D!>>3/.$>^
-00010530: afa0 92a1 acbd f8fd 94b9 0922 8dd9 bfa5  ..........."....
-00010540: 3afe bebc 50fe 397e db46 7529 4600 ae4a  :...P.9~.Fu)F..J
-00010550: 13f9 e003 b87a 789c 3bc8 7490 49dd d0c0  .....zx.;.t.I...
-00010560: c0cc c444 213e 3e33 2fb3 243e 5eaf a092  ...D!>>3/.$>^...
-00010570: c174 45e8 dcbe fee6 096d a7f7 5618 2d9d  .tE......m..V.-.
-00010580: c37b 9f2f fadb 4675 2946 009e d512 7ab1  .{./..Fu)F....z.
-00010590: 0378 9c4b 2bca cf55 d02b 2e49 2c2a 51c8  .x.K+..U.+.I,*Q.
-000105a0: cc2d c807 5260 0e17 1757 7c7c 596a 5171  .-..R`...W||YjQq
-000105b0: 667e 5e7c bc82 ad82 ba81 9ea9 9ea9 3a17  f~^|..........:.
-000105c0: 00b2 210f a5b1 0378 9c4b 2bca cf55 d02b  ..!....x.K+..U.+
-000105d0: 2e49 2c2a 51c8 cc2d c807 5260 0e17 1757  .I,*Q..-..R`...W
-000105e0: 7c7c 596a 5171 667e 5e7c bc82 ad82 ba81  ||YjQqf~^|......
-000105f0: 9ea9 9e89 3a17 00b2 1e0f a4b1 0378 9c4b  ....:........x.K
-00010600: 2bca cf55 d02b 2e49 2c2a 51c8 cc2d c807  +..U.+.I,*Q..-..
-00010610: 5260 0e17 1757 7c7c 596a 5171 667e 5e7c  R`...W||YjQqf~^|
-00010620: bc82 ad82 ba81 9ea9 9eb1 3a17 00b2 1b0f  ..........:.....
-00010630: a33a 35c2 c647 a516 5f74 8dd8 be98 12ee  .:5..G.._t......
-00010640: 6b1c 397b eb                             k.9{.
+0000d6b0: 78e9 000e de91 0e78 9c8d cb4d 0ec2 2010  x......x...M.. .
+0000d6c0: 40e1 3da7 98bd 49c3 5004 9a18 1375 a1d7  @.=...I.P....u..
+0000d6d0: e067 b02c 0a86 4eeb f5ed 117c ebf7 7127  .g.,..N....|..q'
+0000d6e0: 82e8 5c18 4713 bd76 3ab8 8c78 5653 226d  ..\.G..v:..xVS"m
+0000d6f0: 9323 8cda 1be7 6dd2 64cf e2e3 3b55 0613  .#....m.d...;U..
+0000d700: 42b6 4432 e61c 485a 9d25 86a8 4c1a 53c2  B.D2..HZ.%..L.S.
+0000d710: 09bd c92a 7999 330a bff1 dc3a 3c0b bfb6  ...*y.3....:<...
+0000d720: 00b7 c8a5 d515 ee8d e172 05b4 68d5 a4ad  .........r..h...
+0000d730: 7470 9247 22b6 6529 ccf4 3710 8fd9 d737  tp.G".e)..7....7
+0000d740: 25d8 a9af c709 755b c2c1 bf85 67d8 e560  %.....u[....g..`
+0000d750: 0614 3faa 9f43 0991 0e78 9c8d 8b39 0ec2  ..?..C...x...9..
+0000d760: 3010 007b bf62 7ba4 c807 b663 0921 0105  0..{.b{....c.!..
+0000d770: 7c63 bd5e 488a c4c8 d984 ef13 7ec0 4c3b  |c.^H.......~.L;
+0000d780: 238d 198a 37c1 39f3 b45c b037 da17 768e  #...7.9..\.7..v.
+0000d790: 2986 a32b 3622 924e 7d64 938b 7a63 e359  )..+6".N}d..zc.Y
+0000d7a0: c01a f2d1 5be7 8910 f7b4 8454 a24f 444c  ....[......T.ODL
+0000d7b0: f927 7bb2 2660 50b8 ca50 1bdc 4779 ac19  .'{.&`P..P..Gy..
+0000d7c0: 2e24 639d 17b8 5681 d319 4c34 21f5 3ad9  .$c...V...L4!.:.
+0000d7d0: 0407 bda3 a84e d328 c27f 0fea 36e0 fce2  .....N.(....6...
+0000d7e0: 021b b765 2f61 5ea7 bcef 9f51 06d8 7417  ...e/a^....Q..t.
+0000d7f0: 3aad be74 8242 ce91 0e78 9c8d cb4d 0e82  :..t.B...x...M..
+0000d800: 3010 40e1 7d4f 317b 13d2 ffd2 c498 a80b  0.@.}O1{........
+0000d810: bdc6 b433 0a0b 8a81 01af 2f47 f0ad df27  ...3....../G...'
+0000d820: 0b33 30f9 1766 ab5f d696 88b5 8650 7324  .30..f._.....Ps$
+0000d830: 6fb2 27a3 535f 9873 491a 83fa e0c2 4dc0  o.'.S_.sI.....M.
+0000d840: f4c1 91f3 9112 9276 44c5 ea12 7576 6c6b  .......vD...uvlk
+0000d850: 42c3 d4a3 c364 8b55 b8c9 302f f018 e5b9  B....d.U..0/....
+0000d860: 15b8 5619 e7b6 c26d 1638 5fc0 2413 73ca  ..V....m.8_.$.s.
+0000d870: d61b 38e9 2355 e769 1a45 f86f a0ee 03b6  ..8.#U.i.E.o....
+0000d880: 3713 ecbc acc7 096d 9bca c1bf a30c b0eb  7......m........
+0000d890: 2e74 51fd 0034 fd42 3791 0e78 9c8d 8d41  .tQ..4.B7..x...A
+0000d8a0: 0ec2 2010 00ef bc62 ef26 0d2c a52c 8931  .. ....b.&.,.,.1
+0000d8b0: 510f fa0d a08b eda1 ada1 5bfd be3c c139  Q.........[..<.9
+0000d8c0: cf64 a432 03c6 1eb1 7049 4153 f6ce 8571  .d.2....pIAS...q
+0000d8d0: c4e2 cd40 5cb2 f594 c893 4b71 40f5 8e95  ...@\.....Kq@...
+0000d8e0: 5701 a3d1 1987 269b 1c42 f11e 2da5 9e06  W.....&..B..-...
+0000d8f0: 6d13 eb1e 5374 8436 9a40 2a1e 326d 151e  m...St.6.@*.2m..
+0000d900: b33c 8f04 d72c f3b6 ee70 db04 ce17 30ed  .<...,...p....0.
+0000d910: 107c d096 e0a4 1b2a 6fcb 328b f0df 81ba  .|.....*o.2.....
+0000d920: 4f71 7df1 081f ae7b 3361 3d96 d4f2 ef2c  Oq}....{3a=....,
+0000d930: 137c 74e7 3aa7 7e3c 0640 b391 0e78 9c8d  .|t.:.~<.@...x..
+0000d940: cb4d 0e82 3010 40e1 7d4f 317b 1332 ed50  .M..0.@.}O1{.2.P
+0000d950: da26 c644 5de8 35fa 3315 1614 0383 5e5f  .&.D].5.3.....^_
+0000d960: 8ee0 5bbf 4f56 6640 8ec8 e423 eae4 83f5  ..[.OVf@...#....
+0000d970: b5a6 5c4d 7031 3a47 5c2b d360 88fa 82ea  ..\Mp1:G\+.`....
+0000d980: 1d57 6e02 96bd b709 5309 58a2 cf48 3438  .Wn.....S.X..H48
+0000d990: caa6 d4cc 9a7a 2ece 629f 4c0e 2aee 322e  .....z..b.L.*.2.
+0000d9a0: 2b3c 2679 ee09 ae59 a6a5 6d70 5b04 ce17  +<&y...Y..mp[...
+0000d9b0: d04e 0fc1 79ab 039c f048 e565 9e27 11fe  .N..y....H.e.'..
+0000d9c0: 1ba8 fb18 db8b 0b7c 78dd 8e13 da3e a783  .......|x....>..
+0000d9d0: 7f27 19e1 839d ed7a f503 4877 4257 910e  .'.....z..HwBW..
+0000d9e0: 789c 8d8b 390e c230 1000 7bbf 627b a468  x...9..0..{.b{.h
+0000d9f0: 6de3 4b42 4840 01df f0da 1b92 220e 4a36  m.KBH@......".J6
+0000da00: e1fb e409 4c33 cd8c 2ccc 50d9 628f 648b  ....L3..,.P.b.d.
+0000da10: d367 4368 cf2e 5266 d487 c8a7 8c48 64aa  .gCh..Rf.....Hd.
+0000da20: 0ba4 3e79 e126 10b8 f698 3ce5 925c c4a0  ..>y.&....<..\..
+0000da30: 73aa 39f5 2646 e38d d626 a4be fa42 a9aa  s.9.&F...&...B..
+0000da40: bcc9 302f f01c e5b5 11dc 8a8c 735b e13e  ..0/........s[.>
+0000da50: 0b5c aea0 83f6 2944 eb1d 9cf0 4095 799a  .\....)D....@.y.
+0000da60: 4611 fe7b 508f 21b7 3757 d879 598f 12da  F..{P.!.7W.yY...
+0000da70: 36d1 b17f 4719 60c7 ce75 56fd 00f5 c141  6...G.`..uV....A
+0000da80: ea9c 0d78 9c9d cbbb 0ac2 3014 00d0 3d5f  ...x......0...=_
+0000da90: 915d 909b 47f3 0011 2727 a183 7470 bcb9  .]..G...''..tp..
+0000daa0: b9a9 01db 4a48 c1cf d76f 703d 707a 6396  ....JH...op=pzc.
+0000dab0: 8e6c 34ca ea94 3cc5 60a9 1867 29a5 8c21  .l4...<.`..g)..!
+0000dac0: 98ac 21a2 07ad 1c93 7863 e3b5 cb41 1115  ..!.....xc...A..
+0000dad0: 4550 520c 51e5 21da 62b3 f681 0850 272e  EPR.Q.!.b....P'.
+0000dae0: 1038 e7c2 41e0 de9f 5b93 e3ba 3739 dda6  .8..A...[...79..
+0000daf0: fbf8 9027 ec98 b719 5770 9779 c1fa 3ad2  ...'....Wp.y..:.
+0000db00: b69c a5f2 caeb 689d 33f2 0006 40fc 74a9  ......h.3...@.t.
+0000db10: bdf3 7f5b 5ceb 477c 0186 2741 2f9a 4178  ...[\.G|..'A/.Ax
+0000db20: 9c75 93c7 b2a3 5600 44f7 7cc5 dd53 1e32  .u....V.D.|..S.2
+0000db30: 975b 3576 0d49 04f1 8842 20ed c841 2421  .[5v.I...B ..A$!
+0000db40: 82c4 d7cf b3bd b57b d7a7 aaab 37dd cb5c  .......{....7..\
+0000db50: 1480 4434 c596 4cc2 2488 a1d3 a464 d80c  ..D4..L.$....d..
+0000db60: e68c 4025 2c4f 931c 9b16 392d 7008 216c  ..@%,O....9-p.!l
+0000db70: 4ae6 6258 002c 849c a128 9282 7c21 d06c  J.bX.,...(..|!.l
+0000db80: 4af1 df26 2dc8 9445 28a1 4ac8 413a 2f59  J..&-..E(.J.A:/Y
+0000db90: 96c4 9275 a9c7 1938 c33a 83d0 0a03 e706  ...u...8.:......
+0000dba0: 7e26 4b92 8f55 3290 fcaf aa4f 9aee 4736  ~&K..U2....O..G6
+0000dbb0: f67f 010a 5290 1648 16b1 0027 1992 c4be  ....R..H...'....
+0000dbc0: 69df 2c4b 3103 ad59 f435 053f 8771 2ea6  i.,K1..Y.5.?.q..
+0000dbd0: eef3 ab6a 967a 4dff 2756 4dd5 aba9 c01f  ...j.zM.'VM.....
+0000dbe0: 7f4b 5235 c306 aee6 82c0 d06c f112 faea  .KR5.......l....
+0000dbf0: 3f1c 0318 d85f a74c 1245 4916 454f f2cc  ?...._.L.EI.EO..
+0000dc00: 3ee2 e02a fb32 9578 705d b9b0 ee44 519c  >..*.2.xp]...DQ.
+0000dc10: fc97 27aa 692f 1dc2 0352 4bcc fb90 8e02  ..'.i/...RK.....
+0000dc20: e91a b4de 0d03 4def e9de 98cd ba81 b6b3  ......M.........
+0000dc30: 976c 5b49 370f df7f acd9 0d9e a4ea 61c6  .l[I7.........a.
+0000dc40: e5cc 7bf4 a34a 048e 5688 c699 a033 062a  ..{..J..V....3.*
+0000dc50: d7ce e8d8 95f2 8981 4ce0 9c93 f23e 0dac  ........L....>..
+0000dc60: ff89 a08b 1f1b a7d9 c720 9573 f521 83b4  ......... .s.!..
+0000dc70: d1ae f7c9 eab5 d3f6 2cb8 faca f78f e108  ........,.......
+0000dc80: acd7 f615 eb75 eea0 d6c7 0093 42b4 cd19  .....u......B...
+0000dc90: d977 d76d f69a cdb4 2fc5 802e f48a e342  .w.m..../......B
+0000dca0: 6059 bdd2 5966 7d2e 508b 76a2 6bb9 6e42  `Y..Yf}.P.v.k.nB
+0000dcb0: fe5b f0a4 61fb 2eec 3422 c580 1692 8e62  .[..a...4".....b
+0000dcc0: d816 c529 8ae9 98ef 8452 c64b ac14 6970  ...).....R.K..ip
+0000dcd0: 396e 77a6 37af 2796 4b1d bb8d afec 221b  9nw.7.'.K.....".
+0000dce0: 9def 3dc3 dbdd 3b59 82e3 6af0 a662 a06e  ..=...;Y..j..b.n
+0000dcf0: 71fe b9f5 ddb6 2cc1 5887 f711 3eef 5d6b  q.....,.X...>.]k
+0000dd00: 9891 b9c4 f7b6 41a3 6b98 f37d 1999 c6ca  ......A.k..}....
+0000dd10: e05b 7fb3 cbbe a565 e120 cd7b bdda 21c7  .[.....e. .{..!.
+0000dd20: 4044 3f24 e3e2 8e9d 66b7 435c ee63 2543  @D?$....f.C\.c%C
+0000dd30: fe3c 8491 a2da 7bc2 7b8b 2e96 04b2 edce  .<....{.{.......
+0000dd40: 2888 8927 63c4 4fa5 f3d0 28fe 36c6 8332  (..'c.O...(.6..2
+0000dd50: b018 b0a7 a7f3 d634 853c a50f 5add 5d5c  .......4.<..Z.]\
+0000dd60: b8b3 6582 3289 9f55 a3ab 3f6a 8fde 6d85  ..e.2..U..?j..m.
+0000dd70: 5f79 b997 a9a3 4477 c725 3fbb 7cec 1c69  _y....Dw.%?.|..i
+0000dd80: b0af 4dc4 8079 64b4 e2ae 78c2 9934 42bc  ..M..yd...x..4B.
+0000dd90: 6031 ba22 be4c 7990 1745 8391 2d3f e4a2  `1.".Ly..E..-?..
+0000dda0: c8bd a266 65bc 49da 54f5 6267 8e9f 7242  ...fe.I.T.bg..rB
+0000ddb0: 2653 46b9 0106 749e 24fa 0f55 44cf 238c  &SF...t.$..UD.#.
+0000ddc0: bff6 b6d7 de78 8497 4aee b4eb 3538 9f9b  .....x..J...58..
+0000ddd0: e2bd a6bb ccb1 37af 9e74 5cbf 5ed4 1bb1  ......7..t\.^...
+0000dde0: e2fe 27a0 10e9 12df 7ba8 56a3 4a23 2237  ..'.....{.V.J#"7
+0000ddf0: 0273 ac42 d9d6 394a 69e1 8ac8 fc3e e039  .s.B..9Ji....>.9
+0000de00: ffd5 8b81 7640 ffc8 0fc3 4f2b ef1c 3496  ....v@....O+..4.
+0000de10: f788 dcad aa75 3d5c 720f 0325 541d 331a  .....u=\r..%T.3.
+0000de20: 1af6 4cbc 5867 22f4 7733 60e0 cf88 1432  ..L.Xg".w3`....2
+0000de30: ecdf 4fa8 b6f2 df8f c0c2 294f 9602 f8aa  ..O.......)O....
+0000de40: a87c a93f fafc 37bb 5845 999a 4178 9c75  .|.?..7.XE..Ax.u
+0000de50: 93c9 cea3 4600 84ef 3c45 dfad 8cbb 591b  ....F...<E....Y.
+0000de60: 6912 0d60 dcc0 6f30 60f0 c2ad 59cc 6236  i..`..o0`...Y.b6
+0000de70: b3d8 e0a7 9f3f c935 a953 e993 ea50 25d5  .....?.5.S...P%.
+0000de80: 3464 19e0 d93b 8fa8 8421 4bb9 4cfa 3602  4d...;...!K.L.6.
+0000de90: 8d29 ca30 8448 a631 9632 294d 7829 bd33  .).0.H.1.2)Mx).3
+0000dea0: 3d1d b276 0229 2bd0 7b2a 8990 6539 9ee5  =..v.)+.{*..e9..
+0000deb0: 29cd d05d a609 14e3 84bd 4b19 cfa7 09e6  )..]......K.....
+0000dec0: 3984 183a 4f45 3780 633b 0f20 3c84 a7e3  9..:OE7.c;. <...
+0000ded0: 0dfc a413 4dbb 9cb6 50fc 9537 b4ac 7f24  ....M...P..7...$
+0000dee0: 5df3 1740 1292 580c 395e 061b c841 c87c  ]..@..X.9^...A.|
+0000def0: d3a6 9ca6 6c00 a49c 8c39 063f db6e c8fa  ....l....9.?.n..
+0000df00: 7afd 9597 5331 c7ff 13cb fb7c 2c73 f0c7  z...S1.....|,s..
+0000df10: df52 7562 3ac0 252e 3899 c451 82d0 d7ff  .Rub:.%.8..Q....
+0000df20: e10c 60c0 7bdc 27aa a2a8 9aa2 78aa 6735  ..`.{.'.....x.g5
+0000df30: 1741 4835 5f43 d493 e659 088b 5a51 94bb  .AH5_C...Y..ZQ..
+0000df40: 917b 8a19 e544 74bd 5897 0f0f 575f 0a7a  .{...Dt.X...W_.z
+0000df50: 6be1 45d1 1850 05cb 7628 0c3f 5016 180c  k.E..P..v(.?P...
+0000df60: 82f3 884b 8f0e 317e 6075 bd89 8696 e8c9  ...K..1~`u......
+0000df70: e779 ae90 8b8e d2d4 056b 3468 6aaf a7de  .y.......k4hj...
+0000df80: 1692 1d86 fa89 010f a178 1401 0c4a eb55  .........x...J.U
+0000df90: 25fe 4aac 0717 7f5d bc59 1497 fe36 b59b  %.J....].Y...6..
+0000dfa0: c3db b256 be42 cdd0 9edc 66bf f676 cfb5  ...V.B....f..v..
+0000dfb0: 5371 a6c3 58db 96b0 6500 e1fd 67a8 f0f2  Sq..X...e...g...
+0000dfc0: d587 6637 ce66 c435 5262 0631 516b e595  ..f7.f.5Rb.1Qk..
+0000dfd0: 605d bc48 e47c 5d62 2910 dd2d 39d7 917d  `].H.|]b)..-9..}
+0000dfe0: ddec 9bcf f06e e995 df86 1103 585c 7c9a  .....n......X\|.
+0000dff0: 7573 09ea 2a60 b376 c163 f2fe b0fb cfae  us..*`.v.c......
+0000e000: 4e8c d986 9dae 3766 7e66 bdbd 4b02 b83b  N.....7f~f..K..;
+0000e010: 2cdf ada3 4f75 a45f 66f8 454b 6831 a03d  ,...Ou._f.EKh1.=
+0000e020: 1c49 c91a ecaa 732f 4fbe 5acd 5dfb a8fb  .I....s/O.Z.]...
+0000e030: 87c2 d57b f16a b6a2 3bb1 fb43 56a2 ce28  ...{.j..;..CV..(
+0000e040: c7a5 dca2 a83c 5929 da10 e4d9 ef69 243e  .....<Y).....i$>
+0000e050: 0326 b7e6 03f2 e8d6 b452 4eb7 20a1 519b  .&.......RN. .Q.
+0000e060: 1ee7 b9e0 705a 9df5 f1d3 22d9 ed33 01d5  ....pZ...."..3..
+0000e070: 0aea 137c f136 5638 4b8a 8494 a9bf 88f4  ...|.6V8K.......
+0000e080: 6433 60a9 6c8b 2b65 785d a18c 49bf 18c8  d3`.l.+ex]..I...
+0000e090: 2a4f 2a72 841a 59d9 41c2 2c56 549c dbd6  *O*r..Y.A.,VT...
+0000e0a0: e234 8a41 cded 7c14 7832 1dee abb1 bd66  .4.A..|.x2.....f
+0000e0b0: eb13 33a0 bf1f d1b8 333e b7f5 dc8c c47d  ..3.....3>.....}
+0000e0c0: 0656 e569 6779 ffd0 16f7 cbd8 0e46 0cb9  .V.igy.......F..
+0000e0d0: dce9 2f86 c377 5af5 5e4f 4ff8 8cee be19  ../..wZ.^OO.....
+0000e0e0: d4a2 7123 2464 003e b942 9bbe f07b d41c  ..q#$d.>.B...{..
+0000e0f0: 3338 1c35 474a 5ff9 73a6 bd6e 1f87 b3f6  38.5GJ_.s..n....
+0000e100: f5bd de47 68cc 2b71 1dde 57b3 e19e d77d  ...Gh.+q..W....}
+0000e110: c96f e7c8 b961 124d 0cb8 f559 6054 ee61  .o...a.M...Y`T.a
+0000e120: d755 5f88 e3d7 cf5a ecdb 71e7 cfce 39ba  .U_....Z..q...9.
+0000e130: 465d 24bd d0f8 b8a8 15ee 5ab2 dd6c ec22  F]$.......Z..l."
+0000e140: ace4 bacc bc23 3ddb 094c 3c06 58d8 e254  .....#=..L<.X..T
+0000e150: f625 20ef 5550 b2cf e78d f164 c09f b3cc  .% .UP.....d....
+0000e160: de98 7f3f a13b bbff 7e04 13f6 299d 32e0  ...?.;..~...).2.
+0000e170: ebca ced6 7f34 e96f c7b1 4656 9a41 789c  .....4.o..FV.Ax.
+0000e180: 7553 c90e aa48 00bc f315 7d37 f364 916e  uS...H....}7.d.n
+0000e190: 48de 4c1e bb80 a2ec e28d 6647 6991 45d0  H.L.......fGi.E.
+0000e1a0: af7f cecc 75a6 8e95 546a 496a 1a8a 0240  ....u...TjIj...@
+0000e1b0: 9ca5 82c0 d225 cd15 2986 1016 39cd 4048  .....%..)...9.@H
+0000e1c0: 639a e144 888b 1d16 732c f088 ead3 a120  c..D....s,..... 
+0000e1d0: 1328 7804 315b 423a 1784 e22b e158 94e7  .(x.1[B:...+.X..
+0000e1e0: 5cc1 0a05 e4d3 92e1 5996 1172 5a64 a874  \.......Y..rZd.t
+0000e1f0: 9eea c700 4e64 1e40 7808 fd53 027e a653  ....Nd.@x..S.~.S
+0000e200: 9a3f aa94 d0f0 57d5 a5cd fd47 f6e8 fe02  .?....W....G....
+0000e210: 0c62 104d 3388 4360 4373 344d 7dd9 ae99  .b.M3.C`Cs4M}...
+0000e220: a662 0046 33ed 670c 7e92 c750 f4f7 f7af  .b.F3.g.~..P....
+0000e230: aa99 ea19 ff8f acea abb1 a9c0 1f7f 43d6  ..............C.
+0000e240: 0cd3 0167 e30c 7cd3 70a4 20f4 b47f 780a  ...g..|.p. ...x.
+0000e250: 5060 19f5 4c96 2459 9124 5776 ad2e 6276  P`..L.$Y.$Wv..bv
+0000e260: 96e2 294c eaa2 79e6 c3fa 2e49 5298 3c5c  ..)L..y....IR.<\
+0000e270: 499d 04a5 bb27 6fa8 268f f530 859c 9a39  I....'o.&..0...9
+0000e280: f87e a3c0 b10f 768e 6378 0dd4 8dd4 3d6d  .~....v.cx....=m
+0000e290: e096 be96 e4ba 439e db2a deaa 0a5a 1a54  ......C..*...Z.T
+0000e2a0: 7b59 24a2 7c49 1ab8 c95f a799 cda7 4b60  {Y$.|I..._....K`
+0000e2b0: 3a43 32fb 8802 a57e 4037 9678 16dc c254  :C2....~@7.x...T
+0000e2c0: 4be3 2860 e565 8e16 bf68 93ed a4fb 4c7b  K.(`.e...h....L{
+0000e2d0: 5949 9e2e 73ec 378b 7385 9bb3 6feb ce60  YI..s.7.s...o..`
+0000e2e0: 3d73 5d44 b3ab 53e0 ca71 b4ad bc38 d4b0  =s]D..S..q...8..
+0000e2f0: 9385 b347 736a 4ff1 7b3b 4fe6 2c6d ebbd  ...GsjO.{;O.,m..
+0000e300: a31c 84bc 2edb 2c20 3c31 7483 b5f5 a561  ......, <1t....a
+0000e310: dffd e2e5 5995 724e 4581 7317 5fb0 747d  ....Y.rNE.s._.t}
+0000e320: d6a2 266d fd0d 5fc4 eae9 6d8b c99e c34c  ..&m.._...m....L
+0000e330: 1c39 b743 75ff b4c2 5659 e91b 835a 711d  .9.Cu...VY...Zq.
+0000e340: b72c 678f 4ee6 3107 1b0a fb9c 0228 de1f  .,g.N.1......(..
+0000e350: bb63 93bd 02a7 3cd6 f6ba f988 8b71 41de  .c....<......qA.
+0000e360: d047 262f e092 0be2 5b80 8c07 0c6e ab5a  .G&/....[....n.Z
+0000e370: f2d5 8e1b 7ad2 e13d e997 d93c d6df 25ef  ....z..=...<..%.
+0000e380: 366f d96e 567a 7a34 68c1 26ec 2aee a6b9  6o.nVzz4h.&.*...
+0000e390: 6c6b fb89 2ebe af31 7efa dfbc e345 79c6  lk.....1~....Ey.
+0000e3a0: d5bd 9e97 c4b7 d171 2459 1cc2 953d fa36  .......q$Y...=.6
+0000e3b0: 05da 8772 464b 3026 8da8 5fcf 1873 93d8  ...rFK0&.._..s..
+0000e3c0: 9bea 49e9 9f37 1812 da6f 2f08 f712 2217  ..I..7...o/...".
+0000e3d0: d564 2f3e cbea dd47 78b9 a66f 6ead 35b1  .d/>...Gx..on.5.
+0000e3e0: 3495 026c 80b3 599c b8eb 3e79 af6e a398  4..l..Y...>y.n..
+0000e3f0: f93c bc5c 3e8b 5bf4 d173 4d67 ce9c 7c38  .<.\>.[..sMg..|8
+0000e400: ec32 8bb1 d9cb 323e c42e 3e70 4470 7b2c  .2....2>..>pDp{,
+0000e410: d39d 573e 28a0 f5c3 2a9d f9e8 b4be 35af  ..W>(...*.....5.
+0000e420: fa78 def9 d2ea df3a 5174 f097 db54 379b  .x.....:Qt...T7.
+0000e430: ae77 5676 7b33 0c49 bb27 aa2a c577 2b23  .wVv{3.I.'.*.w+#
+0000e440: c7da b8ef 6e81 b852 80ae 9f2c 7919 767c  ....n..R...,y.v|
+0000e450: 8cc8 76fe 9a28 265e 0f50 1e71 e4d4 4b90  ..v..(&^.P.q..K.
+0000e460: f076 a764 cac6 e8d5 21f4 24ab ae57 7f33  .v.d....!.$..W.3
+0000e470: ca65 e156 eb8c aefc 9902 aaf7 1e39 2fdd  .e.V.........9/.
+0000e480: c827 a123 a438 ed5d b3a6 c09f 5642 62ea  .'.#.8.]....VBb.
+0000e490: df4f 688e fadf 8fa0 c23e 4fa7 0278 9aa4  .Oh......>O..x..
+0000e4a0: 1eb5 1f5d fe1b 1022 469e 9a41 789c 7593  ...]..."F..Ax.u.
+0000e4b0: c9ce a346 0084 ef3c 45df ad0c 60b6 469a  ...F...<E...`.F.
+0000e4c0: 44d3 60f6 c5ac 3f86 5bb3 1a9b c566 33f6  D.`...?.[....f3.
+0000e4d0: d3cf 9fe4 9ad4 f193 aa54 87aa 65aa 2ac0  .........T..e.*.
+0000e4e0: 625e e08e 6cc1 e515 2c78 2ea7 aba2 2ea1  b^..l...,x......
+0000e4f0: 20f0 4cc9 c3bc 1644 8a2f 1958 50c4 034f   .L....D./.XP..O
+0000e500: d5b0 8092 e669 9a11 0bb1 8415 8655 cd56  .....i.......U.V
+0000e510: c7b2 604a 8e83 1573 c415 2f16 345f 0918  ..`J...s../.4_..
+0000e520: 1378 5dae e304 cec3 3a81 d88e c373 0a7e  .x].....:....s.~
+0000e530: e205 9763 8307 8aff d5f4 b8ed 7e14 63ff  ...c........~.c.
+0000e540: 17a0 059a 1745 8117 2870 a018 8a22 be69  .....E..(p...".i
+0000e550: df2e 4b35 01ad 5df4 3507 3f87 71aa 1edd  ..K5..].5.?.q...
+0000e560: fb57 d32e d735 ff1f 5bf3 68e6 b601 7ffc  .W...5..[.h.....
+0000e570: 2d49 d10c 1778 9a07 4243 7351 1407 ca3f  -I...x..BCsQ...?
+0000e580: 9c00 0478 cd6a 2121 24c9 08f9 926f f65f  ...x.j!!$....o._
+0000e590: 143b c881 4c63 5f58 572e be76 0821 e6ce  .;..Lc_XW..v.!..
+0000e5a0: fa48 093e d362 4499 55ec cfdb 2795 3f69  .H.>.bD.U...'.?i
+0000e5b0: 5b27 924f 0069 9e33 b826 417f a32a 97ea  ['.O.i.3.&A..*..
+0000e5c0: d9c6 a556 d78f d888 f4af d62a 7026 ac9f  ...V.......*p&..
+0000e5d0: 5f76 2e85 dcfd fed1 7b93 6169 1809 52d0  _v......{.ai..R.
+0000e5e0: d0ee a9e1 53ed 3b41 4d52 e392 e84c b620  ....S.;AMR...L. 
+0000e5f0: 1135 6e10 f076 0d2b d39f 8534 eacf cfcf  .5n..v.+...4....
+0000e600: 5d9d 8a4c 93a8 f91c 8f27 d339 1b57 4d8f  ]..L.....'.9.WM.
+0000e610: 6d27 150e 6706 bebf 3bb8 a73c de1f 9673  m'..g...;..<...s
+0000e620: cfc2 322d 0f2e fa98 f297 2ffb 6e68 8416  ..2-....../.nh..
+0000e630: fe94 7556 d2fd 70b4 af1c a3a5 37f1 d358  ..uV..p.....7..X
+0000e640: aafb aae1 e328 af47 7270 5c02 e090 44fa  .....(.Grp\...D.
+0000e650: 2e75 29af 98c6 20a0 083b e8b5 c997 a5a3  .u)... ..;......
+0000e660: 4889 be6c facc eb5a 717e 8ba9 cbb5 9167  H..l...Zq~.....g
+0000e670: df30 9b0d 2fdd 8085 992e 234d 11c0 4e32  .0../.....#M..N2
+0000e680: 568a 0387 a95c d9d6 6125 1c73 eb48 ea08  V....\..a%.s.H..
+0000e690: bdbf c87e e12f b7ac 9871 adc9 cffe 60e1  ...~./...q....`.
+0000e6a0: f82c 7c6e bd9b b856 af1c e517 5ef2 e0bb  .,|n...V....^...
+0000e6b0: 4366 310c 94ef d1b3 54fd 90db 8ec3 70a6  Cf1.....T.....p.
+0000e6c0: 1acb 9c7d 6875 d3a5 14da fdd6 4e87 56dc  ...}hu......N.V.
+0000e6d0: 54c6 9867 267c 0fcf 041d 4824 5e69 aa0e  T..g&|....H$^i..
+0000e6e0: 3a02 989b d1bd d991 39b4 a791 6cf3 a989  :.......9...l...
+0000e6f0: f351 1778 ac51 3969 8bca 6653 6ccc a36a  .Q.x.Q9i..fSl..j
+0000e700: 2c9e 63b9 a93b f3a8 8789 cc5e c698 d213  ,.c..;.....^....
+0000e710: 97ad 1301 e6af 4adc bc75 b12f 6408 a387  ......J..u./d...
+0000e720: c133 61c4 496a 696d 507b df0d 1c87 753b  .3a.IjimP{....u;
+0000e730: edde 7ef5 caa7 1842 ed65 78b5 00c7 f2c8  ..~....B.ex.....
+0000e740: 5d6f 09a7 1f08 20b8 2fa5 e762 ddf3 f1a2  ]o.... ./..b....
+0000e750: d563 b7ca 9328 ed9e cc5e 5b26 d937 f296  .c...(...^[&.7..
+0000e760: a3d4 38c8 f925 67de 5dd4 776a e0dc a787  ..8..%g.].wj....
+0000e770: 5088 6692 f250 fe7c ef41 0e2d 963b 599c  P.f..P.|.A.-.;Y.
+0000e780: bad3 a474 b5e3 fe22 eb5c e725 ab18 44fb  ...t...".\.%..D.
+0000e790: aa05 2d15 ab6e 7121 d138 5c16 4176 3ca5  ..-..nq!.8\.Av<.
+0000e7a0: c6a4 fe48 cc55 dfe4 7520 c0c5 47f7 17bc  ...H.U..u ..G...
+0000e7b0: 9bd1 dd1c 2b67 9367 cf5d 08f0 e7ee 5036  ....+g.g.]....P6
+0000e7c0: f1ef 2714 f7f4 df8f 20e2 4789 970a 040a  ..'..... .G.....
+0000e7d0: 3a39 ca8f befc 0d82 c144 7a97 4378 9c75  :9.......Dz.Cx.u
+0000e7e0: 94c9 cea3 5614 84f7 3cc5 95b2 4964 25cc  ....V...<...Id%.
+0000e7f0: 93d4 899a c9d8 3f18 6c30 36b0 63b8 cc70  ......?.l06.c..p
+0000e800: f165 30f6 d3c7 9dde 76ce b2a4 da54 d577  .e0.....v....T.w
+0000e810: 660c 2180 3ccd d112 0d19 8113 b34c 9673  f.!.<........L.s
+0000e820: 2e13 a0c0 a579 5664 32cc d884 65f8 b490  .....yVd2...e...
+0000e830: 3962 4c30 1c66 4009 89c4 09b4 c0d0 344b  9bL0.f@.......4K
+0000e840: 718c 54f0 3997 fe70 3309 2ba6 592a 30b9  q.T.9..p3.+.Y*0.
+0000e850: 08e9 8c23 9265 ae10 06ee b060 10d8 81ef  ...#.e.....`....
+0000e860: 46e0 5b32 2739 2a93 8112 be97 7d52 777f  F.[2'9*.....}Rw.
+0000e870: 65a8 ff07 d022 2dc8 1225 5334 d851 2c45  e...."-..%S4.Q,E
+0000e880: 111f b5af e719 6260 d6f3 6149 c1b7 0161  ......b`..aI...a
+0000e890: 3876 afef 653d 574b fa3f b672 2ca7 ba04  8v..e=WK.?.r,...
+0000e8a0: 7ffe 38d5 308f 0e38 9b67 e01f 4d47 b906  ..8.0..8.g..MG..
+0000e8b0: 9ef1 9f4e 0002 3ca7 7da6 2a8a aa29 ca45  ...N..<.}.*..).E
+0000e8c0: bd7c f5b7 e7ab d33c 8d4e 2ee2 b2f0 41d5  .|.....<.N....A.
+0000e8d0: 298a b244 cf8b a26e c925 31ec 5748 f33a  )..D...n.%1.WH.:
+0000e8e0: aa47 9a82 ebdd 8d3a 02b0 6b3d c639 ee2b  .G.....:..k=.9.+
+0000e8f0: f1e8 9192 6818 59e2 d67d 7211 689e 5683  ....h.Y..}r.h.V.
+0000e900: a929 16d7 4bde 5ee3 5493 672f 01c9 d364  .)..K.^.T.g/...d
+0000e910: 31aa 43a4 51d8 349b 2b4b 007c b866 efd9  1.C.Q.4.+K.|.f..
+0000e920: 74e4 c338 382f 6f10 587e a896 c78e c1fc  t..88/o.X~......
+0000e930: 33b5 8cb3 af1e bb0d ab50 6937 4ede 20ff  3........Pi7N. .
+0000e940: f22b 9751 5b88 f372 1cd0 eb44 009b ad67  .+.Q[..r...D...g
+0000e950: d543 5115 88ee e9cd d476 767d c7d7 6a56  .CQ......vv}..jV
+0000e960: d6e6 f9d6 39be 6315 35ec 5d18 3547 b4d7  ....9.c.5.].5G..
+0000e970: 144d 2bfa eafc da32 acc5 8bbf 3005 0104  .M+....2....0...
+0000e980: 2e41 6281 0d74 3fd1 5c10 91ce b6ee 648b  .Ab..t?.\.....d.
+0000e990: cf04 6176 72c3 8dec d7dc 77af 8491 ce07  ..avr.....w.....
+0000e9a0: b369 b1a5 cb45 ca05 d3e3 d89b 0337 3803  .i...E.......78.
+0000e9b0: 015e 7e1f 75b6 7bf6 fc32 f3f3 ce47 f1e3  .^~.u.{..2...G..
+0000e9c0: 1679 79cb 3f5b 8389 8dbb 306d ee9e ef24  .yy.?[....0m...$
+0000e9d0: 8b56 2e8c b557 d3d5 0d0d a755 37f3 d81d  .V...W.....U7...
+0000e9e0: 9f77 9700 c70a 1ec8 327e a81c 1b37 e48a  .w......2~...7..
+0000e9f0: bf98 dec8 a699 3cd9 e7f1 555b d678 df61  ......<...U[.x.a
+0000ea00: 3e4c 3b5e 4e14 e69d 3d6e 211f 25e8 3adc  >L;^N...=n!.%.:.
+0000ea10: c912 3dee da4a 009d 79ac c157 d451 b23c  ..=..J..y..W.Q.<
+0000ea20: 85d5 1e4e e158 85ee ea22 cf65 59e9 f2dc  ...N.X...".eY...
+0000ea30: ae16 5f1a 27bd 682c bfc6 68d0 63c7 4c4f  .._.'.h,..h.c.LO
+0000ea40: 7ba3 b35a 9474 eb83 00ea a5cd ab49 c422  {..Z.t.......I."
+0000ea50: cc69 2f43 e81a 9ebf 2249 dcb3 bb72 4d98  .i/C...."I...rM.
+0000ea60: afa9 8998 9167 b642 8739 df71 d627 a203  .....g.B.9.q.'..
+0000ea70: 3f4b d61d 6fe1 895b c69e 00f4 1493 defa  ?K..o..[........
+0000ea80: 46b7 0d8a 7e28 2c83 15ac bad6 e64e 71d7  F...~(,......Nq.
+0000ea90: 6581 db95 ef96 7bc6 b572 76d8 7963 94d4  e.....{..rv.yc..
+0000eaa0: 58ce b9b9 af74 9214 6f9f e97c da34 9d77  X....t..o..|.4.w
+0000eab0: 736a ecb8 289c dbc6 a936 a3fb 85fc d802  sj..(....6......
+0000eac0: bb43 17f3 7dc0 ed09 e5b0 d197 94d3 925d  .C..}..........]
+0000ead0: 4def e2aa b59f b702 55aa 7a5f 3173 25c0  M.......U.z_1s%.
+0000eae0: 1b52 e651 3e04 f5e5 96cb e649 b478 5227  .R.Q>......I.xR'
+0000eaf0: c0df 695d 37c4 4f26 0c47 ff35 1184 92e7  ..i]7.O&.G.5....
+0000eb00: 3007 131c 7230 c36d 06cf 0f66 60ca 3eff  0...r0.m...f`.>.
+0000eb10: 6198 2a34 8374 9967 3480 df7f 93fe 2088  a.*4.t.g4..... .
+0000eb20: 7f01 b7ab 54fb ec02 854b 789c dbce f19f  ....T....Kx.....
+0000eb30: 7142 bf90 85b9 9982 b681 b181 0157 727e  qB...........Wr~
+0000eb40: 6e6e 6649 49ea c464 1d4e b8e8 640e 160d  nnfII..d.N..d...
+0000eb50: 462e 002e f30b be9c 0d78 9c9d cbbd 0ac2  F........x......
+0000eb60: 3010 00e0 3d4f 915d 90fc de25 20e2 e424  0...=O.]...% ..$
+0000eb70: 7490 0e8e 97e4 520b b695 9082 8faf cfe0  t.....R.........
+0000eb80: fac1 d71b b3e4 80c1 e8e4 4c76 3941 2650  ..........Lv9A&P
+0000eb90: 4133 b892 d011 6280 5c21 e8ca 2cde d478  A3....b.\!..,..x
+0000eba0: ed32 63f5 452b 6f6a b45e b954 abf7 064b  .2c.E+oj.^.T...K
+0000ebb0: b229 99ea 2880 8eb9 7800 417b 7f6e 4d0e  .)..(...x.A{.nM.
+0000ebc0: ebde e478 1bef c343 9ea8 53d9 265a 155c  ...x...C..S.&Z.\
+0000ebd0: a685 e6d7 316f cb59 6ad4 1031 1a63 e541  ....1o.Yj..1.c.A
+0000ebe0: 59a5 c44f 97b9 77fe 6f8b ebfc 115f 2fcb  Y..O..w.o...._/.
+0000ebf0: 407d 980e 789c 9dcc 410a c230 1040 d17d  @}..x...A..0.@.}
+0000ec00: 4e91 bd20 49a6 4918 10f1 004a 17d2 85cb  N.. I.I....J....
+0000ec10: c964 520b 4d2b 21bd bf9e c1ed 87f7 7b13  .dR.M+!.......{.
+0000ec20: d181 0bb2 cf9e 8531 f881 6d22 c816 2359  .......1..m"..#Y
+0000ec30: 7045 9cc9 9990 dc00 ea43 4db6 ae6d 7410  pE.......CM..mt.
+0000ec40: 9c2f 81d8 0896 3410 60f1 094d b62c 2502  ./....4.`..M.,%.
+0000ec50: 71cc 1e52 5274 f4f7 def4 b81d 4d4f f7e9  q..RRt......MO..
+0000ec60: 39be f485 3ae5 7da6 cd84 db5c 6959 cfbc  9...:.}....\iY..
+0000ec70: d7eb 6f69 0346 3416 f4c9 8031 ea57 ebd2  ..oi.F4....1.W..
+0000ec80: bbfc a7d5 63d9 964a ab2e 42fd 68a2 bee7  ....c..J..B.h...
+0000ec90: 2945 f59d 1478 9c9d 8d3d 4ec4 3010 85fb  )E...x...=N.0...
+0000eca0: 9cc2 dd16 0832 76fc 8b10 e200 a02d d016  .....2v......-..
+0000ecb0: 9493 f138 8996 3891 e3dc 1f53 7001 5ef9  ...8..8....Sp.^.
+0000ecc0: f4be efd5 c22c 5488 2a22 9209 a043 904e  .....,T.*"...C.N
+0000ecd0: b131 5a2a 1b9d 8a7a 8803 7034 08da 763b  .1Z*...z..p4..v;
+0000ece0: 16ce 5524 4a14 c8a3 8ea3 8760 d00e 8382  ..U$J......`....
+0000ecf0: 9802 316b c7a3 575e 1129 0e7f 7b44 968e  ..1k..W^.)..{D..
+0000ed00: dac6 811d 1280 b2c6 28c5 e812 45c9 2938  ........(...E.)8
+0000ed10: 492d de74 78d6 792b e29a cf22 6eef b7cf  I-.tx.y+..."n...
+0000ed20: eb97 78c1 8a71 9b30 837d 9b56 5cbe 9f68  ..x..q.0.}.V\..h
+0000ed30: 5b5f 8574 d206 e70d 68f1 0003 40d7 da75  [_.t....h...@..u
+0000ed40: a995 ff47 771f 5c26 1663 c14c b3b8 ac78  ...Gw.\&.c.L...x
+0000ed50: 34d3 456c 49cc b5ee c773 df4f 4b9d cff1  4.ElI....s.OK...
+0000ed60: 17ef b776 d0bc 77cc fdb4 d747 3c8e e5a8  ...v..w....G<...
+0000ed70: 986b f703 295b 6641 9c0d 789c 9dcb b10a  .k..)[fA..x.....
+0000ed80: c230 1080 e13d 4f91 5d90 4b42 2f77 20e2  .0...=O.].KB/w .
+0000ed90: e424 7490 0e8e d75c 520b b695 9082 8faf  .$t....\R.......
+0000eda0: cfe0 fa7f fcad e66c 8954 5370 0a9d 2815  .......l.TSp..(.
+0000edb0: 74a1 43a2 02cc 8174 4c98 2886 a8a1 8879  t.C....tL.(....y
+0000edc0: 4bcd 6bb3 31eb 4f71 94c4 1d41 74c2 2a5c  K.k.1.Oq...At.*\
+0000edd0: 3c91 47ef 9c8f 5c14 d3c8 6a64 6fcf adda  <.G...\...jdo...
+0000ede0: 7edd ab1d 6ec3 bd7f d893 34d1 6d92 15f0  ~...n.....4.m...
+0000edf0: 322d 32bf 8e69 5bce d645 871c a903 6f0f  2-2..i[..E....o.
+0000ee00: 1000 ccaf 2e73 6bf9 bfdb 5ce7 8ff9 0223  .....sk...\....#
+0000ee10: 6840 689d 1478 9c9d 903d 4ec4 3014 84fb  h@h..x...=N.0...
+0000ee20: 9cc2 dd16 08e2 bfe7 1f84 1007 006d 81b6  .............m..
+0000ee30: a07c b69f 9368 8913 39ce fd31 0517 40d3  .|...h..9..1..@.
+0000ee40: 8de6 9b91 a655 2216 2271 9d41 80a0 1c45  .....U"."q.A...E
+0000ee50: f290 c843 f6e8 24b9 2e00 c51d 0523 871d  ...C..$......#..
+0000ee60: 2b95 c602 4850 1253 cc96 acd4 803e 29ee  +...HP.S.....>).
+0000ee70: b9e3 28a2 4b90 9d34 5e04 127f 79f4 2a67  ..(.K..4^...y.*g
+0000ee80: 8b19 1490 801c 8cd6 a812 9a88 5224 ed4d  ............R$.M
+0000ee90: 88de 7172 76c0 b3cd 5b65 d772 5676 7bbf  ..qrv...[e.rVv{.
+0000eea0: 7d5e bfd8 0b36 4cdb 8485 9bb7 69c5 e5fb  }^...6L.....i...
+0000eeb0: 296e eb2b 1356 186f 9dd2 923d 70c5 f9d0  )n.+.V.o...=p...
+0000eec0: dd75 698d fe47 0f1f 54a7 7e44 c512 6776  .ui..G..T.~D..gv
+0000eed0: 59f1 e84d 17b6 6536 b7b6 1fcf e338 2d6d  Y..M..e6.....8-m
+0000eee0: 3ec3 2f3e 6e7d a0f7 deb1 8cd3 de1e f138  >./>n}.........8
+0000eef0: 96a3 6169 c30f aae2 6690 9c0d 789c 9dcb  ..ai....f...x...
+0000ef00: b10a c230 1000 d03d 5f91 5d90 bb24 5e1a  ...0...=_.]..$^.
+0000ef10: 1071 7212 3a48 07c7 bbf4 a205 db4a 48c1  .qr.:H.......JH.
+0000ef20: cfd7 6f70 7df0 5a55 b531 810f a812 424a  ..op}.ZU.1....BJ
+0000ef30: 9091 b980 c7e2 ca28 98ba 9883 1452 5f88  .......(.....R_.
+0000ef40: cd9b ab2e cd0a 6889 8491 a853 643f 4af1  ......h....Sd?J.
+0000ef50: 14b2 5210 7770 1824 9160 27ce 19de da73  ..R.wp.$.`'....s
+0000ef60: adb6 5fb6 6a87 eb70 ebef f6c8 8dc7 f5c1  .._.j..p........
+0000ef70: 0bd0 f931 f3f4 dae7 753e 598c 4829 763e  ...1....u>Y.H)v>
+0000ef80: 80dd 8107 303f 9da7 d6f4 bf6d 2ed3 c77c  ....0?.....m...|
+0000ef90: 0100 4940 30a1 0778 9c33 3430 3033 3151  ..I@0..x.340031Q
+0000efa0: 888f cfcc cb2c 898f d72b a864 7836 f7d1  .....,...+.dx6..
+0000efb0: ec4d 17af 397b 776b ae2b 8fba 71e8 494f  .M..9{wk.+..q.IO
+0000efc0: f044 4388 b2a4 d292 92fc 3c90 a219 aea6  .DC.......<.....
+0000efd0: f946 7343 0b5f 8bda 0be9 a55d 547b 385d  .FsC._.....]T{8]
+0000efe0: 410d aaa8 3833 3d2f 3107 a428 6fe5 e9dc  A...83=/1..(o...
+0000eff0: ceda 901f bf7c 6d59 f728 b979 cc5c dff9  .....|mY.(.y.\..
+0000f000: 0e00 ec3f 2d8a ab15 7801 3331 0002 05bd  ...?-...x.31....
+0000f010: f4cc 928c d224 867b 8f0f 453f e878 db2e  .....$.{..E?.x..
+0000f020: cdbd e7c6 bef9 9e3c 318d 5c87 0c0d 0ccc  .......<1.\.....
+0000f030: 4c4c c04a 32d3 f3f2 8b52 19e6 ba4f b6a9  LL.J2....R...O..
+0000f040: be75 fca1 cbf1 991d 9be7 9fe1 e4fa cb74  .u.............t
+0000f050: 0aaa cac7 d3d9 d52f d895 c1f0 7a61 c0a9  ......./....za..
+0000f060: 777d be6f 2a3e b370 7ef9 c7fb 6a9b e041  w}.o*>.p~...j..A
+0000f070: a812 5f47 3f4f 37d7 e010 bdcc 3c86 953e  .._G?O7.....<..>
+0000f080: 0f17 6eba 71f1 f6ad 943b 4f53 24fa 4b3c  ..n.q....;OS$.K<
+0000f090: f8f5 99a1 ca82 5c1d 5d7c 5df5 7253 1866  ......\.]|].rS.f
+0000f0a0: aeba 9974 7752 f06a a15d 2ba3 4d0e 4cfe  ...twR.j.]+.M.L.
+0000f0b0: d77e 7177 2c54 5152 696e 815e 4125 c3bd  .~qw,TQRin.^A%..
+0000f0c0: 8977 d6a9 ae3a 7e99 698a 4d81 ebcf 86d5  .w...:~.i.M.....
+0000f0d0: a677 4f7b 9880 7d96 5e50 129f 9c9f 5b50  .wO{..}.^P....[P
+0000f0e0: 5a92 5a14 9f58 5c9c 595c 9298 57c2 7060  Z.Z..X\.Y\..W.p`
+0000f0f0: be39 f7d6 49b3 df2a 72a6 9c97 ecf8 f2da  .9..I..*r.......
+0000f100: a3dd 6135 d4cc a2d4 c2d2 cca2 d4dc d4bc  ..a5............
+0000f110: 9262 bd92 8a12 069e 8933 d69c d97c 71ed  .b.......3...|q.
+0000f120: d56c 9769 4f27 fe92 38bd 3ee5 0f54 6d71  .l.iO'..8.>..Tmq
+0000f130: 6a49 29d8 01dc d353 dc33 3755 765c de9d  jI)....S.37Uv\..
+0000f140: b94f b5c5 44e7 6167 070b 0096 3a92 06a1  .O..D.ag....:...
+0000f150: 1478 0133 3430 3033 3151 888f cfcc cb2c  .x.340031Q.....,
+0000f160: 898f d72b a864 98a5 a4bd 50bf bce6 c099  ...+.d....P.....
+0000f170: 8e42 7ddd 9dab 7f66 fe76 5965 6200 040a  .B}....f.vYeb...
+0000f180: 89e9 a979 250c 2dc7 7d76 288b f2df de7d  ...y%.-.}v(....}
+0000f190: d4ba bffb 4b4a a951 04ff 13a8 7c69 4a66  ....KJ.Q....|iJf
+0000f1a0: 3ec3 a58d 9a72 1d36 f673 c326 15db 8abf  >....r.6.s.&....
+0000f1b0: 39a7 5c70 84af c210 624d 7a41 497c 727e  9.\p....bMzAI|r~
+0000f1c0: 6e41 6949 6a51 7c62 7171 6671 4962 5e09  nAiIjQ|bqqfqIb^.
+0000f1d0: c8d2 4372 5fbe b238 5f5f e372 d850 fae6  ..Cr_..8__.r.P..
+0000f1e0: 97c5 cb78 93e2 5f43 0c4d 2fcd 6498 69a1  ...x.._C.M/.d.i.
+0000f1f0: fbe7 dbda 8e90 42be 059b a2f7 c5e4 df9e  ......B.........
+0000f200: 6fbf 076a 644e 4e2e 487f 8926 abdb ad87  o..jdNN.H..&....
+0000f210: 0269 3976 1dff b40c a426 87ee 643d 08d1  .i9v.....&..d=..
+0000f220: 5f9c 5c94 9a9a c770 fe54 7ff3 2d9b 2f5c  _.\....p.T..-./\
+0000f230: 274e 7108 ff78 29b5 4c52 4234 166a 04d0  'Nq..x).LRB4.j..
+0000f240: 1145 6047 28b8 5c5d 303f 5469 6762 b6aa  .E`G(.\]0?Tigb..
+0000f250: 0ec7 c465 2f56 559f 4a81 1852 5a92 9953  ...e/VU.J..RZ..S
+0000f260: ccb0 708d dfa5 f36f dba2 0f67 5436 5859  ..p....o...gT6XY
+0000f270: 2fdc 152c 73d4 1600 7abf 805d ef01 8376  /..,s...z..]...v
+0000f280: 789c bbcd 749b 69c2 7791 33c2 1cad 67ab  x...t.i.w.3...g.
+0000f290: cfd8 30db 096c 5d20 1bf8 7f7b 42fa 92c9  ..0..l] ...{B...
+0000f2a0: dc8c 0100 dd80 0d36 ee01 8159 789c 011e  .......6...Yx...
+0000f2b0: 00e1 ffc1 02c1 0290 a614 3afd 2ed1 5f67  ..........:..._g
+0000f2c0: 3613 7040 b4ef f58b 1a94 f096 7bd1 91ba  6.p@........{...
+0000f2d0: 87d6 710f 3ba1 0778 9c33 3430 3033 3151  ..q.;..x.340031Q
+0000f2e0: 888f cfcc cb2c 898f d72b a864 7836 f7d1  .....,...+.dx6..
+0000f2f0: ec4d 17af 397b 776b ae2b 8fba 71e8 494f  .M..9{wk.+..q.IO
+0000f300: f044 4388 b2a4 d292 92fc 3c90 a253 ec12  .DC.......<..S..
+0000f310: 9c4b a426 1e9d b4fa c1d6 9f7e a7b4 9d97  .K.&.......~....
+0000f320: 5dad 832a 2ace 4ccf 4bcc 0129 ca5b 793a  ]..**.L.K..).[y:
+0000f330: b7b3 36e4 c72f 5f5b d63d 4a6e 1e33 d777  ..6../_[.=Jn.3.w
+0000f340: be03 005e 4c30 2aee 0180 4b78 9c01 1e00  ...^L0*...Kx....
+0000f350: e1ff db02 db02 90a3 14de b375 8014 9021  ...........u...!
+0000f360: e953 3af1 0f9f a50e 29a3 cedc 6491 b7a4  .S:.....)...d...
+0000f370: dcd2 0edb ee01 8078 789c bbcd 749b 69c2  .......xx...t.i.
+0000f380: 6291 a21d 227f de67 cf49 0c97 c8ab d192  b..."..g.I......
+0000f390: 9d67 ed75 935d 71e2 f625 00d3 550d 43ee  .g.u.]q..%..U.C.
+0000f3a0: 0181 2378 9cbb cd74 9b69 c262 11d9 703d  ..#x...t.i.b..p=
+0000f3b0: 8d38 63f7 bf66 53f4 4e06 df29 743b 2a57  .8c..fS.N..)t;*W
+0000f3c0: 7b74 e2f6 2500 bb60 0d59 ec04 8644 789c  {t..%..`.Y...Dx.
+0000f3d0: 014c 00b3 ffdb 02db 0290 a314 8226 9d5b  .L...........&.[
+0000f3e0: 29a5 7cd3 fda0 07c6 c786 d211 19a1 ed23  ).|............#
+0000f3f0: 91b7 4014 44a0 9b43 62d3 2602 7ef2 17a4  ..@.D..Cb.&.~...
+0000f400: e5f4 a8de fd57 8799 930b 013c 141d 2bbf  .....W.....<..+.
+0000f410: 74d8 23f9 8fc2 03f0 82b5 6e91 1ffa 5049  t.#.......n...PI
+0000f420: 2e81 9424 94e0 0381 7d78 9c3b c874 9049  ...$....}x.;.t.I
+0000f430: ddd0 c0c0 ccc4 4421 3e3e 332f b324 3e5e  ......D!>>3/.$>^
+0000f440: afa0 92e1 a764 63eb 611f 41d1 1a47 a9c3  .....dc.a.A..G..
+0000f450: 8b2f be5c e212 927e 71a3 ba14 2300 9379  ./.\...~q...#..y
+0000f460: 11ef ae0e 7801 3334 3030 3331 5188 8fcf  ....x.340031Q...
+0000f470: cccb 2c89 8fd7 2ba8 6448 6835 6bfe 68a8  ..,...+.dHh5k.h.
+0000f480: c272 6862 46e3 ba0c 0b33 89ff aaee 8610  .rhbF....3......
+0000f490: 6589 e9a9 7925 2035 b3af 38fa 4f64 d0a8  e...y% 5..8.Od..
+0000f4a0: 397e 66a3 c90a c6cc 7fd9 cf3e 08c3 d414  9~f........>....
+0000f4b0: 1767 1697 2442 d46d f493 1198 f72d 42cb  .g..$B.m.....-B.
+0000f4c0: e0a7 74fe 1f75 ad4f 2112 d575 5075 4989  ..t..u.O!..uPuI.
+0000f4d0: c9d9 e945 f9a5 7929 2003 9f4f f113 59e2  ...E..y) ..O..Y.
+0000f4e0: 9770 6c59 b7e6 1f6f c380 ed19 5ceb b640  .plY...o....\..@
+0000f4f0: 1526 6724 96c4 6700 cdcc 2faa 0429 5db6  .&g$..g.../..)].
+0000f500: 6b99 d985 af86 ce6a b3a7 f544 1cce 90ec  k......j...D....
+0000f510: 9ec8 fd15 aab4 a028 3f39 39b5 b818 a4ec  .......(?99.....
+0000f520: dadb 5b5a bda5 599b 65e6 ed9f e2b3 c172  ..[Z..Y.e......r
+0000f530: 82ab 9356 3500 7a22 5c7a e403 8170 789c  ...V5.z"\z...px.
+0000f540: 0134 00cb ffdb 02db 0290 f714 297d ac16  .4..........)}..
+0000f550: 0961 f0ae ea73 2374 aae4 2697 5013 3328  .a...s#t..&.P.3(
+0000f560: 930b 013c 1404 88e2 c876 8391 4c32 deaa  ...<.....v..L2..
+0000f570: a866 7e74 97f7 6a04 d857 5b17 4ca1 1478  .f~t..j..W[.L..x
+0000f580: 0133 3430 3033 3151 888f cfcc cb2c 898f  .340031Q.....,..
+0000f590: d72b a864 286b 2f7e 3f65 6e82 4863 f66f  .+.d(k/~?en.Hc.o
+0000f5a0: a98e bf2f 2f94 7f8e df66 6200 040a 89e9  ...//....fb.....
+0000f5b0: a979 250c 4e5e 1b8f 4cbe b786 bbdf 2c5e  .y%.N^..L.....,^
+0000f5c0: f9bb d1df 9217 597b d642 e54b 5332 f319  ......Y{.B.KS2..
+0000f5d0: 2e6d d494 ebb0 b19f 1b36 a9d8 56fc cd39  .m.......6..V..9
+0000f5e0: e582 237c 1586 106b d20b 4ae2 93f3 730b  ..#|...k..J...s.
+0000f5f0: 4a4b 528b e213 8b8b 338b 4b12 f34a 4096  JKR.....3.K..J@.
+0000f600: 8ac5 c8d6 3e99 c5b1 eaeb bc2b 5687 56ee  ....>......+V.V.
+0000f610: cad8 2168 f002 6268 7a69 26c3 82ed 9246  ..!h..bhzi&....F
+0000f620: 1919 0f9e 8b9a f9bc 7d3a df77 33eb c41b  ........}:.w3...
+0000f630: 6e50 2373 7272 41fa 4b34 59dd 6e3d 1448  nP#srrA.K4Y.n=.H
+0000f640: cbb1 ebf8 a765 2035 3974 27eb 4188 fee2  .....e 59t'.A...
+0000f650: e4a2 d4d4 3c86 f3a7 fa9b 6fd9 7ce1 3a71  ....<.....o.|.:q
+0000f660: 8a43 f8c7 4ba9 6592 12a2 b150 2380 8e28  .C..K.e....P#..(
+0000f670: 023b 42c1 e5ea 82f9 a14a 3b13 b355 7538  .;B......J;..Uu8
+0000f680: 262e 7bb1 aafa 540a c490 d292 cc9c 6286  &.{...T.......b.
+0000f690: 856b fc2e 9d7f db16 7d38 a3b2 c1ca 7ae1  .k......}8....z.
+0000f6a0: ae60 99a3 b600 bce1 8202 eb01 8348 789c  .`...........Hx.
+0000f6b0: 7bc7 f88e 71c2 2d91 b50c c7d8 2e3c 5ee5  {...q.-......<^.
+0000f6c0: c8ff e16e c04c 0b0d 6dc5 03ba ae00 b6a1  ...n.L..m.......
+0000f6d0: 0c17 e403 8508 789c 0134 00cb ffdb 02db  ......x..4......
+0000f6e0: 0290 f714 71e3 b40d cca6 a041 4014 fd87  ....q......A@...
+0000f6f0: 843a 2a1f e4ef be80 930b 013c 140a ac16  .:*........<....
+0000f700: 944d 6b28 c7fc 0599 4450 df60 a768 88f4  .Mk(....DP.`.h..
+0000f710: 1f81 1317 bbef 0482 1878 9c3b c874 90c9  .........x.;.t..
+0000f720: ddd0 c0c0 ccc4 4421 3e3e 332f b324 3e5e  ......D!>>3/.$>^
+0000f730: afa0 92c1 7fad 073f 4f09 57c8 5595 e959  .......?O.W.U..Y
+0000f740: 675f 1a67 1a07 f87f 3731 0002 85c4 f4d4  g_.g....71......
+0000f750: bc12 86d5 2efe eb0e 3734 44fd c857 de9d  ........74D..W..
+0000f760: 6ed3 3045 967d 87fb 44f7 5f00 436f 1dc7  n.0E.}..D._.Co..
+0000f770: ef01 801e 789c 011f 00e0 ffdb 02db 0290  ....x...........
+0000f780: f714 a285 ae6d 645e f9a5 b7e0 055c 3d58  .....md^.....\=X
+0000f790: 8af7 85e2 9dda 930b 0150 03b7 0fd3 ee01  .........P......
+0000f7a0: 8009 789c 011e 00e1 ffc1 02c1 0290 3314  ..x...........3.
+0000f7b0: a841 8e57 a4e8 a6f2 8cec 8a95 04e5 f9e7  .A.W............
+0000f7c0: b4a3 1bba 9147 faeb 1e10 aeee 0181 2178  .....G........!x
+0000f7d0: 9c7b c7f8 8e71 82b9 88d1 0b5b ff73 bf8c  .{...q.....[.s..
+0000f7e0: cd99 b59a dc0b e657 0733 6f34 7a39 d17b  .......W.3o4z9.{
+0000f7f0: 3100 c18a 0cb3 e403 872c 789c 0134 00cb  1........,x..4..
+0000f800: ffdb 02db 0290 f714 f633 edd3 c761 2dcc  .........3...a-.
+0000f810: 4ede 3aff 172a e7a0 fb6a 1705 930b 013c  N.:..*...j.....<
+0000f820: 14e2 47ee b062 9dc5 d988 1efe 6844 1c79  ..G..b......hD.y
+0000f830: ffea 8f88 5fc2 8a1a a5e0 0380 1b78 9c3b  ...._........x.;
+0000f840: c874 9049 ddd0 c0c0 ccc4 4421 3e3e 332f  .t.I......D!>>3/
+0000f850: b324 3e5e afa0 9261 55ce aa94 b867 b94d  .$>^...aU....g.M
+0000f860: 0a4f 3add f2a6 46c4 6cd1 58f3 62a3 ba14  .O:...F.l.X.b...
+0000f870: 2300 a037 1288 e403 882c 789c 0134 00cb  #..7.....,x..4..
+0000f880: ffdb 02db 0290 f714 bebc 19a2 8531 46d8  .............1F.
+0000f890: 6974 fc1a 5496 a8ec afc0 7001 930b 013c  it..T.....p....<
+0000f8a0: 1445 08ca 5216 d7d2 3830 a7d1 ec0d f78a  .E..R...80......
+0000f8b0: a26e 33cb 408b fd18 6fe4 0390 3378 9c01  .n3.@...o...3x..
+0000f8c0: 3400 cbff db02 db02 90f7 1452 fcf2 0012  4..........R....
+0000f8d0: 4d29 bb17 cc41 33f1 9661 30ef e293 0793  M)...A3..a0.....
+0000f8e0: 0b01 3c14 18e0 338c ef5d 5645 7263 d691  ..<...3..]VErc..
+0000f8f0: 7a88 abda 7bef 876b 6dc2 185f e403 8932  z...{..km.._...2
+0000f900: 789c 0134 00cb ffdb 02db 0290 f714 cc13  x..4............
+0000f910: 0885 cd7b cc3c 033e 10b5 a01d 51ff b760  ...{.<.>....Q..`
+0000f920: 67a4 930b 013c 140b 9764 4769 b279 88d3  g....<...dGi.y..
+0000f930: bb69 be25 8434 2ce1 8988 0453 0c16 53e4  .i.%.4,....S..S.
+0000f940: 0387 0578 9c01 3400 cbff db02 db02 90f7  ...x..4.........
+0000f950: 141a 03eb 1ab9 38e5 3bcd 1168 cecc 2bf8  ......8.;..h..+.
+0000f960: 6e20 aa76 1b93 0b01 3c14 1d2b bf74 d823  n .v....<..+.t.#
+0000f970: f98f c203 f082 b56e 911f fa50 492e 5f78  .......n...PI._x
+0000f980: 170d e403 8430 789c 0134 00cb ffdb 02db  .....0x..4......
+0000f990: 0290 f714 02e2 e3ff 9b9a b5a5 646b 8d52  ............dk.R
+0000f9a0: d2fc c1c5 ab6c cffa 930b 013c 143e 5f99  .....l.....<.>_.
+0000f9b0: 9b65 e4d5 6529 111a d192 bfc6 de42 5caf  .e..e).......B\.
+0000f9c0: 47f0 b71b 7eef 0143 789c bbcd 749b 69c2  G...~..Cx...t.i.
+0000f9d0: 7791 baea a90f e744 f518 db95 cb3b 7e5a  w......D.....;~Z
+0000f9e0: 5777 4cb8 2ce1 f164 6ec6 0000 f026 0e2e  WwL.,..dn....&..
+0000f9f0: e403 2b78 9c01 3400 cbff db02 db02 90f7  ..+x..4.........
+0000fa00: 14bb f307 ff3c e72e 6cf8 df49 bc07 ab19  .....<..l..I....
+0000fa10: eac8 f0bf 6b93 0b01 3c14 0488 e2c8 7683  ....k...<.....v.
+0000fa20: 914c 32de aaa8 667e 7497 f76a 04d8 cce3  .L2...f~t..j....
+0000fa30: 1ac3 ef01 833c 789c 011f 00e0 ffdb 02db  .....<x.........
+0000fa40: 0290 f714 f98a 9ff7 dbca 4e98 b5ba 343a  ..........N...4:
+0000fa50: 83cd 588a 0d29 54a5 930b 0150 103d 0f27  ..X..)T....P.=.'
+0000fa60: be88 0178 9cbd 5561 6fdb 3610 fdae 5f71  ...x..Uao.6..._q
+0000fa70: 7380 2009 46db b225 c71e 920c 59d2 aeed  s. .F..%....Y...
+0000fa80: 96b5 a853 0443 1120 27ea 6471 9148 8da4  ...S.C. '.dq.H..
+0000fa90: 92f8 dfef 2829 ce3a 6cfb b40e 3024 99bc  ....().:l...0$..
+0000faa0: 3b1e dfbb 77b7 073f 7eb8 860b 5337 ad27  ;...w..?~...S7.'
+0000fab0: 0be7 ce29 e751 fbe8 8dfa 167c a91c f00f  ...).Q.....|....
+0000fac0: 35b4 da14 8592 0a2b 7834 f61e 0a63 a1b1  5......+x4...c..
+0000fad0: e641 e54a 6fe0 a244 1fe2 5ca1 7cbf 066c  .A.Jo..D..\.|..l
+0000fae0: 1af0 066e 94ce cd63 f0ce e167 a5db a731  ...n...c...g...1
+0000faf0: bcd5 7dcc 47dc be04 87c2 922b 3b33 3e3a  ..}.G......+;3>:
+0000fb00: aba8 3b61 0cbf 9a16 241f 4de8 54b5 05a5  ..;a....$.M.T...
+0000fb10: 79b7 aa00 1d7c d8fa d268 a854 66d1 6ebb  y....|...h.Tf.n.
+0000fb20: 5cba 685e d504 59eb e191 6328 b66d 2c35  \.h^..Y...c(.m,5
+0000fb30: 6889 cf68 5443 95d2 1412 7bc9 5ba3 570f  h..hTC....{.[.W.
+0000fb40: b40b eda4 558d 7770 30a6 273a 1c47 5174  ....U.wp0.':.GQt
+0000fb50: 8250 5a2a 4e47 a5f7 8dfb 6e32 c995 93c6  .PZ*NG....n2....
+0000fb60: e6e3 cd66 f2fb 79f3 babe b9f2 cba7 d1d9  ...f..y.........
+0000fb70: 89aa 3780 953f 1dad 3dc7 94f0 03e6 1b1a  ..7..?..=.......
+0000fb80: 81b3 f2c5 976d c6ae 5454 e56e accc 240b  .....m..TT.n..$.
+0000fb90: 2693 cb3e a078 6794 fede f96d 45a7 ce04  &..>.xg....mE...
+0000fba0: 9cf7 2bb3 31a7 c379 23be 4fee cbd3 389d  ..+.1..y#.O...8.
+0000fbb0: 9e9d 4cf0 8c53 8bf6 f6e0 021b cc54 a5bc  ..L..S.......T..
+0000fbc0: 2217 9dfb 3fa1 c008 94c8 57ab 5107 e80a  "...?.....W.Q...
+0000fbd0: 8bce db56 fa96 d1a0 8a6a d27e 0c37 04bf  ...V.....j.~.7..
+0000fbe0: b5ce 03aa fa05 17f6 2d0d 93c0 b1f4 3d47  ........-.....=G
+0000fbf0: 636a f966 9630 0f81 7654 33c9 0c10 0838  cj.f.0..vT3....8
+0000fc00: 3a5a 4b4b a4e1 239b 1c1d 85a5 2b25 ad69  :ZKK..#.....+%.i
+0000fc10: 9822 1a0c b6ce 530d e76d aecc 6041 b5b1  ."....S..m..`A..
+0000fc20: db28 1222 fc7b dfb0 7be0 5f56 c651 08fd  .(.".{..{._V.Q..
+0000fc30: b20a adad fa28 1795 6a32 8376 3864 4d68  .....(..j2.v8dMh
+0000fc40: 6509 aff4 8669 75bd c950 1821 d4fa 0d57  e....iu..P.!...W
+0000fc50: 1b97 3497 003f 5def 7363 192a e63d 187c  ..4..?].sc.*.=.|
+0000fc60: 6cb5 0edf eb9e f4b0 fdc9 8585 ad69 2d5c  l............i-\
+0000fc70: 3348 1b8b 9cb4 94a6 653d f0f6 4fda 3c56  3H......e=..O.<V
+0000fc80: c4a4 719d 6bdc 7420 763c 3013 d726 3791  ..q.k.t v<0..&7.
+0000fc90: 80cf 4fb7 8c83 23cf d97b 65f4 b0b4 6e98  ..O...#..{e...n.
+0000fca0: a3ee e4ca 84e3 0310 6e0c 0737 cc57 c3b2  ........n..7.W..
+0000fcb0: c346 f54c b8b6 698c f570 329b d6d9 e1e0  .F.L..i..p2.....
+0000fcc0: 7d4d 4f9e a167 8502 1733 0eab ef82 bd0f  }MO..g...3......
+0000fcd0: 5bb5 61d2 0eb4 8107 a324 c3a7 dd23 d967  [.a......$...#.g
+0000fce0: e7f3 3ca7 1c72 5514 6439 df40 72a1 2a06  ..<..rU.d9.@r.*.
+0000fcf0: 8cb7 e116 ae0c 17c4 2bde 947c 957e e959  ........+..|.~.Y
+0000fd00: b741 04c3 5227 df41 2dcf 8e9d d487 a5ae  .A..R'.A-.......
+0000fd10: 183f 3175 121d 878e 4e3a 1d9f 4500 27de  .?1u....N:..E.'.
+0000fd20: 8657 f8c8 7b95 7c21 898d f265 9b8d a5a9  .W..{.|!...e....
+0000fd30: 2746 b716 3dde a39e 6c1a 2fe4 d092 043e  'F..=...l./....>
+0000fd40: b7a4 097f 9177 9324 3e5e cd56 cbd9 244b  .....w.$>^.V..$K
+0000fd50: 3029 e298 449a 2e97 2259 a40b 91a5 f9b1  0)..D..."Y......
+0000fd60: c816 f10c 5738 5ba6 6936 ea55 798d f7cc  ....W8[.i6.Uy...
+0000fd70: 1a51 c7c1 2fc6 937b 56d4 289d 4e47 1316  .Q../..{V.(.NG..
+0000fd80: 15e7 f7b5 124d 5644 288f a722 9bcf 5124  .....MVD(.."..Q$
+0000fd90: 2413 b18c 67a9 5824 f1ec 7831 8b29 5fcc  $...g.X$..x1.)_.
+0000fda0: 8644 2f31 f4ba 5d1b fe87 2cf9 6dbf 36ba  .D/1..]...,.m.6.
+0000fdb0: f134 5bac 305e 8ae9 7c2e 4592 2f63 b144  .4[.0^..|.E./c.D
+0000fdc0: b912 4542 73b9 48b3 7425 e743 d241 f970  ..EBs.H.t%.C.A.p
+0000fdd0: 69e4 ff0a eab4 4896 f30c 4914 0516 2299  i.....H...I...".
+0000fde0: c79c df22 9d0b 39cd e522 29b2 9432 1af2  ..."..9..")..2..
+0000fdf0: bb30 5db7 ff57 5439 c968 872c 3ffb 02ee  .0]..WT9.h.,?...
+0000fe00: eb9a b51e 7df3 d974 8a76 b707 ff49 faab  ....}..t.v...I..
+0000fe10: b8a0 6912 e722 c139 a78f 0b12 bc91 88d9  ..i..".9........
+0000fe20: 54d2 acc0 58e2 7c71 c8c2 3a3a 82f3 228c  T...X.|q..::..".
+0000fe30: e642 5916 bcac 94bc 0fcd 9a07 639f 50df  .BY.........c.P.
+0000fe40: a195 9655 cb6d a0de b55e e0a9 e8fa c6db  ...U.m...^......
+0000fe50: f59b d0d7 4013 3703 f676 de34 0c82 0f63  ....@.7..v.4...c
+0000fe60: d7f8 92c3 ef02 3be4 f1d1 871e 77f7 7fdb  ......;.....w...
+0000fe70: 4f47 ec0e dbdf 0f8d 338a eeee ee24 83c1  OG......3....$..
+0000fe80: 8322 e2d1 3adf 8dd0 bfbf 7d30 ffc2 e7d9  ."..:.....}0....
+0000fe90: e42f 167f 0074 23cc e06c 8739 789c eb13  ./...t#..l.9x...
+0000fea0: 6c11 dcb0 8271 f326 c63b 6c00 1f56 04d6  l....q.&.;l..V..
+0000feb0: e004 8750 789c eb13 7c2e b041 8e91 5331  ...Px...|..A..S1
+0000fec0: 3a33 afa4 283f 5663 b202 abab 6a8a 8949  :3..(?Vc....j..I
+0000fed0: 8a41 6a5a 8aae b9b1 a989 ae89 a1b1 a56e  .AjZ...........n
+0000fee0: 5262 aaa9 ae69 5a72 5aa2 a579 b289 45a2  Rb...iZrZ..y..E.
+0000fef0: 91e6 e61d 8cd7 d800 6795 130a 6c4c 789c  ........g...lLx.
+0000ff00: 7b2e 7044 6043 34d3 e63a a697 ac00 2325  {.pD`C4..:....#%
+0000ff10: 04fa e003 9a43 789c 3bc8 7490 49dd d0c0  .....Cx.;.t.I...
+0000ff20: c0cc c444 213e 3e33 2fb3 243e 5eaf a092  ...D!>>3/.$>^...
+0000ff30: 41d2 c1e0 92e3 5eb1 c7ce 51fb 1257 bb7e  A.....^...Q..W.~
+0000ff40: da39 7d9f f3fc 8dea 528c 008e 9c12 17b1  .9}.....R.......
+0000ff50: 0378 9c4b 2bca cf55 d02b 2e49 2c2a 51c8  .x.K+..U.+.I,*Q.
+0000ff60: cc2d c807 5260 0e17 1757 7c7c 596a 5171  .-..R`...W||YjQq
+0000ff70: 667e 5e7c bc82 ad82 ba81 9e99 9ea1 3a17  f~^|..........:.
+0000ff80: 00b2 1a0f a2eb 0195 2378 9c7b c7f8 8e71  ........#x.{...q
+0000ff90: c22d 91bf 2edd 0af9 96ab 2e74 ddbf 1527  .-.........t...'
+0000ffa0: cff9 d0b5 fbdc 7579 00be e60d a9eb 0191  ......uy........
+0000ffb0: 0378 9c7b c7f8 8e71 c22d 11bb ed7b c29e  .x.{...q.-...{..
+0000ffc0: dc9f 7ecf 31e3 5bf1 a5b5 3ced 93bd 6c5c  ..~.1.[...<...l\
+0000ffd0: 00cd 700e 1dba 3b78 9cbd 52bb 6edc 3010  ..p...;x..R.n.0.
+0000ffe0: ecf5 150b b991 8203 3f20 c015 2912 2040  ........? ..). @
+0000fff0: 0ac3 4e8a 2008 e43d 6a25 11a1 489a 5cda  ..N. ..=j%..H.\.
+00010000: f1df 6749 ddc3 38b8 4a61 16a2 48cd ccee  ..gI..8.Ja..H...
+00010010: 8c76 8a7e 05a5 ac5d c1ac c147 860f 4d59  .v.~...]...G..MY
+00010020: 53b9 b7e8 e639 6258 945e 48ff 09de 3856  S....9bX.^H...8V
+00010030: e9d1 1aa6 13fa be9e eef1 8962 f316 3144  ...........b..1D
+00010040: 3a64 63f9 84d7 0bf2 8033 391e e82f e9cc  :dc......39../..
+00010050: 3e9e 4839 24ef 8c3e 21bf 9b59 34d9 7b9b  >.H9$..>!..Y4.{.
+00010060: 60bf 9dba 7e3b 2b72 78b0 34a0 d087 488f  `...~;+rx.4...H.
+00010070: d944 5a45 b200 bfa0 4d74 a66d f0d2 8e14  .DZE....Mt.m....
+00010080: 364e 0446 9a60 a6eb 1eba fe63 03b2 2271  6N.F.`.....c.."q
+00010090: 8eee ad2e 958e 844c 4351 1c34 5a6b dc7c  .......LCQ.4Zk.|
+000100a0: a117 c5d5 8f64 bb7e b715 ed4b 186d db5e  .....d.~...K.m.^
+000100b0: 02a9 1da8 aa9a ce26 057a 8510 d140 d114  .......&.z...@..
+000100c0: 3f68 5566 2301 1b3a 336e 5f78 f1ee eef3  ?hUf#..:3n_x....
+000100d0: edb7 26d4 5709 2058 b17a f920 2e6f e0a7  ..&.W. X.z. .o..
+000100e0: cfa0 51ac d4b6 8117 aa7d c903 02a6 5476  ..Q......}....Tv
+000100f0: f95a bb69 8a42 3556 8296 adab 5938 5c69  .Z.i.B5V....Y8\i
+00010100: dfbe 2ad2 eeea fd48 4947 13d8 78b7 6f3f  ..*....HIG..x.o?
+00010110: 1deb 425a c85a 053f 52a9 65aa fe96 0ec1  ..BZ.Z.?R.e.....
+00010120: 2601 daaf 2bba 3129 f8ea 4266 61f8 6c47  &...+.1)..Bfa.lG
+00010130: 3810 203c a135 e315 5070 13bc 888d 6774  8. <.5..Pp....gt
+00010140: 5cf4 126d 3e7c e6c2 f7d3 46cc b4ab b0a3  \..m>|....F.....
+00010150: 5e88 32a5 60b8 c0e0 d9f0 020f f5aa 534a  ^.2.`.........SJ
+00010160: f50f ea68 62ca 4eef 5f79 5331 bb5d d3ff  ...hb.N._yS1.]..
+00010170: d7fc bec3 48fd 3aff a2df 7d9d aaa6 f907  ....H.:...}.....
+00010180: 8fbe 5167 ba26 789c 8d90 4f4b c430 10c5  ..Qg.&x...OK.0..
+00010190: effd 14a1 a714 245d f5b6 d08b 7a58 4111  ......$]....zXA.
+000101a0: 5d2f 2212 d224 ed0e e6cf 9aa4 8722 7e77  ]/"..$......."~w
+000101b0: 63da ba6e a968 6e99 79bf 9979 af71 5623  c..n.hn.y..y.qV#
+000101c0: c54c cb77 0c0c e556 ebce 40e8 49fc 07aa  .L.w...V..@.I...
+000101d0: a5f7 ac95 7407 3e58 07d2 23d0 7beb 02da  ....t.>X..#.{...
+000101e0: dedf 5c46 c1ed d0df a476 9f35 5fc3 48cd  ..\F.....v.5_.H.
+000101f0: f86b eb6c 67c4 a456 4a8f 237a 6aa1 05c3  .k.lg..VJ.#zj...
+00010200: 5496 8d3d eb47 8c74 0194 27a2 9ea8 5686  T..=.G.t..'...V.
+00010210: 6f4a d459 7c42 36a9 ba70 5b8f 8b75 86e2  oJ.Y|B6..p[..u..
+00010220: db3b 3001 e79b ebed e3dd c313 baba c84f  .;0............O
+00010230: 6693 7051 2425 b7c6 481e c01a 542d 1bc2  f.pQ$%..H...T-..
+00010240: 49e7 632d 8a28 882a 6735 3f3d 3b8f 230f  I.c-.(.*g5?=;.#.
+00010250: 30f5 21ae 6cab 26f7 6f0a 825c 9765 f93e  0.!.l.&.o..\.e.>
+00010260: dff8 910f 3ba1 414a 1a7c a0c9 68c3 17a8  ....;.AJ.|..h...
+00010270: aad0 6af0 707c 1d61 424c 6ef1 4294 cfab  ..j.p|.aBLn.B...
+00010280: 9722 4b9c 93a1 73e6 073a 9487 e0b8 92cc  ."K...s..:......
+00010290: 0dd1 cd22 fb3d 5292 205c fc25 fbcf 859f  ...".=R. \.%....
+000102a0: f97d d72f b8d6 0278 9ced 574b 8fdb 3610  .}./...x..WK..6.
+000102b0: befb 5710 3e49 cd46 4872 5cc0 c716 4d90  ..W.>I.FHr\...M.
+000102c0: 1712 2f7a d82e 085a a22d 66f9 1048 2a5d  ../z...Z.-f..H*]
+000102d0: fdfb 0e49 917a 39b1 9383 1ba0 f6c1 9686  ...I.z9.........
+000102e0: 33df 3c38 fc86 de6b 2550 5170 2e10 138d  3.<8...k%PQp....
+000102f0: d216 fdb6 da7b 1931 8619 4ba4 1d16 fa95  .....{.1..K.....
+00010300: b226 16d7 b0a8 74b7 582c 485b 3155 586b  .&....t.X,H[1UXk
+00010310: e292 a54f 165b 854d 4369 594f d58c 4df0  ...O.[.MCiYO..M.
+00010320: 61d9 293a 8319 9ca6 a5d2 5554 f532 5c11  a.):......UT.2\.
+00010330: 4b56 49ef d0b2 c2b0 8324 3c01 fa37 5c13  KVI......$<..7\.
+00010340: 5971 aa57 ab18 4ead 29a9 983c 44db a63b  Yq.W..N.)..<D..;
+00010350: 1041 a395 604f 4e39 6933 41e3 b306 2425  .A..`ON9i3A...$%
+00010360: a2c3 d632 6e8a 6a37 aac0 6a08 67be 6a3a  ...2n.j7..j.g.j:
+00010370: 63a9 c046 b5b2 c25c 95c4 3225 6fc0 5b89  c..F...\..2%o.[.
+00010380: 436e 23e1 97d6 586c 4a4d a934 b5b2 b821  Cn#...XlJM.4...!
+00010390: b6be 4133 01b8 aae8 1e35 5a95 d418 ec4b  ..A3.....5Z....K
+000103a0: 9259 f248 4796 9bad 6ee9 0d0a d210 80d7  .Y.HG...n.......
+000103b0: dbfc 41b8 8185 4a49 7044 be52 cc04 39d0  ..A...JIpD.R..9.
+000103c0: 20ce 6f57 083e 07ae 7650 cb71 a99d 387c   .oW.>..vP.q..8|
+000103d0: 5b28 05b8 618d 0b18 6d66 7b97 1dc9 2a0f  [(..a...mf{...*.
+000103e0: 866c bf8c e636 2c2d 705f 2d81 8f56 b187  .l...6,-p_-..V..
+000103f0: f65f d0c7 98c9 a6b5 60bb befb fcfb a75b  ._......`......[
+00010400: b47e 3641 fd5e 1c31 8c01 e519 c0a0 bf25  .~6A.^.1.......%
+00010410: fa60 6baa 91da a3a3 98af 56c9 b96a 6df0  .`k.......V..jm.
+00010420: 9e8e 4f96 d06e d081 5aec 4f8f 803d 838a  ..O..n..Z.O..=..
+00010430: c753 94e5 452f 31bd 1267 144c f3c5 b66f  .S..E/1..g.L...o
+00010440: 66ef 4326 498e 28ec 227a af24 cd5d 43f6  f.C&I.(."z.$.]C.
+00010450: e9ce f67a 48b6 6cb5 065f bc8b 4119 88fe  ...zH.l.._..A...
+00010460: 8c40 13c0 3282 01dc 9785 9884 03d0 4b7f  .@..2.........K.
+00010470: f7cf 5f3e 1425 c407 e2fb 170f 13e3 a536  .._>.%.........6
+00010480: 7081 505f 6976 1c27 5f4d ccbf 9347 c929  p.P_iv.'_M...G.)
+00010490: d159 3e51 df2b 8d62 a44c 1e71 3ecd ec84  .Y>Q.+.b.L.q>...
+000104a0: 0752 5551 9af5 bff9 b9d1 8d6d ff6c 0591  .RUQ.......m.l..
+000104b0: effa 97be 4e9b fb71 591f f23e ef33 1187  ....N..qY..>.3..
+000104c0: 4e0d 355b 74ef 5421 6e4e f0d1 6806 adb9  N.5[t.T!nN..h...
+000104d0: feab 569c a2b7 6fdf a10f 77db 8f77 dbf5  ..V...o...w..w..
+000104e0: 59ed 9d0f 6775 cacf c3bc 01ea 308d 9286  Y...gu......0...
+000104f0: 6247 d45d 4105 8393 901a 5942 8733 833d  bG.]A.....YB.3.=
+00010500: 49fa d122 5445 3926 a565 d015 f9b0 4309  I.."TE9&.e....C.
+00010510: c69f 93cd 6c0e 8d6a 30ea 194f a99c 7481  ....l..j0..O..t.
+00010520: 6ef2 e976 c749 d340 964a 8021 d578 3125  n..v.I.@.J.!.x1%
+00010530: 8128 c269 c73b f534 3177 e764 bc58 58f5  .(.i.;.41w.d.XX.
+00010540: 9113 26b7 de15 da00 d5ac 97fd 3535 31d4  ..&.........551.
+00010550: 7af5 71f0 49f5 481a 612c ccf2 1825 3891  z.q.I.H.a,...%8.
+00010560: fbd1 5730 c98e 2f88 d6b0 b2e0 8a54 d9a4  ..W0../......T..
+00010570: b4df d675 8e66 50ff d40c ba66 ace4 9a66  ...u.fP....f...f
+00010580: d79a 6e1e a54f 1ea6 6f61 38a5 4df6 a278  ..n..O..oa8.M..x
+00010590: 3945 3add 3ed0 7b4d 43ab d840 4399 d2a3  9E:.>.{MC..@C...
+000105a0: 0b70 47ca 471c 2e05 ae49 e2ed a0d8 fa27  .pG.G....I.....'
+000105b0: 18a9 1a22 dc0c d5cc bf65 0d97 19a2 a323  ...".....e.....#
+000105c0: c7c1 b717 69ab 1f68 909f a9da cfd6 ca65  ....i..h.......e
+000105d0: 7aba 54b3 5bcc 3042 5c91 4ecd f5f5 6b7f  z.T.[.0B\.N...k.
+000105e0: 55f2 d307 91d1 a42c 3c91 77aa 4556 010d  U......,<.w.EV..
+000105f0: 082a 7690 2b7a e394 0de9 907a 2cd6 632a  .*v.+z.....z,.c*
+00010600: 7324 f6fa 3d70 18ca 3ce0 8094 03ab 25df  s$..=p..<.....%.
+00010610: f905 c7fc b13b 601e 6e98 1721 fae8 e717  .....;`.n..!....
+00010620: 22e9 4b1c a62b 47a3 5f84 a3d3 d3b8 2257  ".K..+G._....."W
+00010630: aefe 0fb9 7ad8 9b29 69fb 3a79 88d3 941d  ....z..)i.:y....
+00010640: feda 5f90 47d3 dfa0 0bd1 e679 fb76 e5cc  .._.G......y.v..
+00010650: 2b67 5e39 f3ff c499 ff02 5136 db93 e002  +g^9......Q6....
+00010660: 863a 789c 7ba1 7559 6b43 2dfb e618 a142  .:x.{.uYkC-....B
+00010670: c6cd 5f39 7458 802c 1ee6 cd26 028a 4c60  .._9tX.,...&..L`
+00010680: 1600 cae7 0a31 e523 2878 9cbb acf5 d770  .....1.#(x.....p
+00010690: c31e 4689 9cc4 e292 f8c4 ccf8 a2d4 e282  ..F.............
+000106a0: fcbc e254 055b 05bf fcbc 54ae c93b 190b  ...T.[....T..;..
+000106b0: 8574 14d0 a537 6b31 35b2 b072 2900 c1e4  .t...7k15..r)...
+000106c0: 956c 87c4 d373 f293 1273 3094 4d8e 63d7  .l...s...s0.M.c.
+000106d0: 6256 c82f 9a9c cb2e 2986 2e69 05d1 de28  bV./....)..i...(
+000106e0: 62a5 0862 6071 414e 4e6e 7c7e 6949 4169  b..b`qANNn|~iIAi
+000106f0: c9e6 ddec b798 a441 ca70 d9e4 28a0 b079  .......A.p..(..y
+00010700: 2b57 2c23 33c8 4c7b c16f f470 9231 e3e6  +W,#3.L{.o.p.1..
+00010710: 6ebe cd8c 930f 0888 cb42 b4e2 76dd 44ad  n........B..v.D.
+00010720: e2e4 a2d4 d4bc e28c fc92 f882 c492 0c4d  ...............M
+00010730: 2e2e b016 6585 a0d4 dcfc b254 8592 8c54  ....e......T...T
+00010740: 85cc dcc4 7460 a0ff 6376 9c9c cc62 3a99  ....t`..cv...b:.
+00010750: 8945 68f2 2616 d5c9 8eac d293 7fb1 f04c  .Eh.&..........L
+00010760: e663 d506 b24d 8058 7df2 1220 5ec1 9dc9  .c...M.X}.. ^...
+00010770: 0276 b183 e057 ba79 781e 2300 5f6c c101  .v...W.yx.#._l..
+00010780: b9c2 0578 9ced 5a6d 73db 3612 feae 5f81  ...x..Zms.6..._.
+00010790: 533e 986c 64d6 961d 5fea 19df 4cde e369  S>.ld..._...L..i
+000107a0: 7295 2de7 7adf 3810 0949 a829 8205 40cb  r.-.z.8..I.)..@.
+000107b0: eadd fdf7 db05 f802 bec8 b253 a7c9 dd54  ...........S...T
+000107c0: 93c8 24b0 bb58 3cbb 582c 169a 4bb1 2201  ..$..X<.X,..K.".
+000107d0: 5db0 5407 d192 ea70 c995 1672 43f8 2a13  ].T....p...rC.*.
+000107e0: 5293 ef06 7387 822a 05dd 34d5 edee 2459  R...s..*..4...$Y
+000107f0: 6de1 c0ef feae 198d ae17 52e4 695c f717  m.........R.i\..
+00010800: 048b 9c07 8a2f 529a b459 b167 966b 2dd2  ...../R..Y.g.k-.
+00010810: 0e53 ae79 a282 78e6 7414 4f4b aa96 099f  .S.y..x.t.OK....
+00010820: 95af 6aa3 ca47 bd94 8cc6 3c5d 940d 33aa  ..j..G....<]..3.
+00010830: d8c9 71d5 cd57 ac7c 9634 8dc5 aa7c 4bf3  ..q..W.|.4...|K.
+00010840: 55b6 2154 9134 abc4 e254 6276 c323 861d  U.!T.4...Tbv.#..
+00010850: 2a6e 74cc 7962 9be7 8342 e16c b3a0 2b56  *nt.yb...B.l..+V
+00010860: 6abb e2b7 4c96 1c2b aa97 9668 b2b9 d0cf  j...L..+...h....
+00010870: 820b fd33 8f17 4cab 92fa e245 9625 3ca2  ...3..L....E.%<.
+00010880: 9a8b 7444 2e3e 529e fecc 41bf 35bc fce3  ..tD.>R...A.5...
+00010890: a5b8 fd40 3722 d7f0 62f9 9ab2 dee5 bc92  ...@7"..b.......
+000108a0: f351 e48a bdb9 017b 00f1 04c4 6826 f189  .Q.....{....h&..
+000108b0: a1d8 9732 572d 3d5e 0959 a97c 813c 5700  ...2W-=^.Y.|.<W.
+000108c0: 1172 5cb2 085e b3cd af7a 6a0c 074d 3fcd  .r\..^...zj..M?.
+000108d0: 7e81 c6ed 63ff c836 53f6 6bce d288 dd3d  ~...c..6S.k....=
+000108e0: d9e9 12fe 44b9 2ee1 1195 fd54 c4b3 4dc0  ....D......T..M.
+000108f0: 45b0 a637 25c2 c5e3 e031 0144 4800 8b97  E..7%....1.DH...
+00010900: c6f3 e0e5 039d 319c e2fb 8a74 074c 1301  ......1....t.L..
+00010910: d0ee 50e9 35a7 8958 b415 2887 fac0 53f6  ..P.5..X..(...S.
+00010920: 26e6 4d55 1c81 f570 855c 2044 b8b7 e37f  &.MU...p.\ D....
+00010930: 1e81 00fb c924 a8e7 0dcf 4d0f 8b09 4d12  .....$....M...M.
+00010940: 022b 4652 c999 1afa 83c1 a077 249c a615  .+FR.......w$...
+00010950: a0e5 e674 40e0 53f4 457a 9331 655a 561b  ...t@.S.Ez.1eZV.
+00010960: 9a65 3c26 6764 4fa4 b9a4 9a5e d334 5864  .e<&gdO....^.4Xd
+00010970: 3a8c c42a cbc1 e1c2 2aae 98f5 7db8 479e  :..*....*...}.G.
+00010980: 102a 675c c3f8 1ba2 b4c4 058a a2ac d460  .*g\...........`
+00010990: 0d96 4a92 402d 5992 1c8d 8329 d3af 7229  ..J.@-Y....)..r)
+000109a0: c187 2752 444c a937 b768 5bae c1c6 9f14  ..'RDL.7.h[.....
+000109b0: 931f 45cc 92f3 d75e a188 3f60 b711 cbb4  ..E....^..?`....
+000109c0: d537 83b1 41fd 250b 790a ca84 3371 0b9a  .7..A.%.y...3q..
+000109d0: fe5d a438 b128 815e 523b 87e7 388a 6ff9  .].8.(.^R;..8.o.
+000109e0: 6336 2721 f072 1d86 9e62 c9bc 68c7 8fca  c6'!.r...b..h...
+000109f0: 3326 3d3f a8fa fdba 0b28 03c5 b495 f536  3&=?.....(.....6
+00010a00: a10b e55d e8e0 ad84 9090 c014 6cfb 7bb0  ...]........l.{.
+00010a10: 0af9 3700 1dd8 f7a9 a61b f553 7a25 32ec  ..7........Sz%2.
+00010a20: f109 e074 c956 e286 41a4 d2e0 fd33 2a09  ...t.V..A....3*.
+00010a30: 8429 90ae c9da 7010 2dc0 986b 6023 1032  .)....p.-..k`#.2
+00010a40: b5c8 2a0d 5aaa 68aa 199a 88c7 09db 43c1  ..*.Z.h.......C.
+00010a50: 1301 4699 8150 d3a5 4e8b ae11 d9d3 34b9  ..F..P..N.....4.
+00010a60: 068b 98c7 254f cd73 535a 9627 8a85 183d  ....%O.sSZ.'...=
+00010a70: 6509 66a3 1fe1 f874 de86 c3c6 f570 0933  e.f....t.....p.3
+00010a80: 480c a3f5 f1f7 f6dd 826b 3443 a380 c5c8  H........k4C....
+00010a90: 7a29 40bf da24 44d8 88d3 902a 9238 cc84  z)@..$D....*.8..
+00010aa0: e2b8 d241 a6d5 4f28 cf88 7a2b 2401 fc60  ...A..O(..z+$..`
+00010ab0: 0605 5e83 caa8 858e 6d93 36ec 7685 a87b  ..^.....m.6.v..{
+00010ac0: 7bef 2657 fbc7 62af 6bdd 774c ac18 2c0d  {.&W..b.k.wL..,.
+00010ad0: eff0 e060 44cc d7b8 f832 c3bf 887f c995  ...`D....2......
+00010ae0: 3673 51fc 3713 bd52 c662 16d7 56aa 9ec0  6sQ.7..R.b..V...
+00010af0: 7743 1e99 3998 651c 98f5 eb60 5812 0434  wC..9.e....`X..4
+00010b00: 8edf 4200 f4f0 253c 3c09 33d8 4d46 c56a  ..B...%<<.3.MF.j
+00010b10: 0d2e a630 9077 7832 3a3c f177 f18e 8ffb  ...0.wx2:<.w....
+00010b20: 78c7 c7a3 f1f1 4ede a371 1fef d178 7434  x.....N..q...xt4
+00010b30: dec9 7bfc bc8f f7f8 f9e8 f8f9 6e9d 9ff5  ..{.........n...
+00010b40: 4e18 9a47 f0df dfb6 020d 96a5 44bf 463d  N..G........D.F=
+00010b50: 82a8 2269 12ae 4d4c 45ec 6d74 b57e d111  .."i..MLE.mt.~..
+00010b60: f6ca 9217 344d e69a 3a31 b11d 85d5 91be  ....4M..:1......
+00010b70: 435c 513f 21af c049 20f8 566b bc39 ac69  C\Q?!..I .Vk.9.i
+00010b80: 0e71 e9df a95d 4586 7abe 856c 237e cff8  .q...]E.z..l#~..
+00010b90: 62a9 bdb1 f545 88a2 8492 3976 90a5 e921  b....E....9v...!
+00010ba0: 7358 1de8 9bbb 060e eb09 d51b a2d7 a4d9  sX..............
+00010bb0: a64d c16b c013 907d a45a 7da4 72c1 53e5  .M.k...}.Z}.r.S.
+00010bc0: c142 29fe dd83 799a d108 96b1 77e0 20e7  .B)...y.....w. .
+00010bd0: 1027 b88b a282 663b f586 76c9 0e47 e42e  .'....f;..v..G..
+00010be0: a44a f1e0 600e aeae c4f6 6051 2220 f015  .J..`.....`Q" ..
+00010bf0: 09ea 99bb 537b c37f f68f e6b2 54a6 b13e  ....S{......T..>
+00010c00: 6b22 c55d e411 6c73 d72c 0ec0 6753 087c  k".]..ls.,..gS.|
+00010c10: 5e4d f1c0 29b9 5271 b76f 7a6a 3f00 c6a8  ^M..).Rq.ozj?...
+00010c20: 8e97 be88 6322 c05d 24f9 744e 6013 5ba1  ....c".]$.tN`.[.
+00010c30: 2d09 8084 bbd0 762f 322c bbd6 57bf 1e2e  -.....v/2,..W...
+00010c40: 6bdb 1295 4bda 8741 67a9 165e 6abb 3b13  k...K..Ag..^j.;.
+00010c50: b966 9b99 a012 b6d2 22f7 542d 0145 73a8  .f......".T-.Es.
+00010c60: 22c9 580a af46 f932 53f5 dce4 d61b bed2  ".X..F.2S.......
+00010c70: 3279 7a38 f47b 1da0 4754 4023 cd6f 60db  2yz8.{..GT@#.o`.
+00010c80: ad4d 9bd0 d52c a6a7 7d3b 6580 9b88 c3ed  .M...,..};e.....
+00010c90: f97e 39c0 ef56 7afc c594 d662 b100 2f92  .~9..Vz....b../.
+00010ca0: 2c12 124f 601e e485 2c84 b399 66ab 90e6  ,..O`...,...f...
+00010cb0: 3117 6757 3267 7edb b0d5 c8a9 78c0 3cd8  1.gW2g~.....x.<.
+00010cc0: ae79 34a4 7dd3 5339 fa43 a7d2 1056 4dc3  .y4.}.S9.C...VM.
+00010cd0: 5d2e e770 e282 3415 124d a0c3 2c92 1293  ]..p..4..M..,...
+00010ce0: 4a13 4ca5 a175 2634 ee5e 099b 6b93 9c52  J.L..u&4.^..k..R
+00010cf0: 1818 fe14 41b2 2690 b8e7 d482 dd74 bc3a  ....A.&......t.:
+00010d00: fcb4 c242 4583 0b7a 92d0 8841 4618 3379  ...BE..z...AF.3y
+00010d10: c56e e134 7305 8705 d8ca 24d8 be9f a34a  .n.4s.....$....J
+00010d20: cf8e 0e2c a281 ddf8 2037 dc27 2765 b276  ...,.... 7.''e.v
+00010d30: e484 e045 2266 3421 8de3 42d5 d93e 44d4  ...E"f4!..B..>D.
+00010d40: 14f5 ac6c 6659 b487 0884 e764 9746 4387  ...lfY.....d.FC.
+00010d50: 20d0 3811 9ffc e58c 0c87 4db2 caec 2d03   .8.......M...-.
+00010d60: 5a5e c3d7 16e3 7704 34d0 b0a0 0dbb 5477  Z^....w.4.....Tw
+00010d70: 69df 083b 5f68 22ee 188f 37a7 beed c2d9  i..;_h"...7.....
+00010d80: 602a 31cd 4cac f470 586b fc37 c857 c019  `*1.L..pXk.7.W..
+00010d90: 8a0d a624 2aa6 d19b 12f5 c932 c97f bd20  ...$*......2... 
+00010da0: 1cb5 00dd fe4c 620a 5d3d c944 45df c90b  .....Lb.]=.DE...
+00010db0: 9a36 dbaa 451d 82da ba54 3d5b 347a 3aad  .6..E....T=[4z:.
+00010dc0: 28ba 8ab5 9977 a8e7 98bb b32d a39a 5688  (....w.....-..V.
+00010dd0: c2c8 81af f7b4 4423 77a8 90f2 7713 b7b5  ......D#w...w...
+00010de0: f76d c1a3 e13d 55e8 6558 3fdb 15c0 2f99  .m...=U.eX?.../.
+00010df0: ce65 ba2b 8a1b 513d d1fb 0eb0 3e4f a7c7  .e.+..Q=....>O..
+00010e00: 54c7 ef62 5323 5a2c 8206 d27e 0f94 eb72  T..bS#Z,...~...r
+00010e10: 9d60 b859 6181 7222 b1aa 8355 4ab3 018c  .`.Ya.r"...UJ...
+00010e20: 08c3 e753 b77c e904 1f08 3ca6 bf88 2810  ...S.|....<...(.
+00010e30: 76ce f0cc 1c7c 801d c83a 6c33 02f5 9509  v....|...:l3....
+00010e40: ac00 1bee 2758 2d68 69f4 51dc b07b 2b14  ....'X-hi.Q..{+.
+00010e50: b344 53b3 64b0 0ae8 7564 c36e d3d1 c1df  .DS.d...ud.n....
+00010e60: 361d d533 9fa2 e8d3 38e5 e569 8ca5 2f50  6..3....8..i../P
+00010e70: a71d 980d 2156 8d6c 167d 0b02 9f5a 1df1  ....!V.l.}...Z..
+00010e80: b9d8 0937 4eeb a61d 671f 8858 8675 e50e  ...7N...g..X.u..
+00010e90: 5a8e 5699 2d3c 1b88 ec63 6ba3 2f08 30a4  Z.V.-<...ck./.0.
+00010ea0: 5f32 9c18 d6bf bc92 3878 916a 4e13 4e15  _2......8x.jN.N.
+00010eb0: 642c e630 fb26 a558 baa2 4ebb 39cd aa95  d,.0.&.X..N.9...
+00010ec0: 8043 0361 b0b4 559f f009 4bbd 0bf3 0570  .C.a..U...K....p
+00010ed0: 433e 713d 22cf b192 104c 45c2 63cc 42fc  C>q="....LE.c.B.
+00010ee0: 5ea5 4ca5 dcbb 28fe 54bc 25e3 846a 204c  ^.L...(.T.%..j L
+00010ef0: fd56 6101 0e2f 9827 1c1e 1c98 5a94 397a  .Va../.'....Z.9z
+00010f00: db76 72bb 1f09 9381 c162 6bf3 6c80 e787  .vr......bk.l...
+00010f10: 2ecb c665 71bd c72d f09d d5e5 bba6 533c  ...eq..-......S<
+00010f20: 21af 255d c3ce 86b5 3baa 11b0 88cb 0840  !.%]....;......@
+00010f30: 5c73 40ac 04ce 4249 53be 32a5 f386 0849  \s@...BIS.2....I
+00010f40: 639e abf0 864a 4e0b a778 46be 23de 2138  c....JN..xF.#.!8
+00010f50: 12de 6804 c0eb 39f5 c139 163b 81c0 f465  ..h...9..9.;...e
+00010f60: 9c7c 8f48 b43c cdca 0449 7f3d 0029 ed11  .|.H.<...I.=.)..
+00010f70: 1aa4 a539 6298 c79b 24e1 1978 3e7a 4985  ...9b...$..x>zI.
+00010f80: f47e 29ed 7b32 0637 77fa 367d 7db6 a1f9  .~).{2.7w.6}}...
+00010f90: 522b c792 1e64 cb6a 681b da15 5e07 283c  R+...d.jh...^.(<
+00010fa0: 08ff 89ee 9de8 3af0 2a76 ba4d d7af 68f6  ......:.*v.M..h.
+00010fb0: 5631 c6d8 104f 4b26 d3bb b41b e217 03a5  V1...OK&........
+00010fc0: 58a3 0a0e 6718 ef57 34c1 3a79 e148 4562  X...g..W4.:y.HEb
+00010fd0: 4675 f33c 55e9 8bd4 a113 75cc 04d6 3cd6  Fu.<U.....u...<.
+00010fe0: 4bb3 011d 1df4 936e 4a52 e768 f443 9bb6  K......nJR.h.C..
+00010ff0: b2cd f859 273a b6ed d252 64bf 29a2 c6a2  ...Y':...Rd.)...
+00011000: a5c5 0eba 0672 8da6 6db6 2be4 6fb1 e01f  .....r..m.+.o...
+00011010: afe5 e073 ed8c 07eb ed66 3e3a 685c 3470  ...s.....f>:h\4p
+00011020: 4512 ee5e c7fc 9fd9 fa0e 1b9b 02c4 d7b6  E..^............
+00011030: f103 4dac 45f6 c8f6 3d71 e859 bc95 e37f  ..M.E...=q.Y....
+00011040: daca 21c2 f66d 5b1a 030e 4d17 1d63 3f34  ..!..m[...M..c?4
+00011050: 683f b2f1 7b6d fd35 61ec 3134 4217 1a9c  h?..{m.5a.14B...
+00011060: be01 3b57 c095 f11b cf3b 7916 434a 189a  ..;W.....;y.CJ..
+00011070: c4b0 38f1 a46c 6ddf 3b77 c9c5 c57b 4550  ..8..lm.;w...{EP
+00011080: 9bc0 fc26 633e 9c1a 0a2b 333e 25ff aa28  ...&c>...+3>%..(
+00011090: ff33 6c1c 12ab f63b b2fc 4e7e 7846 9ad9  .3l....;..N~xF..
+000110a0: 5499 d43a 37f8 5bca 750e 054c 4264 5eb7  T..:7.[.u..LBd^.
+000110b0: c8b6 ebb7 005b 68ec 6f8a 5a27 c0de 71f1  .....[h.o.Z'..q.
+000110c0: 1b8b 0b8d fb2f 4b60 c3c1 0e7e 804b 6aef  ...../K`...~.Kj.
+000110d0: 592b ab6f 01d9 9fd4 ff89 640f 92ee 6d65  Y+.o......d...me
+000110e0: 7d40 da8a c07d 667f afdf 93d8 c561 7fd2  }@...}f......a..
+000110f0: 7105 a161 0174 1462 ac89 624e 1dc2 994f  q..a.t.b..bN...O
+00011100: ef0f 3b5c 7b3e 8583 79e7 14ed 12fc cd9c  ..;\{>..y.......
+00011110: dc1f e015 0d55 7f6f 85ab 7dfe 40cb 698a  .....U.o..}.@.i.
+00011120: d7e6 b610 637e e2d2 57f8 d975 e113 839c  ....c~..W..u....
+00011130: 50d1 1b16 c229 74c1 ec95 4fdf b1b7 9d3f  P....)t...O....?
+00011140: 3f9a 063d 574e bbc6 c75d ffd1 c6df 727b  ?..=WN...]....r{
+00011150: 771f 1d70 47fa 5c3d 3ab7 b883 ad23 36b7  w..pG.\=:....#6.
+00011160: c0cf 1d50 318d 9508 1566 22cb 3377 3cfc  ...P1....f".3w<.
+00011170: 0c9a 9fff 020c 520d 1cb6 f502 789c ed58  ......R.....x..X
+00011180: 4b6f e336 10be eb57 10ce 2152 61e8 d64b  Ko.6...W..!Ra..K
+00011190: 001f b29b b44d 9b87 9d35 ba47 8296 689b  .....M...5.G..h.
+000111a0: 8d4c 0a12 b589 51f4 bf77 48bd f890 6c2b  .L....Q..wH...l+
+000111b0: d7d6 2791 9cf9 389c f966 3874 b02d c401  ..'...8..f8t.-..
+000111c0: c525 db71 9221 76c8 4521 d14f 4150 4fc7  .%.q.!v.E!.OAPO.
+000111d0: a44a 9988 0b9a 8822 f557 cba4 a094 c7e5  .J.....".W......
+000111e0: 5ec8 01d5 1de5 32ce 0b91 24b4 2cc7 d693  ^.....2...$.,...
+000111f0: 3d91 78cf 4a29 8a63 2b93 6494 14d8 5c09  =.x.J).c+.d...\.
+00011200: 8266 293f 924a 8a5d c582 da26 c677 58ee  .f)?.J.]...&.wX.
+00011210: 0b4a 52b4 40cf 82d3 a0c3 af24 cbca 38dd  .JR.@......$..8.
+00011220: b4a8 b5b1 ca56 9c13 b99f a392 fca0 98e4  .....V..........
+00011230: 0cbf d1e3 1c65 82a4 fd88 2492 fd20 92e2  .....e....$.. ..
+00011240: bfaa 5262 493f 243e 8894 6673 94d2 f135  ..RbI?$>..fs...5
+00011250: 56ba 7358 0b53 d88c c2b6 85d8 b20c 06bb  V.sX.S..........
+00011260: 7e70 c295 92bc 51dc 5b1d 04ed d996 c795  ~p....Q.[.......
+00011270: fc39 5ec9 ef2c 05a4 ceb5 ab3b 4632 b19b  .9^..,.....;F2..
+00011280: a3d5 9f5f c4c7 2339 8a4a c2e0 916c 946d  ..._..#9.J...l.m
+00011290: ab47 c6e9 7dca d4d4 b22a f75f 2a29 0507  .G..}....*._*)..
+000112a0: c824 2310 9e7a f81b e169 468b 30ba 0910  .$#..z...iF.0...
+000112b0: fc52 ba45 1833 ce24 c661 49b3 ed1c 1d08  .R.E.3.$.aI.....
+000112c0: e3f8 9df1 54bc 3742 eaa7 d6e2 2e22 108a  ....T.7B....."..
+000112d0: 5f48 5652 7bd9 d004 0163 648b 29c2 005f  _HVR{....cd.).._
+000112e0: b066 9e1b db4e 52d3 15ef 6b73 fb9d 7129  .f...NR...ks..q)
+000112f0: 4921 691a 2782 739a 486d 742c 38f6 24a2  I!i.'.s.Hmt,8.$.
+00011300: 4bb0 449e 9fc1 d212 a358 e058 e02f e1c0  K.D......X.X./..
+00011310: 883d e36f a0e2 81f9 2217 a015 b4cc 052f  .=.o...."....../
+00011320: 2956 ce39 9ec0 b405 a720 8f1d 7e5c 340a  )V.9..... ..~\4.
+00011330: 828e 3490 a2bb 8cf6 9e6a c8c3 85c1 e785  ..4......j......
+00011340: e6c8 bca1 f9b1 94f4 5007 bd5d 4805 eca2  ........P..]H...
+00011350: 9394 1da0 58d4 d340 baee 146c eb10 af27  ....X..@...l...'
+00011360: a43e 24d8 6598 10d9 8ba7 194b 6160 a35d  .>$.e......Ka`.]
+00011370: a135 186a 5411 b4a1 5b51 c08c 2294 c2e8  .5.jT...[Q.."...
+00011380: d02c 3d30 9283 b075 741b 599b d3c3 2efa  .,=0...ut.Y.....
+00011390: 2217 f7d3 60fe 09a5 58b9 2974 2a9c a3e1  "...`...X.)t*...
+000113a0: 1fdf b209 f6b5 c681 2fef 450a 74bc 395f  ......../.E.t.9_
+000113b0: cd89 2328 3933 f656 bb4c 6ce0 2a72 ebbb  ..#(93.V.Ll.*r..
+000113c0: eb54 affe b352 1709 240a ed70 773d 86e2  .T...R..$..pw=..
+000113d0: 4c32 a8c5 61e4 bb7f e032 a93f 54ca aef5  L2..a....2.?T...
+000113e0: 5708 6186 6abb d0e1 ee69 0557 45b1 2b17  W.a.j....i.WE.+.
+000113f0: a1e7 8779 149d dd26 d660 2e33 cfd5 367a  ...y...&.`.3..6z
+00011400: 601d 1d54 b20d 9537 9d70 a70a f4ba a8c6  `..T...7.p......
+00011410: eb73 5ce5 a9ba e000 4cd2 f05a 924c 15a6  .s\.....L..Z.L..
+00011420: eb68 6c4b 9dff ee96 79c1 b80c 672f cfe8  .hlK....y...g/..
+00011430: f5fe ebcb ebdd c3f3 afe8 dbfa 65b9 bcbf  ............e...
+00011440: 9b45 9fbd 395c cb9a 9a79 1d79 4561 f01e  .E..9\...y.yEa..
+00011450: 7138 322a 384a 96f3 05be 898e 9705 23f7  q82*8J........#.
+00011460: da18 cd2c f196 649d cd56 a6ce 8793 733e  ...,..d..V....s>
+00011470: 987d d185 a675 d434 aaba ee6d 8c92 e404  .}...u.4...m....
+00011480: bcfb 701a 97d0 89f6 273d d103 5e80 679a  ..p.....'=..^.g.
+00011490: 6f1e e1e4 0d36 9834 e3e4 6340 81eb 6804  o....6.4..c@..h.
+000114a0: bbe5 c344 4c83 d067 6cd6 37fa 54f4 2e91  ...DL..gl.7.T...
+000114b0: 4d9f 406b aaee af12 e722 af72 17f2 0a7d  M.@k.....".r...}
+000114c0: 85ad 2445 a413 44a9 6e34 1124 0162 bc64  ..$E..D.n4.$.b.d
+000114d0: 2924 d416 3168 dc5b 49d5 00c3 525e 4944  )$..1h.[I...R^ID
+000114e0: 36d0 8622 9153 4e58 db5f 6b4d 8236 bae7  6..".SNX._kM.6..
+000114f0: 8466 41b7 e200 609c a331 a9d9 69d1 36b7  .fA...`..1..i.6.
+00011500: 1697 2c99 18c6 dff5 a1d7 4c66 349c 7d6b  ..,.......Lf4.}k
+00011510: d667 17a8 3c89 14d2 5d1e c395 8c6f f33c  .g..<...]....o.<
+00011520: 6309 914c 703d 6d5c a303 fa75 9b1d 1a2d  c..Lp=m\...u...-
+00011530: 7718 8d6f 9835 1231 49d3 ba7b 0feb fe1c  w..o.5.1I..{....
+00011540: ea24 78e8 f601 dd2e 1fd0 1ff4 3833 401a  .$x.........83@.
+00011550: a7e1 da9f 8bbe 930f 3d19 5835 df31 be40  ........=.X5.1.@
+00011560: 0da2 0c5f 4388 c266 7692 c116 92a1 a94a  ..._C..fv......J
+00011570: 4c13 d185 f9c4 8048 c0d2 6c50 324e c0d5  L......H..lP2N..
+00011580: 6f46 9b99 91c3 2625 37d6 dbcc de31 56dc  oF....&%7....1V.
+00011590: 021f 4fb2 d9d8 d208 e715 ba4d 8187 5055  ..O........M..PU
+000115a0: f7b4 30d8 0839 4625 3ad0 837a 79b6 c27a  ..0..9F%:..zy..z
+000115b0: 12d7 9323 e77c d57a 4f5a c438 ef80 a677  ...#.|.zOZ.8...w
+000115c0: 6eff c93b e97c 035b 5c70 4e48 c94d 4675  n..;.|.[\pNH.MFu
+000115d0: 59af 3356 3f59 3bb5 fe29 3b7c dcfb 5afd  Y.3V?Y;..);|..Z.
+000115e0: 77a5 aed8 849e 94fa ec44 be0c 58ee 6e12  w........D..X.n.
+000115f0: 59ed fde8 83da bd97 5d98 8ee1 b33b 568e  Y.......]....;V.
+00011600: 9879 52df 0dd0 f8b3 bf07 f21f 0d67 61c7  .yR..........ga.
+00011610: 418d f075 65b5 ae00 f0ea 38e8 0aaa ab66  A..ue.....8....f
+00011620: 1f4e 600f 87f6 bafd 6361 4210 da1a b4ac  .N`.....caB.....
+00011630: 55cd e2d3 a00d 169f 61a1 cef5 c6bf 1c13  U.......a.......
+00011640: 6ba2 85e7 db72 79a9 19d0 182f 3986 b9f6  k....ry..../9...
+00011650: 813e 5371 0676 ee7a a921 08fa 4113 7cea  .>Sq.v.z.!..A.|.
+00011660: 76db 8b77 bb1b d3b6 69ca 34af 6bf5 39d4  v..w....i.4.k.9.
+00011670: 8efd e77b 68e5 98ee 9da6 be3f d104 fb5e  ...{h......?...^
+00011680: 773b 612f 0093 def4 13df f2ff 0777 3cb8  w;a/.........w<.
+00011690: 73f4 f6ae c77f cf1c 2fce 6e9c 897f 2612  s......./.n...&.
+000116a0: c18e c1f8 ef5f be3c b3fb e934 8931 789c  ....._.<...4.1x.
+000116b0: 8d92 314f c240 14c7 5335 51b1 2996 8340  ..1O.@..S5Q.)..@
+000116c0: 10e3 d9c4 a42c 8d92 b8e8 a006 351a 178d  .....,......5...
+000116d0: ee97 5a0e 692c b4f6 4e03 8b8c babf c1af  ..Z.i,..N.......
+000116e0: e064 4858 9dfd 063a f801 dc9d 5dbc 42d3  .dHX...:....].B.
+000116f0: 0a18 c29b 5ef2 feff fffd eeee 7d18 df9b  ....^.......}...
+00011700: 9d55 b954 f5dd 3a36 8c2b 8f13 cbad 7bb7  .U.T..:6.+....{.
+00011710: 9cfa c464 cc66 dc6c 706c d73d d7e7 98d7  ...d.f.lpl.=....
+00011720: 28b1 1b62 482e dd66 3727 9f4f b513 38ac  (..bH..f7'.O..8.
+00011730: 0aad 6266 de51 627a 36b9 a62d a287 4d71  ..bf.Qbz6..-..Mq
+00011740: 2bd2 04f5 5713 4906 1403 a718 8cf2 0bda  +...W.I.........
+00011750: e4ba 762e 8c15 bc77 7a8c 4f68 4b0b 2d70  ..v....wz.OhK.-p
+00011760: 83b2 7396 e332 aa17 13b0 aba4 e15e 599b  ..s..2.......^Y.
+00011770: 8fce 8665 b40d 5fca ed20 a6e5 50d3 2756  ...e.._.. ..P.'V
+00011780: cde4 a426 2ee8 fa02 7688 7254 a24f 0459  ...&....v.rT.O.Y
+00011790: 0e7c 02b3 2c9c f8a8 ef14 ac33 3d56 0fe5  .|..,......3=V..
+000117a0: 6256 9c2c 4056 55e1 2199 9208 74e4 3cac  bV.,@VU.!...t.<.
+000117b0: 28a8 fb96 d424 a902 7b8b 85d9 9016 d6a5  (....$..{.......
+000117c0: a5f4 085f 1027 06a5 21aa 3164 fb36 332f  ..._.'..!.1d.63/
+000117d0: 1d1a 6423 f859 9481 a374 4c73 a61a a0ab  ..d#.Y...tLs....
+000117e0: 798d c479 d461 742b 3110 1f3c 1eb4 d55c  y..y.at+1..<...\
+000117f0: e63f 9ede 6463 72a0 83c6 589e 4389 749f  .?..dcr...X.C.t.
+00011800: d41d 6968 c328 279e ef56 6d87 123d 6c86  ..ih.('..Vm..=l.
+00011810: 172c 9644 8ac9 f7eb b4ef d022 0b30 9489  .,.D.......".0..
+00011820: b9de 53bb e2b7 32c8 824f b400 afb2 028f  ..S...2..O......
+00011830: 48ee bea0 e7e9 5f2d ecef f0b1 3a78 9c7d  H....._-....:x.}
+00011840: 535d 6fd4 3010 7cf7 af30 ee43 2f28 1f95  S]o.0.|..0.C/(..
+00011850: 2a10 8a64 4425 0a42 a22a 82f6 0155 2872  *..dD%.B.*...U(r
+00011860: 93bd 9cb9 c436 de35 ed81 f8ef f89c 0ba8  .....6.5........
+00011870: 55ef f2e0 8799 f1ee ecac 73f4 ac0a e8ab  U.........s.....
+00011880: 5b6d 2ab7 a195 35a7 ec88 17cf 0bde da4e  [m*...5........N
+00011890: 9bbe e681 96c5 ab2d c2d8 d2db 9123 5070  .......-.....#Pp
+000118a0: 64ed 805c 8fce 7a9a 10c6 ee34 adb8 7560  d..\..z....4..u`
+000118b0: 16c7 1e7e 04ed 6104 4358 d23d 1d67 5c21  ...~..a.CX.=.g\!
+000118c0: 5fba 9af1 f869 83a4 86a1 d9a9 90cb 4895  _....i........H.
+000118d0: 1e54 b7c8 582a b648 3aa3 4690 a277 d4b4  .T..X*.H:.F..w..
+000118e0: 7674 81c0 370a 51c7 cb86 449e 243f c1a3  vt..7.Q...D.$?..
+000118f0: b646 8a93 f245 79ba 033b c0d6 6b47 8910  .F...Ey..;..kG..
+00011900: e2fd a7ab 784e d460 4ddf 3ce4 cbef 569b  ....xN.`M.<...V.
+00011910: 45f2 2d3e 9f9f bdbd 382f c74e e41c cc94  E.->....8/.N....
+00011920: 8014 2901 9125 8783 3680 8b2c 7bba 5c34  ..)..%..6..,{.\4
+00011930: 6a28 0edd d0c6 45eb 04f7 548d caaf 3b7b  j(....E...T...;{
+00011940: 6776 0e82 1fa4 5811 39ac abaa 8f91 85db  gv....X.9.......
+00011950: 328e 5759 13bc 22b5 56a6 8a13 17f3 c4c5  2.WY..".V.......
+00011960: e389 5588 4bf2 525c 463d 3f4b 17f8 f5c7  ..U.K.R\F=?K....
+00011970: eb2f 975f 1f08 1a18 958e 9d62 c9ce f6ca  ./._.......b....
+00011980: 9cbc 7cd3 6f91 6daf 390b dd82 c168 f3e2  ..|.o.m.9....h..
+00011990: c3d5 0e72 aa5d ab1e 50de ec8d 9def 61ca  ...r.]..P.....a.
+000119a0: 78ef 20df 077d 808d 1102 9803 8240 7ac0  x. ..}.......@z.
+000119b0: 43ed 43a7 adf8 963f f9c2 e463 6092 45c3  C.C....?...c`.E.
+000119c0: 7ed3 b8b8 7f42 f93b 41db 4fc4 2da2 1da0  ~....B.;A.O.-...
+000119d0: 99f6 8aa2 e637 626e f9af a3dc 3709 294f  .....7bn....7.)O
+000119e0: 753a 673b 7ff2 a9f0 9471 facb fe5b 13af  u:g;.....q...[..
+000119f0: 259f 5fee 2fed 1a54 4b90 efd4 8090 b38c  %._./..TK.......
+00011a00: 31f6 17ed 8339 286c 824c 789c 5bc8 be90  1....9(l.Lx.[...
+00011a10: 7dc2 6946 938d 67ae 3201 0020 5905 356c  }.iF..g.2.. Y.5l
+00011a20: 1878 9c5b c8be 907d c269 46d3 8d67 ae32  .x.[...}.iF..g.2
+00011a30: 0100 205e 0536 6c17 789c 5bc8 be90 7dc2  .. ^.6l.x.[...}.
+00011a40: 6946 b38d 67ae 3201 0020 6305 376e 1778  iF..g.2.. c.7n.x
+00011a50: 9c5b c8be 907d c249 6633 3d83 8d67 ae32  .[...}.If3=..g.2
+00011a60: 0100 282b 0595 6c19 789c 5bc8 be90 7dc2  ..(+..l.x.[...}.
+00011a70: 6946 c38d 67ae 3201 0020 4a05 32b1 0378  iF..g.2.. J.2..x
+00011a80: 9c4b 2bca cf55 d02b 2e49 2c2a 51c8 cc2d  .K+..U.+.I,*Q..-
+00011a90: c807 5260 0e17 1757 7c7c 596a 5171 667e  ..R`...W||YjQqf~
+00011aa0: 5e7c bc82 ad82 ba81 9e99 9e81 3a17 00b2  ^|..........:...
+00011ab0: 170f a1b1 0378 9c4b 2bca cf55 d02b 2e49  .....x.K+..U.+.I
+00011ac0: 2c2a 51c8 cc2d c807 5260 0e17 1757 7c7c  ,*Q..-..R`...W||
+00011ad0: 596a 5171 667e 5e7c bc82 ad82 ba81 9ea9  YjQqf~^|........
+00011ae0: 9e99 3a17 00b2 240f a6e0 03c9 6c78 9c3b  ..:...$.....lx.;
+00011af0: c874 9049 ddd0 c0c0 ccc4 4421 3e3e 332f  .t.I......D!>>3/
+00011b00: b324 3e5e afa0 92e1 a764 63eb 611f 41d1  .$>^.....dc.a.A.
+00011b10: 1a47 a9c3 8b2f be5c e212 927e 71a3 ba14  .G.../.\...~q...
+00011b20: 2300 9379 11ef e003 c711 789c 3bc8 7490  #..y......x.;.t.
+00011b30: 49dd d0c0 c0cc c444 213e 3e33 2fb3 243e  I......D!>>3/.$>
+00011b40: 5eaf a092 a1c0 6959 40f5 eeb3 a97b 5a7f  ^.....iY@....{Z.
+00011b50: cf6e 53bb 9bf1 4af9 53c0 4675 2946 00a9  .nS...J.S.Fu)F..
+00011b60: d913 5ee0 03c7 4e78 9c3b c874 9049 ddd0  ..^...Nx.;.t.I..
+00011b70: c0c0 ccc4 4421 3e3e 332f b324 3e5e afa0  ....D!>>3/.$>^..
+00011b80: 9261 55ce aa94 b867 b94d 0a4f 3add f2a6  .aU....g.M.O:...
+00011b90: 46c4 6cd1 58f3 62a3 ba14 2300 a037 1288  F.l.X.b...#..7..
+00011ba0: ee01 7a78 9c3b c874 9069 82b1 4890 f894  ..zx.;.t.i..H...
+00011bb0: 62ad 76c7 a6cb 5137 dcdf 2cba eb7a 61e2  b.v...Q7..,..za.
+00011bc0: e5c0 89ee bf00 c4f6 0e95 e003 2a78 9c3b  ............*x.;
+00011bd0: c874 9049 ddd0 c0c0 ccc4 4421 3e3e 332f  .t.I......D!>>3/
+00011be0: b324 3e5e afa0 92a1 acbd f8fd 94b9 0922  .$>^..........."
+00011bf0: 8dd9 bfa5 3afe bebc 50fe 397e db46 7529  ....:...P.9~.Fu)
+00011c00: 4600 ae4a 13f9 e003 c64d 789c 3bc8 7490  F..J.....Mx.;.t.
+00011c10: 49dd d0c0 c0cc c444 213e 3e33 2fb3 243e  I......D!>>3/.$>
+00011c20: 5eaf a092 c174 45e8 dcbe fee6 096d a7f7  ^....tE......m..
+00011c30: 5618 2d9d c37b 9f2f fadb 4675 2946 009e  V.-..{./..Fu)F..
+00011c40: d512 7ab1 0378 9c4b 2bca cf55 d02b 2e49  ..z..x.K+..U.+.I
+00011c50: 2c2a 51c8 cc2d c807 5260 0e17 1757 7c7c  ,*Q..-..R`...W||
+00011c60: 596a 5171 667e 5e7c bc82 ad82 ba81 9ea9  YjQqf~^|........
+00011c70: 9ea9 3a17 00b2 210f a5b1 0378 9c4b 2bca  ..:...!....x.K+.
+00011c80: cf55 d02b 2e49 2c2a 51c8 cc2d c807 5260  .U.+.I,*Q..-..R`
+00011c90: 0e17 1757 7c7c 596a 5171 667e 5e7c bc82  ...W||YjQqf~^|..
+00011ca0: ad82 ba81 9ea9 9e89 3a17 00b2 1e0f a4b1  ........:.......
+00011cb0: 0378 9c4b 2bca cf55 d02b 2e49 2c2a 51c8  .x.K+..U.+.I,*Q.
+00011cc0: cc2d c807 5260 0e17 1757 7c7c 596a 5171  .-..R`...W||YjQq
+00011cd0: 667e 5e7c bc82 ad82 ba81 9ea9 9eb1 3a17  f~^|..........:.
+00011ce0: 00b2 1b0f a335 71ec 173e d5eb cad6 0b56  .....5q..>.....V
+00011cf0: dc66 99a5 1d6a 1871 0c                   .f...j.q.
```

### Comparing `gpt_computer_assistant-0.6.0/.github/workflows/deploys.yml` & `gpt_computer_assistant-0.6.1/.github/workflows/deploys.yml`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.github/workflows/release.yml` & `gpt_computer_assistant-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.github/workflows/release_generation.yml` & `gpt_computer_assistant-0.6.1/.github/workflows/release_generation.yml`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/.gitignore` & `gpt_computer_assistant-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/LICENSE` & `gpt_computer_assistant-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/PKG-INFO` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
-Name: gpt_computer_assistant
-Version: 0.6.0
+Name: gpt-computer-assistant
+Version: 0.6.1
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
         
-        ![intro](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-4139-bae5-5fcfa97c48a2)
+        
+        <a href="https://discord.gg/qApFmWMt8x"><img alt="Static Badge" src="https://img.shields.io/badge/Discord-Join?style=social&logo=discord" width=150></a>
+        
         
         
         ## Capabilities
         At this time we have many infrastructure element. We just aim to provide whole thinks that already in ChatGPT app.
         
          - **Screen Read**
          - Microphone
          - **System Audio**
          - Memory
         
         --
-        
+         - Open and close app
+         - Open a url
          - **Clipboard**
          - Search Engines
          - **Python and SH Interpreters**
          - Writing and Running Scripts
          - Using your Telegram Account
          - Knowledge Management
         
@@ -54,15 +57,15 @@
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/10b69a18-033c-4d81-8ac9-f4e3c65b59c3" alt="Read Docs" width="500"/></td>
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/0f483bae-ffaf-4311-8653-c0dc64fb5ebe" alt="Coding Assistant" width="500"/></td>   
         
           </tr>
         </table>
         
         ## Usage
-        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/5a744f7e-5b2e-40e5-ba3e-ea370aee5c0d)
+        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/91fe041d-4a3f-4a6e-9294-20ce2fa1ca36)
         
         
         ** After first click to an option that include microphone or system audio you need to stop with another click to same option.
         
         ## Installation && Run
         
         ```console
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: gpt_computer_assistant Version: 0.6.0 Summary: GPT
+Metadata-Version: 2.1 Name: gpt-computer-assistant Version: 0.6.1 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant Author: Onur
 Atakan ULUSOY Author-email: atadogan06@gmail.com License: MIT Description: #
 GPT Computer Assistant Hi, this is an unofficial work for providing ChatGPT
 MacOS app to Windows and Linux. In this way this is a fresh and stable work.
 You can easily install as Python library for this time but we will prepare a
-pipeline to providing native install scripts (.exe). ![intro](https://
-github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
-4139-bae5-5fcfa97c48a2) ## Capabilities At this time we have many
-infrastructure element. We just aim to provide whole thinks that already in
-ChatGPT app. - **Screen Read** - Microphone - **System Audio** - Memory -- -
+pipeline to providing native install scripts (.exe). _[_S_t_a_t_i_c_ _B_a_d_g_e_]##
+Capabilities At this time we have many infrastructure element. We just aim to
+provide whole thinks that already in ChatGPT app. - **Screen Read** -
+Microphone - **System Audio** - Memory -- - Open and close app - Open a url -
 **Clipboard** - Search Engines - **Python and SH Interpreters** - Writing and
 Running Scripts - Using your Telegram Account - Knowledge Management #### Todo
 - [x] Reset Option - [x] Splitting long audios. (Whisper api just support
 <20mb) - [x] Text input area - [x] Just text mode (no voice answer) - [x] Added
 different profiles - [ ] More Effect - [ ] Windows .exe - [ ] Linux native -
 [ ] MacOS native ## Use cases
 [Take Meeting Notes] [Daily Assistant]
 [Read Docs]          [Coding Assistant]
 ## Usage ![options](https://github.com/onuratakan/gpt-computer-assistant/
-assets/41792982/5a744f7e-5b2e-40e5-ba3e-ea370aee5c0d) ** After first click to
+assets/41792982/91fe041d-4a3f-4a6e-9294-20ce2fa1ca36) ** After first click to
 an option that include microphone or system audio you need to stop with another
 click to same option. ## Installation && Run ```console pip3 install gpt-
 computer-assistant ``` ```console computerassistant ``` Platform: UNKNOWN
 Requires-Python: >= 3 Description-Content-Type: text/markdown
```

### Comparing `gpt_computer_assistant-0.6.0/README.md` & `gpt_computer_assistant-0.6.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # GPT Computer Assistant
 Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
 
-![intro](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-4139-bae5-5fcfa97c48a2)
+
+<a href="https://discord.gg/qApFmWMt8x"><img alt="Static Badge" src="https://img.shields.io/badge/Discord-Join?style=social&logo=discord" width=150></a>
+
 
 
 ## Capabilities
 At this time we have many infrastructure element. We just aim to provide whole thinks that already in ChatGPT app.
 
  - **Screen Read**
  - Microphone
  - **System Audio**
  - Memory
 
 --
-
+ - Open and close app
+ - Open a url
  - **Clipboard**
  - Search Engines
  - **Python and SH Interpreters**
  - Writing and Running Scripts
  - Using your Telegram Account
  - Knowledge Management
 
@@ -46,15 +49,15 @@
     <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/10b69a18-033c-4d81-8ac9-f4e3c65b59c3" alt="Read Docs" width="500"/></td>
     <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/0f483bae-ffaf-4311-8653-c0dc64fb5ebe" alt="Coding Assistant" width="500"/></td>   
 
   </tr>
 </table>
 
 ## Usage
-![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/5a744f7e-5b2e-40e5-ba3e-ea370aee5c0d)
+![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/91fe041d-4a3f-4a6e-9294-20ce2fa1ca36)
 
 
 ** After first click to an option that include microphone or system audio you need to stop with another click to same option.
 
 ## Installation && Run
 
 ```console
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
 # GPT Computer Assistant Hi, this is an unofficial work for providing ChatGPT
 MacOS app to Windows and Linux. In this way this is a fresh and stable work.
 You can easily install as Python library for this time but we will prepare a
-pipeline to providing native install scripts (.exe). ![intro](https://
-github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
-4139-bae5-5fcfa97c48a2) ## Capabilities At this time we have many
-infrastructure element. We just aim to provide whole thinks that already in
-ChatGPT app. - **Screen Read** - Microphone - **System Audio** - Memory -- -
+pipeline to providing native install scripts (.exe). _[_S_t_a_t_i_c_ _B_a_d_g_e_]##
+Capabilities At this time we have many infrastructure element. We just aim to
+provide whole thinks that already in ChatGPT app. - **Screen Read** -
+Microphone - **System Audio** - Memory -- - Open and close app - Open a url -
 **Clipboard** - Search Engines - **Python and SH Interpreters** - Writing and
 Running Scripts - Using your Telegram Account - Knowledge Management #### Todo
 - [x] Reset Option - [x] Splitting long audios. (Whisper api just support
 <20mb) - [x] Text input area - [x] Just text mode (no voice answer) - [x] Added
 different profiles - [ ] More Effect - [ ] Windows .exe - [ ] Linux native -
 [ ] MacOS native ## Use cases
 [Take Meeting Notes] [Daily Assistant]
 [Read Docs]          [Coding Assistant]
 ## Usage ![options](https://github.com/onuratakan/gpt-computer-assistant/
-assets/41792982/5a744f7e-5b2e-40e5-ba3e-ea370aee5c0d) ** After first click to
+assets/41792982/91fe041d-4a3f-4a6e-9294-20ce2fa1ca36) ** After first click to
 an option that include microphone or system audio you need to stop with another
 click to same option. ## Installation && Run ```console pip3 install gpt-
 computer-assistant ``` ```console computerassistant ```
```

### Comparing `gpt_computer_assistant-0.6.0/bump.py` & `gpt_computer_assistant-0.6.1/bump.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/agent.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/agent.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/assistant.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/background.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/background.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/chat_history.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/chat_history.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/agent/proccess.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/agent/proccess.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/record.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/record.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/stt.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/stt.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/audio/tts.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/audio/tts.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/gpt_computer_assistant.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/gpt_computer_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/gui/button.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/gui/button.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,60 +94,92 @@
     def on_assistant_response_ready(self):
         self.main_window.update_state('talking')
 
 
 
 
     def settings_popup(self):
+        from ..gpt_computer_assistant import the_input_box
         # Create a settings dialog and inside of it create a text input about openai_api_key and a button to save it
         settings_dialog = QDialog()
         settings_dialog.setWindowTitle("Settings")
         settings_dialog.setWindowModality(Qt.ApplicationModal)
 
         settings_dialog.setLayout(QVBoxLayout())
         settings_dialog.layout().addWidget(QLabel("OpenAI API Key"))
         api_key_input = QLineEdit()
         api_key = load_api_key()
         api_key_input.setText(api_key)
         settings_dialog.layout().addWidget(api_key_input)
         save_button = QPushButton("Save")
-        save_button.clicked.connect(lambda: save_api_key(api_key_input.text()))
+
+        def save_api_key_(api_key):
+            save_api_key(api_key)
+            the_input_box.setText("Saved API Key")
+            settings_dialog.close()
+
+        save_button.clicked.connect(lambda: save_api_key_(api_key_input.text()))
         settings_dialog.layout().addWidget(save_button)
 
         # Add another button to reset memory
         reset_memory_button = QPushButton("Reset Memory")
-        reset_memory_button.clicked.connect(clear_chat_history)
+
+        def clear_chat_history_():
+            clear_chat_history()
+            the_input_box.setText("Cleared Chat History")
+            settings_dialog.close()
+
+        reset_memory_button.clicked.connect(clear_chat_history_)
         settings_dialog.layout().addWidget(reset_memory_button)
 
         # Add another button to enable just text model
         just_text_button = QPushButton("Enable Just Text Model")
 
         settings_dialog.layout().addWidget(just_text_button)
 
         if is_just_text_model_active():
-            just_text_button.setText("Disable Just Text Model")
-            just_text_button.clicked.connect(deactivate_just_text_model)
+            just_text_button.setText("Disabled Just Text Model")
+
+            def deactivate_just_text_model_():
+                deactivate_just_text_model()
+                the_input_box.setText("Disabled Just Text Model")
+                settings_dialog.close()
+
+            just_text_button.clicked.connect(deactivate_just_text_model_)
         else:
-            just_text_button.clicked.connect(activate_just_text_model)
+
+            def activate_just_text_model_():
+                activate_just_text_model()
+                the_input_box.setText("Enabled Just Text Model")
+                settings_dialog.close()
+
+            just_text_button.clicked.connect(activate_just_text_model_)
 
 
         #create a input form and save button to change profile
         settings_dialog.layout().addWidget(QLabel("Profile"))
         profile_input = QLineEdit()
 
         profile_input.setText(get_profile())
         settings_dialog.layout().addWidget(profile_input)
         profile_save_button = QPushButton("Save")
-        profile_save_button.clicked.connect(lambda: set_profile(profile_input.text()))
+
+        def set_profile_(profile):
+            set_profile(profile)
+            the_input_box.setText("Saved Profile")
+            settings_dialog.close()
+
+        profile_save_button.clicked.connect(lambda: set_profile_(profile_input.text()))
         settings_dialog.layout().addWidget(profile_save_button)
 
 
 
+        
         settings_dialog.exec_()
-        settings_dialog.show()
+    
 
 
 
     def input_text(self, text):
         
         self.main_window.update_state('thinking')
         if self.process_audio_thread is None or not self.process_audio_thread.is_alive():
```

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/start.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/start.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/db.py` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/db.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_24.png` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_24.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_256.png` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_256.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_32.png` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_32.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant/utils/media/icon_48.png` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant/utils/media/icon_48.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/PKG-INFO` & `gpt_computer_assistant-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
-Name: gpt-computer-assistant
-Version: 0.6.0
+Name: gpt_computer_assistant
+Version: 0.6.1
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
         
-        ![intro](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-4139-bae5-5fcfa97c48a2)
+        
+        <a href="https://discord.gg/qApFmWMt8x"><img alt="Static Badge" src="https://img.shields.io/badge/Discord-Join?style=social&logo=discord" width=150></a>
+        
         
         
         ## Capabilities
         At this time we have many infrastructure element. We just aim to provide whole thinks that already in ChatGPT app.
         
          - **Screen Read**
          - Microphone
          - **System Audio**
          - Memory
         
         --
-        
+         - Open and close app
+         - Open a url
          - **Clipboard**
          - Search Engines
          - **Python and SH Interpreters**
          - Writing and Running Scripts
          - Using your Telegram Account
          - Knowledge Management
         
@@ -54,15 +57,15 @@
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/10b69a18-033c-4d81-8ac9-f4e3c65b59c3" alt="Read Docs" width="500"/></td>
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/0f483bae-ffaf-4311-8653-c0dc64fb5ebe" alt="Coding Assistant" width="500"/></td>   
         
           </tr>
         </table>
         
         ## Usage
-        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/5a744f7e-5b2e-40e5-ba3e-ea370aee5c0d)
+        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/91fe041d-4a3f-4a6e-9294-20ce2fa1ca36)
         
         
         ** After first click to an option that include microphone or system audio you need to stop with another click to same option.
         
         ## Installation && Run
         
         ```console
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: gpt-computer-assistant Version: 0.6.0 Summary: GPT
+Metadata-Version: 2.1 Name: gpt_computer_assistant Version: 0.6.1 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant Author: Onur
 Atakan ULUSOY Author-email: atadogan06@gmail.com License: MIT Description: #
 GPT Computer Assistant Hi, this is an unofficial work for providing ChatGPT
 MacOS app to Windows and Linux. In this way this is a fresh and stable work.
 You can easily install as Python library for this time but we will prepare a
-pipeline to providing native install scripts (.exe). ![intro](https://
-github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
-4139-bae5-5fcfa97c48a2) ## Capabilities At this time we have many
-infrastructure element. We just aim to provide whole thinks that already in
-ChatGPT app. - **Screen Read** - Microphone - **System Audio** - Memory -- -
+pipeline to providing native install scripts (.exe). _[_S_t_a_t_i_c_ _B_a_d_g_e_]##
+Capabilities At this time we have many infrastructure element. We just aim to
+provide whole thinks that already in ChatGPT app. - **Screen Read** -
+Microphone - **System Audio** - Memory -- - Open and close app - Open a url -
 **Clipboard** - Search Engines - **Python and SH Interpreters** - Writing and
 Running Scripts - Using your Telegram Account - Knowledge Management #### Todo
 - [x] Reset Option - [x] Splitting long audios. (Whisper api just support
 <20mb) - [x] Text input area - [x] Just text mode (no voice answer) - [x] Added
 different profiles - [ ] More Effect - [ ] Windows .exe - [ ] Linux native -
 [ ] MacOS native ## Use cases
 [Take Meeting Notes] [Daily Assistant]
 [Read Docs]          [Coding Assistant]
 ## Usage ![options](https://github.com/onuratakan/gpt-computer-assistant/
-assets/41792982/5a744f7e-5b2e-40e5-ba3e-ea370aee5c0d) ** After first click to
+assets/41792982/91fe041d-4a3f-4a6e-9294-20ce2fa1ca36) ** After first click to
 an option that include microphone or system audio you need to stop with another
 click to same option. ## Installation && Run ```console pip3 install gpt-
 computer-assistant ``` ```console computerassistant ``` Platform: UNKNOWN
 Requires-Python: >= 3 Description-Content-Type: text/markdown
```

### Comparing `gpt_computer_assistant-0.6.0/gpt_computer_assistant.egg-info/SOURCES.txt` & `gpt_computer_assistant-0.6.1/gpt_computer_assistant.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 ./.git/logs/refs/remotes/origin/Added-input-box-and-button
 ./.git/logs/refs/remotes/origin/Added-just-text-mode
 ./.git/logs/refs/remotes/origin/Added-reset-system
 ./.git/logs/refs/remotes/origin/Added-send-text-with-screenshot-button
 ./.git/logs/refs/remotes/origin/Added-splitting-long-audios
 ./.git/logs/refs/remotes/origin/Fixed-high-delay-problem
 ./.git/logs/refs/remotes/origin/master
-./.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.idx
-./.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.pack
-./.git/objects/pack/pack-3a35c2c647a5165f748dd8be9812ee6b1c397beb.rev
+./.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.idx
+./.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.pack
+./.git/objects/pack/pack-3571ec173ed5ebcad60b56dc6699a51d6a18710c.rev
 ./.git/refs/heads/master
 ./.git/refs/remotes/origin/Added-different-profiles-mode
 ./.git/refs/remotes/origin/Added-icon
 ./.git/refs/remotes/origin/Added-input-box-and-button
 ./.git/refs/remotes/origin/Added-just-text-mode
 ./.git/refs/remotes/origin/Added-reset-system
 ./.git/refs/remotes/origin/Added-send-text-with-screenshot-button
@@ -63,14 +63,15 @@
 ./.git/refs/tags/v0.5.1
 ./.git/refs/tags/v0.5.2
 ./.git/refs/tags/v0.5.3
 ./.git/refs/tags/v0.5.4
 ./.git/refs/tags/v0.5.5
 ./.git/refs/tags/v0.5.6
 ./.git/refs/tags/v0.6.0
+./.git/refs/tags/v0.6.1
 ./.github/workflows/deploys.yml
 ./.github/workflows/release.yml
 ./.github/workflows/release_generation.yml
 ./gpt_computer_assistant/__init__.py
 ./gpt_computer_assistant/gpt_computer_assistant.py
 ./gpt_computer_assistant/llm.py
 ./gpt_computer_assistant/start.py
```

### Comparing `gpt_computer_assistant-0.6.0/setup.py` & `gpt_computer_assistant-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="gpt_computer_assistant",
-    version="0.6.0",
+    version="0.6.1",
     description="""GPT""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/onuratakan/gpt-computer-assistant",
     author="Onur Atakan ULUSOY",
     author_email="atadogan06@gmail.com",
     license="MIT",
```


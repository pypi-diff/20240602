# Comparing `tmp/harmon_ai-1.4.0.tar.gz` & `tmp/harmon_ai-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmon_ai-1.4.0.tar", last modified: Sat Jun  1 09:50:34 2024, max compression
+gzip compressed data, was "harmon_ai-1.5.1.tar", last modified: Sun Jun  2 10:48:52 2024, max compression
```

## Comparing `harmon_ai-1.4.0.tar` & `harmon_ai-1.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:50:34.551941 harmon_ai-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-06-01 09:50:34.551941 harmon_ai-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:50:34.547941 harmon_ai-1.4.0/harmon_ai/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/harmon_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:50:34.551941 harmon_ai-1.4.0/harmon_ai/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/badges_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/config.example.yml
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/important_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/readme_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/sections_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/templates/sns_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/harmon_ai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:50:34.551941 harmon_ai-1.4.0/harmon_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-06-01 09:50:34.000000 harmon_ai-1.4.0/harmon_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-01 09:50:34.000000 harmon_ai-1.4.0/harmon_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 09:50:34.000000 harmon_ai-1.4.0/harmon_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 09:50:34.000000 harmon_ai-1.4.0/harmon_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 09:50:34.000000 harmon_ai-1.4.0/harmon_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 09:50:34.000000 harmon_ai-1.4.0/harmon_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 09:50:34.551941 harmon_ai-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-01 09:50:30.000000 harmon_ai-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:48:52.376757 harmon_ai-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-06-02 10:48:52.376757 harmon_ai-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:48:52.372757 harmon_ai-1.5.1/harmon_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/harmon_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:48:52.376757 harmon_ai-1.5.1/harmon_ai/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/badges_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/config.example.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/important_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/readme_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/sections_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/templates/sns_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/harmon_ai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:48:52.376757 harmon_ai-1.5.1/harmon_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-06-02 10:48:52.000000 harmon_ai-1.5.1/harmon_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-02 10:48:52.000000 harmon_ai-1.5.1/harmon_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:48:52.000000 harmon_ai-1.5.1/harmon_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 10:48:52.000000 harmon_ai-1.5.1/harmon_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 10:48:52.000000 harmon_ai-1.5.1/harmon_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 10:48:52.000000 harmon_ai-1.5.1/harmon_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:48:52.376757 harmon_ai-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 10:48:48.000000 harmon_ai-1.5.1/setup.py
```

### Comparing `harmon_ai-1.4.0/LICENSE` & `harmon_ai-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `harmon_ai-1.4.0/PKG-INFO` & `harmon_ai-1.5.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,136 +1,132 @@
-Metadata-Version: 2.1
-Name: harmon_ai
-Version: 1.4.0
-Home-page: https://github.com/your_username/gaiah
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyyaml
-Requires-Dist: loguru
-
----
-title: HarmonAI II
-emoji: 🌖
-colorFrom: purple
-colorTo: gray
-sdk: streamlit
-sdk_version: 1.33.0
-app_file: app.py
-pinned: false
-license: mit
----
-
-
-<p align="center">
-<img src="https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/HarmonAI_II_icon.jpeg" width="100%">
-<br>
-<h1 align="center">HarmonAI II</h1>
-<h2 align="center">
-  ～AI Harmony, Infinite Possibilities～
-
-[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/HarmonAI_II)
-[![HarmonAI_II - Sunwood-ai-labs](https://img.shields.io/static/v1?label=HarmonAI_II&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/HarmonAI_II/Sunwood-ai-labs "Go to GitHub repo")
-[![stars - Sunwood-ai-labs](https://img.shields.io/github/stars/HarmonAI_II/Sunwood-ai-labs?style=social)](https://github.com/HarmonAI_II/Sunwood-ai-labs)
-[![forks - Sunwood-ai-labs](https://img.shields.io/github/forks/HarmonAI_II/Sunwood-ai-labs?style=social)](https://github.com/HarmonAI_II/Sunwood-ai-labs)
-[![GitHub Last Commit](https://img.shields.io/github/last-commit/Sunwood-ai-labs/HarmonAI_II)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
-[![GitHub Top Language](https://img.shields.io/github/languages/top/Sunwood-ai-labs/HarmonAI_II)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
-[![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/HarmonAI_II?sort=date&color=red)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
-[![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/HarmonAI_II?color=orange)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
-
-  <br>
-
-</h2>
-
-</p>
-
->[!IMPORTANT]
->このリポジトリは[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
-
-
-## 🌟 はじめに
-
-HarmonAI IIは、AIとの調和と無限の可能性を追求するプロジェクトです。このリポジトリは、HarmonAI IIの開発テンプレートとして機能し、以下のような特長を備えています:
-
-### 1. 開発スピードの向上
-- GitHub ActionsとHugging Faceの連携による自動デプロイ
-- 定型的な設定ファイル(.gitignore, .SourceSageignoreなど)の事前準備
-
-### 2. リポジトリの品質向上
-- 豊富なバッジによるプロジェクト情報の可視化
-- 体系的に整えられたREADMEテンプレート
-- SourceSageによるAI支援でのコミットメッセージ、リリースノート生成
-
-このテンプレートを活用することで、リポジトリ作成時の初期コストを抑えつつ、品質と開発速度を担保することができます。AI時代の開発スタイルを先取りした、生産性の高いテンプレートとしてご利用ください。
-
-## 🎥 デモ
-
-HarmonAI IIのデモアプリケーションは、GitHub Actionsと連携し、自動的にデプロイされています。デモアプリを体験することで、HarmonAI IIの機能を直感的に理解することができます。
-
-（準備中。。。）
-
-[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/HarmonAI_II)
-
-## 🚀 使い方
-
-### インストール
-HarmonAI IIは、以下のコマンドでインストールできます:
-
-```bash
-pip install harmon_ai
-```
-
-### 使用方法
-HarmonAI IIは、コマンドラインインターフェース(CLI)から簡単に使用できます。以下のコマンドを実行することで、プロジェクトのREADMEファイルを生成できます:
-
-```bash
-harmon-ai --repo_name=HarmonAI_II --owner_name=Sunwood-ai-labs --package_name=harmon_ai --icon_url=https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/HarmonAI_II_icon.jpeg --title="Harmon AI"
-```
-
-生成されたREADMEファイルは、プロジェクトのルートディレクトリに `README.md` として保存されます。
-
-### カスタマイズ
-HarmonAI IIは、ユーザーのニーズに合わせてカスタマイズ可能です。設定ファイルを編集することで、プロジェクトの動作を柔軟に調整できます。
-
-## 📝 アップデート
-
-### v1.3.0 (2024-05-13)
-- SNSテンプレートの追加とSNSバッジ生成機能の実装
-- CLIの強化とREADMEの更新
-- GitHub Actionsトリガーの更新
-- リファクタリングとコードのクリーンアップ
-
-### v1.2.0 (2024-05-13)
-- `harmon_ai`パッケージの刷新とCLIの導入
-- READMEテンプレートファイルの拡充
-- `harmon_ai`クラスのテストケースの実装
-- パッケージのセットアップ設定の更新
-
-### v1.1.0 (2024-04-24)
-- フロントページの作成とREADMEの改善
-- GitHub Actionsを使用したHugging Face hubへの自動シンク機能の追加
-- プロジェクト名の変更
-
-### v1.0.0 (2024-04-20)
-- 初回リリースと基本的な機能の実装
-
-## 🤝 コントリビューション
-HarmonAI IIへのご協力は大歓迎です！バグ報告、機能要求、プルリクエストなどを通じて、プロジェクトの改善にご協力ください。詳細は[CONTRIBUTING.md](CONTRIBUTING.md)をご覧ください。
-
-## 📄 ライセンス
-HarmonAI IIは[MIT License](LICENSE)の下でリリースされています。
-
-## 🙏 謝辞
-HarmonAI IIの開発にあたり、以下の方々に感謝いたします:
-
-- [Sunwood-ai-labs](https://github.com/Sunwood-ai-labs)チームのメンバー
-- [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)プロジェクト
-- [claude.ai](https://claude.ai/)チーム
-
-引き続き、HarmonAI IIプロジェクトをよろしくお願いいたします！
+---
+title: HarmonAI II
+emoji: 🌖
+colorFrom: purple
+colorTo: gray
+sdk: streamlit
+sdk_version: 1.33.0
+app_file: app.py
+pinned: false
+license: mit
+---
+
+
+<p align="center">
+<img src="https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/HarmonAI_II_icon.jpeg" width="100%">
+<br>
+<h1 align="center">HarmonAI II</h1>
+<h2 align="center">
+  ～AI Harmony, Infinite Possibilities～
+
+[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/HarmonAI_II)
+[![HarmonAI_II - Sunwood-ai-labs](https://img.shields.io/static/v1?label=HarmonAI_II&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/HarmonAI_II/Sunwood-ai-labs "Go to GitHub repo")
+[![stars - Sunwood-ai-labs](https://img.shields.io/github/stars/HarmonAI_II/Sunwood-ai-labs?style=social)](https://github.com/HarmonAI_II/Sunwood-ai-labs)
+[![forks - Sunwood-ai-labs](https://img.shields.io/github/forks/HarmonAI_II/Sunwood-ai-labs?style=social)](https://github.com/HarmonAI_II/Sunwood-ai-labs)
+[![GitHub Last Commit](https://img.shields.io/github/last-commit/Sunwood-ai-labs/HarmonAI_II)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
+[![GitHub Top Language](https://img.shields.io/github/languages/top/Sunwood-ai-labs/HarmonAI_II)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
+[![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/HarmonAI_II?sort=date&color=red)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
+[![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/HarmonAI_II?color=orange)](https://github.com/Sunwood-ai-labs/HarmonAI_II)
+
+  <br>
+
+</h2>
+
+</p>
+
+>[!IMPORTANT]
+>このリポジトリのリリースノートやREADME、コミットメッセージの9割近くは[claude.ai](https://claude.ai/)や[ChatGPT4](https://chatgpt.com/)を活用した[AIRA](https://github.com/Sunwood-ai-labs/AIRA), [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage), [Gaiah](https://github.com/Sunwood-ai-labs/Gaiah), [HarmonAI_II](https://github.com/Sunwood-ai-labs/HarmonAI_II)で生成しています。
+
+## Project: HarmonAI II
+
+```plaintext
+OS: nt
+Directory: C:\Prj\HarmonAI_II
+
+├─ harmon_ai/
+│  ├─ cli.py
+│  ├─ harmon_ai.py
+│  ├─ utils.py
+│  ├─ __init__.py
+├─ script/
+│  ├─ activate-harmon_ai_dev.bat
+├─ app.py
+├─ MANIFEST.in
+├─ README.md
+├─ setup.py
+```
+
+## 🌟 HarmonAI IIへようこそ！
+
+HarmonAI IIは、AIとの調和と無限の可能性を追求するプロジェクトです。私たちは、開発者の皆様がAIの力を最大限に活用し、効率的かつ高品質なソフトウェア開発を行えるよう、ユーザーフレンドリーなテンプレートを提供しています。
+
+## 🚀 HarmonAI IIの特長
+
+### 1. 簡単セットアップ
+HarmonAI IIは、わずか数ステップでセットアップが完了します。`pip install harmon_ai`コマンドを実行し、設定ファイル(`config.yml`)を編集するだけで、すぐに開発を始められます。
+
+### 2. カスタマイズ性の高さ
+設定ファイルを編集することで、プロジェクトの各種設定を自由にカスタマイズできます。リポジトリ名やパッケージ名、アイコン画像のURLなど、プロジェクトの詳細を簡単に変更できます。
+
+### 3. 自動化されたワークフロー
+GitHub ActionsとHugging Faceの連携により、コードのプッシュやリリースタグの作成をトリガーとして、自動的にパッケージのビルドとデプロイが行われます。面倒な手作業を省略し、開発に集中できます。
+
+### 4. 充実したドキュメンテーション
+HarmonAI IIは、プロジェクトの概要や使い方、アップデート履歴などを体系的にまとめたREADMEテンプレートを提供します。ドキュメントの作成に悩むことなく、わかりやすいREADMEを簡単に生成できます。
+
+### 5. AIによる開発サポート
+HarmonAI IIは、SourceSageとclaude.aiを活用し、コミットメッセージやリリースノートの自動生成をサポートします。AIの力を借りることで、開発者は本質的なタスクに集中できます。
+
+## 🛠️ 使い方
+
+1. `pip install harmon_ai`コマンドを実行し、HarmonAI IIをインストールします。
+2. プロジェクトのルートディレクトリに`.harmon_ai`ディレクトリを作成し、`config.yml`ファイルを配置します。
+3. `config.yml`ファイルを編集し、プロジェクトの各種設定を行います。
+4. `harmon-ai`コマンドを実行し、カスタマイズされたREADMEファイルを生成します。
+
+詳細な使用方法については、[ドキュメント](docs/intoro.md)をご覧ください。
+
+## 📝 アップデート
+
+### v1.5.0 (2024-06-02)
+- READMEの自動置換機能
+- Gaiah設定ファイルの追加
+
+### v1.4.0 (2024-06-01)
+- YAMLによる設定ファイル管理
+- CI/CDファイルの自動コピー
+
+### v1.3.0 (2024-05-13)
+- SNSテンプレートの追加とSNSバッジ生成機能の実装
+- CLIの強化とREADMEの更新
+- GitHub Actionsトリガーの更新
+- リファクタリングとコードのクリーンアップ
+
+### v1.2.0 (2024-05-13)
+- `harmon_ai`パッケージの刷新とCLIの導入
+- READMEテンプレートファイルの拡充
+- `harmon_ai`クラスのテストケースの実装
+- パッケージのセットアップ設定の更新
+
+### v1.1.0 (2024-04-24)
+- フロントページの作成とREADMEの改善
+- GitHub Actionsを使用したHugging Face hubへの自動シンク機能の追加
+- プロジェクト名の変更
+
+### v1.0.0 (2024-04-20)
+- 初回リリースと基本的な機能の実装
+
+
+
+## 🤝 コントリビューション
+
+HarmonAI IIは、オープンソースプロジェクトとして、コミュニティからの貢献を歓迎しています。バグ報告や機能リクエスト、プルリクエストなどを通じて、プロジェクトの改善にご協力ください。コントリビューションガイドラインについては、[CONTRIBUTING.md](CONTRIBUTING.md)をご覧ください。
+
+## 📄 ライセンス
+
+HarmonAI IIは、MITライセンスの下で公開されています。詳細については、[LICENSE](LICENSE)ファイルをご確認ください。
+
+## 🙏 謝辞
+
+HarmonAI IIの開発にあたり、Sunwood-ai-labsチームのメンバー、SourceSageプロジェクト、そしてclaude.aiチームに深く感謝いたします。皆様のご支援なくしては、このプロジェクトは実現できませんでした。
+
+HarmonAI IIは、これからもAIと人間の調和を目指し、開発者の皆様に最高のエクスペリエンスを提供できるよう尽力してまいります。ぜひ、HarmonAI IIを活用し、AIの力を開発に役立ててください！
```

### Comparing `harmon_ai-1.4.0/harmon_ai/cli.py` & `harmon_ai-1.5.1/harmon_ai/cli.py`

 * *Files identical despite different names*

### Comparing `harmon_ai-1.4.0/harmon_ai/harmon_ai.py` & `harmon_ai-1.5.1/harmon_ai/harmon_ai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import os
 from pathlib import Path
 from .utils import load_config, load_file_content, copy_cicd_file_if_missing, config_preview
 from art import tprint
+from loguru import logger
 
 class HarmonAI:
-    def __init__(self):
-        config_path = os.path.expanduser("./.harmon_ai/config.yml")
-        self.config = load_config(config_path, os.path.join(Path(__file__).parent, "templates/config.example.yml"))
-
+    def __init__(self, config_path="./.harmon_ai/config.yml", config=None):
+        
+        if(config is None):
+            config_path = os.path.expanduser(config_path)
+            self.config = load_config(config_path, os.path.join(Path(__file__).parent, "templates/config.example.yml"))
+        else:
+            self.config = config
+            
         tprint("-- HarmonAI --")
         config_preview(self.config)
 
         output_dir = self.config['harmon_ai']['development']['output_dir']
         os.makedirs(output_dir, exist_ok=True)
 
         self.important_message = load_file_content(
@@ -49,21 +54,31 @@
         template = template.replace("{sections_content}", self.sections_content)
         template = template.replace("{sns_badges}", sns_badges)
 
         output_path = os.path.join(self.config['harmon_ai']['development']['output_dir'], self.config['harmon_ai']['product']['output_file'])
         with open(output_path, "w", encoding="utf8") as file:
             file.write(template)
 
+        if(self.config['harmon_ai']['main']['replace_readme']):
+            
+            main_readme_path = os.path.join(self.config['harmon_ai']['main']['main_dir'], "README.md")
+            logger.success(f"README.mdが置換されました ({main_readme_path})")
+            with open(main_readme_path, "w", encoding="utf8") as file:
+                file.write(template)
+        
     def generate_badges(self):
         template = self.load_template("badges_template")
         template = template.replace("{repo_name}", self.config['harmon_ai']['environment']['repo_name'])
         template = template.replace("{owner_name}", self.config['harmon_ai']['environment']['owner_name'])
         template = template.replace("{package_name}", self.config['harmon_ai']['environment']['package_name'])
         return template
 
     def generate_sns_badges(self):
         template = self.load_template("sns_template")
         template = template.replace("{website_url}", self.config['harmon_ai']['environment']['website_url'])
         template = template.replace("{github_url}", self.config['harmon_ai']['environment']['github_url'])
         template = template.replace("{twitter_url}", self.config['harmon_ai']['environment']['twitter_url'])
         template = template.replace("{blog_url}", self.config['harmon_ai']['environment']['blog_url'])
-        return template
+        return template
+    
+    
+
```

### Comparing `harmon_ai-1.4.0/harmon_ai/templates/badges_template.md` & `harmon_ai-1.5.1/harmon_ai/templates/badges_template.md`

 * *Files identical despite different names*

### Comparing `harmon_ai-1.4.0/harmon_ai/templates/publish-to-pypi.yml` & `harmon_ai-1.5.1/harmon_ai/templates/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `harmon_ai-1.4.0/harmon_ai/utils.py` & `harmon_ai-1.5.1/harmon_ai/utils.py`

 * *Files identical despite different names*

### Comparing `harmon_ai-1.4.0/harmon_ai.egg-info/SOURCES.txt` & `harmon_ai-1.5.1/harmon_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harmon_ai-1.4.0/setup.py` & `harmon_ai-1.5.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="harmon_ai",
-    version="1.4.0",
+    version="1.5.1",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         # Add any dependencies here
         'pyyaml',
         'loguru'
     ],
```

